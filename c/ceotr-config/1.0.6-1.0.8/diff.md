# Comparing `tmp/ceotr_config-1.0.6.tar.gz` & `tmp/ceotr_config-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ceotr_config-1.0.6.tar", last modified: Sun Mar 26 17:57:37 2023, max compression
+gzip compressed data, was "ceotr_config-1.0.8.tar", last modified: Fri Apr  5 14:49:44 2024, max compression
```

## Comparing `ceotr_config-1.0.6.tar` & `ceotr_config-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxrwxr-x   0 ceotr     (1001) ceotr     (1001)        0 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)       39 2023-01-06 18:42:53.000000 ceotr_config-1.0.6/MANIFEST.in
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)      322 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/PKG-INFO
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)      683 2023-01-05 20:38:39.000000 ceotr_config-1.0.6/README.md
-drwxrwxr-x   0 ceotr     (1001) ceotr     (1001)        0 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config/
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)      957 2023-01-05 20:38:39.000000 ceotr_config-1.0.6/ceotr_config/__init__.py
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)     8104 2023-03-26 17:57:31.000000 ceotr_config-1.0.6/ceotr_config/config_handler.py
-drwxrwxr-x   0 ceotr     (1001) ceotr     (1001)        0 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config/template/
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)        0 2023-01-05 20:38:39.000000 ceotr_config-1.0.6/ceotr_config/template/__init__.py
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)       93 2023-01-05 20:38:39.000000 ceotr_config-1.0.6/ceotr_config/template/default_django_setting.yml-tpl
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)       45 2023-01-05 20:38:39.000000 ceotr_config-1.0.6/ceotr_config/template/default_setting.yml-tpl
-drwxrwxr-x   0 ceotr     (1001) ceotr     (1001)        0 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config.egg-info/
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)      322 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config.egg-info/PKG-INFO
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)      429 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config.egg-info/SOURCES.txt
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)        1 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config.egg-info/dependency_links.txt
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)        7 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config.egg-info/requires.txt
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)       13 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config.egg-info/top_level.txt
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)        1 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/ceotr_config.egg-info/zip-safe
--rw-rw-r--   0 ceotr     (1001) ceotr     (1001)       38 2023-03-26 17:57:37.000000 ceotr_config-1.0.6/setup.cfg
--rwxrwxr-x   0 ceotr     (1001) ceotr     (1001)      710 2023-03-26 17:57:31.000000 ceotr_config-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.848637 ceotr_config-1.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      336 2024-04-05 14:49:44.848637 ceotr_config-1.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2024-04-05 14:34:18.000000 ceotr_config-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.846637 ceotr_config-1.0.8/ceotr_config/
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10977 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/config_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.847637 ceotr_config-1.0.8/ceotr_config/template/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/template/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/template/default_django_setting.yml-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       45 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/ceotr_config/template/default_setting.yml-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.847637 ceotr_config-1.0.8/ceotr_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      336 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      568 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 14:49:44.000000 ceotr_config-1.0.8/ceotr_config.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 14:49:44.848637 ceotr_config-1.0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      716 2024-04-05 14:47:42.000000 ceotr_config-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.847637 ceotr_config-1.0.8/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.847637 ceotr_config-1.0.8/test/ceotr_conifg_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/test/ceotr_conifg_test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 14:49:44.848637 ceotr_config-1.0.8/test/ceotr_conifg_test/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/test/ceotr_conifg_test/resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16730 2024-04-04 21:28:32.000000 ceotr_config-1.0.8/test/ceotr_conifg_test/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ceotr_config-1.0.6/ceotr_config/__init__.py` & `ceotr_config-1.0.8/ceotr_config/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,29 +4,35 @@
 class BaseConfigAgent:
     def __init__(self, default_template):
         self._debug = True
         self._config_yml = None
         self.default_template = default_template
 
     @property
-    def DEBUG(self):
+    def debug(self):
         if hasattr(self, 'general_info'):
             return self.general_info['ENVIRONMENT'] != 'prod'
         return self._debug
 
     def load(self, setting_path=None, setting_template=None):
         self._config_yml = ConfigHandler(setting_path, setting_template, self.default_template).build_or_load()
         self._load(self._config_yml)
 
     def _load(self, config_yml):
         for item, value in config_yml.items():
             setattr(self, item, value)
 
+    def dict(self):
+        return self._config_yml
+
 
 class DjangoConfigAgent(BaseConfigAgent):
     def __init__(self):
         super().__init__('default_django_setting.yml-tpl')
 
 
 class ConfigAgent(BaseConfigAgent):
     def __init__(self):
         super().__init__('default_setting.yml-tpl')
+
+
+config_agent = ConfigAgent()
```

### Comparing `ceotr_config-1.0.6/ceotr_config/config_handler.py` & `ceotr_config-1.0.8/ceotr_config/config_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import yaml
 import copy
 import json
+import warnings
+DOCKER_ENVIRONMENT = "docker"
 
 
 def check_create_dir(file_dir, recursively=False):
     """
     If dir exist just return the path, else create the dir and return the path
     """
     if not os.path.isdir(file_dir):
@@ -21,55 +23,111 @@
     file_name = os.path.basename(setting_path)
     if not file_name.endswith(".yml"):
         msg = "Given setting name {} must end with .yml".format(setting_path)
         raise ValueError(msg)
 
 
 class ConfigHandler(object):
+    DEFAULT_DOCKER_KEYWORDS = ["DATABASE"]
+
+    def __init__(self, setting_path, template_dir, default_template_name, check_value_update=False, project_root=None):
 
-    def __init__(self, setting_path, template_dir, default_template_name, check_value_update=False):
         """
         :param setting_path: Setting file path for the project
         :param template_dir:
         :param default_template_name: Default template name, the template is under app_common.config.template
         """
+        self.project_root = project_root
         self.template_path = template_dir
         self.default_template_name = default_template_name
         self.setting_path = setting_path
         self.check_value_update = check_value_update
         setting_file_path_validation(setting_path)
         self.yml_config = None
         self.possible_unchanged_field = []
+        self._docker_keywords = []
+
+    def build_sys_value_mapping(self, yml_template):
+        system_mapping = copy.deepcopy(yml_template)
+        for key, item in system_mapping.items():
+            for item_name, item_value in item.items():
+                value_name = key + "_" + item_name
+                item[item_name] = value_name.upper()
+        return system_mapping
+
+    def is_docker_environment(self):
+        return os.environ.get("ENVIRONMENT", "None").lower() == "docker"
+
+    def setup_docker_keywords(self, keywords):
+        """
+           Extends the list of Docker-related keywords with the provided keywords.
+
+           Parameters:
+           - keywords (iterable): An iterable of keywords to add or a str
+
+           Raises:
+           - TypeError: If `keywords` is not an iterable.
+           """
+
+        if isinstance(keywords, str):
+            keywords = [keywords]
+        elif not isinstance(keywords, (list, tuple, set)):
+            raise TypeError("keywords must be a string or an iterable (e.g., list, tuple, set)")
+        self._docker_keywords.extend(keywords)
+
+    def init_conifg_yml(self, merged_yml_template):
+        dump_yml_to_path(self.setting_path, merged_yml_template)
+        msg = "Please fill all the required info at {}".format(self.setting_path)
+        if os.environ.get("ENVIRONMENT", None) == DOCKER_ENVIRONMENT:
+            warnings.warn(msg)
+        else:
+            raise FileNotFoundError(msg)
+
+    def load_config_yml(self, merged_yml_template):
+        cfg = load_yml_from_path(self.setting_path)
+        is_yml_template_updated = self.is_yaml_dict_different(merged_yml_template, cfg)
+        if is_yml_template_updated:
+            new_merged_yaml = self.merge_yml(merged_yml_template, cfg)
+            dump_yml_to_path(self.setting_path, new_merged_yaml)
+            msg = "Config file updated, please fill in the new required info {}".format(self.setting_path)
+            raise ValueError(msg)
+        self.yml_config = load_yml_from_path(self.setting_path)
+        if self.check_value_update:
+            self.find_unchanged_field()
 
     def build_or_load(self):
+        ret_dict = self._build_or_load()
+        if self.is_docker_environment():
+            return self.load_environment_variable(ret_dict)
+        return ret_dict
+
+    def load_environment_variable(self, ret_dict):
+        copy_ret_dict = copy.deepcopy(ret_dict)
+        env_mapping_dict = self.build_sys_value_mapping(ret_dict)
+        for key, value in env_mapping_dict.items():
+            for item_key, mapping_key in value.items():
+                if mapping_key in os.environ:
+                    copy_ret_dict[key][item_key] = os.environ[mapping_key]
+        return copy_ret_dict
+
+    def _build_or_load(self):
         """
-        Check the target yml,
-        if it is ok, load the yml
-        :return:
+        Build the config YML if it not already exist
+        Update the config YML if the template is updated
+        READ the config YML
+        :return: YML in dict
         """
         user_tpl = self.check_user_yml_template()
         default_yml_template = self.load_default_yml_template()
         merged_yml_template = self.merge_yml(default_yml_template, user_tpl)
         try:
             if not os.path.isfile(self.setting_path):
-                dump_yml_to_path(self.setting_path, merged_yml_template)
-                msg = "Please fill all the required info at {}".format(self.setting_path)
-                raise FileNotFoundError(msg)
-            else:
-                cfg = load_yml_from_path(self.setting_path)
-                is_yml_template_updated = self.is_yaml_dict_different(merged_yml_template, cfg)
-                if is_yml_template_updated:
-                    new_merged_yaml = self.merge_yml(merged_yml_template, cfg)
-                    dump_yml_to_path(self.setting_path, new_merged_yaml)
-                    msg = "Config file updated, please fill in the new required info {}".format(self.setting_path)
-                    raise ValueError(msg)
-                self.yml_config = load_yml_from_path(self.setting_path)
-                if self.check_value_update:
-                    self.find_unchanged_field()
-                return self.yml_config
+                self.init_conifg_yml(merged_yml_template)
+            self.load_config_yml(merged_yml_template)
+            return self.yml_config
         except FileNotFoundError as e:
             if self._if_sys_value_contain(merged_yml_template):
                 self.setup_value_from_sys_environment(merged_yml_template)
                 return self.yml_config
             else:
                 raise e
         except ValueError as e:
@@ -81,89 +139,100 @@
 
     def setup_value_from_sys_environment(self, merged_yml_template):
         for name in merged_yml_template:
             merged_yml_template[name] = json.loads(os.environ[name])
         self.yml_config = merged_yml_template
 
     def _if_sys_value_contain(self, merged_yml_template):
-        os_env = os.environ
-        for name in merged_yml_template:
-            if name not in os.environ:
-                return False
-        else:
-            return True
+        os_keys = []
+        for key, item in merged_yml_template.items():
+            for item_name in item:
+                value_name = key + "_" + item_name
+                value_name_upper = value_name.upper()
+                os_keys.append(value_name_upper)
+        if any(x not in os.environ for x in os_keys):
+            return False
+        return True
 
     def _find_unchanged_field(self, target_dict):
         for key, item in target_dict.items():
             if type(item) is dict:
                 self._find_unchanged_field(item)
             else:
-                if type(item) is str:
-                    if key.lower() == item.lower():
-                        self.possible_unchanged_field.append(key)
+                if type(item) is str and key.lower() == item.lower():
+                    self.possible_unchanged_field.append(key)
 
     def find_unchanged_field(self):
         self._find_unchanged_field(self.yml_config)
         if self.possible_unchanged_field:
             msg = "The key and value are the same for fields {} in the config {}. You may need to change these fields from their default values."
             fields = ", ".join(self.possible_unchanged_field)
             msg = msg.format(fields, self.setting_path)
-            raise ValueError("some file didn't change {}".format(msg))
+            warnings.warn("some file didn't change {}".format(msg))
 
     def load_default_yml_template(self):
         tpl_dir_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "template")
         tpl_path = os.path.join(tpl_dir_path, self.default_template_name)
         tpl_yml_dict = load_yml_from_path(tpl_path)
         return tpl_yml_dict
 
-    def merge_yml(self, target_yml, merge_into_yml):
+    def _merge_yml(self, first_yml, second_yml, merged_yml):
+        for default_yml_key, default_yml_value in first_yml.items():
+            # If key in both first and second YML compare the content
+            if default_yml_key in second_yml:
+                for key, item in default_yml_value.items():
+                    # Add the key into final YML if it not already exist in second YML
+                    if key not in second_yml[default_yml_key]:
+                        merged_yml[default_yml_key][key] = item
+            else:
+                # not already in the second YML, copy to the final result
+                merged_yml[default_yml_key] = default_yml_value
+        return merged_yml
+
+    def merge_yml(self, first_yml, second_yml):
         """
-        merge first yml into second yml,
-        if both yml has same value, use value from second yml
-        :param target_yml:
-        :param merge_into_yml:
-        :return:
+        Merge the first YML into second YML
+        There are three case
+        1. First YML exist but second YML doesn't exist
+        2. first, second YML both exist and they are equals
+        3. First YML and second YML both exist but not equal
+            value from second YML is preferable
+        :param first_yml: template YML
+        :param second_yml: configration YML
+        :return: dictionary
         """
-        merged_yml = copy.deepcopy(merge_into_yml)
+        # Use second yml as base
+        merged_yml = copy.deepcopy(second_yml)
         if merged_yml:
-            for default_yml_key, default_yml_value in target_yml.items():
-                if default_yml_key in merge_into_yml:
-                    for key, item in default_yml_value.items():
-                        if key not in merge_into_yml[default_yml_key]:
-                            merged_yml[default_yml_key][key] = item
-                else:
-                    merged_yml[default_yml_key] = default_yml_value
+            return self._merge_yml(first_yml, second_yml, merged_yml)
         else:
-            return target_yml
-        return merged_yml
+            return first_yml
 
     def is_yaml_dict_different(self, yml1, yml2):
         """
         Compare two yaml dict to see if the yaml structure is difference (compare key only)
         :param yml1:
         :param yml2:
         :return: True for is different and False means it is same
         """
-        DIFFERENT = True
-        SAME = False
-        difference = SAME
+        different = True
+        same = False
         if type(yml1) is not dict and type(yml2) is not dict:
-            return SAME
+            return same
         elif type(yml1) is dict and type(yml2) is dict:
             for key, value in yml1.items():
                 if key in yml2:
                     difference = self.is_yaml_dict_different(value, yml2[key])
                 else:
-                    difference = DIFFERENT
-                if difference is DIFFERENT:
-                    return DIFFERENT
-            else:
-                return SAME
+                    difference = different
+                if difference is different:
+                    return different
+            return same
         else:
-            difference = DIFFERENT
+            difference = different
             return difference
 
     def compare_and_merge_yamls(self, tpl_yml, target_yml):
         difference = False
         for tpl_key, tpl_value in tpl_yml.items():
             if target_yml and tpl_key in target_yml:
                 target_value = target_yml[tpl_key]
@@ -184,15 +253,16 @@
         if os.path.isfile(self.template_path):
             user_yml_template_obj = load_yml_from_path(self.template_path)
             return user_yml_template_obj
         else:
             msg = 'User Setting Yml template {} does not exist'.format(self.template_path)
             raise FileNotFoundError(msg)
 
-    def _exam_the_value(selfm, section, res):
+    @staticmethod
+    def _exam_the_value(section, res):
         for key, value in res.items():
             if not value:
                 msg = "Please fill info for {} {}:".format(section, key)
                 raise ValueError(msg)
 
 
 def read_file_as_str(file_path):
```

### Comparing `ceotr_config-1.0.6/setup.py` & `ceotr_config-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import platform
 import os
 from setuptools import setup, find_packages
 
 path_to_my_project = os.path.dirname(__file__)  # Do any sort of fancy resolving of the path here if you need to
 
 
 install_requires = [
     "PyYAML",
+      "python-dotenv"
 ]
 packages = find_packages(exclude=['tests'])
 
 setup(name='ceotr_config',
-      version='1.0.6',
+      version='1.0.8',
       description="Common python library for CEOTR data team",
       author="CEOTR",
       author_email="support@ceotr.ca",
       url="https://gitlab.oceantrack.org/ceotr-public/ceotr_app_common/ceotr_config",
       packages=packages,
       include_package_data=True,
       license="GNU General Public License v3 (GPLv3)",
```

