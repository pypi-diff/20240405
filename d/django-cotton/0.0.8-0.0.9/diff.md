# Comparing `tmp/django_cotton-0.0.8.tar.gz` & `tmp/django_cotton-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cotton-0.0.8.tar", max compression
+gzip compressed data, was "django_cotton-0.0.9.tar", max compression
```

## Comparing `django_cotton-0.0.8.tar` & `django_cotton-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2024-04-04 12:43:29.400761 django_cotton-0.0.8/LICENSE
--rw-r--r--   0        0        0      194 2024-04-04 12:43:29.400761 django_cotton-0.0.8/README.md
--rw-r--r--   0        0        0       40 2024-04-04 12:43:29.400761 django_cotton-0.0.8/django_cotton/__init__.py
--rw-r--r--   0        0        0     2356 2024-04-04 12:43:29.400761 django_cotton-0.0.8/django_cotton/apps.py
--rwxr-xr-x   0        0        0    12697 2024-04-04 12:43:29.400761 django_cotton-0.0.8/django_cotton/cotton_loader.py
--rw-r--r--   0        0        0        0 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/__init__.py
--rw-r--r--   0        0        0     1924 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/_component.py
--rw-r--r--   0        0        0     1362 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/_props.py
--rw-r--r--   0        0        0     2525 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/_props_frame.py
--rw-r--r--   0        0        0     1686 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/_slot.py
--rw-r--r--   0        0        0      996 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/templatetags/cotton.py
--rw-r--r--   0        0        0     1701 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/urls.py
--rw-r--r--   0        0        0      786 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/views.py
--rw-r--r--   0        0        0      405 2024-04-04 12:43:29.404761 django_cotton-0.0.8/django_cotton/wsgi.py
--rw-r--r--   0        0        0     1233 2024-04-04 12:43:33.184802 django_cotton-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 django_cotton-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-05 11:26:15.642376 django_cotton-0.0.9/LICENSE
+-rw-r--r--   0        0        0      194 2024-04-05 11:26:15.642376 django_cotton-0.0.9/README.md
+-rw-r--r--   0        0        0       40 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/__init__.py
+-rw-r--r--   0        0        0     2356 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/apps.py
+-rwxr-xr-x   0        0        0    11629 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/cotton_loader.py
+-rw-r--r--   0        0        0        0 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/templatetags/__init__.py
+-rw-r--r--   0        0        0     2318 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/templatetags/_component.py
+-rw-r--r--   0        0        0     1362 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/templatetags/_props.py
+-rw-r--r--   0        0        0     2580 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/templatetags/_props_frame.py
+-rw-r--r--   0        0        0     1686 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/templatetags/_slot.py
+-rw-r--r--   0        0        0      996 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/templatetags/cotton.py
+-rw-r--r--   0        0        0     1765 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/urls.py
+-rw-r--r--   0        0        0      935 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/views.py
+-rw-r--r--   0        0        0      405 2024-04-05 11:26:15.642376 django_cotton-0.0.9/django_cotton/wsgi.py
+-rw-r--r--   0        0        0     1233 2024-04-05 11:26:17.058391 django_cotton-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 django_cotton-0.0.9/PKG-INFO
```

### Comparing `django_cotton-0.0.8/LICENSE` & `django_cotton-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cotton-0.0.8/django_cotton/apps.py` & `django_cotton-0.0.9/django_cotton/apps.py`

 * *Files identical despite different names*

### Comparing `django_cotton-0.0.8/django_cotton/cotton_loader.py` & `django_cotton-0.0.9/django_cotton/cotton_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from django.template import Template
 from django.core.cache import cache
 from django.template import Origin
 from django.conf import settings
 
 from bs4 import BeautifulSoup, MarkupResemblesLocatorWarning
 
-
 warnings.filterwarnings("ignore", category=MarkupResemblesLocatorWarning)
 
 
 class Loader(BaseLoader):
     is_usable = True
 
     def __init__(self, engine, dirs=None):
@@ -27,45 +26,14 @@
         self.dirs = dirs
         self.django_syntax_placeholders = []
 
     def get_template_from_string(self, template_string):
         """Create and return a Template object from a string. Used primarily for testing."""
         return Template(template_string, engine=self.engine)
 
-    def get_template(self, template_name, skip=None):
-        """
-        Call self.get_template_sources() and re
-        turn a Template object for
-        the first template matching template_name. If skip is provided, ignore
-        template origins in skip. This is used to avoid recursion during
-        template extending.
-        """
-
-        tried = []
-
-        for origin in self.get_template_sources(template_name):
-            if skip is not None and origin in skip:
-                tried.append((origin, "Skipped to avoid recursion"))
-                continue
-
-            try:
-                contents = self.get_contents(origin)
-            except TemplateDoesNotExist:
-                tried.append((origin, "Source does not exist"))
-                continue
-            else:
-                return Template(
-                    contents,
-                    origin,
-                    origin.template_name,
-                    self.engine,
-                )
-
-        raise TemplateDoesNotExist(template_name, tried=tried)
-
     def get_contents(self, origin):
         # check if file exists, whilst getting the mtime for cache key
         try:
             mtime = os.path.getmtime(origin.name)
         except FileNotFoundError:
             raise TemplateDoesNotExist(origin)
 
@@ -118,21 +86,21 @@
             content,
             flags=re.DOTALL,
         )
 
         content = re.sub(
             r"\{%.*?%\}",
             lambda x: self.django_syntax_placeholders.append(x.group(0))
-            or f"__django_syntax__{len(self.django_syntax_placeholders)}__",
+                      or f"__django_syntax__{len(self.django_syntax_placeholders)}__",
             content,
         )
         content = re.sub(
             r"\{\{.*?\}\}",
             lambda x: self.django_syntax_placeholders.append(x.group(0))
-            or f"__django_syntax__{len(self.django_syntax_placeholders)}__",
+                      or f"__django_syntax__{len(self.django_syntax_placeholders)}__",
             content,
         )
 
         return content
 
     def _replace_placeholders_with_syntax(self, content):
         """After modifying the content, replace the placeholders with the django template tags and variables."""
@@ -280,18 +248,16 @@
                 opening_tag += ' {}="{}"'.format(attr, value)
             opening_tag += " %}"
 
             # Construct the closing tag
             closing_tag = "{% end_cotton_component %}"
 
             if tag.contents:
-                component_key = component_name
-
                 tag_soup = BeautifulSoup(tag.decode_contents(), "html.parser")
-                self._transform_components(tag_soup, component_key)
+                self._transform_components(tag_soup, component_name)
 
                 # Create new content with opening tag, tag content, and closing tag
                 new_content = opening_tag + str(tag_soup) + closing_tag
 
             else:
                 # Create new content with opening tag and closing tag
                 new_content = opening_tag + closing_tag
```

### Comparing `django_cotton-0.0.8/django_cotton/templatetags/_component.py` & `django_cotton-0.0.9/django_cotton/templatetags/_props_frame.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 from django import template
-from django.template import Node
-from django.template.loader import render_to_string
+from django.template.base import token_kwargs
+from django.utils.safestring import mark_safe
 
+register = template.Library()
 
-def cotton_component(parser, token):
-    bits = token.split_contents()
-    tag_name = bits[0]
-    template_path = bits[1]
-    component_key = bits[2]
-
-    kwargs = {}
-    for bit in bits[3:]:
-        key, value = bit.split("=")
-        kwargs[key] = str(value.strip("'\""))
 
-    nodelist = parser.parse(("end_cotton_component",))
-    parser.delete_first_token()
+def cotton_props_frame(parser, token):
+    """The job of the props frame is to filter component kwargs (attributes) against declared props. It has to be
+    second component because we desire to declare props (<c-props />) inside the component template and therefore the
+    component can not manipulate its own context from it's own template, instead we declare the props frame
+    directly inside component"""
+    bits = token.split_contents()[1:]  # Skip the tag name
+    # Parse token kwargs while maintaining token order
+    tag_kwargs = token_kwargs(bits, parser)
 
-    return CottonComponentNode(nodelist, template_path, component_key, kwargs)
+    nodelist = parser.parse(("endcotton_props_frame",))
+    parser.delete_first_token()
+    return CottonPropsFrameNode(nodelist, tag_kwargs)
 
 
-class CottonComponentNode(Node):
-    def __init__(self, nodelist, template_path, component_key, kwargs):
+class CottonPropsFrameNode(template.Node):
+    def __init__(self, nodelist, kwargs):
         self.nodelist = nodelist
-        self.template_path = template_path
-        self.component_key = component_key
         self.kwargs = kwargs
 
     def render(self, context):
-        local_context = context.flatten()
-
-        attrs = {}
+        # Assume 'attrs' are passed from the parent and are available in the context
+        parent_attrs = context.get("attrs_dict", {})
 
-        # Process attrs + props
+        # Initialize props based on the frame's kwargs and parent attrs
+        props = {}
         for key, value in self.kwargs.items():
-            try:
-                resolved_value = template.Variable(value).resolve(context)
-                attrs.update({key: resolved_value})
-            except TypeError:
-                attrs.update({key: value})
-            except template.VariableDoesNotExist:
-                attrs.update({key: value})
-
-        # Add the remainder as the default slot
-        rendered = self.nodelist.render(context)
-        local_context.update({"slot": rendered})
-
-        slots = context.get("cotton_slots", {})
-        component_slots = slots.get(self.component_key, {})
-
-        local_context.update(component_slots)
-        local_context.update(attrs)
-
-        local_context.update({"attrs_dict": attrs})
-
-        rendered = render_to_string(self.template_path, local_context)
-
-        # Now reset the component slots in context
-        slots[self.component_key] = {}
-        context.update({"cotton_slots": slots})
+            # Attempt to resolve each kwarg value (which may include template variables)
+            resolved_value = value.resolve(context)
+            # Check if the prop exists in parent attrs; if so, use it, otherwise use the resolved default
+            if key in parent_attrs:
+                props[key] = parent_attrs[key]
+            else:
+                props[key] = resolved_value
+
+        # Overwrite 'attrs' in the local context by excluding keys that are identified as props
+        attrs_without_props = {k: v for k, v in parent_attrs.items() if k not in props}
+        context["attrs_dict"] = attrs_without_props
+
+        # Provide all of the attrs as a string to pass to the component
+        def ensure_quoted(value):
+            if isinstance(value, str) and value.startswith('"') and value.endswith('"'):
+                return value
+            else:
+                return f'"{value}"'
+
+        attrs = " ".join(
+            [
+                f"{key}={ensure_quoted(value)}"
+                for key, value in attrs_without_props.items()
+            ]
+        )
+
+        context.update({"attrs": mark_safe(attrs)})
+        context.update(attrs_without_props)
+        context.update(props)
 
-        return rendered
+        return self.nodelist.render(context)
```

### Comparing `django_cotton-0.0.8/django_cotton/templatetags/_props.py` & `django_cotton-0.0.9/django_cotton/templatetags/_props.py`

 * *Files identical despite different names*

### Comparing `django_cotton-0.0.8/django_cotton/templatetags/_slot.py` & `django_cotton-0.0.9/django_cotton/templatetags/_slot.py`

 * *Files identical despite different names*

### Comparing `django_cotton-0.0.8/django_cotton/templatetags/cotton.py` & `django_cotton-0.0.9/django_cotton/templatetags/cotton.py`

 * *Files identical despite different names*

### Comparing `django_cotton-0.0.8/django_cotton/urls.py` & `django_cotton-0.0.9/django_cotton/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,9 @@
     path("attribute-passing", views.attribute_passing_test_view),
     path("django-syntax-decoding", views.django_syntax_decoding_test_view),
     path(
         "string-with-spaces",
         TemplateView.as_view(template_name="string_with_spaces.cotton.html"),
     ),
     path("props-test", TemplateView.as_view(template_name="props_test.cotton.html")),
+    path("variable-parsing", views.variable_parsing_test_view),
 ]
```

### Comparing `django_cotton-0.0.8/django_cotton/views.py` & `django_cotton-0.0.9/django_cotton/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,7 +28,13 @@
 
 def attribute_passing_test_view(request):
     return render(request, "attribute_passing_test.cotton.html")
 
 
 def django_syntax_decoding_test_view(request):
     return render(request, "django_syntax_decoding_test.cotton.html")
+
+
+def variable_parsing_test_view(request):
+    return render(
+        request, "variable_parsing_test.cotton.html", {"variable": "some-class"}
+    )
```

### Comparing `django_cotton-0.0.8/pyproject.toml` & `django_cotton-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-cotton"
-version = "0.0.8"
+version = "0.0.9"
 description = "Bringing component based design to Django templates."
 authors = [ "Will Abbott <wabbott@dyvenia.com>",]
 license = "MIT"
 readme = "README.md"
 classifiers = [ "Development Status :: 3 - Alpha", "Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Programming Language :: Python :: 3.10", "Framework :: Django",]
 keywords = [ "django", "cotton", "reusable", "app",]
 exclude = [ "dev", "docs", "django_cotton/tests", "django_cotton/templates",]
```

### Comparing `django_cotton-0.0.8/PKG-INFO` & `django_cotton-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cotton
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bringing component based design to Django templates.
 License: MIT
 Keywords: django,cotton,reusable,app
 Author: Will Abbott
 Author-email: wabbott@dyvenia.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 3 - Alpha
```

