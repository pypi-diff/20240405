# Comparing `tmp/regex-compose-0.0.2.tar.gz` & `tmp/regex-compose-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-compose-0.0.2.tar", last modified: Fri Apr  5 00:21:04 2024, max compression
+gzip compressed data, was "regex-compose-0.0.3.tar", last modified: Fri Apr  5 19:12:54 2024, max compression
```

## Comparing `regex-compose-0.0.2.tar` & `regex-compose-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-05 00:21:04.456065 regex-compose-0.0.2/
--rw-r--r--   0 shae      (1000) shae      (1000)      555 2024-04-04 16:38:40.000000 regex-compose-0.0.2/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     4876 2024-04-05 00:21:04.452731 regex-compose-0.0.2/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     3844 2024-04-04 23:44:54.000000 regex-compose-0.0.2/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1093 2024-04-05 00:20:34.000000 regex-compose-0.0.2/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-05 00:21:04.456065 regex-compose-0.0.2/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-05 00:21:04.452731 regex-compose-0.0.2/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-05 00:21:04.452731 regex-compose-0.0.2/src/regex_compose.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     4876 2024-04-05 00:21:04.000000 regex-compose-0.0.2/src/regex_compose.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      217 2024-04-05 00:21:04.000000 regex-compose-0.0.2/src/regex_compose.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-05 00:21:04.000000 regex-compose-0.0.2/src/regex_compose.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       14 2024-04-05 00:21:04.000000 regex-compose-0.0.2/src/regex_compose.egg-info/top_level.txt
--rw-r--r--   0 shae      (1000) shae      (1000)    11697 2024-04-05 00:19:29.000000 regex-compose-0.0.2/src/regex_compose.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-05 19:12:54.492743 regex-compose-0.0.3/
+-rw-r--r--   0 shae      (1000) shae      (1000)      555 2024-04-04 16:38:40.000000 regex-compose-0.0.3/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     5100 2024-04-05 19:12:54.492743 regex-compose-0.0.3/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     4068 2024-04-05 19:11:51.000000 regex-compose-0.0.3/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1093 2024-04-05 18:41:28.000000 regex-compose-0.0.3/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-05 19:12:54.496076 regex-compose-0.0.3/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-05 19:12:54.489410 regex-compose-0.0.3/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-05 19:12:54.492743 regex-compose-0.0.3/src/regex_compose.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     5100 2024-04-05 19:12:54.000000 regex-compose-0.0.3/src/regex_compose.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      217 2024-04-05 19:12:54.000000 regex-compose-0.0.3/src/regex_compose.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-05 19:12:54.000000 regex-compose-0.0.3/src/regex_compose.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       14 2024-04-05 19:12:54.000000 regex-compose-0.0.3/src/regex_compose.egg-info/top_level.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)    11760 2024-04-05 18:57:30.000000 regex-compose-0.0.3/src/regex_compose.py
```

### Comparing `regex-compose-0.0.2/LICENSE` & `regex-compose-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `regex-compose-0.0.2/PKG-INFO` & `regex-compose-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-compose
-Version: 0.0.2
+Version: 0.0.3
 Summary: Compose multiple regular expressions into one using a special syntax
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Shae/RegExCompose
 Project-URL: Issues, https://codeberg.org/Shae/RegExCompose/issues
 Keywords: re,regex,regular,expression
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -115,13 +115,18 @@
 | `%pragma.stop:;`   | `(?m)%(?P<key>(?:\w\|\d\|\.)+):(?P<val>.*?);`
 | `%pragma.delim:=;` | `(?m)%(?P<key>(?:\w\|\d\|\.)+)=(?P<val>.*?);`
 
 ## Further examples
 For further examples, see [https://codeberg.org/Shae/RegExCompose/src/branch/main/examples](https://codeberg.org/Shae/RegExCompose/src/branch/main/examples)
 
 # Changelog
+
+## v0.0.3
+- Fixed an issue in `PatternComposer.multiadd()` due to incorrect name access
+- Fixed `refpatt_patt` not being passed to `get_refpatt_parts` in `PatternComposer.multiadd()`, causing an error when in `bytes_mode`
+
 ## v0.0.2
 - Added support for bytes
 
 # Links
 - Source code: [https://codeberg.org/Shae/RegExCompose](https://codeberg.org/Shae/RegExCompose)
 - License: [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `regex-compose-0.0.2/README.md` & `regex-compose-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -90,13 +90,18 @@
 | `%pragma.stop:;`   | `(?m)%(?P<key>(?:\w\|\d\|\.)+):(?P<val>.*?);`
 | `%pragma.delim:=;` | `(?m)%(?P<key>(?:\w\|\d\|\.)+)=(?P<val>.*?);`
 
 ## Further examples
 For further examples, see [https://codeberg.org/Shae/RegExCompose/src/branch/main/examples](https://codeberg.org/Shae/RegExCompose/src/branch/main/examples)
 
 # Changelog
+
+## v0.0.3
+- Fixed an issue in `PatternComposer.multiadd()` due to incorrect name access
+- Fixed `refpatt_patt` not being passed to `get_refpatt_parts` in `PatternComposer.multiadd()`, causing an error when in `bytes_mode`
+
 ## v0.0.2
 - Added support for bytes
 
 # Links
 - Source code: [https://codeberg.org/Shae/RegExCompose](https://codeberg.org/Shae/RegExCompose)
 - License: [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `regex-compose-0.0.2/pyproject.toml` & `regex-compose-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "regex-compose"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Compose multiple regular expressions into one using a special syntax"
 readme = "README.md"
 keywords = ["re", "regex", "regular", "expression"]
```

### Comparing `regex-compose-0.0.2/src/regex_compose.egg-info/PKG-INFO` & `regex-compose-0.0.3/src/regex_compose.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex-compose
-Version: 0.0.2
+Version: 0.0.3
 Summary: Compose multiple regular expressions into one using a special syntax
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Shae/RegExCompose
 Project-URL: Issues, https://codeberg.org/Shae/RegExCompose/issues
 Keywords: re,regex,regular,expression
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -115,13 +115,18 @@
 | `%pragma.stop:;`   | `(?m)%(?P<key>(?:\w\|\d\|\.)+):(?P<val>.*?);`
 | `%pragma.delim:=;` | `(?m)%(?P<key>(?:\w\|\d\|\.)+)=(?P<val>.*?);`
 
 ## Further examples
 For further examples, see [https://codeberg.org/Shae/RegExCompose/src/branch/main/examples](https://codeberg.org/Shae/RegExCompose/src/branch/main/examples)
 
 # Changelog
+
+## v0.0.3
+- Fixed an issue in `PatternComposer.multiadd()` due to incorrect name access
+- Fixed `refpatt_patt` not being passed to `get_refpatt_parts` in `PatternComposer.multiadd()`, causing an error when in `bytes_mode`
+
 ## v0.0.2
 - Added support for bytes
 
 # Links
 - Source code: [https://codeberg.org/Shae/RegExCompose](https://codeberg.org/Shae/RegExCompose)
 - License: [http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `regex-compose-0.0.2/src/regex_compose.py` & `regex-compose-0.0.3/src/regex_compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,20 +205,20 @@
                     and waits to execute updates until all patterns have been added
             If any patterns already exist, and not `replace`, then `exceptions.PatternExistsError` is raised
         '''
         if (not replace) and (exists := (patts.keys() & self.patterns.keys())):
             e = exceptions.PatternExistsError(f'Cannot replace {len(exists)} existing pattern(s)')
             e.add_note(f'Existing patterns: {(b", " if self.bytes_mode else ", ").join(exists)}')
             raise e
+        patts = dict(zip(map(_tostr, patts.keys()), patts.values()))
         for n,p in patts.items():
-            self._fail_type(patt, f'Incorrect type for pattern in patts for {name!r}: {patt!r}')
+            self._fail_type(p, f'Incorrect type for pattern in patts for {n!r}: {p!r}')
         for n,p in patts.items():
-            n = _tostr(name)
             self.patterns[n] = p
-            self.references[n] = frozenset(get_refpatt_parts(p))
+            self.references[n] = frozenset(get_refpatt_parts(p, refpatt_patt=self.refpatt_patt))
         self.multiupdate(*patts.keys())
 
     def remove(self, name: str | bytes, *, update_referrers: bool | None = True, ignore_missing: bool = False) -> None:
         '''
             Removes a pattern
             If `update_referrers` is `None`, referrers are ignored;
                 other falsey values will cause an `exceptions.RequiredPatternError` to be raised if referrers are present
```

