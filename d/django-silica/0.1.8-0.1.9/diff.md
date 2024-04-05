# Comparing `tmp/django_silica-0.1.8.tar.gz` & `tmp/django_silica-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_silica-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_silica-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_silica-0.1.8.tar` & `django_silica-0.1.9.tar`

### file list

```diff
@@ -1,59 +1,67 @@
--rw-r--r--   0        0        0     1064 2023-10-18 13:09:27.731058 django_silica-0.1.8/LICENSE
--rw-r--r--   0        0        0       33 2023-10-18 13:09:27.731058 django_silica-0.1.8/MANIFEST.in
--rw-r--r--   0        0        0       72 2023-10-18 13:09:27.731058 django_silica-0.1.8/README.md
--rw-r--r--   0        0        0      661 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/EventManager.py
--rw-r--r--   0        0        0    12816 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/SilicaComponent.py
--rw-r--r--   0        0        0     2644 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/SilicaTemplateResponse.py
--rw-r--r--   0        0        0        0 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/__init__.py
--rw-r--r--   0        0        0     4609 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/call_method_parser.py
--rw-r--r--   0        0        0     2047 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/concerns/Paginator.py
--rw-r--r--   0        0        0      591 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/errors.py
--rw-r--r--   0        0        0     1114 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/inline_template_loader.py
--rw-r--r--   0        0        0     6328 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/mixins/ValidatesProperties.py
--rw-r--r--   0        0        0    11979 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/static/morphdom.js
--rw-r--r--   0        0        0    15125 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/static/silica.js
--rw-r--r--   0        0        0        0 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/templates/index.html
--rw-r--r--   0        0        0       99 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/templates/tag_props.html
--rw-r--r--   0        0        0        0 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/templatetags/__init__.py
--rw-r--r--   0        0        0     4290 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/templatetags/silica.py
--rw-r--r--   0        0        0      496 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/templatetags/silica_scripts.py
--rw-r--r--   0        0        0     5846 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/SilicaTestCase.py
--rw-r--r--   0        0        0        0 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/__init__.py
--rw-r--r--   0        0        0      372 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/CacheOps.py
--rw-r--r--   0        0        0      752 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/ChildComponent.py
--rw-r--r--   0        0        0      711 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/ConcurrencyTest.py
--rw-r--r--   0        0        0      335 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/EventReceiver.py
--rw-r--r--   0        0        0      327 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/EventSender.py
--rw-r--r--   0        0        0      198 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/InlineTemplate.py
--rw-r--r--   0        0        0      223 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/JsCalls.py
--rw-r--r--   0        0        0      576 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/Lazy.py
--rw-r--r--   0        0        0     1022 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/Lifecycle.py
--rw-r--r--   0        0        0      448 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/Methods.py
--rw-r--r--   0        0        0      637 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/ParentComponent.py
--rw-r--r--   0        0        0      207 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/Properties.py
--rw-r--r--   0        0        0      369 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/Redirect.py
--rw-r--r--   0        0        0      488 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/TagProps.py
--rw-r--r--   0        0        0        0 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/components/__init__.py
--rw-r--r--   0        0        0      145 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/templates/concurrency_test_view.html
--rw-r--r--   0        0        0       99 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/templates/tag_props_view.html
--rw-r--r--   0        0        0      395 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_cache_expiry.py
--rw-r--r--   0        0        0     2982 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_events.py
--rw-r--r--   0        0        0      569 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_inline_template.py
--rw-r--r--   0        0        0      341 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_js_calls.py
--rw-r--r--   0        0        0     1748 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_lazy_loading.py
--rw-r--r--   0        0        0     1261 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_lifecycle_hooks.py
--rw-r--r--   0        0        0      655 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_methods.py
--rw-r--r--   0        0        0     2993 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_ops.py
--rw-r--r--   0        0        0        4 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_pagination.py
--rw-r--r--   0        0        0      452 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_properties.py
--rw-r--r--   0        0        0      907 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_query_params.py
--rw-r--r--   0        0        0      387 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_redirect.py
--rw-r--r--   0        0        0     2408 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_request_concurrency.py
--rw-r--r--   0        0        0      659 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_tag_props.py
--rw-r--r--   0        0        0      159 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/test_validation.py
--rw-r--r--   0        0        0      695 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/tests/urls.py
--rw-r--r--   0        0        0     1028 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/urls.py
--rw-r--r--   0        0        0    10010 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/utils.py
--rw-r--r--   0        0        0     1861 2023-10-18 13:09:28.083062 django_silica-0.1.8/django_silica/views/__init__.py
--rw-r--r--   0        0        0     1441 2023-10-18 13:09:27.731058 django_silica-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 django_silica-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-10-23 11:26:06.641934 django_silica-0.1.9/LICENSE
+-rw-r--r--   0        0        0       33 2023-10-23 11:26:06.641934 django_silica-0.1.9/MANIFEST.in
+-rw-r--r--   0        0        0       72 2023-10-23 11:26:06.641934 django_silica-0.1.9/README.md
+-rw-r--r--   0        0        0      661 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/EventManager.py
+-rw-r--r--   0        0        0    14549 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/SilicaComponent.py
+-rw-r--r--   0        0        0     2644 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/SilicaTemplateResponse.py
+-rw-r--r--   0        0        0        0 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/__init__.py
+-rw-r--r--   0        0        0     4609 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/call_method_parser.py
+-rw-r--r--   0        0        0     2047 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/concerns/Paginator.py
+-rw-r--r--   0        0        0      591 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/errors.py
+-rw-r--r--   0        0        0     1114 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/inline_template_loader.py
+-rw-r--r--   0        0        0        0 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/management/commands/__init__.py
+-rw-r--r--   0        0        0     2326 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/management/commands/silica_create.py
+-rw-r--r--   0        0        0     6328 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/mixins/ValidatesProperties.py
+-rw-r--r--   0        0        0      247 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/ShortName.py
+-rw-r--r--   0        0        0        0 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/__init__.py
+-rw-r--r--   0        0        0      372 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/CacheOps.py
+-rw-r--r--   0        0        0      752 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/ChildComponent.py
+-rw-r--r--   0        0        0      711 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/ConcurrencyTest.py
+-rw-r--r--   0        0        0      335 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/EventReceiver.py
+-rw-r--r--   0        0        0      327 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/EventSender.py
+-rw-r--r--   0        0        0      198 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/InlineTemplate.py
+-rw-r--r--   0        0        0      223 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/JsCalls.py
+-rw-r--r--   0        0        0      576 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/Lazy.py
+-rw-r--r--   0        0        0     1022 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/Lifecycle.py
+-rw-r--r--   0        0        0      448 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/Methods.py
+-rw-r--r--   0        0        0      587 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/ParentComponent.py
+-rw-r--r--   0        0        0      207 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/Properties.py
+-rw-r--r--   0        0        0      369 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/Redirect.py
+-rw-r--r--   0        0        0      488 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/TagProps.py
+-rw-r--r--   0        0        0        0 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/__init__.py
+-rw-r--r--   0        0        0      248 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/subfolder/ComponentInSubfolder.py
+-rw-r--r--   0        0        0        0 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/silica/tests/subfolder/__init__.py
+-rw-r--r--   0        0        0    11979 2023-10-23 11:26:06.969934 django_silica-0.1.9/django_silica/static/morphdom.js
+-rw-r--r--   0        0        0    15125 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/static/silica.js
+-rw-r--r--   0        0        0        0 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/templatetags/__init__.py
+-rw-r--r--   0        0        0     4290 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/templatetags/silica.py
+-rw-r--r--   0        0        0      496 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/templatetags/silica_scripts.py
+-rw-r--r--   0        0        0     5847 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/SilicaTestCase.py
+-rw-r--r--   0        0        0        0 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/__init__.py
+-rw-r--r--   0        0        0       71 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/templates/component_subfolder_test.html
+-rw-r--r--   0        0        0       44 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/templates/component_tag_test.html
+-rw-r--r--   0        0        0      104 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/templates/concurrency_test_view.html
+-rw-r--r--   0        0        0       65 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/templates/tag_props_view.html
+-rw-r--r--   0        0        0      395 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_cache_expiry.py
+-rw-r--r--   0        0        0      801 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_component_tag.py
+-rw-r--r--   0        0        0     2982 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_events.py
+-rw-r--r--   0        0        0      565 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_inline_template.py
+-rw-r--r--   0        0        0      337 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_js_calls.py
+-rw-r--r--   0        0        0     1748 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_lazy_loading.py
+-rw-r--r--   0        0        0     1257 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_lifecycle_hooks.py
+-rw-r--r--   0        0        0      651 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_methods.py
+-rw-r--r--   0        0        0     2887 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_ops.py
+-rw-r--r--   0        0        0        4 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_pagination.py
+-rw-r--r--   0        0        0      448 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_properties.py
+-rw-r--r--   0        0        0      907 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_query_params.py
+-rw-r--r--   0        0        0      383 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_redirect.py
+-rw-r--r--   0        0        0     2404 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_request_concurrency.py
+-rw-r--r--   0        0        0      655 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_tag_props.py
+-rw-r--r--   0        0        0      159 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/test_validation.py
+-rw-r--r--   0        0        0     1023 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/tests/urls.py
+-rw-r--r--   0        0        0     1024 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/urls.py
+-rw-r--r--   0        0        0    10010 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/utils.py
+-rw-r--r--   0        0        0     1861 2023-10-23 11:26:06.973934 django_silica-0.1.9/django_silica/views/__init__.py
+-rw-r--r--   0        0        0     1441 2023-10-23 11:26:06.641934 django_silica-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 django_silica-0.1.9/PKG-INFO
```

### Comparing `django_silica-0.1.8/LICENSE` & `django_silica-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/EventManager.py` & `django_silica-0.1.9/django_silica/EventManager.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/SilicaComponent.py` & `django_silica-0.1.9/django_silica/SilicaComponent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+import importlib
 import json
 import re
+from abc import abstractmethod
 from typing import Dict, Any
-
 import shortuuid
+
+from django.apps import apps
 from django.core.cache import cache
 from django.http import HttpRequest
 from django.template.loader import render_to_string
-from django.utils.decorators import classonlymethod
 from django.utils.module_loading import import_string
+from django.utils.decorators import classonlymethod
 from django.views.generic import TemplateView
 
 from django_silica.SilicaTemplateResponse import SilicaTemplateResponse
 from django_silica.mixins.ValidatesProperties import ValidatesProperties
 from django_silica.utils import pascal_to_snake
-from django_silica.EventManager import EventManager
 
 
 class SilicaComponent(TemplateView, ValidatesProperties):
     component_id: str = ""
     component_name: str = ""
     query_params: dict = {}
     has_rendered: bool = False
@@ -71,17 +73,19 @@
 
         if inline_template := self.inline_template():
             self.template_name = f"::silica-inline::{inline_template}"
             return
 
         self.template_name = f"silica/{self.get_template_name()}"
 
+    # abstract
     def inline_template(self):
         pass
 
+    # abstract
     def inline_placeholder(self):
         pass
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context["component_id"] = self.component_id
 
@@ -189,15 +193,17 @@
     ) -> "SilicaComponent":
 
         if "lazy" in kwargs:
             lazy = kwargs["lazy"]
         else:
             lazy = False
 
-        ComponentClass = import_string(component_name)
+        ComponentClass = SilicaComponent.get_component_class_from_name(component_name)
+
+        # ComponentClass = import_string(component_name)
         component_instance = ComponentClass(
             component_id=component_id,
             component_name=component_name,
             lazy=lazy,
         )
         component_instance._set_state_from_cache()
         component_instance.js_calls = []
@@ -221,19 +227,14 @@
     def render_to_string(self):
         template_name = f"silica/{self.get_template_name()}"
         return render_to_string(template_name, self.get_context_data())
 
     def reset_js_calls(self):
         self.js_calls = []
 
-    # def get_template_names(self):
-    #     # Return the inline template as if it was a template name
-    #     # Our custom loader will handle it properly
-    #     return ["Hello, {{ name }}!"]
-
     def dispatch(self, request, *args, **kwargs):
         """
         Called by the `as_view` class method when utilizing a component directly as a view.
         """
 
         # how to provide request in kwargs to mount()?
         self.request = request
@@ -386,14 +387,24 @@
     def get_absolute_path(self):
         module_name = (
             self.__module__
         )  # gives the module name in which the class is defined
         class_name = self.__class__.__name__  # gives the name of the class
         return f"{module_name}.{class_name}"
 
+    def get_component_path(self):
+        absolute_path = self.get_absolute_path()
+        if ".silica." in absolute_path:
+            return absolute_path.split(".silica.", 1)[1].rsplit(".", 1)[0]
+        else:
+            # Handle this case accordingly.
+            # You can return the original string or a placeholder/error message.
+            return absolute_path
+
+
     # Hooks
     def mount(self):
         pass
 
     def rendered(self, html):
         """
         Hook that gets called after the component has been rendered.
@@ -415,9 +426,41 @@
     def _is_jsonable(self, x):
         try:
             json.dumps(x)
             return True
         except (TypeError, OverflowError):
             return False
 
+
+    @staticmethod
+    def get_component_class_from_name(component_name: str):
+        for app in apps.get_app_configs():
+
+            # Attempt to load the 'silica' module from each app
+            try:
+                silica_module = importlib.import_module(f"{app.name}.silica.{component_name}")
+
+                # class_name will always be the last portion of the path, the last part of the string after the last dot, dots may not exist
+                class_name = component_name.split(".")[-1]
+
+                # If we don't encounter an ImportError, try to get the component
+                component_class = getattr(silica_module, class_name, None)
+                if component_class:
+                    # If found, use it (or return, or whatever your logic is)
+                    return component_class
+            except ImportError:
+                continue
+
+        # finally, try and import the component_name itself if it's a direct path to a component
+        try:
+            component_class = import_string(component_name)
+            if component_class:
+                # If found, use it (or return, or whatever your logic is)
+                return component_class
+        except ImportError:
+            pass
+
+        # If the component wasn't found in any app's 'silica' module, raise an error
+        raise ImportError(f"Component {component_name} not found in any app's 'silica' module")
+
     def __repr__(self):
         return f"ComponentRequest(name='{self.component_name}' id='{self.component_id}'"
```

### Comparing `django_silica-0.1.8/django_silica/SilicaTemplateResponse.py` & `django_silica-0.1.9/django_silica/SilicaTemplateResponse.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/call_method_parser.py` & `django_silica-0.1.9/django_silica/call_method_parser.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/concerns/Paginator.py` & `django_silica-0.1.9/django_silica/concerns/Paginator.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/errors.py` & `django_silica-0.1.9/django_silica/errors.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/inline_template_loader.py` & `django_silica-0.1.9/django_silica/inline_template_loader.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/mixins/ValidatesProperties.py` & `django_silica-0.1.9/django_silica/mixins/ValidatesProperties.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/static/morphdom.js` & `django_silica-0.1.9/django_silica/static/morphdom.js`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/static/silica.js` & `django_silica-0.1.9/django_silica/static/silica.js`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/templatetags/silica.py` & `django_silica-0.1.9/django_silica/templatetags/silica.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/tests/SilicaTestCase.py` & `django_silica-0.1.9/django_silica/tests/SilicaTestCase.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         return self
 
     def _send_message(self, actions: List):
         # prepare request
         data = json.dumps(
             {
                 "id": self.component.component_id,
-                "name": self.component.get_absolute_path(),
+                "name": self.component.get_component_path(),
                 "actions": actions,
             }
         )
 
         factory = RequestFactory()
         request = factory.post(
             "/silica/message", data, content_type="application/json"
```

### Comparing `django_silica-0.1.8/django_silica/tests/components/ChildComponent.py` & `django_silica-0.1.9/django_silica/silica/tests/ChildComponent.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/tests/components/ConcurrencyTest.py` & `django_silica-0.1.9/django_silica/silica/tests/ConcurrencyTest.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/tests/components/Lazy.py` & `django_silica-0.1.9/django_silica/silica/tests/Lazy.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/tests/components/Lifecycle.py` & `django_silica-0.1.9/django_silica/silica/tests/Lifecycle.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/tests/components/ParentComponent.py` & `django_silica-0.1.9/django_silica/silica/tests/ParentComponent.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,11 +7,11 @@
             <div class="p-5 border m-5">
                 {% load silica %}
                 
                 <div class="text-sm text-gray-500">silica id: {{ component_id }}</div>
                 
                 <p>I'm a parent!</p>
                 
-                <div>{% silica "django_silica.tests.components.ChildComponent.ChildComponent" %}</div>
-                <div>{% silica "django_silica.tests.components.ChildComponent.ChildComponent" %}</div>
+                <div>{% silica "tests.ChildComponent.ChildComponent" %}</div>
+                <div>{% silica "tests.ChildComponent.ChildComponent" %}</div>
             </div>
         """
```

### Comparing `django_silica-0.1.8/django_silica/tests/test_events.py` & `django_silica-0.1.9/django_silica/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/tests/test_inline_template.py` & `django_silica-0.1.9/django_silica/tests/test_inline_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django_silica.tests.SilicaTestCase import SilicaTestCase, SilicaTest
-from django_silica.tests.components.InlineTemplate import InlineTemplate
+from django_silica.silica.tests.InlineTemplate import InlineTemplate
 
 
 class LifecycleTestCase(SilicaTestCase):
     def test_inline_template_is_rendered(self):
         SilicaTest(component=InlineTemplate).assertSee("Hello World!")
 
     def test_subsequent_requests_render_from_inline_template(self):
```

### Comparing `django_silica-0.1.8/django_silica/tests/test_lazy_loading.py` & `django_silica-0.1.9/django_silica/tests/test_lazy_loading.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/tests/test_lifecycle_hooks.py` & `django_silica-0.1.9/django_silica/tests/test_lifecycle_hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.test import RequestFactory, Client
 
 from django_silica.tests.SilicaTestCase import SilicaTestCase, SilicaTest
-from django_silica.tests.components.Lifecycle import Lifecycle
+from django_silica.silica.tests.Lifecycle import Lifecycle
 
 
 class LifecycleTestCase(SilicaTestCase):
     def setUp(self):
         self.factory = RequestFactory()
         self.client = Client()
```

### Comparing `django_silica-0.1.8/django_silica/tests/test_methods.py` & `django_silica-0.1.9/django_silica/tests/test_methods.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django_silica.tests.SilicaTestCase import SilicaTestCase, SilicaTest
-from django_silica.tests.components.Methods import Methods
+from django_silica.silica.tests.Methods import Methods
 
 
 class MethodsTestCase(SilicaTestCase):
     def test_method_calling_without_args(self):
         (
             SilicaTest(component=Methods)
             .assertSet("fruit", "banana")
```

### Comparing `django_silica-0.1.8/django_silica/tests/test_ops.py` & `django_silica-0.1.9/django_silica/tests/test_ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 
 from django.core.cache import cache
 from django.contrib.auth.models import AnonymousUser
 from django.test import RequestFactory, Client
 
 from django_silica.tests.SilicaTestCase import SilicaTestCase
-from django_silica.tests.components.CacheOps import CacheOps
+from django_silica.silica.tests.CacheOps import CacheOps
 
 class OpsTestCase(SilicaTestCase):
     def setUp(self):
         self.client = Client()
 
     def test_can_see_cached_property(self):
         request = RequestFactory().get("/")
@@ -22,15 +22,15 @@
         cache.set(f"silica:component:{component_id}", {"first_name": "James"})
 
         response = self.client.post(
             "/silica/message",
             json.dumps(
                 {
                     "id": component_id,
-                    "name": "django_silica.tests.components.CacheOps.CacheOps",
+                    "name": "tests.CacheOps",
                 }
             ),
             content_type="application/json",
         )
 
         self.assertContains(response, "James")
 
@@ -46,29 +46,29 @@
 
         # Simulate a /message request
         response = self.client.post(
             "/silica/message",
             json.dumps(
                 {
                     "id": component_id,
-                    "name": "django_silica.tests.components.CacheOps.CacheOps",
+                    "name": "tests.CacheOps",
                 }
             ),
             content_type="application/json",
         )
 
         self.assertContains(response, "James")
 
         # A subsequent request to /message should return the same state
         response = self.client.post(
             "/silica/message",
             json.dumps(
                 {
                     "id": component_id,
-                    "name": "django_silica.tests.components.CacheOps.CacheOps",
+                    "name": "tests.CacheOps",
                 }
             ),
             content_type="application/json",
         )
 
         self.assertContains(response, "James")
```

### Comparing `django_silica-0.1.8/django_silica/tests/test_query_params.py` & `django_silica-0.1.9/django_silica/tests/test_query_params.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/tests/test_request_concurrency.py` & `django_silica-0.1.9/django_silica/tests/test_request_concurrency.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.contrib.staticfiles.testing import StaticLiveServerTestCase
 from django.urls import path
 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 
 from django_silica.tests.SilicaTestCase import SilicaStaticLiveServerTestCase
-from django_silica.tests.components.ConcurrencyTest import ConcurrencyTest
+from django_silica.silica.tests.ConcurrencyTest import ConcurrencyTest
 from django_silica.urls import urlpatterns as silica_urlpatterns
 
 urlpatterns = silica_urlpatterns + [
     path("silica/tests/concurrency", ConcurrencyTest.as_view()),
 ]
 
 class ConcurrencyTestCase(SilicaStaticLiveServerTestCase):
```

### Comparing `django_silica-0.1.8/django_silica/tests/test_tag_props.py` & `django_silica-0.1.9/django_silica/tests/test_tag_props.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.test import TestCase, RequestFactory, Client, override_settings
 
 from django_silica.tests.SilicaTestCase import SilicaTest, SilicaTestCase
-from django_silica.tests.components.TagProps import TagProps
+from django_silica.silica.tests.TagProps import TagProps
 
 
 class TestTagProps(SilicaTestCase):
     def test_props_can_be_set_programmatically(self):
         (
             SilicaTest(component=TagProps, bool_val=None)
             .assertSet("bool_val", None)
```

### Comparing `django_silica-0.1.8/django_silica/urls.py` & `django_silica-0.1.9/django_silica/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.views.generic import TemplateView
 from django.urls import include, path
 
-from django_silica.tests.components.ConcurrencyTest import ConcurrencyTest
+from django_silica.silica.tests.ConcurrencyTest import ConcurrencyTest
 from django_silica.views import message
 
 
 class TestView(TemplateView):
     template_name = "tag_props.html"
```

### Comparing `django_silica-0.1.8/django_silica/utils.py` & `django_silica-0.1.9/django_silica/utils.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/django_silica/views/__init__.py` & `django_silica-0.1.9/django_silica/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django_silica-0.1.8/pyproject.toml` & `django_silica-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "django-silica"
 description = "A reusable Django app for Silica functionalities."
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{ name = "Dyvenia" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Framework :: Django",
@@ -19,15 +19,15 @@
     "selenium~=4.13.0",
     "chromedriver-py~=117.0.5938.92",
     "webdriver-manager~=4.0.1"
 ]
 
 [tool.poetry]
 name = "django-silica"
-version = "0.1.8"
+version = "0.1.9"
 description = "A fullstack HTML over the wire framework for Django."
 authors = ["Will Abbott <wabbott@dyvenia.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Django = "^4.0"
 shortuuid = "~1.0.11"
```

### Comparing `django_silica-0.1.8/PKG-INFO` & `django_silica-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silica
-Version: 0.1.8
+Version: 0.1.9
 Summary: A reusable Django app for Silica functionalities.
 Keywords: django,silica,reusable,app
 Author: Dyvenia
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

