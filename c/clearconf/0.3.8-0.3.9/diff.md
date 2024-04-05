# Comparing `tmp/clearconf-0.3.8.tar.gz` & `tmp/clearconf-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearconf-0.3.8.tar", max compression
+gzip compressed data, was "clearconf-0.3.9.tar", max compression
```

## Comparing `clearconf-0.3.8.tar` & `clearconf-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.8/README.md
--rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/assets/example_conf.py
--rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/assets/init.py
--rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/assets/stub_conf.py
--rw-r--r--   0        0        0     7795 2023-07-26 20:51:47.448711 clearconf-0.3.8/clearconf/base_config.py
--rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/cli/__init__.py
--rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/cli/defaults.py
--rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/cli/main.py
--rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/utils/conf.py
--rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/utils/file.py
--rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.8/clearconf/utils/stdout.py
--rw-r--r--   0        0        0      729 2023-07-26 20:51:16.200246 clearconf-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 clearconf-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.9/README.md
+-rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/assets/example_conf.py
+-rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/assets/init.py
+-rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/assets/stub_conf.py
+-rw-r--r--   0        0        0     7912 2023-07-26 21:21:16.669769 clearconf-0.3.9/clearconf/base_config.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/cli/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/cli/defaults.py
+-rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/utils/conf.py
+-rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/utils/file.py
+-rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.9/clearconf/utils/stdout.py
+-rw-r--r--   0        0        0      729 2023-07-26 21:21:31.005918 clearconf-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 clearconf-0.3.9/PKG-INFO
```

### Comparing `clearconf-0.3.8/README.md` & `clearconf-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.8/clearconf/assets/example_conf.py` & `clearconf-0.3.9/clearconf/assets/example_conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.8/clearconf/assets/init.py` & `clearconf-0.3.9/clearconf/assets/init.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.8/clearconf/base_config.py` & `clearconf-0.3.9/clearconf/base_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         for attr in [a for a in target.mro() 
                      if a.__name__ not in [target.__name__, f'{target.__name__}_mod', target.__name__[:-4], 'BaseConfig', 'Config', 'object']]:
             # The allows inheritance between configs but I guess there are better solutions
             if 'configs' not in attr.__module__:
                 target_attr = target_attr - set(dir(attr))
 
         for k in target_attr:
-            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
+            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg', 'parent']:
                 attr = getattr(target, k)
 
                 # If it's a module get inside
                 if hasattr(attr, '__module__'):
 
                     # If it's a class inside config, get inside it,
                     # else just log module and name in the dict as a string.
@@ -90,29 +90,30 @@
     @classmethod
     def _subclass(cls):
 
         target = cls
 
         res = {}
         for k in dir(target):
-            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
+            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg', 'parent']:
                 attr = getattr(target, k)
                 # If it's a class inside config, get inside it,
                 # else just log module and name in the dict as a string
                 if hasattr(attr, '__module__') and type(attr).__name__ != 'function':
 
                     # if we are executing the config the module is __main__. If we are importing it is config
                     # Not ideal but config could be anywhere in the name
                     # Need to find a better way to do this
                     if attr.__module__.split('.')[0] == '__main__' or 'config' in attr.__module__:
                         # This way the module keeps its subclasses but it is also subclassed by
                         # BaseConfig inheriting its method. A security check could be used to assure
                         # that the new methods are not overriding any old one.
                         if 'BaseConfig' not in [a.__name__ for a in attr.mro()]:
                             setattr(target, k, type(f'{k}_mod', (BaseConfig, ) + tuple(attr.__mro__), dict(list(dict(vars(BaseConfig)).items()) + list(dict(vars(attr)).items()))))
+                            setattr((getattr(target, k)), 'parent', target)
         return res
 
     @classmethod
     def to_flat_dict(cls) -> dict:
         import torch
         res = cls.to_dict()
         res = flatten(res)
@@ -120,15 +121,15 @@
 
     @classmethod
     def to_list(cls):
         target = cls
 
         res = []
         for k in dir(target):
-            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
+            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg', 'parent']:
                 attr = getattr(target, k)
                 # If it's a class inside config, get inside it,
                 # else just log module and name in the dict as a string
                 if type(attr) == type:
                     if attr.__module__.split('.')[0] in ['configs', '__main__']:
                         res.append(attr.to_list())
                     else:
@@ -150,15 +151,15 @@
         for attr in [a for a in target.mro() 
                      if a.__name__ not in [target.__name__, f'{target.__name__}_mod', target.__name__[:-4], 'BaseConfig', 'Config', 'object']]:
             # The allows inheritance between configs but I guess there are better solutions
             if 'configs' not in attr.__module__:
                 target_attr = target_attr - set(dir(attr))
         
         for k in target_attr:
-            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
+            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg', 'parent']:
                 attr = getattr(target, k)
                 setattr(self, k, attr)
     
     def __getattribute__(self, item):
         return object.__getattribute__(self, item)
```

### Comparing `clearconf-0.3.8/clearconf/cli/defaults.py` & `clearconf-0.3.9/clearconf/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.8/clearconf/cli/main.py` & `clearconf-0.3.9/clearconf/cli/main.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.8/clearconf/utils/conf.py` & `clearconf-0.3.9/clearconf/utils/conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.8/clearconf/utils/file.py` & `clearconf-0.3.9/clearconf/utils/file.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.8/pyproject.toml` & `clearconf-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clearconf"
-version = "0.3.8"
+version = "0.3.9"
 description = "ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class."
 authors = ["Andrea Rosasco <andrearosasco.ar@gmail.com>"]
 homepage = "https://github.com/andrearosasco/clearconf"
 repository = "https://github.com/andrearosasco/clearconf"
 readme = "README.md"
```

### Comparing `clearconf-0.3.8/PKG-INFO` & `clearconf-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearconf
-Version: 0.3.8
+Version: 0.3.9
 Summary: ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class.
 Home-page: https://github.com/andrearosasco/clearconf
 Author: Andrea Rosasco
 Author-email: andrearosasco.ar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

