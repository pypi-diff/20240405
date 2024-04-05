# Comparing `tmp/craft-grammar-1.1.2.tar.gz` & `tmp/craft-grammar-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-grammar-1.1.2.tar", last modified: Fri Dec  1 12:39:53 2023, max compression
+gzip compressed data, was "craft-grammar-1.2.0.tar", last modified: Fri Apr  5 16:09:16 2024, max compression
```

## Comparing `craft-grammar-1.1.2.tar` & `craft-grammar-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-12-01 12:39:53.652242 craft-grammar-1.1.2/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2022-02-22 14:21:12.000000 craft-grammar-1.1.2/LICENSE
--rw-r--r--   0 claudio   (1000) claudio   (1000)     4767 2023-12-01 12:39:53.652242 craft-grammar-1.1.2/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1384 2022-02-22 14:21:12.000000 craft-grammar-1.1.2/README.md
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-12-01 12:39:53.644242 craft-grammar-1.1.2/craft_grammar/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     1267 2023-12-01 12:38:55.000000 craft-grammar-1.1.2/craft_grammar/__init__.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2189 2022-03-18 21:26:43.000000 craft-grammar-1.1.2/craft_grammar/_compound.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3561 2022-03-18 21:26:43.000000 craft-grammar-1.1.2/craft_grammar/_on.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    10748 2022-03-18 21:26:43.000000 craft-grammar-1.1.2/craft_grammar/_processor.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5596 2022-03-18 21:26:43.000000 craft-grammar-1.1.2/craft_grammar/_statement.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     3628 2022-03-18 21:26:43.000000 craft-grammar-1.1.2/craft_grammar/_to.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2308 2022-03-18 21:26:43.000000 craft-grammar-1.1.2/craft_grammar/_try.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2009 2022-03-18 21:26:43.000000 craft-grammar-1.1.2/craft_grammar/errors.py
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5780 2022-08-08 12:46:46.000000 craft-grammar-1.1.2/craft_grammar/models.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-12-01 12:39:53.648242 craft-grammar-1.1.2/craft_grammar.egg-info/
--rw-r--r--   0 claudio   (1000) claudio   (1000)     4767 2023-12-01 12:39:53.000000 craft-grammar-1.1.2/craft_grammar.egg-info/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      492 2023-12-01 12:39:53.000000 craft-grammar-1.1.2/craft_grammar.egg-info/SOURCES.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-12-01 12:39:53.000000 craft-grammar-1.1.2/craft_grammar.egg-info/dependency_links.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2022-02-22 14:45:59.000000 craft-grammar-1.1.2/craft_grammar.egg-info/not-zip-safe
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      702 2023-12-01 12:39:53.000000 craft-grammar-1.1.2/craft_grammar.egg-info/requires.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       14 2023-12-01 12:39:53.000000 craft-grammar-1.1.2/craft_grammar.egg-info/top_level.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      648 2023-11-20 21:45:44.000000 craft-grammar-1.1.2/pyproject.toml
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     2481 2023-12-01 12:39:53.652242 craft-grammar-1.1.2/setup.cfg
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      789 2022-02-23 13:07:03.000000 craft-grammar-1.1.2/setup.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-04-05 16:09:16.371492 craft-grammar-1.2.0/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2022-02-22 14:21:12.000000 craft-grammar-1.2.0/LICENSE
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     4767 2024-04-05 16:09:16.371492 craft-grammar-1.2.0/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1384 2022-02-22 14:21:12.000000 craft-grammar-1.2.0/README.md
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-04-05 16:09:16.368493 craft-grammar-1.2.0/craft_grammar/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     1267 2024-04-05 16:05:47.000000 craft-grammar-1.2.0/craft_grammar/__init__.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2189 2022-03-18 21:26:43.000000 craft-grammar-1.2.0/craft_grammar/_compound.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3561 2022-03-18 21:26:43.000000 craft-grammar-1.2.0/craft_grammar/_on.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    10940 2024-04-05 15:45:59.000000 craft-grammar-1.2.0/craft_grammar/_processor.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5596 2022-03-18 21:26:43.000000 craft-grammar-1.2.0/craft_grammar/_statement.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     3628 2022-03-18 21:26:43.000000 craft-grammar-1.2.0/craft_grammar/_to.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2308 2022-03-18 21:26:43.000000 craft-grammar-1.2.0/craft_grammar/_try.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2009 2022-03-18 21:26:43.000000 craft-grammar-1.2.0/craft_grammar/errors.py
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     9359 2024-04-05 15:45:59.000000 craft-grammar-1.2.0/craft_grammar/models.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2024-04-05 16:09:16.369493 craft-grammar-1.2.0/craft_grammar.egg-info/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     4767 2024-04-05 16:09:16.000000 craft-grammar-1.2.0/craft_grammar.egg-info/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      492 2024-04-05 16:09:16.000000 craft-grammar-1.2.0/craft_grammar.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2024-04-05 16:09:16.000000 craft-grammar-1.2.0/craft_grammar.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2022-02-22 14:45:59.000000 craft-grammar-1.2.0/craft_grammar.egg-info/not-zip-safe
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      702 2024-04-05 16:09:16.000000 craft-grammar-1.2.0/craft_grammar.egg-info/requires.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       14 2024-04-05 16:09:16.000000 craft-grammar-1.2.0/craft_grammar.egg-info/top_level.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      648 2023-11-20 21:45:44.000000 craft-grammar-1.2.0/pyproject.toml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     2481 2024-04-05 16:09:16.372493 craft-grammar-1.2.0/setup.cfg
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      789 2022-02-23 13:07:03.000000 craft-grammar-1.2.0/setup.py
```

### Comparing `craft-grammar-1.1.2/LICENSE` & `craft-grammar-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/PKG-INFO` & `craft-grammar-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-grammar
-Version: 1.1.2
+Version: 1.2.0
 Summary: "Advance Grammar for Craft Parts"
 Home-page: https://github.com/canonical/craft-grammar
 Author: Canonical Ltd.
 Author-email: snapcraft@lists.snapcraft.io
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Documentation, https://craft-grammar.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/canonical/craft-grammar.git
```

### Comparing `craft-grammar-1.1.2/README.md` & `craft-grammar-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/craft_grammar/__init__.py` & `craft-grammar-1.2.0/craft_grammar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 """Enhance part definitions with advanced grammar."""
 
-__version__ = "1.1.2"
+__version__ = "1.2.0"
 
 
 from . import errors
 from ._compound import CompoundStatement
 from ._on import OnStatement
 from ._processor import GrammarProcessor
 from ._statement import CallStack, Grammar, Statement
```

### Comparing `craft-grammar-1.1.2/craft_grammar/_compound.py` & `craft-grammar-1.2.0/craft_grammar/_compound.py`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/craft_grammar/_on.py` & `craft-grammar-1.2.0/craft_grammar/_on.py`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/craft_grammar/_processor.py` & `craft-grammar-1.2.0/craft_grammar/_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,14 +116,17 @@
                     )
 
                 # If this section does not belong to a statement, it is
                 # a primitive to be recorded.
                 if statement is None:
                     primitives.append(section)
 
+            elif isinstance(section, (int | float | bool | list)):
+                # If the section is a number, boolean, or list, it's a primitive.
+                primitives.append(section)
             else:
                 # jsonschema should never let us get here.
                 raise GrammarSyntaxError(
                     "expected grammar section to be either of type 'str' or "
                     f"type 'dict', but got {type(section)!r}"
                 )
```

### Comparing `craft-grammar-1.1.2/craft_grammar/_statement.py` & `craft-grammar-1.2.0/craft_grammar/_statement.py`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/craft_grammar/_to.py` & `craft-grammar-1.2.0/craft_grammar/_to.py`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/craft_grammar/_try.py` & `craft-grammar-1.2.0/craft_grammar/_try.py`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/craft_grammar/errors.py` & `craft-grammar-1.2.0/craft_grammar/errors.py`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/craft_grammar/models.py` & `craft-grammar-1.2.0/craft_grammar/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 _compound_pattern = re.compile(r"^on\s+(.+)\s+to\s+(.+)\s*$")
 
 _ELSE_FAIL = "else fail"
 _ELSE = "else"
 _TRY = "try"
 
 
+_GrammarType = Dict[str, Any]
+
+
 class _GrammarBase(abc.ABC):
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
     @abc.abstractmethod
@@ -46,18 +49,85 @@
         if item == _ELSE_FAIL:
             _mark_and_append(entry, item)
         else:
             key, value = tuple(item.items())[0]
             _mark_and_append(entry, {key: cls.validate(value)})
 
 
-_GrammarType = Dict[str, Any]
+# Public types for grammar-enabled attributes
+class GrammarBool(_GrammarBase):
+    """Grammar-enabled bool field."""
 
+    __root__: Union[bool, _GrammarType]
 
-# Public types for grammar-enabled attributes
+    @classmethod
+    @overrides
+    def validate(cls, entry):
+        # GrammarBool entry can be a list if it contains clauses
+        if isinstance(entry, list):
+            new_entry = []
+            for item in entry:
+                if _is_grammar_clause(item):
+                    cls._grammar_append(new_entry, item)
+                else:
+                    raise TypeError(f"value must be a list of bool: {entry!r}")
+            return new_entry
+
+        if isinstance(entry, bool):
+            return entry
+
+        raise TypeError(f"value must be a bool: {entry!r}")
+
+
+class GrammarInt(_GrammarBase):
+    """Grammar-enabled integer field."""
+
+    __root__: Union[int, _GrammarType]
+
+    @classmethod
+    @overrides
+    def validate(cls, entry):
+        # GrammarInt entry can be a list if it contains clauses
+        if isinstance(entry, list):
+            new_entry = []
+            for item in entry:
+                if _is_grammar_clause(item):
+                    cls._grammar_append(new_entry, item)
+                else:
+                    raise TypeError(f"value must be a list of integer: {entry!r}")
+            return new_entry
+
+        if isinstance(entry, int):
+            return entry
+
+        raise TypeError(f"value must be a integer: {entry!r}")
+
+
+class GrammarFloat(_GrammarBase):
+    """Grammar-enabled float field."""
+
+    __root__: Union[float, _GrammarType]
+
+    @classmethod
+    @overrides
+    def validate(cls, entry):
+        # GrammarFloat entry can be a list if it contains clauses
+        if isinstance(entry, list):
+            new_entry = []
+            for item in entry:
+                if _is_grammar_clause(item):
+                    cls._grammar_append(new_entry, item)
+                else:
+                    raise TypeError(f"value must be a list of float: {entry!r}")
+            return new_entry
+
+        if isinstance(entry, (int, float)):
+            return float(entry)
+
+        raise TypeError(f"value must be a float: {entry!r}")
 
 
 class GrammarStr(_GrammarBase):
     """Grammar-enabled string field."""
 
     __root__: Union[str, _GrammarType]
 
@@ -124,14 +194,61 @@
                         f"value must be a list of single-entry dictionaries: {entry!r}"
                     )
             return new_entry
 
         raise TypeError(f"value must be a list of single-entry dictionaries: {entry!r}")
 
 
+class GrammarDict(_GrammarBase):
+    """Grammar-enabled dictionary field."""
+
+    __root__: Union[Dict[str, Any], _GrammarType]
+
+    @classmethod
+    @overrides
+    def validate(cls, entry):
+        # GrammarDict entry can be a list if it contains clauses
+        if isinstance(entry, list):
+            new_entry = []
+            for item in entry:
+                if _is_grammar_clause(item):
+                    cls._grammar_append(new_entry, item)
+                else:
+                    raise TypeError(f"value must be a list of dictionaries: {entry!r}")
+            return new_entry
+
+        if isinstance(entry, dict):
+            return entry
+
+        raise TypeError(f"value must be a dictionary: {entry!r}")
+
+
+class GrammarDictList(_GrammarBase):
+    """Grammar-enabled list of dictionary field."""
+
+    __root__: Union[List[Dict[str, Any]], _GrammarType]
+
+    @classmethod
+    @overrides
+    def validate(cls, entry):
+        # GrammarDictList will always be a list
+        if isinstance(entry, list):
+            new_entry = []
+            for item in entry:
+                if _is_grammar_clause(item):
+                    cls._grammar_append(new_entry, item)
+                elif isinstance(item, dict):
+                    new_entry.append(item)
+                else:
+                    raise TypeError(f"value must be a list of dictionaries: {entry!r}")
+            return new_entry
+
+        raise TypeError(f"value must be a list of dictionary: {entry!r}")
+
+
 def _ensure_selector_valid(selector: str, *, clause: str) -> None:
     """Verify selector syntax."""
     # spaces are not allowed in selector
     if " " in selector:
         raise ValueError(f"spaces are not allowed in {clause!r} selector")
 
     # selector items should be separated by comma
```

### Comparing `craft-grammar-1.1.2/craft_grammar.egg-info/PKG-INFO` & `craft-grammar-1.2.0/craft_grammar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-grammar
-Version: 1.1.2
+Version: 1.2.0
 Summary: "Advance Grammar for Craft Parts"
 Home-page: https://github.com/canonical/craft-grammar
 Author: Canonical Ltd.
 Author-email: snapcraft@lists.snapcraft.io
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Documentation, https://craft-grammar.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/canonical/craft-grammar.git
```

### Comparing `craft-grammar-1.1.2/craft_grammar.egg-info/requires.txt` & `craft-grammar-1.2.0/craft_grammar.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/pyproject.toml` & `craft-grammar-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/setup.cfg` & `craft-grammar-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `craft-grammar-1.1.2/setup.py` & `craft-grammar-1.2.0/setup.py`

 * *Files identical despite different names*

