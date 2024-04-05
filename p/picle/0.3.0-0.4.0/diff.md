# Comparing `tmp/picle-0.3.0.tar.gz` & `tmp/picle-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picle-0.3.0.tar", max compression
+gzip compressed data, was "picle-0.4.0.tar", max compression
```

## Comparing `picle-0.3.0.tar` & `picle-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-01-01 02:30:45.840067 picle-0.3.0/LICENSE
--rw-r--r--   0        0        0       80 2023-03-05 10:26:23.338732 picle-0.3.0/picle/__init__.py
--rw-r--r--   0        0        0     4531 2024-03-16 10:14:19.744008 picle-0.3.0/picle/cache.py
--rw-r--r--   0        0        0    23470 2024-03-16 10:21:50.628910 picle-0.3.0/picle/picle.py
--rw-r--r--   0        0        0      354 2024-03-16 10:14:19.703537 picle-0.3.0/picle/utils.py
--rw-r--r--   0        0        0     1529 2024-03-16 10:22:15.938688 picle-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      417 2023-01-01 02:47:33.693216 picle-0.3.0/README.md
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 picle-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-01 02:30:45.840067 picle-0.4.0/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-05 01:13:50.673276 picle-0.4.0/picle/__init__.py
+-rw-r--r--   0        0        0     4531 2024-03-16 10:14:19.744008 picle-0.4.0/picle/cache.py
+-rw-r--r--   0        0        0     3193 2024-04-05 08:48:59.627598 picle-0.4.0/picle/models.py
+-rw-r--r--   0        0        0    28317 2024-04-05 08:48:59.808228 picle-0.4.0/picle/picle.py
+-rw-r--r--   0        0        0      354 2024-04-05 03:31:06.926191 picle-0.4.0/picle/utils.py
+-rw-r--r--   0        0        0     1529 2024-04-05 08:48:38.046270 picle-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1329 2024-03-19 10:44:18.402593 picle-0.4.0/README.md
+-rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 picle-0.4.0/PKG-INFO
```

### Comparing `picle-0.3.0/LICENSE` & `picle-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picle-0.3.0/picle/cache.py` & `picle-0.4.0/picle/cache.py`

 * *Files identical despite different names*

### Comparing `picle-0.3.0/picle/picle.py` & `picle-0.4.0/picle/picle.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 class FieldKeyError(Exception):
     """
     Raised if parameter not in model's fields and none of the
     fields names starts with parameter.
     """
 
 
+class SyntaxError(Exception):
+    """
+    Command syntax error
+    """
+
+
 class App(cmd.Cmd):
     """
     PICLE App class to construct shell.
 
     :param root: Root/Top Pydantic model
     """
 
@@ -147,47 +153,86 @@
         else:
             self.shell(**data)
 
     def parse_command(
         self, command: str, validate: bool = False, add_default_values: bool = False
     ) -> list:
         """
-        Function to parse command string and construct list of model 
+        Function to parse command string and construct list of model
         references and fields values.
 
         :param command: command string
 
-        Returns a list of dictionaries with collected models details
+        Returns a list of lists of dictionaries with collected models details
         each dictionary containing ``model``, ``fields`` and ``parameter``
         keys.
         """
         current_model = {"model": self.shell, "fields": [], "parameter": ...}
         current_field = {}
         models = [current_model]
         parameters = [i for i in command.split(" ") if i.strip()]
+        pipe_models = None
+        ret = [models]
 
         # iterate over command parameters and decide if its a reference
         # to a model or model's field value
         while parameters:
             parameter = parameters.pop(0)
+            # handle pipe - "|"
+            if parameter == "|":
+                # check if current model has pipe defined
+                if hasattr(current_model["model"], "PicleConfig") and getattr(
+                    current_model["model"].PicleConfig, "pipe", None
+                ):
+                    if current_model["model"].PicleConfig.pipe == "self":
+                        # reference pipe model to current model
+                        current_model = {
+                            "model": current_model["model"],
+                            "fields": [],
+                            "parameter": parameter,
+                        }
+                    else:
+                        # goto pipe model
+                        current_model = {
+                            "model": current_model["model"].PicleConfig.pipe,
+                            "fields": [],
+                            "parameter": parameter,
+                        }
+                    models = [current_model]
+                    ret.append(models)
+                else:
+                    raise SyntaxError(
+                        f"'{current_model['model']}' does not support pipe handling"
+                    )
             # collect single quoted field value
-            if '"' in parameter and current_field:
+            elif '"' in parameter and current_field:
                 value_items = [parameter.replace('"', "")]
                 # collect further values if first parameter not double quoted value e.g. "nrp1"
                 if parameter.count('"') != 2:
                     while parameters:
                         parameter = parameters.pop(0)
                         value_items.append(parameter.replace('"', ""))
                         if '"' in parameter:
                             break
                 value = " ".join(value_items)  # form value string
                 self._save_collected_value(current_field, value)
             # handle reference to model
-            elif current_model["model"].model_fields.get(parameter):
-                field = current_model["model"].model_fields[parameter]
+            elif current_model["model"].model_fields.get(parameter) or any(
+                parameter == f.alias
+                for f in current_model["model"].model_fields.values()
+            ):
+                # source field by name
+                if current_model["model"].model_fields.get(parameter):
+                    field = current_model["model"].model_fields[parameter]
+                else:
+                    # source field by alias
+                    for f_name, field in current_model["model"].model_fields.items():
+                        if parameter == field.alias:
+                            parameter = f_name  # use actual field name
+                            break
                 # handle next level model reference
                 if isinstance(field.annotation, ModelMetaclass):
                     # goto next model
                     current_model = {
                         "model": field.annotation,
                         "fields": [],
                         "parameter": parameter,
@@ -254,74 +299,90 @@
         ):
             value = current_field["field"].json_schema_extra["presence"]
             self._save_collected_value(current_field, value)
         # validated collected values
         if validate:
             self._validate_values(models)
 
-        return models
+        return ret
 
     def print_model_help(
-        self, model: dict, verbose: bool = False, match: str = None
+        self, models: list, verbose: bool = False, match: str = None
     ) -> None:
         """
         Function to form and print help message for model fields.
 
         :param match: only collect help for fields that start with ``match`` string
         """
+        model = models[-1][-1]  # get last model
         last_field = model["fields"][-1] if model["fields"] else None
         lines = {}  # dict of {cmd: cmd_help}
         width = 0  # record longest command width for padding
         # print help message only for last collected field
         if last_field and last_field["values"] == ...:
             field = model["model"].model_fields[last_field["name"]]
-            name = f"<{last_field['name']} value>"
+            name = f"<'{last_field['name']}' value>"
+            # check if field is callable
+            if field.annotation is Callable:
+                name = "<ENTER>"
+                lines[name] = "Execute command"
+                width = max(width, len(name))
             # add options for enumerations
-            if isinstance(field.annotation, enum.EnumMeta):
+            elif isinstance(field.annotation, enum.EnumMeta):
                 options = [i.value for i in field.annotation]
                 lines[name] = ", ".join(options)
             # check if model has method to source field choices
             elif hasattr(model["model"], f"source_{last_field['name']}"):
                 options = getattr(model["model"], f"source_{last_field['name']}")()
                 lines[name] = ", ".join(options)
             else:
                 lines[name] = f"{field.description}"
                 if verbose:
                     lines[name] += (
                         f"; default '{field.get_default()}', type '{str(field.annotation)}', "
                         f"is required - {field.is_required()}"
                     )
-            width = max(width, len(name))
         # collect help message for all fields of this model
         else:
             # check if model supports subshell
             if (
                 hasattr(model["model"], "PicleConfig")
                 and getattr(model["model"].PicleConfig, "subshell", None) is True
                 # exclude <ENTER> if already in model's shell
                 and not self.shells[-1] == model["model"]
             ):
                 name = "<ENTER>"
                 lines[name] = "Enter command subshell"
                 width = max(width, len(name))
             # iterate over model fields
             for name, field in model["model"].model_fields.items():
+                # check if field has alias
+                if field.alias:
+                    name = field.alias
                 # skip fields that already have values
                 if any(f["name"] == name for f in model["fields"]):
                     continue
                 # filter fields
                 if match and not name.startswith(match):
                     continue
                 lines[name] = f"{field.description}"
                 if verbose:
                     lines[name] += (
                         f"; default '{field.get_default()}', type '{str(field.annotation)}', "
                         f"is required - {field.is_required()}"
                     )
                 width = max(width, len(name))
+        # check if model has pipe defined
+        if hasattr(model["model"], "PicleConfig") and getattr(
+            model["model"].PicleConfig, "pipe", None
+        ):
+            name = "|"
+            lines[name] = "Execute pipe command"
+            width = max(width, len(name))
+        width = max(width, len(name))
         # form help lines
         help_msg = []
         for k in sorted(lines.keys()):
             padding = " " * (width - len(k)) + (" " * 4)
             help_msg.append(f"{k}{padding}{lines[k]}")
         # print help message
         self.write(self.newline.join(help_msg))
@@ -330,25 +391,25 @@
         """
         This method called for every  command parameter on
         complete key hit except for the very first one.
         """
         fieldnames = []
         try:
             command_models = self.parse_command(line)
-            last_model = command_models[-1]["model"]
+            last_model = command_models[-1][-1]["model"]
             # check if last model has fields collected
-            if command_models[-1]["fields"]:
-                last_field_name = command_models[-1]["fields"][-1]["name"]
+            if command_models[-1][-1]["fields"]:
+                last_field_name = command_models[-1][-1]["fields"][-1]["name"]
                 last_field = last_model.model_fields[last_field_name]
-                last_field_value = command_models[-1]["fields"][-1]["values"]
+                last_field_value = command_models[-1][-1]["fields"][-1]["values"]
                 if isinstance(last_field_value, list):
                     last_field_value = last_field_value[-1]
                 elif last_field_value == ...:
                     last_field_value = ""
-                # check if need to exctract enum values
+                # check if need to extract enum values
                 if isinstance(last_field.annotation, enum.EnumMeta):
                     fieldnames = [
                         i.value
                         for i in last_field.annotation
                         if i.value.startswith(last_field_value)
                     ]
                 # check if model has method to source field choices
@@ -359,15 +420,15 @@
                     ]
             # return a list of all model fields
             else:
                 fieldnames = list(last_model.model_fields)
         except FieldLooseMatchOnly as e:
             model, parameter = e.args
             fieldnames = [
-                name
+                f.alias or name
                 for name, f in model["model"].model_fields.items()
                 # skip fields with already collected values from complete prompt
                 if name.startswith(parameter)
                 and not any(
                     True
                     for collected_field in model["fields"]
                     if collected_field["name"] == name
@@ -393,15 +454,15 @@
             if method_name.startswith("do_"):
                 name = method_name.replace("do_", "")
                 if name.startswith(line):
                     fieldnames.append(name)
         # collect model arguments
         try:
             command_models = self.parse_command(line)
-            fieldnames.extend(command_models[-1]["model"].model_fields)
+            fieldnames.extend(command_models[-1][-1]["model"].model_fields)
         # collect arguments that startswith last parameter
         except FieldLooseMatchOnly as e:
             model, parameter = e.args
             for name, f in model["model"].model_fields.items():
                 if name.startswith(parameter):
                     fieldnames.append(name)
         # raised if no model fields matched last parameter
@@ -409,15 +470,15 @@
             pass
         return sorted(fieldnames)
 
     def do_help(self, arg):
         """Print help message"""
         command_models = self.parse_command(arg.strip("?"))
         self.print_model_help(
-            command_models[-1], verbose=True if arg.strip().endswith("?") else False
+            command_models, verbose=True if arg.strip().endswith("?") else False
         )
         # print help for global top commands
         if len(arg.strip().split(" ")) == 1:
             lines = {}  # dict of {cmd: cmd_help}
             width = 0  # record longest command width for padding
             for method_name in dir(self):
                 if method_name.startswith("do_"):
@@ -468,15 +529,15 @@
         # print help for given command or commands
         if line.strip().endswith("?"):
             try:
                 command_models = self.parse_command(line.strip().rstrip("?"))
             except FieldLooseMatchOnly as e:
                 model, parameter = e.args
                 self.print_model_help(
-                    model,
+                    [[model]],
                     verbose=True if line.strip().endswith("??") else False,
                     match=parameter,
                 )
             except FieldKeyError as e:
                 model, parameter = e.args
                 model_name = (
                     model["model"].__name__
@@ -484,27 +545,27 @@
                     else model["model"].__repr_name__()
                 )
                 self.write(
                     f"Incorrect command, '{parameter}' not part of '{model_name}' model fields"
                 )
             else:
                 self.print_model_help(
-                    command_models[-1],
+                    command_models,
                     verbose=True if line.strip().endswith("??") else False,
                 )
         else:
             try:
                 command_models = self.parse_command(
                     line, validate=True, add_default_values=True
                 )
             except FieldLooseMatchOnly as e:
                 model, parameter = e.args
                 # filter fields to return message for
                 fields = [
-                    name
+                    f.alias or name
                     for name, f in model["model"].model_fields.items()
                     if name.startswith(parameter)
                 ]
                 self.write(
                     f"Incomplete command, possible completions: " f"{', '.join(fields)}"
                 )
             except FieldKeyError as e:
@@ -516,61 +577,96 @@
                 )
                 self.write(
                     f"Incorrect command, '{parameter}' not part of '{model_name}' model fields"
                 )
             except ValidationError as e:
                 self.write(e)
             else:
-                # collect arguments
-                run_kwargs = {
-                    f["name"]: f["values"]
-                    for model in command_models
-                    for f in model["fields"]
-                    if f["values"] is not ...
-                }
-                # run model "run" function if it exits
-                model = command_models[-1]["model"]
-                if run_kwargs and hasattr(model, "run"):
-                    ret = model.run(**run_kwargs)
-                # check if model has subshell
-                elif (
-                    hasattr(model, "PicleConfig")
-                    and getattr(model.PicleConfig, "subshell", None) is True
-                ):
-                    # collect parent shells
-                    for item in command_models[:-1]:
-                        m = item["model"]
-                        if (
-                            hasattr(m, "PicleConfig")
-                            and getattr(m.PicleConfig, "subshell", None) is True
-                        ):
-                            if m not in self.shells:
-                                self.shells.append(m)
-                    # update prompt value
-                    self.prompt = getattr(model.PicleConfig, "prompt", self.prompt)
-                    self.shell = model
-                    self.shells.append(self.shell)
-                elif command_models[-1]["fields"]:
-                    # check if last field refers to callable e.g. function
-                    last_field_name = command_models[-1]["fields"][-1]["name"]
-                    last_field = model.model_fields[last_field_name]
-                    if last_field.annotation is Callable:
-                        method_name = last_field.get_default()
-                        if method_name and hasattr(model, method_name):
-                            ret = getattr(model, method_name)(**run_kwargs)
+                # go over collected commands separated by pipe
+                for index, command in enumerate(command_models):
+                    # collect arguments
+                    run_kwargs = {
+                        f["name"]: f["values"]
+                        for model in command
+                        for f in model["fields"]
+                        if f["values"] is not ...
+                    }
+                    # run model "run" function if it exits
+                    model = command[-1]["model"]
+                    if run_kwargs and hasattr(model, "run"):
+                        # call first command using collected arguments only
+                        if index == 0:
+                            ret = model.run(**run_kwargs)
+                        # pipe results through subsequent commands
+                        else:
+                            ret = model.run(ret, **run_kwargs)
+                    # check if model has subshell
+                    elif (
+                        hasattr(model, "PicleConfig")
+                        and getattr(model.PicleConfig, "subshell", None) is True
+                    ):
+                        # collect parent shells
+                        for item in command[:-1]:
+                            m = item["model"]
+                            if (
+                                hasattr(m, "PicleConfig")
+                                and getattr(m.PicleConfig, "subshell", None) is True
+                            ):
+                                if m not in self.shells:
+                                    self.shells.append(m)
+                        # update prompt value
+                        self.prompt = getattr(model.PicleConfig, "prompt", self.prompt)
+                        self.shell = model
+                        self.shells.append(self.shell)
+                    elif command[-1]["fields"]:
+                        last_field_name = command[-1]["fields"][-1]["name"]
+                        last_field = model.model_fields[last_field_name]
+                        json_schema_extra = (
+                            getattr(last_field, "json_schema_extra") or {}
+                        )
+                        # check if last field refers to callable e.g. function
+                        if last_field.annotation is Callable:
+                            method_name = last_field.get_default()
+                            if method_name and hasattr(model, method_name):
+                                # call first command using collected arguments only
+                                if index == 0:
+                                    ret = getattr(model, method_name)(**run_kwargs)
+                                # pipe results through subsequent commands
+                                else:
+                                    ret = getattr(model, method_name)(ret, **run_kwargs)
+                            else:
+                                self.write(
+                                    f"Model '{model.__name__}' has no '{method_name}' "
+                                    f"method defined for '{last_field_name}' Callable field"
+                                )
+                        # check if last field has `function` parameter defined
+                        elif json_schema_extra.get("function"):
+                            method_name = json_schema_extra["function"]
+                            if hasattr(model, method_name):
+                                # call first command using collected arguments only
+                                if index == 0:
+                                    ret = getattr(model, method_name)(**run_kwargs)
+                                # pipe results through subsequent commands
+                                else:
+                                    ret = getattr(model, method_name)(ret, **run_kwargs)
+                            else:
+                                self.write(
+                                    f"Model '{model.__name__}' has no '{method_name}' "
+                                    f"method defined for '{last_field_name}' function"
+                                )
                         else:
                             self.write(
-                                f"Model '{model.__name__}' has no '{method_name}' "
-                                f"method defined for '{last_field_name}' Callable field"
+                                f"Model '{model.__name__}' has no 'run' method defined"
                             )
+                        # run result through processors if any
+                        for processor in json_schema_extra.get("processors", []):
+                            ret = processor(ret)
                     else:
-                        self.write(
-                            f"Model '{model.__name__}' has no 'run' method defined"
-                        )
-                else:
-                    self.write(f"Incorrect command")
+                        self.write(f"Incorrect command")
+                        continue
+
         # returning True will close the shell
         if ret is True:
             return True
         elif ret:
             self.write(ret)
         return None
```

### Comparing `picle-0.3.0/pyproject.toml` & `picle-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "picle"
-version = "0.3.0"
+version = "0.4.0"
 description = "Python Interactive Command Line Shells"
 authors = ["Denis Mulyalin <d.mulyalin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dmulyalin/picle"
 repository = "https://github.com/dmulyalin/picle"
 documentation = "https://dmulyalin.github.io/picle/"
```

