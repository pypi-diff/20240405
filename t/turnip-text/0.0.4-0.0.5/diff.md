# Comparing `tmp/turnip_text-0.0.4.tar.gz` & `tmp/turnip_text-0.0.5.tar.gz`

## Comparing `turnip_text-0.0.4.tar` & `turnip_text-0.0.5.tar`

### file list

```diff
@@ -1,57 +1,68 @@
--rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 turnip_text-0.0.4/Cargo.toml
--rw-r--r--   0     1001      127      202 2023-09-16 16:10:52.000000 turnip_text-0.0.4/.cargo/config.toml
--rw-r--r--   0     1001      127     2745 2023-09-16 16:10:52.000000 turnip_text-0.0.4/.github/workflows/CI.yaml
--rw-r--r--   0     1001      127       82 2023-09-16 16:10:52.000000 turnip_text-0.0.4/.gitignore
--rw-r--r--   0     1001      127      833 2023-09-16 16:10:52.000000 turnip_text-0.0.4/.vscode/settings.json
--rw-r--r--   0     1001      127      855 2023-09-16 16:10:52.000000 turnip_text-0.0.4/Justfile
--rw-r--r--   0     1001      127    10847 2023-09-16 16:10:52.000000 turnip_text-0.0.4/LICENSE-APACHE
--rw-r--r--   0     1001      127     1056 2023-09-16 16:10:52.000000 turnip_text-0.0.4/LICENSE-MIT
--rw-r--r--   0     1001      127     4391 2023-09-16 16:10:52.000000 turnip_text-0.0.4/README.md
--rw-r--r--   0     1001      127       10 2023-09-16 16:11:02.000000 turnip_text-0.0.4/dist/turnip_text-0.0.4.tar.gz
--rw-r--r--   0     1001      127      858 2023-09-16 16:10:52.000000 turnip_text-0.0.4/examples/experiment.pytext
--rw-r--r--   0     1001      127     3372 2023-09-16 16:10:52.000000 turnip_text-0.0.4/examples/phdprop.py
--rw-r--r--   0     1001      127    21637 2023-09-16 16:10:52.000000 turnip_text-0.0.4/examples/phdprop.ttxt
--rw-r--r--   0     1001      127     6171 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/analysis/asciidoctor.md
--rw-r--r--   0     1001      127        0 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/analysis/docbook.md
--rw-r--r--   0     1001      127      113 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/analysis/latex.md
--rw-r--r--   0     1001      127      135 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/analysis/restructuredtext.md
--rw-r--r--   0     1001      127       22 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/analysis/sphinx.md
--rw-r--r--   0     1001      127    10866 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/code_syntax.md
--rw-r--r--   0     1001      127    10166 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/content_v_formatting.md
--rw-r--r--   0     1001      127      188 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/goals.md
--rw-r--r--   0     1001      127      908 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/labels.md
--rw-r--r--   0     1001      127     2476 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/opinionated_text.md
--rw-r--r--   0     1001      127     2151 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/pandoc.md
--rw-r--r--   0     1001      127       33 2023-09-16 16:10:52.000000 turnip_text-0.0.4/notes/raw_string_syntax.md
--rw-r--r--   0     1001      127      787 2023-09-16 16:10:52.000000 turnip_text-0.0.4/pyproject.toml
--rw-r--r--   0     1001      127     2726 2023-09-16 16:10:52.000000 turnip_text-0.0.4/python/turnip_text/__init__.py
--rw-r--r--   0     1001      127     3173 2023-09-16 16:10:52.000000 turnip_text-0.0.4/python/turnip_text/helpers.py
--rw-r--r--   0     1001      127        0 2023-09-16 16:10:52.000000 turnip_text-0.0.4/python/turnip_text/py.typed
--rw-r--r--   0     1001      127    25823 2023-09-16 16:10:52.000000 turnip_text-0.0.4/python/turnip_text/renderers/__init__.py
--rw-r--r--   0     1001      127     6461 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/_wip/labels.py
--rw-r--r--   0     1001      127     3022 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/dictify.py
--rw-r--r--   0     1001      127       31 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/latex/__init__.py
--rw-r--r--   0     1001      127     2220 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/latex/base.py
--rw-r--r--   0     1001      127    13179 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/latex/plugins.py
--rw-r--r--   0     1001      127       35 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/markdown/__init__.py
--rw-r--r--   0     1001      127     3015 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/markdown/base.py
--rw-r--r--   0     1001      127    22034 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/markdown/plugins.py
--rw-r--r--   0     1001      127     2673 2023-09-16 16:10:53.000000 turnip_text-0.0.4/python/turnip_text/renderers/std_plugins.py
--rw-r--r--   0     1001      127    11510 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/cli.rs
--rw-r--r--   0     1001      127    19518 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/lexer.rs
--rw-r--r--   0     1001      127     1905 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/lexer_charofs_row_col.rs
--rw-r--r--   0     1001      127      102 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/lib.rs
--rw-r--r--   0     1001      127    19276 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/python/interop.rs
--rw-r--r--   0     1001      127     8360 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/python/interp/eval_bracket.rs
--rw-r--r--   0     1001      127    24277 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/python/interp/mod.rs
--rw-r--r--   0     1001      127    27940 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/python/interp/para.rs
--rw-r--r--   0     1001      127      943 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/python/mod.rs
--rw-r--r--   0     1001      127     2859 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/python/typeclass.rs
--rw-r--r--   0     1001      127      530 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/tests/mod.rs
--rw-r--r--   0     1001      127    11327 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/tests/test_lexer.rs
--rw-r--r--   0     1001      127    10913 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/tests/test_lexer_parser.rs
--rw-r--r--   0     1001      127    34571 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/tests/test_parser.rs
--rw-r--r--   0     1001      127     1287 2023-09-16 16:10:53.000000 turnip_text-0.0.4/src/util.rs
--rw-r--r--   0     1001      127     3387 2023-09-16 16:10:53.000000 turnip_text-0.0.4/turnip_text.pyi
--rw-r--r--   0     1001      127    11057 2023-09-16 16:10:52.000000 turnip_text-0.0.4/Cargo.lock
--rw-r--r--   0        0        0     5184 1970-01-01 00:00:00.000000 turnip_text-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 turnip_text-0.0.5/Cargo.toml
+-rw-r--r--   0     1001      127      202 2024-04-03 19:42:35.000000 turnip_text-0.0.5/.cargo/config.toml
+-rw-r--r--   0     1001      127     2745 2024-04-03 19:42:35.000000 turnip_text-0.0.5/.github/workflows/CI.yaml
+-rw-r--r--   0     1001      127       82 2024-04-03 19:42:35.000000 turnip_text-0.0.5/.gitignore
+-rw-r--r--   0     1001      127     1148 2024-04-03 19:42:35.000000 turnip_text-0.0.5/.vscode/settings.json
+-rw-r--r--   0     1001      127     1207 2024-04-03 19:42:35.000000 turnip_text-0.0.5/Justfile
+-rw-r--r--   0     1001      127    10847 2024-04-03 19:42:35.000000 turnip_text-0.0.5/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1056 2024-04-03 19:42:35.000000 turnip_text-0.0.5/LICENSE-MIT
+-rw-r--r--   0     1001      127     4391 2024-04-03 19:42:35.000000 turnip_text-0.0.5/README.md
+-rw-r--r--   0     1001      127      858 2024-04-03 19:42:35.000000 turnip_text-0.0.5/examples/experiment.pytext
+-rw-r--r--   0     1001      127     4401 2024-04-03 19:42:35.000000 turnip_text-0.0.5/examples/phdprop.py
+-rw-r--r--   0     1001      127    18977 2024-04-03 19:42:35.000000 turnip_text-0.0.5/examples/phdprop.ttext
+-rw-r--r--   0     1001      127     1740 2024-04-03 19:42:35.000000 turnip_text-0.0.5/examples/phdprop_subfile_first_year_plan.ttext
+-rw-r--r--   0     1001      127     6171 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/analysis/asciidoctor.md
+-rw-r--r--   0     1001      127        0 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/analysis/docbook.md
+-rw-r--r--   0     1001      127      113 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/analysis/latex.md
+-rw-r--r--   0     1001      127      135 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/analysis/restructuredtext.md
+-rw-r--r--   0     1001      127       22 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/analysis/sphinx.md
+-rw-r--r--   0     1001      127      958 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/anchors_and_counters.md
+-rw-r--r--   0     1001      127    11783 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/code_syntax.md
+-rw-r--r--   0     1001      127    10166 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/content_v_formatting.md
+-rw-r--r--   0     1001      127      188 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/goals.md
+-rw-r--r--   0     1001      127      908 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/labels.md
+-rw-r--r--   0     1001      127     2476 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/opinionated_text.md
+-rw-r--r--   0     1001      127     2151 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/pandoc.md
+-rw-r--r--   0     1001      127       33 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/raw_string_syntax.md
+-rw-r--r--   0     1001      127     4935 2024-04-03 19:42:35.000000 turnip_text-0.0.5/notes/structure_first_parsing.md
+-rw-r--r--   0     1001      127     3390 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/__init__.py
+-rw-r--r--   0     1001      127     5341 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/__init__.pyi
+-rw-r--r--   0     1001      127    14757 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/build_system.py
+-rw-r--r--   0     1001      127    18765 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/doc/__init__.py
+-rw-r--r--   0     1001      127     3108 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/doc/anchors.py
+-rw-r--r--   0     1001      127    13014 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/doc/std_plugins.py
+-rw-r--r--   0     1001      127     1351 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/doc/user_nodes.py
+-rw-r--r--   0     1001      127     3561 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/helpers.py
+-rw-r--r--   0     1001      127        0 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/py.typed
+-rw-r--r--   0     1001      127    17486 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/__init__.py
+-rw-r--r--   0     1001      127    10027 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/counters.py
+-rw-r--r--   0     1001      127     2342 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/dyn_dispatch.py
+-rw-r--r--   0     1001      127        0 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/latex/__init__.py
+-rw-r--r--   0     1001      127     5372 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/latex/backrefs.py
+-rw-r--r--   0     1001      127    17157 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/latex/renderer.py
+-rw-r--r--   0     1001      127    17867 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/latex/setup.py
+-rw-r--r--   0     1001      127    10005 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/latex/std_plugins.py
+-rw-r--r--   0     1001      127     3583 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/manual_numbering.py
+-rw-r--r--   0     1001      127        0 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/markdown/__init__.py
+-rw-r--r--   0     1001      127    12178 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/markdown/renderer.py
+-rw-r--r--   0     1001      127    14361 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/render/markdown/std_plugins.py
+-rw-r--r--   0     1001      127     6018 2024-04-03 19:42:35.000000 turnip_text-0.0.5/python/turnip_text/system.py
+-rw-r--r--   0     1001      127    15078 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/error.rs
+-rw-r--r--   0     1001      127     8663 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/interpreter/eval_bracket.rs
+-rw-r--r--   0     1001      127    37164 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/interpreter/mod.rs
+-rw-r--r--   0     1001      127    28957 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/interpreter/para.rs
+-rw-r--r--   0     1001      127    24196 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/interpreter/python/interop.rs
+-rw-r--r--   0     1001      127      415 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/interpreter/python/mod.rs
+-rw-r--r--   0     1001      127     4097 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/interpreter/python/typeclass.rs
+-rw-r--r--   0     1001      127     1994 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/lexer/line_col_char_posn.rs
+-rw-r--r--   0     1001      127    22894 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/lexer/mod.rs
+-rw-r--r--   0     1001      127      106 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/lib.rs
+-rw-r--r--   0     1001      127     4033 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/parser.rs
+-rw-r--r--   0     1001      127      531 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/tests/mod.rs
+-rw-r--r--   0     1001      127    11010 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/tests/test_lexer.rs
+-rw-r--r--   0     1001      127    10398 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/tests/test_lexer_parser.rs
+-rw-r--r--   0     1001      127    39341 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/tests/test_parser.rs
+-rw-r--r--   0     1001      127     2126 2024-04-03 19:42:35.000000 turnip_text-0.0.5/src/util.rs
+-rw-r--r--   0     1001      127    11057 2024-04-03 19:42:35.000000 turnip_text-0.0.5/Cargo.lock
+-rw-r--r--   0     1001      127      787 2024-04-03 19:42:35.000000 turnip_text-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5184 1970-01-01 00:00:00.000000 turnip_text-0.0.5/PKG-INFO
```

### Comparing `turnip_text-0.0.4/Cargo.toml` & `turnip_text-0.0.5/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "turnip_text"
-version = "0.0.4"
+version = "0.0.5"
 description = "Document description language that allows embedded Python to describe document structure"
 license = "MIT OR Apache-2.0"
 authors = ["Samuel Stark"]
 edition = "2021"
 
 # "cdylib" is necessary to produce a shared library for Python to import from.
 #
```

### Comparing `turnip_text-0.0.4/.github/workflows/CI.yaml` & `turnip_text-0.0.5/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/Justfile` & `turnip_text-0.0.5/Justfile`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 	{{VENV_LOCATION}}/Scripts/Activate.ps1
 	just _test
 
 [unix]
 test:
 	#!/usr/bin/env bash
 	source {{VENV_LOCATION}}/bin/activate
+	export LD_LIBRARY_PATH="{{VENV_LOCATION}}/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}"
 	just _test
 
 _test:
 	# Make sure pip and maturin are installed/up-to-date in the venv
 	python -m pip install --upgrade pip
 	python -m pip install maturin
 
@@ -26,7 +27,23 @@
 	# python -m pip install . --use-feature=in-tree-build
 	maturin develop --extras=typing,test
 
 	# Run tests
 	cargo testall
 	mypy ./python/turnip_text --strict
 	pytest tests
+
+[windows]
+example:
+	#!powershell.exe
+	{{VENV_LOCATION}}/Scripts/Activate.ps1
+	just _example
+
+[unix]
+example:
+	#!/usr/bin/env bash
+	source {{VENV_LOCATION}}/bin/activate
+	just _example
+
+_example:
+	maturin develop --extras=typing,test
+	python ./examples/phdprop.py
```

### Comparing `turnip_text-0.0.4/LICENSE-APACHE` & `turnip_text-0.0.5/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/LICENSE-MIT` & `turnip_text-0.0.5/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/README.md` & `turnip_text-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/examples/experiment.pytext` & `turnip_text-0.0.5/examples/experiment.pytext`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/examples/phdprop.ttxt` & `turnip_text-0.0.5/examples/phdprop.ttext`

 * *Files 14% similar despite different names*

```diff
@@ -1,199 +1,206 @@
-[section("Introduction/Extended Abstract")]{
-    # 500-1000 words
+[[
+section=heading1
+subsection=heading2
+]]
 
-    # It should be comprehensible to an intelligent but non-expert audience 
-    # (Cambridge Trust Panels, for example) and so explain acronyms or leave them 
-    # out. 
-
-    # Talk about your idea’s wider application and why it is an important, exciting 
-    # topic to research.
-
-
-    CHERI[footnote]{See [url("https://www.cl.cam.ac.uk/research/security/ctsrd/cheri/")]} is a project within the Cambridge Computer Lab which adds fine-grained memory security to computer architecture.
-    Instead of allowing programs to access arbitrary memory locations, which malicious code can exploit to access data it shouldn't, CHERI requires that memory is accessed through unforgeable `capabilities'.
-    The computer hardware enforces that if a program receives a capability referring to a specific area of memory, the program cannot manipulate the capability to point outside that range.
-    When a capability is `dereferenced', e.g. the memory it points to is accessed, one can be sure that it points to valid memory the program is allowed to access.
-    This feature can resolve many security issues and bugs in modern programs, and industry seems to agree that CHERI is worthwhile. 
-    Arm Ltd have developed a test chip using these capabilities in collaboration with Cambridge, and CHERI overall is aiming for wide adoption.
-
-    CHERI initially focused on Central Processing Units (CPUs), the core elements of modern computers, and the CAPcelerate[footnote]{See [url("https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/V000381/1")]} sub-project (also at Cambridge) is now investigating capabilities for hardware accelerators such as Graphics Processing Units (GPUs).
-    While a modern computer may have eight to sixteen CPUs, which are flexible, GPUs have thousands of small less-flexible cores.
-    While GPUs were initially used for graphics, their high degree of parallelism is also useful for large-scale data processing such as Machine Learning (ML) in the cloud.
-    GPUs can hold data that's sensitive at small-scale (e.g. data for displaying personalized web pages) and at large-scale (e.g. audio data used for training speech recognition), and adding capabilities to GPUs help protect this data from attackers.
-    However, as the next section will show, CHERI's CPU-centric capabilities may need to adapt to work well with GPUs.
-
-    #----------------------
-    [subsection("Problem Definition", num=False)]{
-        Current systems that use CHERI capabilities make a few basic assumptions:
-
-        [enumerate]{
-            [item]{
-                Capabilities hold memory addresses that are controlled by the Operating System (OS) from the CPU
-
-                and I want to write a new paragraph!
-            }
-            [item]{
-                Capabilities have the same format
-            }
-            [item]{
-                Capabilities can be used in the same way from anywhere
-            }
-        }
-
-        This is reasonable for homogeneous multi-CPU systems, where memory is used in the same way by all elements, or systems where main memory is shared between the CPUs and GPUs.
-        However, high-performance external GPUs tend to use memory differently than CPUs, and could benefit from handling capabilities differently.
-        This would create two distinct `capability domains': that of the CPU and of the GPU.
-        My proposal is to investigate communication between different capability domains specifically in the context of differing CPU and GPU capabilities.
-        In the rest of this section I'll outline some of the CPU-GPU differences.
-
-        External GPUs typically have their own memory that can only be accessed by the CPU through PCIe (a relatively slow connection).
-        Instead of going through the CPU and operating system (OS), it's preferred to use direct GPU-to-GPU (e.g. NVLink) and GPU-to-device (GPUDirect) connections to transfer data.
-        For example, a cloud server may have a direct connection between a GPU and an NVMe storage device for transferring large ML datasets.
-        This principle is also extending to consumer devices with Microsoft DirectStorage, which reduces CPU overhead without entirely removing it, but this is much slower than the direct connections e.g. <10GB/s vs 100+GB/s.
-        Overall, it's clear the GPU can benefit from not relying on the OS to do e.g. memory allocation.
-
-        Unlike CPU programs, which can run for a long time, GPU tasks are often ephemeral.
-        Rendering (generating an image of a 3D scene) is split into many short-lived tasks, and ML inference (evaluating a model to make decisions about data) typically doesn't take very long.
-        This means the capabilities they hold only need to be valid for short amounts of time, and in some cases data itself can be short-lived.
-        This could inform a new approach to capability [emph]{revocation}, a complex problem on the CPU[footnote]{See [url("https://www.cl.cam.ac.uk/research/security/ctsrd/pdfs/2020oakland-cornucopia.pdf")]}, where capabilities could have a fixed lifetime instead of remaining valid forever.
-        Graphics tasks in particular expose simple units of lifetime, such as the number of frames rendered onscreen - a capability could only be valid for a fixed number of frames.
-        To exploit this for revocation, GPUs would need a unique representation of capabilities that may not be compatible with existing CPU representations.
-
-        GPUs support special memory transactions beyond simple reads and writes, such as [enquote]{texture reads} for graphics workloads.
-        These are more complex than memory accesses on the CPU, requiring dedicated hardware for performing filtering and decoding/decompressing image formats.
-        On top of this, the GPU is often allowed to choose the format of images based on the situation, rather than the programmer controlling it like on the CPU.
-        Because the GPU controls the image format, and has hardware to decode the format, allowing programs to read arbitrary bytes out of that data is unnecessary here.
-        Separating [enquote]{texture capabilities} from normal capabilities could enforce that these are accessed through correct hardware, but as this hardware isn't available on CPUs one would have to prevent CPUs from dereferencing them.
-    }
+[section()]{
+    Introduction/Extended Abstract
+}
+
+# 500-1000 words
+
+# It should be comprehensible to an intelligent but non-expert audience 
+# (Cambridge Trust Panels, for example) and so explain acronyms or leave them 
+# out. 
+
+# Talk about your idea’s wider application and why it is an important, exciting 
+# topic to research.
+
+
+CHERI[footnote]{See [url("https://www.cl.cam.ac.uk/research/security/ctsrd/cheri/")]} is a project within the Cambridge Computer Lab which adds fine-grained memory security to computer architecture.
+Instead of allowing programs to access arbitrary memory locations, which malicious code can exploit to access data it shouldn't, CHERI requires that memory is accessed through unforgeable `capabilities'.
+The computer hardware enforces that if a program receives a capability referring to a specific area of memory, the program cannot manipulate the capability to point outside that range.
+When a capability is `dereferenced', e.g. the memory it points to is accessed, one can be sure that it points to valid memory the program is allowed to access.
+This feature can resolve many security issues and bugs in modern programs, and industry seems to agree that CHERI is worthwhile. 
+Arm Ltd have developed a test chip using these capabilities in collaboration with Cambridge, and CHERI overall is aiming for wide adoption.
+
+CHERI initially focused on Central Processing Units (CPUs), the core elements of modern computers, and the CAPcelerate[footnote]{See [url("https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/V000381/1")]} sub-project (also at Cambridge) is now investigating capabilities for hardware accelerators such as Graphics Processing Units (GPUs).
+While a modern computer may have eight to sixteen CPUs, which are flexible, GPUs have thousands of small less-flexible cores.
+While GPUs were initially used for graphics, their high degree of parallelism is also useful for large-scale data processing such as Machine Learning (ML) in the cloud.
+GPUs can hold data that's sensitive at small-scale (e.g. data for displaying personalized web pages) and at large-scale (e.g. audio data used for training speech recognition), and adding capabilities to GPUs help protect this data from attackers.
+However, as the next section will show, CHERI's CPU-centric capabilities may need to adapt to work well with GPUs.
+
+#----------------------
+[subsection(num=False)]{
+    Problem Definition
+}
+
+Current systems that use CHERI capabilities make a few basic assumptions:
+
+[enumerate]{
+    [item]{
+        Capabilities hold memory addresses that are controlled by the Operating System (OS) from the CPU
 
-    #----------------------
-    [subsection("Potential Approach", num=False)]{
-        As shown above, GPU and CPU memory have different characteristics, and GPUs could benefit from having separate capability types.
-        However, even if these capability types could only be dereferenced on the GPU, they will need to be created or manipulated from the CPU - the gap between domains needs to be crossed.
-        I believe graphics-specific GPU drivers are a great place to start investigating this.
-
-        Rather than handing out addresses in GPU memory, graphics APIs usually deal in `resource IDs'.
-        The translation between resource IDs and GPU addresses is entirely delegated to the GPU driver, making it a natural starting point for adding domain-crossing.
-        As CAPcelerate is investigating, naive implementations of this model can be insecure, but this does not affect the principles of domain-crossing.
-        Once domain-crossing approaches have been developed in this context, they can be extended to support lower-level APIs.
+        and I want to write a new paragraph!
     }
+    [item]{
+        Capabilities have the same format
+    }
+    [item]{
+        Capabilities can be used in the same way from anywhere
+    }
+}
+
+This is reasonable for homogeneous multi-CPU systems, where memory is used in the same way by all elements, or systems where main memory is shared between the CPUs and GPUs.
+However, high-performance external GPUs tend to use memory differently than CPUs, and could benefit from handling capabilities differently.
+This would create two distinct `capability domains': that of the CPU and of the GPU.
+My proposal is to investigate communication between different capability domains specifically in the context of differing CPU and GPU capabilities.
+In the rest of this section I'll outline some of the CPU-GPU differences.
+
+External GPUs typically have their own memory that can only be accessed by the CPU through PCIe (a relatively slow connection).
+Instead of going through the CPU and operating system (OS), it's preferred to use direct GPU-to-GPU (e.g. NVLink) and GPU-to-device (GPUDirect) connections to transfer data.
+For example, a cloud server may have a direct connection between a GPU and an NVMe storage device for transferring large ML datasets.
+This principle is also extending to consumer devices with Microsoft DirectStorage, which reduces CPU overhead without entirely removing it, but this is much slower than the direct connections e.g. <10GB/s vs 100+GB/s.
+Overall, it's clear the GPU can benefit from not relying on the OS to do e.g. memory allocation.
+
+Unlike CPU programs, which can run for a long time, GPU tasks are often ephemeral.
+Rendering (generating an image of a 3D scene) is split into many short-lived tasks, and ML inference (evaluating a model to make decisions about data) typically doesn't take very long.
+This means the capabilities they hold only need to be valid for short amounts of time, and in some cases data itself can be short-lived.
+This could inform a new approach to capability [emph]{revocation}, a complex problem on the CPU[footnote]{See [url("https://www.cl.cam.ac.uk/research/security/ctsrd/pdfs/2020oakland-cornucopia.pdf")]}, where capabilities could have a fixed lifetime instead of remaining valid forever.
+Graphics tasks in particular expose simple units of lifetime, such as the number of frames rendered onscreen - a capability could only be valid for a fixed number of frames.
+To exploit this for revocation, GPUs would need a unique representation of capabilities that may not be compatible with existing CPU representations.
+
+GPUs support special memory transactions beyond simple reads and writes, such as [enquote]{texture reads} for graphics workloads.
+These are more complex than memory accesses on the CPU, requiring dedicated hardware for performing filtering and decoding/decompressing image formats.
+On top of this, the GPU is often allowed to choose the format of images based on the situation, rather than the programmer controlling it like on the CPU.
+Because the GPU controls the image format, and has hardware to decode the format, allowing programs to read arbitrary bytes out of that data is unnecessary here.
+Separating [enquote]{texture capabilities} from normal capabilities could enforce that these are accessed through correct hardware, but as this hardware isn't available on CPUs one would have to prevent CPUs from dereferencing them.
+
+#----------------------
+[subsection(num=False)]{
+    Potential Approach
 }
 
+As shown above, GPU and CPU memory have different characteristics, and GPUs could benefit from having separate capability types.
+However, even if these capability types could only be dereferenced on the GPU, they will need to be created or manipulated from the CPU - the gap between domains needs to be crossed.
+I believe graphics-specific GPU drivers are a great place to start investigating this.
+
+Rather than handing out addresses in GPU memory, graphics APIs usually deal in `resource IDs'.
+The translation between resource IDs and GPU addresses is entirely delegated to the GPU driver, making it a natural starting point for adding domain-crossing.
+As CAPcelerate is investigating, naive implementations of this model can be insecure, but this does not affect the principles of domain-crossing.
+Once domain-crossing approaches have been developed in this context, they can be extended to support lower-level APIs.
+
 #-------------------
-[section("Related Work")]{
-    While capabilities themselves haven't yet addressed domain-crossing, there is a vast amount of previous work for sharing memory with legacy pointers.
-    This section will highlight three broad topics that require domain crossing, which domain-crossing capability systems may need to be compatible with or build on.
-
-    # ------------------------------------
-    [subsection("DMA")]{
-        Modern System on Chips (SoCs) can contain much more than just CPUs and GPUs.
-        Mobile SoCs are a great example due to their high connectivity - custom hardware is included to support connections over mobile networks (4G/5G), Bluetooth, and Wi-Fi.
-        On top of these, extra accelerators can be included e.g. for AI processing \
-        [cite("qualcommSnapdragonGenMobile2021","kressinSnapdragon855Deep","samsungExynos980Release")].
-        Internally, these peripherals will often contain their own CPUs, potentially with vastly different parameters to the main CPUs on the SoC.
-        For example, Arm's Cortex R8 ([cite("armltdARMCortexR8Processor2016","armltdCortexR8")]) is a 32-bit processor for 5G modems, as well as hard-disk/SSD controllers, which has to interface with 64-bit systems (potentially with more than 4GB of addressable memory).
-
-        These peripherals are usually configured using special registers which are exposed to the CPU as addresses in the memory map.
-        The mapping of register to physical address is done statically at design time.
-        Software must either be recompiled for each SoC with different mappings, or use some dynamic runtime solution to understand which peripherals are mapped to which addresses.
-        Linux does the latter by parsing a SoC-specific device tree file at boot time[cite("linuxkernelLinuxAndTheDevicetree")].
-        Peripherals will store larger datasets, such as decoded Bluetooth audio signals, in their own internal buffers (essentially a separate [emph]{domain} to the rest of the system).
-        To access this data, the main CPU has to request a Direct Memory Access (DMA) from this buffer into main memory.
-
-        DMAs are performed by setting registers in a DMA Controller (DMAC) peripheral[footnote]{One such example is the Arm AMBA DMA-330 [cite("armltdAMBADMAController2009")]}, including the base address in the source and destination domains.
-        For a peripheral-to-memory transfer, the source address will be in the peripheral domain, and the destination address could be a physical address.
-        The DMAC then pulls data from the peripheral domain and writes it out to the physical main memory domain, pulling data across the domain boundary.
-        This is a very simple example of domain crossing for physically separated hardware domains, but it isn't enough for dynamic software domains.
-        For example, accessing peripherals from Virtual Machines (VMs) adds a layer of translation between the guest-domains and the host-domains.
-    }
+[section()]{
+    Related Work
+}
 
-    # ------------------------------------
-    [subsection("Virtualization")]{
-        When a VM tries to DMA data to/from a peripheral, it will specify a guest-domain address (guest-physical, or potentially guest-virtual) which needs to be translated into a host-physical address which the DMAC can use.
-        AMD[cite("amdAMDIOVirtualizationTechnology2021")], Arm[cite("armltdArmSMMUVer3")], and Intel[cite("intelIOMMUSpecRev3p3")] each have their own IOMMU (I/O Memory Management Unit) design which performs this translation dynamically.
-        Each device is assigned a page table, and devices can optionally be split into different domains with different tables.
-        The IOMMU can reuse page tables from the MMU, effectively granting peripherals the same permissions and address space as a specific process or VM.
-
-        Unfortunately, IOMMUs are only as secure as their configuration[footnote]{[cite("morganIOMMUProtectionAttacks2018","markuzeTrueIOMMUProtection2016")] are examples of IOMMU attacks relying on windows of misconfigured protection} can have high overheads.
-        An I/O TLB is essential to avoid walking the page table on every DMA operation, but it may not be large enough to handle high VM counts.
-        PCIe's Address Translation Service (ATS) takes a different approach, effectively distributing the IOTLB across PCIe devices[cite("pcisigAddressTranslationServices2009")].
-        The PCIe device consults the ATS for guest-to-host address translations, and stores them in an internal cache.
-        When it sends a DMA request, it applies a cached translation.
-        # itself
-        # already-translated host-domain physical address.
-        The downside of this approach is that the system must trust the translated addresses the PCIe device spits back out, and trusting external peripherals is not always a good idea[cite("markettosThunderclapExploringVulnerabilities2019")].
-        [cite("markettosPositionPaperDefending2020")] proposes CHERI-based alternatives to better protect the system from peripherals.
-        # Of course, all of this work only protects main memory from peripherals, and not peripherals from the rest of the system.
-        Peripherals that include their own external memory, like GPUs or network accelerators, still need to protect themselves from the rest of the system.
-
-        # External GPUs that are multiplexed across multiple VMs, e.g. used by multiple VMs concurrently, can protect those VMs from each other by implementing PCIe Single-Root I/O Virtualization (SR-IOV).
-        External GPUs that are used by multiple VMs concurrently can protect those VMs from each other by implementing PCIe Single-Root I/O Virtualization (SR-IOV)[cite("intelPCISIGSingleRoot2008")].
-        The GPU exposes a single Physical Function (PF) to the hypervisor, which controls the whole device.
-        Each guest VM is then given a different Virtual Function (VF) connected to the original PF, controlling a subset of the device.
-        This system allows data transfer between the VF and the VM to avoid passing through the hypervisor stack, which is faster, but the GPUs still have to ensure the VFs they expose are correctly isolated.
-
-        Modern GPUs use physical hardware segmentation and software support to effectively partition VMs from each other.
-        AMD's MxGPU virtualization physically segments GPU memory and gives each VM a timeslice during which only their partition is active[cite("amdAMDApproachGPU2017")].
-        When using SR-IOV, Nvidia's vGPU technology physically segments both the memory and the actual computation units, to avoid side-channel attacks, and allows multiple VMs to execute on different partitions at once.
-        Integrated GPUs (e.g. Arm Mali GPUs, packaged on the same SoC as the CPU) don't necessarily use SR-IOV, but do isolate resources similarly[cite("armltdArmMaliG78AEProduct2020")].
-    }
+While capabilities themselves haven't yet addressed domain-crossing, there is a vast amount of previous work for sharing memory with legacy pointers.
+This section will highlight three broad topics that require domain crossing, which domain-crossing capability systems may need to be compatible with or build on.
 
-    # ------------------------------------
-    [subsection("GPU Virtual Memory")]{
-        On top of isolating VMs from each other, a further level of translation is added on the GPU side: Nvidia and AMD external GPUs have their own dedicated MMUs for virtual-to-physical address translation.
-        This is in large part due to the idea of [enquote]{Shared Virtual Memory} (SVM), where the CPU and GPU share an address space, and pointers to SVM can be seamlessly dereferenced on both.
-        OpenCL~2.0 and Nvidia's CUDA APIs both support this concept [cite("intelOpenCLSharedVirtual2014","nvidiacorporationUnifiedMemoryCUDA2017")] to varying degrees.
-
-        In most cases, SVM has to be allocated through special API functions (e.g. CUDA Managed Memory, OpenCL Buffer Memory) and coherence is coarse: on CUDA, SVM pages are dynamically migrated between the CPU and GPU on-demand, rather than synchronizing individual loads and stores.
-        This means page tables on CUDA devices track the [enquote]{Aperture} of each page, denoting which memory the page currently occupies[cite("nvidiacorporationPascalMMUFormat2016")].
-        Not content with this, Nvidia and AMD are pushing for more granular coherence and increasing memory sharing.
-
-        In the HPC space, some systems connect the CPU and GPU using Nvidia's proprietary NVLINK connection standard, rather than PCIe [cite("ibmpower9nputeamFunctionalityPerformanceNVLink2018")].
-        These connections have much higher bandwidth, and allow for coherence at the cache-line granularity on SVM [cite(("nvidiacorporationCUDAProgrammingGuide", "N.1.7"))] and directly accessing CPU page tables from the GPU [cite(("nvidiacorporationCUDAProgrammingGuide", "N.1.6"))].
-        The latter is only available on IBM Power9 systems, but expands SVM to [emph]{all memory in the system}, not just memory specifically allocated by CUDA.
-        On more conventional PCIe based systems, this isn't yet possible, and drivers have to manually synchronize the GPU and CPU MMUs.
-        Linux has introduced a Heterogeneous Memory Management kernel module[cite("linuxkernelHeterogeneousMemoryManagement","hubbardGPUsHMMHeterogeneous2017")] to make this process easier, and it's currently used by the unofficial Nouveau drivers for Nvidia GPUs[cite("larabelMesa20Nouveau2020")] and the official AMD ROCm drivers[cite("larabelRadeonROCmReleased2021")].
-
-        Nvidia's Arm-based Tegra SoCs take a different approach where both the CPU and GPU use the same System MMU and DRAM[cite("nvidiacorporationNVIDIAJetsonTX22017")].
-        This is also done on SoCs with Arm GPUs[cite("armltdMemoryManagementEmbedded2013")].
-        On Tegra, GPUs can also snoop the CPU cache without using NVLink[cite(("nvidiacorporationS8868CUDAXavier2018", r"Slide~24"))], which they call I/O Coherency.
-
-        The computing industry as a whole is leaning towards unifying device-attached memory with processor memory.
-        CXL[cite("cxlconsortiumComputeExpressLink2021")] is a standardized protocol from Intel built on PCIe which uses three sub-protocols (CXL.io, CXL.cache, CXL.memory) to allow fine-grained coherence between device and host memory.
-        # coherent device-to-processor-memory and processor-to-device-memory accesses, including allowing the device to cache processor memory.
-        This is a promising protocol, and it has the backing of Nvidia, AMD, and Arm.
-        It may become more relevant for GPUs in the future, but for now at least Nvidia has no reason to move away from NVLink.
-        It also hasn't yet been widely implemented.
-        The first Intel CPUs to support it (Sapphire Rapids microarchitecture [cite(("intelAcceleratingPossibilitiesHPC2021", r"Slide~16"))]) are due to come out in 2022 [cite("intelUpdatesIntelNextGen2021")].
-
-        The idea of a coherent, unified address space and view of memory across all devices is compelling, especially given the convenience it affords some software.
-        However, if not applied with care, it could compromise security and performance.
-        If the GPU can now access the entire virtual address space for a process, it becomes an attack surface for exposing sensitive data that was previously CPU-only.
-        Additionally, while a unified address space does benefit pointer-heavy compute work such as graph workloads, current graphics APIs have little to gain:
-        they already abstract the concept of GPU pointers away in favor of e.g. resource IDs, and many modern game engines rely on careful control of which data is sent to the GPU and when.
-        Recent graph programs [cite("wangGrusUnifiedmemoryefficientHighperformance2021","minEMOGIEfficientMemoryaccess2021")] have even reported performance issues with automatic page migration, relying on carefully configuring or entirely disabling it to regain performance.
-
-        To be clear, low-end SoCs with shared CPU-GPU memory can benefit from unifying accesses as much as possible, because it mirrors the underlying hardware.
-        However, desktop and server systems will use external GPUs with dedicated memory for a while yet, and as long as that's the case translating between the CPU-GPU domains will be important.
-        This dichotomy between a unified view and a more performant, domain-aware view will remain in place for the foreseeable future, and if CHERI is going to reach widespread adoption it needs to be able to handle it.
-    }
+# ------------------------------------
+[subsection()]{
+    DMA
 }
 
-#-------------------------
-[section("First-Year Plan")]{
-    The first year of the PhD will focus on reducing the broad idea of diverging CPU/GPU capabilities to a concrete set of potential approaches.
-    This problem space is bounded by two restrictions: how current drivers and programming models use pointers, and how the CPU and GPU domains are separated in hardware.
-    Indeed, integrated and external GPUs may require entirely different approaches.
-    On top of this, CHERI's preestablished utility for compartmentalization[cite("watsonCHERIHybridCapabilitySystem2015")] may make GPU virtualization easier.
-    Recently [citeauthor("markettosPositionPaperDefending2020")] investigated using CHERI capabilities to protect DMA accesses[cite("markettosPositionPaperDefending2020")], briefly considering shared memory but not allowing capabilities to flow/be dereferenced across domains.
-    My work should build on this.
-
-    With the above in mind, I have identified four goals to achieve before writing the first-year report.
-    First, I will study the flow for accessing external memory across PCIe, including address translation for virtualized GPUs, then I will see how this changes with a more unified address space provided by CXL.
-    Next, I will investigate open-source drivers for Arm Mali (e.g. integrated) and Nvidia/AMD (e.g. external) GPUs, to see how they use pointers and how they implement their semi-unified address spaces.
-    Finally, based on this background I will define two preliminary split CPU/GPU capability domains.
-    These will serve to expose any unforeseen issues with split domains and CHERI capabilities.
-    After reporting on this progress, I will start experimenting with the split domains, potentially using a graphics API model as described above.
+Modern System on Chips (SoCs) can contain much more than just CPUs and GPUs.
+Mobile SoCs are a great example due to their high connectivity - custom hardware is included to support connections over mobile networks (4G/5G), Bluetooth, and Wi-Fi.
+On top of these, extra accelerators can be included e.g. for AI processing \
+[cite("qualcommSnapdragonGenMobile2021","kressinSnapdragon855Deep","samsungExynos980Release")].
+Internally, these peripherals will often contain their own CPUs, potentially with vastly different parameters to the main CPUs on the SoC.
+For example, Arm's Cortex R8 ([cite("armltdARMCortexR8Processor2016","armltdCortexR8")]) is a 32-bit processor for 5G modems, as well as hard-disk/SSD controllers, which has to interface with 64-bit systems (potentially with more than 4GB of addressable memory).
+
+These peripherals are usually configured using special registers which are exposed to the CPU as addresses in the memory map.
+The mapping of register to physical address is done statically at design time.
+Software must either be recompiled for each SoC with different mappings, or use some dynamic runtime solution to understand which peripherals are mapped to which addresses.
+Linux does the latter by parsing a SoC-specific device tree file at boot time[cite("linuxkernelLinuxAndTheDevicetree")].
+Peripherals will store larger datasets, such as decoded Bluetooth audio signals, in their own internal buffers (essentially a separate [emph]{domain} to the rest of the system).
+To access this data, the main CPU has to request a Direct Memory Access (DMA) from this buffer into main memory.
+
+DMAs are performed by setting registers in a DMA Controller (DMAC) peripheral[footnote_ref("amba_example")], including the base address in the source and destination domains.
+For a peripheral-to-memory transfer, the source address will be in the peripheral domain, and the destination address could be a physical address.
+The DMAC then pulls data from the peripheral domain and writes it out to the physical main memory domain, pulling data across the domain boundary.
+This is a very simple example of domain crossing for physically separated hardware domains, but it isn't enough for dynamic software domains.
+For example, accessing peripherals from Virtual Machines (VMs) adds a layer of translation between the guest-domains and the host-domains.
+
+[footnote_text("amba_example")]{
+    One such example is the Arm AMBA DMA-330 [cite("armltdAMBADMAController2009")]
+}
 
-    # TODO plan
-}
+# ------------------------------------
+[subsection()]{
+    Virtualization
+}
+
+When a VM tries to DMA data to/from a peripheral, it will specify a guest-domain address (guest-physical, or potentially guest-virtual) which needs to be translated into a host-physical address which the DMAC can use.
+AMD[cite("amdAMDIOVirtualizationTechnology2021")], Arm[cite("armltdArmSMMUVer3")], and Intel[cite("intelIOMMUSpecRev3p3")] each have their own IOMMU (I/O Memory Management Unit) design which performs this translation dynamically.
+Each device is assigned a page table, and devices can optionally be split into different domains with different tables.
+The IOMMU can reuse page tables from the MMU, effectively granting peripherals the same permissions and address space as a specific process or VM.
+
+Unfortunately, IOMMUs are only as secure as their configuration[footnote]{[cite("morganIOMMUProtectionAttacks2018","markuzeTrueIOMMUProtection2016")] are examples of IOMMU attacks relying on windows of misconfigured protection} can have high overheads.
+An I/O TLB is essential to avoid walking the page table on every DMA operation, but it may not be large enough to handle high VM counts.
+PCIe's Address Translation Service (ATS) takes a different approach, effectively distributing the IOTLB across PCIe devices[cite("pcisigAddressTranslationServices2009")].
+The PCIe device consults the ATS for guest-to-host address translations, and stores them in an internal cache.
+When it sends a DMA request, it applies a cached translation.
+# itself
+# already-translated host-domain physical address.
+The downside of this approach is that the system must trust the translated addresses the PCIe device spits back out, and trusting external peripherals is not always a good idea[cite("markettosThunderclapExploringVulnerabilities2019")].
+[cite("markettosPositionPaperDefending2020")] proposes CHERI-based alternatives to better protect the system from peripherals.
+# Of course, all of this work only protects main memory from peripherals, and not peripherals from the rest of the system.
+Peripherals that include their own external memory, like GPUs or network accelerators, still need to protect themselves from the rest of the system.
+
+# External GPUs that are multiplexed across multiple VMs, e.g. used by multiple VMs concurrently, can protect those VMs from each other by implementing PCIe Single-Root I/O Virtualization (SR-IOV).
+External GPUs that are used by multiple VMs concurrently can protect those VMs from each other by implementing PCIe Single-Root I/O Virtualization (SR-IOV)[cite("intelPCISIGSingleRoot2008")].
+The GPU exposes a single Physical Function (PF) to the hypervisor, which controls the whole device.
+Each guest VM is then given a different Virtual Function (VF) connected to the original PF, controlling a subset of the device.
+This system allows data transfer between the VF and the VM to avoid passing through the hypervisor stack, which is faster, but the GPUs still have to ensure the VFs they expose are correctly isolated.
+
+Modern GPUs use physical hardware segmentation and software support to effectively partition VMs from each other.
+AMD's MxGPU virtualization physically segments GPU memory and gives each VM a timeslice during which only their partition is active[cite("amdAMDApproachGPU2017")].
+When using SR-IOV, Nvidia's vGPU technology physically segments both the memory and the actual computation units, to avoid side-channel attacks, and allows multiple VMs to execute on different partitions at once.
+Integrated GPUs (e.g. Arm Mali GPUs, packaged on the same SoC as the CPU) don't necessarily use SR-IOV, but do isolate resources similarly[cite("armltdArmMaliG78AEProduct2020")].
+
+# ------------------------------------
+[subsection()]{
+    GPU Virtual Memory
+}
+
+On top of isolating VMs from each other, a further level of translation is added on the GPU side: Nvidia and AMD external GPUs have their own dedicated MMUs for virtual-to-physical address translation.
+This is in large part due to the idea of [enquote]{Shared Virtual Memory} (SVM), where the CPU and GPU share an address space, and pointers to SVM can be seamlessly dereferenced on both.
+OpenCL~2.0 and Nvidia's CUDA APIs both support this concept [cite("intelOpenCLSharedVirtual2014","nvidiacorporationUnifiedMemoryCUDA2017")] to varying degrees.
+
+In most cases, SVM has to be allocated through special API functions (e.g. CUDA Managed Memory, OpenCL Buffer Memory) and coherence is coarse: on CUDA, SVM pages are dynamically migrated between the CPU and GPU on-demand, rather than synchronizing individual loads and stores.
+This means page tables on CUDA devices track the [enquote]{Aperture} of each page, denoting which memory the page currently occupies[cite("nvidiacorporationPascalMMUFormat2016")].
+Not content with this, Nvidia and AMD are pushing for more granular coherence and increasing memory sharing.
+
+In the HPC space, some systems connect the CPU and GPU using Nvidia's proprietary NVLINK connection standard, rather than PCIe [cite("ibmpower9nputeamFunctionalityPerformanceNVLink2018")].
+These connections have much higher bandwidth, and allow for coherence at the cache-line granularity on SVM [cite("nvidiacorporationCUDAProgrammingGuide")]{N.1.7} and directly accessing CPU page tables from the GPU [cite("nvidiacorporationCUDAProgrammingGuide")]{N.1.6}.
+The latter is only available on IBM Power9 systems, but expands SVM to [emph]{all memory in the system}, not just memory specifically allocated by CUDA.
+On more conventional PCIe based systems, this isn't yet possible, and drivers have to manually synchronize the GPU and CPU MMUs.
+Linux has introduced a Heterogeneous Memory Management kernel module[cite("linuxkernelHeterogeneousMemoryManagement","hubbardGPUsHMMHeterogeneous2017")] to make this process easier, and it's currently used by the unofficial Nouveau drivers for Nvidia GPUs[cite("larabelMesa20Nouveau2020")] and the official AMD ROCm drivers[cite("larabelRadeonROCmReleased2021")].
+
+Nvidia's Arm-based Tegra SoCs take a different approach where both the CPU and GPU use the same System MMU and DRAM[cite("nvidiacorporationNVIDIAJetsonTX22017")].
+This is also done on SoCs with Arm GPUs[cite("armltdMemoryManagementEmbedded2013")].
+On Tegra, GPUs can also snoop the CPU cache without using NVLink[cite("nvidiacorporationS8868CUDAXavier2018")]{Slide~24}, which they call I/O Coherency.
+
+The computing industry as a whole is leaning towards unifying device-attached memory with processor memory.
+CXL[cite("cxlconsortiumComputeExpressLink2021")] is a standardized protocol from Intel built on PCIe which uses three sub-protocols (CXL.io, CXL.cache, CXL.memory) to allow fine-grained coherence between device and host memory.
+# coherent device-to-processor-memory and processor-to-device-memory accesses, including allowing the device to cache processor memory.
+This is a promising protocol, and it has the backing of Nvidia, AMD, and Arm.
+It may become more relevant for GPUs in the future, but for now at least Nvidia has no reason to move away from NVLink.
+It also hasn't yet been widely implemented.
+The first Intel CPUs to support it (Sapphire Rapids microarchitecture [cite("intelAcceleratingPossibilitiesHPC2021")]{Slide~16}) are due to come out in 2022 [cite("intelUpdatesIntelNextGen2021")].
+
+The idea of a coherent, unified address space and view of memory across all devices is compelling, especially given the convenience it affords some software.
+However, if not applied with care, it could compromise security and performance.
+If the GPU can now access the entire virtual address space for a process, it becomes an attack surface for exposing sensitive data that was previously CPU-only.
+Additionally, while a unified address space does benefit pointer-heavy compute work such as graph workloads, current graphics APIs have little to gain:
+they already abstract the concept of GPU pointers away in favor of e.g. resource IDs, and many modern game engines rely on careful control of which data is sent to the GPU and when.
+Recent graph programs [cite("wangGrusUnifiedmemoryefficientHighperformance2021","minEMOGIEfficientMemoryaccess2021")] have even reported performance issues with automatic page migration, relying on carefully configuring or entirely disabling it to regain performance.
+
+To be clear, low-end SoCs with shared CPU-GPU memory can benefit from unifying accesses as much as possible, because it mirrors the underlying hardware.
+However, desktop and server systems will use external GPUs with dedicated memory for a while yet, and as long as that's the case translating between the CPU-GPU domains will be important.
+This dichotomy between a unified view and a more performant, domain-aware view will remain in place for the foreseeable future, and if CHERI is going to reach widespread adoption it needs to be able to handle it.
+
+#-------------------------
+[subfile("phdprop_subfile_first_year_plan.ttext")]
```

### Comparing `turnip_text-0.0.4/notes/analysis/asciidoctor.md` & `turnip_text-0.0.5/notes/analysis/asciidoctor.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/notes/code_syntax.md` & `turnip_text-0.0.5/notes/code_syntax.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 ## TODO
 - DONE Allow scopeless eval-brackets at the starts of paragraphs to return things fitting Block and inject them directly into the document. (This behaviour already works for Inline)
   - NOTDONE Don't allow subsequent text to start a new paragraph - e.g. `[block_expr] some extra text` shouldn't be valid
 - DONE Allow scopeless eval-brackets to return None and do no emitting
 - DONE Support assignment and recall `[x=5] \n\n [UnescapedText(x)]` -> "5"
 - DONE Better raw-scope-owning behaviour: maybe a raw-scope-owner is just something with a function that takes str? and can return either Block or Inline, and the parser adapts to this? (See above)
-- Add a context variable to all(?) plugin functions, so they can call out to other functions without knowing
+- DONE Add a context variable to all(?) plugin functions, so they can call out to other functions without knowing
+- Figure out how properties work!!! If you're going to invoke the dict directly, using properties requires `__get__`.
+  We originally thought it would be bad to evaluate properties because they might be impure, and @stateful properties are *very* impure.
+  That's because @stateful checks doc.frozen to see if it's allowed to run.
+  But we don't need it if you just delete the ability to call those functions when the document is frozen!
+  Throwing away the stateful side of the doc plugins is effectively equivalent: so maybe we can count all @stateful/@stateless properties as pure and evaluate them once for the document dict, even if @stateful would not be pure when the document is frozen, because those evaluations are thrown away once the document is parsed.
+  NOTE: This requires the DocState to actually be thrown away :))))) which we currently don't do because it has functions for pulling out floats.
 
 ## Current syntax
 
 Code exists in two contexts: block-level and inline-level.
 If an eval-bracket `[]` is opened outside of a paragraph, the contents are evaluated and two checks are performed:
   - if the result fits the `BlockScopeOwner` typeclass, it is expected that the eval brackets will be followed by a block scope (opened with squiggly brace + newline). The eval-result will be called with the contents of that scope (TODO when the block scope is closed), and *that* result will be `render()`-ed in the finalization phase.
```

### Comparing `turnip_text-0.0.4/notes/content_v_formatting.md` & `turnip_text-0.0.5/notes/content_v_formatting.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/notes/labels.md` & `turnip_text-0.0.5/notes/labels.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/notes/opinionated_text.md` & `turnip_text-0.0.5/notes/opinionated_text.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/notes/pandoc.md` & `turnip_text-0.0.5/notes/pandoc.md`

 * *Files identical despite different names*

### Comparing `turnip_text-0.0.4/pyproject.toml` & `turnip_text-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "turnip_text"
-version = "0.0.4"
+version = "0.0.5"
 description = "Document description language that allows embedded Python to describe document structure"
 license = { text = "MIT OR Apache-2.0" }
 readme = "README.md"
 authors = [{ name = "Samuel Stark", email = "popgoestoast@gmail.com" }]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `turnip_text-0.0.4/python/turnip_text/__init__.py` & `turnip_text-0.0.5/python/turnip_text/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,100 @@
 import abc
-from typing import List, Optional, Protocol, Union, runtime_checkable
+from typing import (
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Protocol,
+    Sequence,
+    Union,
+    runtime_checkable,
+)
 
 __all__ = [
     "Block",
     "BlockScope",
     "Inline",
     "InlineScope",
     "Paragraph",
     "RawText",
     "Sentence",
     "UnescapedText",
+    "coerce_to_block",
     "coerce_to_block_scope",
+    "coerce_to_inline",
     "coerce_to_inline_scope",
     "BlockScopeBuilder",
     "InlineScopeBuilder",
     "RawScopeBuilder",
     "CoercibleToInline",
     "CoercibleToInlineScope",
     "CoercibleToBlock",
     "CoercibleToBlockScope",
     "parse_file_native",
-    "parse_str_native",
+    "InsertedFile",
 ]
 
 from ._native import (  # type: ignore
     BlockScope,
+    DocSegment,
     InlineScope,
+    InsertedFile,
     Paragraph,
     RawText,
     Sentence,
     UnescapedText,
+    coerce_to_block,
     coerce_to_block_scope,
+    coerce_to_inline,
     coerce_to_inline_scope,
 )
 from ._native import parse_file as parse_file_native
-from ._native import parse_str as parse_str_native
 
 
 @runtime_checkable
 class Inline(Protocol):
     is_inline: bool = True
 
 
 @runtime_checkable
 class Block(Protocol):
     is_block: bool = True
 
 
+@runtime_checkable
+class DocSegmentHeader(Protocol):
+    is_segment_header: bool = True
+    weight: int = 0
+
+
 class BlockScopeBuilder(abc.ABC):
     @abc.abstractmethod
-    def build_from_blocks(self, bs: BlockScope) -> Optional[Block]:
+    def build_from_blocks(self, bs: BlockScope) -> Optional[Block | DocSegmentHeader]:
         ...
 
-    def __matmul__(self, maybe_b: 'CoercibleToBlockScope') -> Optional[Block]:
+    def __matmul__(
+        self, maybe_b: "CoercibleToBlockScope"
+    ) -> Optional[Block | DocSegmentHeader]:
         bs = coerce_to_block_scope(maybe_b)
         return self.build_from_blocks(bs)
 
 
 class InlineScopeBuilder(abc.ABC):
     @abc.abstractmethod
-    def build_from_inlines(self, inls: InlineScope) -> Inline:
+    def build_from_inlines(self, inls: InlineScope) -> Inline | DocSegmentHeader:
         ...
 
-    def __matmul__(self, maybe_inls: 'CoercibleToInlineScope') -> Inline:
+    def __matmul__(
+        self, maybe_inls: "CoercibleToInlineScope"
+    ) -> Inline | DocSegmentHeader:
         inls = coerce_to_inline_scope(maybe_inls)
         return self.build_from_inlines(inls)
-    
+
+
 @runtime_checkable
 class RawScopeBuilder(Protocol):
     def build_from_raw(self, raw: str) -> Union[Inline, Block]:
         ...
 
 
 # The types that can be coerced into an Inline, in the order they are checked and attempted.
@@ -87,7 +112,15 @@
 # The types that can be coerced into a Block, in the order they are checked and attempted
 CoercibleToBlock = Union[
     List[Block], Block, Paragraph, Sentence, CoercibleToInlineScope
 ]
 
 # The types that can be coerced into a BlockScope, in the order they are checked and attempted
 CoercibleToBlockScope = Union[BlockScope, CoercibleToBlock]
+
+
+def join_inlines(inlines: Iterable[Inline], joiner: Inline) -> InlineScope:
+    """Equivalent of string.join, but for joining any set of Inlines with a joiner Inline"""
+    new_inlines = [val for i in inlines for val in (i, joiner)]
+    if new_inlines:
+        new_inlines.pop()
+    return InlineScope(new_inlines)
```

### Comparing `turnip_text-0.0.4/python/turnip_text/helpers.py` & `turnip_text-0.0.5/python/turnip_text/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import Any, Callable, List, Optional, Union
+from typing import Any, Callable, List, Optional, TypeVar, Union
 
 from turnip_text import (
     Block,
     BlockScope,
     BlockScopeBuilder,
-    CoercibleToBlockScope,
-    CoercibleToInlineScope,
+    CoercibleToInline,
+    DocSegmentHeader,
     Inline,
     InlineScope,
     InlineScopeBuilder,
+    Paragraph,
     RawScopeBuilder,
-    coerce_to_block_scope,
-    coerce_to_inline_scope,
+    Sentence,
+    coerce_to_inline,
 )
 
 # TODO tests for the helpers
 
 
 class block_scope_builder(BlockScopeBuilder):
     """
@@ -38,20 +39,22 @@
 
     It also supports the matmul operator, which tries to coerce the right-hand-side into a BlockScope before calling the function:
     ```python
     block(name="greg") @ "The contents of greg"
     ```
     """
 
-    func: Callable[[BlockScope], Optional[Block]]
+    func: Callable[[BlockScope], Optional[Block | DocSegmentHeader]]
 
-    def __init__(self, func: Callable[[BlockScope], Optional[Block]]) -> None:
+    def __init__(
+        self, func: Callable[[BlockScope], Optional[Block | DocSegmentHeader]]
+    ) -> None:
         self.func = func
 
-    def build_from_blocks(self, b: BlockScope) -> Optional[Block]:
+    def build_from_blocks(self, b: BlockScope) -> Optional[Block | DocSegmentHeader]:
         return self.func(b)
 
 
 class inline_scope_builder(InlineScopeBuilder):
     """
     Decorator which allows a function to fit the InlineScopeBuilder typeclass.
 
@@ -114,7 +117,24 @@
 
     def __matmul__(self, maybe_str: Any) -> Union[Block, Inline]:
         if isinstance(maybe_str, str):
             return self.func(maybe_str)
         raise TypeError(
             f"Invoked RawScopeBuilder on {maybe_str}, which wasn't a string"
         )
+
+
+def paragraph_of(i: CoercibleToInline) -> Paragraph:
+    return Paragraph([Sentence([coerce_to_inline(i)])])
+
+
+class Unset:
+    def __eq__(self, __value: object) -> bool:
+        if isinstance(__value, Unset):
+            return True
+        return False
+
+
+UNSET = Unset()
+
+T = TypeVar("T")
+MaybeUnset = Union[T, Unset]
```

### Comparing `turnip_text-0.0.4/python/turnip_text/renderers/latex/plugins.py` & `turnip_text-0.0.5/python/turnip_text/render/latex/std_plugins.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,432 +1,282 @@
-import uuid
-from dataclasses import dataclass
-from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union, cast
-
-from turnip_text import (
-    Block,
-    BlockScope,
-    BlockScopeBuilder,
-    Inline,
-    InlineScope,
-    InlineScopeBuilder,
-    Paragraph,
-    Sentence,
-    UnescapedText,
-)
-from turnip_text.helpers import block_scope_builder, inline_scope_builder
-from turnip_text.renderers import (
-    CustomEmitDispatch,
-    MutableState,
-    Plugin,
-    Renderer,
-    StatelessContext,
-    stateful,
-    stateless,
-)
-from turnip_text.renderers.std_plugins import (
-    CitationPluginInterface,
-    CiteKey,
-    FootnotePluginInterface,
-    FormatPluginInterface,
-    SectionPluginInterface,
-)
-
-from .base import LatexRenderer, RawLatex
-
-CiteKeyWithOptionNote = Tuple[CiteKey, Optional[UnescapedText]]
-
-
-@dataclass(frozen=True)
-class FootnoteAnchor(Inline):
-    label: str
-
-
-@dataclass(frozen=True)
-class HeadedBlock(Block):
-    latex_name: str
-    name: UnescapedText
-    contents: BlockScope
-    label: Optional[str] = None
-    num: bool = True
-
-
-@dataclass(frozen=True)
-class Citation(Inline):
-    # List of (label, note?)
-    labels: List[CiteKeyWithOptionNote]
+from typing import Dict, Iterator, List, Optional
 
-
-@dataclass(frozen=True)
-class NamedUrl(Inline, InlineScopeBuilder):
-    url: str
-    name: Optional[InlineScope] = None
-
-    def build_from_inlines(self, inls: InlineScope) -> Inline:
-        assert self.name is None
-        return NamedUrl(self.url, inls)
-
-
-@dataclass(frozen=True)
-class DisplayList(Block):
-    # TODO allow nested lists
-    # items: List[Union[BlockNode, List]]
-    items: List["DisplayListItem"]
-    mode: str
-
-
-@dataclass(frozen=True)
-class DisplayListItem(Block):
-    item: Block
-
-
-@dataclass(frozen=True)
-class Formatted(Inline):
-    format_type: str  # e.g. "emph"
-    items: InlineScope
+from turnip_text import BlockScope, DocSegment
+from turnip_text.doc import FormatContext
+from turnip_text.doc.std_plugins import (
+    Bibliography,
+    Citation,
+    CiteAuthor,
+    DisplayList,
+    DisplayListItem,
+    DisplayListType,
+    FootnoteContents,
+    FootnoteRef,
+    InlineFormatted,
+    InlineFormattingType,
+    NamedUrl,
+    StructureBlockHeader,
+)
+from turnip_text.render import RenderPlugin
+from turnip_text.render.latex.backrefs import LatexBackrefMethod
+from turnip_text.render.latex.renderer import LatexCounterStyle, LatexRenderer
+from turnip_text.render.latex.setup import LatexCounterDecl, LatexSetup
+from turnip_text.render.manual_numbering import SimpleCounterFormat
+
+LatexPlugin = RenderPlugin[LatexRenderer, LatexSetup]
+
+
+def STD_LATEX_ARTICLE_RENDER_PLUGINS(
+    use_chapters: bool,
+    indent_list_items: bool = True,
+    requested_counter_links: Optional[Dict[Optional[str], str]] = None,
+) -> List[LatexPlugin]:
+    return [
+        ArticleRenderPlugin(use_chapters),
+        UncheckedBiblatexRenderPlugin(),
+        FootnoteRenderPlugin(),
+        ListRenderPlugin(indent_list_items),
+        InlineFormatRenderPlugin(),
+        UrlRenderPlugin(),
+    ]
 
 
-class LatexCitationPlugin(Plugin[LatexRenderer], CitationPluginInterface):
-    # TODO require biblatex
+class ArticleRenderPlugin(LatexPlugin):
+    level_to_latex: List[Optional[str]]
 
-    _citations: Dict[str, Any]
+    # TODO this might need to enable \part?
 
-    def __init__(self) -> None:
+    def __init__(self, use_chapters: bool) -> None:
         super().__init__()
+        if use_chapters:
+            self.level_to_latex = [
+                None,
+                "chapter",
+                "section",
+                "subsection",
+                "subsubsection",
+            ]
+        else:
+            self.level_to_latex = [None, "section", "subsection", "subsubsection"]
 
-        # TODO load citations from somewhere
-        self._citations = {}
-
-    def _add_emitters(self, handler: CustomEmitDispatch[LatexRenderer]) -> None:
-        handler.add_custom_inline(Citation, self._emit_citation)
+    def _register(self, setup: LatexSetup) -> None:
+        setup.reqire_document_class("article")
+        # TODO enable more backref methods
+        backref_methods = (LatexBackrefMethod.Cleveref, LatexBackrefMethod.Hyperlink)
+        # Declare the preexisting LaTeX counters
+        counters = [
+            (None, "part"),
+            ("part", "chapter"),
+            ("chapter", "section"),
+            ("section", "subsection"),
+            ("subsection", "subsubsection"),
+        ]
+        for parent, counter in counters:
+            setup.declare_latex_counter(
+                counter,
+                LatexCounterDecl(
+                    provided_by_docclass_or_package=True,
+                    default_reset_latex_counter=parent,
+                    fallback_fmt=SimpleCounterFormat(counter, LatexCounterStyle.Arabic),
+                ),
+                backref_methods,
+            )
+        # Map the turnip_text counters to the LaTeX counter
+        for i in [1, 2, 3, 4]:
+            tt_counter = f"h{i}"
+            if i < len(self.level_to_latex):
+                latex_counter = self.level_to_latex[i]
+                if latex_counter is not None:
+                    setup.declare_tt_counter(tt_counter, latex_counter)
 
-    def _postamble_handlers(self) -> Iterable[Tuple[str, Callable[[LatexRenderer], None]]]:
-        return ((self._BIBLIOGRAPHY_POSTAMBLE_ID, self._emit_bibliography),)
+        setup.emitter.register_header(StructureBlockHeader, self._emit_structure)
 
-    def _emit_citation(
+    def _emit_structure(
         self,
+        head: StructureBlockHeader,
+        contents: BlockScope,
+        subsegments: Iterator[DocSegment],
         renderer: LatexRenderer,
-        ctx: StatelessContext[LatexRenderer],
-        citation: Citation,
+        ctx: FormatContext,
     ) -> None:
-        if any(note for _, note in citation.labels):
-            # We can't add a citenote for multiple citations at a time in Latex - split individually
-            for key, note in citation.labels:
-                renderer.emit_macro("cite")
-                if note:
-                    renderer.emit_sqr_bracketed(note)
-                renderer.emit_braced(str(key))
+        latex_name = self.level_to_latex[head.weight]
+        if latex_name is None:
+            raise ValueError(
+                f"Can't emit {head} because it uses an unusable weight: {head.weight}"
+            )
+        if head.anchor:
+            # This is a numbered entry with a label
+            renderer.emit_macro(latex_name)  # i.e. r"\section"
         else:
-            renderer.emit_macro("cite")
-            renderer.emit_braced(",".join(key for key, _ in citation.labels))
-
-    def _emit_bibliography(self, renderer: LatexRenderer) -> None:
-        renderer.emit("""{
-\\raggedright
-\\printbibliography
-}""")
-
-    @stateless
-    def cite(
-        self, ctx: StatelessContext[LatexRenderer], *labels: Union[str, Tuple[str, str]]
-    ) -> Inline:
-        # Convert ["label"] to [("label", None)] so Citation has a consistent format
-        adapted_labels = [
-            (label, None)
-            if isinstance(label, str)
-            else (label[0], UnescapedText(label[1]))
-            for label in labels
-        ]
-        return Citation(adapted_labels)
-
-    # TODO make this output \citeauthor
-    @stateless
-    def citeauthor(self, ctx: StatelessContext[LatexRenderer], label: str) -> Inline:
-        return Citation([(label, None)])
-
+            renderer.emit_macro(latex_name + "*")
+        renderer.emit_braced(head.contents)  # i.e. r"\section*" + "{Section Name}"
+        if head.anchor:
+            renderer.emit(
+                head.anchor
+            )  # i.e. r"\section*{Section Name}\label{h1:Section_Name}"
+        renderer.emit_break_paragraph()
+        # Now emit the rest of the damn doc :)
+        renderer.emit_blockscope(contents)
+        for s in subsegments:
+            renderer.emit_segment(s)
 
-class LatexFootnotePlugin(Plugin[LatexRenderer], FootnotePluginInterface):
-    _footnotes: Dict[str, Block]
 
-    def __init__(self) -> None:
-        super().__init__()
+class UncheckedBiblatexRenderPlugin(LatexPlugin):
+    def _register(self, setup: LatexSetup) -> None:
+        setup.emitter.register_block_or_inline(Citation, self._emit_cite)
+        setup.emitter.register_block_or_inline(CiteAuthor, self._emit_citeauthor)
+        setup.emitter.register_block_or_inline(Bibliography, self._emit_bibliography)
 
-        self._footnotes = {}
-
-    def _add_emitters(self, handler: CustomEmitDispatch[LatexRenderer]) -> None:
-        handler.add_custom_inline(FootnoteAnchor, self._emit_footnote_anchor)
+    def _emit_cite(
+        self, cite: Citation, renderer: LatexRenderer, ctx: FormatContext
+    ) -> None:
+        renderer.emit_macro("cite")
+        if cite.contents:
+            renderer.emit_sqr_bracketed(cite.contents)
+        renderer.emit_braced(",".join(cite.citekeys))
 
-    def _emit_footnote_anchor(
+    def _emit_citeauthor(
         self,
+        citeauthor: CiteAuthor,
         renderer: LatexRenderer,
-        ctx: StatelessContext[LatexRenderer],
-        footnote: FootnoteAnchor,
+        ctx: FormatContext,
     ) -> None:
-        # TODO - intelligent footnotetext placement using floats?
-        renderer.emit_macro("footnote")
-        renderer.emit_braced(self._footnotes[footnote.label])
-
-    @property
-    @stateful
-    def footnote(self, state: MutableState[LatexRenderer]) -> InlineScopeBuilder:
-        @inline_scope_builder
-        def footnote_builder(contents: InlineScope) -> Inline:
-            label = str(uuid.uuid4())
-            self._footnotes[label] = Paragraph([Sentence([contents])])
-            return FootnoteAnchor(label)
-
-        return footnote_builder
-
-    @stateless
-    def footnote_ref(self, ctx: StatelessContext[LatexRenderer], label: str) -> Inline:
-        return FootnoteAnchor(label)
-
-    @stateful
-    def footnote_text(
-        self, state: MutableState[LatexRenderer], label: str
-    ) -> BlockScopeBuilder:
-        # Store the contents of a block scope and associate them with a specific footnote label
-        @block_scope_builder
-        def handle_block_contents(contents: BlockScope) -> Optional[Block]:
-            self._footnotes[label] = contents
-            return None
-
-        return handle_block_contents
-
-
-class LatexSectionPlugin(Plugin[LatexRenderer], SectionPluginInterface):
-    _pagebreak_before: List[str]
+        renderer.emit_macro("citeauthor")
+        renderer.emit_braced(citeauthor.citekey)
 
-    def __init__(self, pagebreak_before: List[str] = []) -> None:
-        super().__init__()
-        self._pagebreak_before = pagebreak_before
-
-    def _add_emitters(self, handler: CustomEmitDispatch[LatexRenderer]) -> None:
-        handler.add_custom_block(HeadedBlock, self._emit_headed_block)
-
-    def _emit_headed_block(
+    def _emit_bibliography(
         self,
+        bib: Bibliography,
         renderer: LatexRenderer,
-        ctx: StatelessContext[LatexRenderer],
-        block: HeadedBlock,
+        ctx: FormatContext,
     ) -> None:
-        if block.latex_name in self._pagebreak_before:
-            renderer.emit_raw("\\pagebreak\n")
-        if block.num:
-            renderer.emit_macro(block.latex_name) # i.e. r"\section"
-        else:
-            renderer.emit_macro(block.latex_name + "*")
-        renderer.emit_braced(block.name) # i.e. r"\section*" + "{Section Name}"
-        if block.label:
-            renderer.emit_macro("label")
-            renderer.emit_braced(block.label) # i.e. r"\section*{Section Name}" + r"\label{block_label}"
+        renderer.emit("{")
+        renderer.emit_break_sentence()
+        with renderer.indent(4):
+            renderer.emit("\\raggedright")
+            renderer.emit_break_sentence()
+            renderer.emit("\\printbibliography[heading=none]")
+            renderer.emit_break_sentence()
+        renderer.emit("}")
         renderer.emit_break_paragraph()
-        renderer.emit_blockscope(block.contents)
-
-    @stateful
-    def section(
-        self,
-        state: MutableState[LatexRenderer],
-        name: str,
-        label: Optional[str] = None,
-        num: bool = True,
-    ) -> BlockScopeBuilder:
-        @block_scope_builder
-        def handle_block_contents(contents: BlockScope) -> Block:
-            return HeadedBlock(
-                latex_name="section",
-                name=UnescapedText(name),
-                label=label,
-                num=num,
-                contents=contents,
-            )
-
-        return handle_block_contents
-
-    @stateful
-    def subsection(
-        self,
-        state: MutableState[LatexRenderer],
-        name: str,
-        label: Optional[str] = None,
-        num: bool = True,
-    ) -> BlockScopeBuilder:
-        @block_scope_builder
-        def handle_block_contents(contents: BlockScope) -> Block:
-            return HeadedBlock(
-                latex_name="subsection",
-                name=UnescapedText(name),
-                label=label,
-                num=num,
-                contents=contents,
-            )
-
-        return handle_block_contents
-
-    @stateful
-    def subsubsection(
-        self,
-        state: MutableState[LatexRenderer],
-        name: str,
-        label: Optional[str] = None,
-        num: bool = True,
-    ) -> BlockScopeBuilder:
-        @block_scope_builder
-        def handle_block_contents(contents: BlockScope) -> Block:
-            return HeadedBlock(
-                latex_name="subsubsection",
-                name=UnescapedText(name),
-                label=label,
-                num=num,
-                contents=contents,
-            )
-
-        return handle_block_contents
 
 
-@inline_scope_builder
-def emph_builder(items: InlineScope) -> Inline:
-    return Formatted("emph", items)
-
-
-@inline_scope_builder
-def italic_builder(items: InlineScope) -> Inline:
-    return Formatted("textit", items)
-
-
-@inline_scope_builder
-def bold_builder(items: InlineScope) -> Inline:
-    return Formatted("textbf", items)
-
-
-class LatexFormatPlugin(Plugin[LatexRenderer], FormatPluginInterface):
-    def _add_emitters(self, handler: CustomEmitDispatch[LatexRenderer]) -> None:
-        handler.add_custom_inline(Formatted, self._emit_formatted)
+class FootnoteRenderPlugin(LatexPlugin):
+    def _register(self, setup: LatexSetup) -> None:
+        setup.emitter.register_block_or_inline(FootnoteRef, self._emit_footnote)
+        setup.emitter.register_block_or_inline(
+            FootnoteContents, lambda _, __, ___: None
+        )
+        # This internally uses the footnote counter but it's a *magic* counter that doesn't correspond 1:1 to a turnip_text counter in value
+        # For example the value is page dependent
+        # => don't treat it as a normal counter
+        setup.declare_magic_tt_and_latex_counter(
+            tt_counter="footnote", latex_counter="footnote"
+        )
 
-    def _emit_formatted(
+    def _emit_footnote(
         self,
+        footnote: FootnoteRef,
         renderer: LatexRenderer,
-        ctx: StatelessContext[LatexRenderer],
-        item: Formatted,
+        ctx: FormatContext,
     ) -> None:
-        renderer.emit_macro(item.format_type)
-        renderer.emit_braced(item.items)
-
-    emph = emph_builder
-    italic = italic_builder
-    bold = bold_builder
-
-    OPEN_DQUOTE = RawLatex("``")
-    CLOS_DQUOTE = RawLatex("''")
-
-    @property
-    @stateless
-    def enquote(self, ctx: StatelessContext[LatexRenderer]) -> InlineScopeBuilder:
-        @inline_scope_builder
-        def enquote_builder(items: InlineScope) -> Inline:
-            return InlineScope(
-                [LatexFormatPlugin.OPEN_DQUOTE]
-                + list(items)
-                + [LatexFormatPlugin.CLOS_DQUOTE]
-            )
-
-        return enquote_builder
+        footnote_backref = footnote.portal_to
+        _, footnote_contents = renderer.anchors.lookup_backref_float(footnote_backref)
+        if footnote_contents is None:
+            raise ValueError(f"Reference to nonexistant footnote {footnote_backref}")
+        assert isinstance(footnote_contents, FootnoteContents)
+        renderer.emit_macro("footnote")
+        renderer.emit_braced(footnote_contents.contents)
 
 
-class LatexListPlugin(Plugin[LatexRenderer]):
+class ListRenderPlugin(LatexPlugin):
     indent_list_items: bool = True
 
     def __init__(self, indent_list_items: bool = True):
         self.indent_list_items = indent_list_items
 
-    def _add_emitters(self, handler: CustomEmitDispatch[LatexRenderer]) -> None:
-        handler.add_custom_block(DisplayList, self._emit_list)
-        handler.add_custom_block(DisplayListItem, self._emit_list_item)
+    def _register(self, setup: LatexSetup) -> None:
+        setup.emitter.register_block_or_inline(DisplayList, self._emit_list)
+        setup.emitter.register_block_or_inline(DisplayListItem, self._emit_list_item)
 
     def _emit_list(
         self,
-        renderer: LatexRenderer,
-        ctx: StatelessContext[LatexRenderer],
         list: DisplayList,
+        renderer: LatexRenderer,
+        ctx: FormatContext,
     ) -> None:
-        with renderer.emit_env(list.mode):
-            renderer.emit(*list.items, joiner=renderer.emit_break_paragraph)
+        mode = {
+            DisplayListType.Itemize: "itemize",
+            DisplayListType.Enumerate: "enumerate",
+        }[list.list_type]
+        with renderer.emit_env(mode):
+            renderer.emit(*list.contents, joiner=renderer.emit_break_paragraph)
 
     def _emit_list_item(
         self,
-        renderer: LatexRenderer,
-        ctx: StatelessContext[LatexRenderer],
         list_item: DisplayListItem,
+        renderer: LatexRenderer,
+        ctx: FormatContext,
     ) -> None:
         renderer.emit_macro("item")
         # Put {} after \item so square brackets at the start of render_block don't get swallowed as arguments
         renderer.emit("{} ")
         indent_width = len("\\item{} ")
         with renderer.indent(indent_width):
-            renderer.emit(list_item.item)
+            renderer.emit(list_item.contents)
 
-    @property
-    @stateless
-    def enumerate(self, ctx: StatelessContext[LatexRenderer]) -> BlockScopeBuilder:
-        @block_scope_builder
-        def enumerate_builder(contents: BlockScope) -> Block:
-            items = list(contents)
-            if any(not isinstance(x, DisplayListItem) for x in items):
-                raise TypeError(
-                    f"Found blocks in this list that were not list [item]s!"
-                )
-            return DisplayList(
-                mode="enumerate", items=cast(List[DisplayListItem], items)
-            )
-
-        return enumerate_builder
-
-    @property
-    @stateless
-    def itemize(self, ctx: StatelessContext[LatexRenderer]) -> BlockScopeBuilder:
-        @block_scope_builder
-        def itemize_builder(contents: BlockScope) -> Block:
-            items = list(contents)
-            if any(not isinstance(x, DisplayListItem) for x in items):
-                raise TypeError(
-                    f"Found blocks in this list that were not list [item]s!"
-                )
-            return DisplayList(mode="itemize", items=cast(List[DisplayListItem], items))
-
-        return itemize_builder
-
-    @property
-    @stateless
-    def item(self, ctx: StatelessContext[LatexRenderer]) -> BlockScopeBuilder:
-        @block_scope_builder
-        def item_builder(block_scope: BlockScope) -> Block:
-            return DisplayListItem(block_scope)
 
-        return item_builder
+FORMAT_TYPE_TO_MACRO = {
+    InlineFormattingType.Bold: "textbf",
+    InlineFormattingType.Italic: "textit",
+    InlineFormattingType.Underline: "underline",
+    InlineFormattingType.Emph: "emph",
+    InlineFormattingType.Strong: "strong",
+}
+
+
+class InlineFormatRenderPlugin(LatexPlugin):
+    # TODO If we don't use squotes,dquotes manually it would make sense to use enquote from csquotes package
+    def _register(self, setup: LatexSetup) -> None:
+        setup.emitter.register_block_or_inline(InlineFormatted, self._emit_formatted)
 
+    def _emit_formatted(
+        self,
+        f: InlineFormatted,
+        renderer: LatexRenderer,
+        fmt: FormatContext,
+    ) -> None:
+        if f.format_type == InlineFormattingType.SingleQuote:
+            renderer.emit("`", f.contents, "'")
+        elif f.format_type == InlineFormattingType.DoubleQuote:
+            renderer.emit("``", f.contents, "''")
+        else:
+            # All other kinds are just the contents wrapped in a macro
+            renderer.emit_macro(FORMAT_TYPE_TO_MACRO[f.format_type])
+            renderer.emit_braced(f.contents)
 
-class LatexUrlPlugin(Plugin[LatexRenderer]):
-    # TODO add dependency on hyperref!!
 
-    def _add_emitters(self, handler: CustomEmitDispatch[LatexRenderer]) -> None:
-        handler.add_custom_inline(NamedUrl, self._emit_url)
+class UrlRenderPlugin(LatexPlugin):
+    def _register(self, setup: LatexSetup) -> None:
+        setup.request_latex_package("hyperref", "URL rendering")
+        setup.emitter.register_block_or_inline(NamedUrl, self._emit_url)
 
     def _emit_url(
-        self, renderer: LatexRenderer, ctx: StatelessContext[LatexRenderer], url: NamedUrl
+        self,
+        url: NamedUrl,
+        renderer: LatexRenderer,
+        fmt: FormatContext,
     ) -> None:
-        assert "}" not in url.url
-        assert "#" not in url.url
-        if url.name is None:
+        if "}" in url.url:
+            raise RuntimeError(
+                f"Can't handle url {url.url} with a }} in it. Please use proper percent-encoding to escape it."
+            )
+
+        # TODO this breaks if the hash is already escaped :|
+
+        if url.contents is None:
             renderer.emit_macro("url")
-            renderer.emit_braced(url.url)
+            renderer.emit_braced(url.url.replace("#", "\\#"))
         else:
             renderer.emit_macro("href")
-            renderer.emit_braced(url.url)
-            renderer.emit_braced(url.name)
-
-    @stateless
-    def url(
-        self, ctx: StatelessContext[LatexRenderer], url: str, name: Optional[str] = None
-    ) -> Inline:
-        return NamedUrl(
-            url, name=InlineScope([UnescapedText(name)]) if name is not None else None
-        )
+            renderer.emit_braced(url.url.replace("#", "\\#"))
+            renderer.emit_braced(url.contents)
```

### Comparing `turnip_text-0.0.4/src/lexer.rs` & `turnip_text-0.0.5/src/lexer/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,63 @@
+use lexer_rs::LexerOfStr;
 use lexer_rs::PosnInCharStream;
 use lexer_rs::SimpleParseError;
 use lexer_rs::{CharStream, Lexer, LexerParseResult};
 
-use crate::lexer_charofs_row_col::LineColumnChar;
-use crate::util::{ParsePosn, ParseSpan};
+mod line_col_char_posn;
+use line_col_char_posn::LineColumnChar;
+
+use crate::util::ParseSpan;
+
+#[derive(Debug)]
+pub enum LexedStrIterator {
+    Exhausted,
+    Error(LexError),
+    Tokenizing(UnitsToTokensIterator),
+}
+impl Iterator for LexedStrIterator {
+    type Item = Result<TTToken, LexError>;
+
+    fn next(&mut self) -> Option<Self::Item> {
+        let (should_exhaust, ret) = match self {
+            LexedStrIterator::Exhausted => (false, None),
+            // TODO sucks we have to clone this :/
+            LexedStrIterator::Error(e) => (true, Some(Err(e.clone()))),
+            LexedStrIterator::Tokenizing(tokenizer) => match tokenizer.next() {
+                Some(tok) => (false, Some(Ok(tok))),
+                None => (true, None),
+            },
+        };
+        if should_exhaust {
+            *self = LexedStrIterator::Exhausted;
+        }
+        ret
+    }
+}
+/// TODO right now we have to store all the first-level lex tokens in a vector. This sucks.
+fn lex_units_only(file_idx: usize, data: &str) -> Result<Vec<Unit>, LexError> {
+    let lexer = LexerOfStr::<LexPosn, LexToken, LexError>::new(data);
+
+    let mut units: Vec<Unit> = vec![];
+    for u in lexer.iter(&[
+        Box::new(|stream, state, ch| Unit::parse_special(file_idx, stream, state, ch)),
+        Box::new(|stream, state, ch| Unit::parse_other(file_idx, stream, state, ch)),
+    ]) {
+        units.push(u?);
+    }
+
+    Ok(units)
+}
+pub fn lex(file_idx: usize, data: &str) -> LexedStrIterator {
+    let units = lex_units_only(file_idx, data);
+    match units {
+        Ok(units) => LexedStrIterator::Tokenizing(UnitsToTokensIterator::new(units)),
+        Err(e) => LexedStrIterator::Error(e),
+    }
+}
 
 /// Sequences that can define the start of a [SimpleToken]
 #[derive(Debug, Copy, Clone, PartialEq, Eq)]
 pub enum LexerPrefixSeq {
     /// `\r`
     CarriageReturn,
     /// `\n`
@@ -128,15 +178,15 @@
     ///
     /// Current escapable characters/sequences are `[, ], {, }, \, #, \r, \n, \r\n`.
     /// TODO include `%` when [SimpleToken::Percent] is uncommented
     Escaped(ParseSpan, Escapable),
     /// '\' that does not participate in a [Self::Escaped]
     ///
     /// TODO - A LaTeX-output backend could choose to disallow plain backslashes, as they would interact with LaTeX in potentially unexpected ways.
-    Backslash(ParsePosn),
+    Backslash(ParseSpan),
     /// N `[` characters not preceded by a backslash
     CodeOpen(ParseSpan, usize),
     /// N `]` characters not preceded by a backslash
     CodeClose(ParseSpan, usize),
     /// `{` character not preceded by a backslash
     ScopeOpen(ParseSpan),
     /// `}` character not preceded by a backslash
@@ -150,14 +200,15 @@
     Whitespace(ParseSpan),
     // TODO
     // /// `%` character not preceded by a backslash
     // Percent(P),
 }
 impl Unit {
     fn parse_n_chars<L>(
+        file_idx: usize,
         stream: &L,
         state: L::State,
         target_ch: char,
     ) -> LexerParseResult<LexPosn, usize, L::Error>
     where
         L: CharStream<LexPosn>,
         L: Lexer<Token = Self, State = LexPosn>,
@@ -168,100 +219,108 @@
                 _ => Ok(None),
             }
         } else {
             Ok(None)
         }
     }
     pub fn parse_special<L>(
+        file_idx: usize,
         stream: &L,
         state: L::State,
         ch: char,
     ) -> LexerParseResult<LexPosn, Self, L::Error>
     where
         L: CharStream<LexPosn>,
         L: Lexer<Token = Self, State = LexPosn>,
     {
         if let Some((seq, n_chars_in_seq)) = LexerPrefixSeq::try_extract(stream, state, ch) {
             let start = state;
             let state_after_seq = stream.consumed(state, n_chars_in_seq);
-            let seq_span = ParseSpan::from_lex(start, state_after_seq);
+            let seq_span = ParseSpan::from_lex(file_idx, start, state_after_seq);
             match seq {
                 // Backslash => check if the following character is special, in which case Escaped(), else Backslash()
                 LexerPrefixSeq::Backslash => {
                     match Escapable::try_extract(stream, state_after_seq) {
                         Some((escapable, n_chars)) => {
                             // Consume the initial backslash + the number of characters in the escaped sequence
                             let end = stream.consumed(state, n_chars + 1);
-                            let span = ParseSpan::from_lex(start, end);
+                            let span = ParseSpan::from_lex(file_idx, start, end);
                             Ok(Some((end, Self::Escaped(span, escapable))))
                         }
-                        None => Ok(Some((state_after_seq, Self::Backslash(state.into())))),
+                        None => {
+                            let end = stream.consumed(state, 1);
+                            Ok(Some((
+                                state_after_seq,
+                                Self::Backslash(ParseSpan::from_lex(file_idx, start, end)),
+                            )))
+                        }
                     }
                 }
                 // CRLF or (CR outside CRLF) or (LF outside CRLF) => Newline()
                 LexerPrefixSeq::CRLF
                 | LexerPrefixSeq::CarriageReturn
                 | LexerPrefixSeq::LineFeed => Ok(Some((state_after_seq, Self::Newline(seq_span)))),
                 // SqrOpen => CodeOpen()
                 LexerPrefixSeq::SqrOpen => {
                     // Run will have at least one [, because it's starting with this character.
-                    match Self::parse_n_chars(stream, state, '[')? {
+                    match Self::parse_n_chars(file_idx, stream, state, '[')? {
                         Some((hash_end, n)) => Ok(Some((
                             hash_end,
-                            Self::CodeOpen(ParseSpan::from_lex(start, hash_end), n),
+                            Self::CodeOpen(ParseSpan::from_lex(file_idx, start, hash_end), n),
                         ))),
                         None => unreachable!(),
                     }
                 }
                 // SqrClose => CodeClose
                 LexerPrefixSeq::SqrClose => {
                     // Run will have at least one hash, because it's starting with this character.
-                    match Self::parse_n_chars(stream, state, ']')? {
+                    match Self::parse_n_chars(file_idx, stream, state, ']')? {
                         Some((hash_end, n)) => Ok(Some((
                             hash_end,
-                            Self::CodeClose(ParseSpan::from_lex(start, hash_end), n),
+                            Self::CodeClose(ParseSpan::from_lex(file_idx, start, hash_end), n),
                         ))),
                         None => unreachable!(),
                     }
                 }
                 // SqrOpen => ScopeOpen()
                 LexerPrefixSeq::SqgOpen => Ok(Some((state_after_seq, Self::ScopeOpen(seq_span)))),
                 // SqgClose => ScopeClose
                 LexerPrefixSeq::SqgClose => Ok(Some((state_after_seq, Self::ScopeClose(seq_span)))),
                 // Hash => Hash
                 LexerPrefixSeq::Hash => {
                     // Run will have at least one #, because it's starting with this character.
-                    match Self::parse_n_chars(stream, state, '#')? {
+                    match Self::parse_n_chars(file_idx, stream, state, '#')? {
                         Some((hash_end, n)) => Ok(Some((
                             hash_end,
-                            Self::Hashes(ParseSpan::from_lex(start, hash_end), n),
+                            Self::Hashes(ParseSpan::from_lex(file_idx, start, hash_end), n),
                         ))),
                         None => unreachable!(),
                     }
                 }
                 // Whitespace => Whitespace
                 LexerPrefixSeq::Whitespace => {
                     // Match all whitespace except newlines
                     match stream.do_while(state, ch, &|_, ch| {
                         ch.is_whitespace() && ch != '\n' && ch != '\r'
                     }) {
                         // We peeked a Whitespace prefix, so there must be at least one whitespace char
                         (end, Some(_)) => Ok(Some((
                             end,
-                            Self::Whitespace(ParseSpan::from_lex(start, end)),
+                            Self::Whitespace(ParseSpan::from_lex(file_idx, start, end)),
                         ))),
                         _ => unreachable!(),
                     }
                 }
             }
         } else {
             Ok(None)
         }
     }
     pub fn parse_other<L>(
+        file_idx: usize,
         stream: &L,
         start: L::State,
         start_ch: char,
     ) -> LexerParseResult<LexPosn, Self, L::Error>
     where
         L: CharStream<LexPosn>,
         L: Lexer<Token = Self, State = LexPosn>,
@@ -295,28 +354,28 @@
                 Some(ch2) => end_ch = ch2,
                 None => break, // End of stream => break
             }
         }
         if start == end {
             Ok(None)
         } else {
-            let span = ParseSpan::from_lex(start, end);
+            let span = ParseSpan::from_lex(file_idx, start, end);
             Ok(Some((end, Self::OtherText(span))))
         }
     }
 }
 
 #[derive(Debug, Copy, Clone)]
 pub enum TTToken {
     /// See [Unit::Newline]
     Newline(ParseSpan),
     /// See [Unit::Escaped]
     Escaped(ParseSpan, Escapable),
     /// See [Unit::Backslash]
-    Backslash(ParsePosn),
+    Backslash(ParseSpan),
     /// N `[` characters not preceded by a backslash
     CodeOpen(ParseSpan, usize),
     /// N `]` characters not preceded by a backslash, not followed by a scope open
     CodeClose(ParseSpan, usize),
     /// N `]` characters followed by inline scope open (`{` not followed by newline)
     CodeCloseOwningInline(ParseSpan, usize),
     /// N `]` characters followed by raw scope open (N' hashes followed by `{`)
@@ -363,88 +422,126 @@
         assert!(n_consumed > 0);
         toks.push(tok);
         i += n_consumed;
     }
     toks
 }
 
+#[derive(Debug)]
+pub struct UnitsToTokensIterator {
+    units: Vec<Unit>,
+    idx: usize,
+}
+impl UnitsToTokensIterator {
+    pub fn new(units: Vec<Unit>) -> UnitsToTokensIterator {
+        UnitsToTokensIterator { units, idx: 0 }
+    }
+}
+impl Iterator for UnitsToTokensIterator {
+    type Item = TTToken;
+
+    fn next(&mut self) -> Option<Self::Item> {
+        let i = self.idx;
+        let len = self.units.len();
+        if i >= len {
+            None
+        } else {
+            let (tok, n_consumed) = TTToken::units_to_token((
+                &self.units[i],
+                if i + 1 < self.units.len() {
+                    Some(&self.units[i + 1])
+                } else {
+                    None
+                },
+                if i + 2 < self.units.len() {
+                    Some(&self.units[i + 2])
+                } else {
+                    None
+                },
+            ));
+            assert!(n_consumed > 0);
+            self.idx += n_consumed;
+            Some(tok)
+        }
+    }
+}
+
 impl TTToken {
     fn units_to_token(units: (&Unit, Option<&Unit>, Option<&Unit>)) -> (Self, usize) {
         match units {
             (Unit::Newline(s), _, _) => (TTToken::Newline(*s), 1),
             (Unit::Escaped(s, e), _, _) => (TTToken::Escaped(*s, *e), 1),
             (Unit::Backslash(p), _, _) => (TTToken::Backslash(*p), 1),
             (Unit::OtherText(s), _, _) => (TTToken::OtherText(*s), 1),
             (Unit::Whitespace(s), _, _) => (TTToken::Whitespace(*s), 1),
 
             // Code open and close
             (Unit::CodeOpen(s, n), _, _) => (TTToken::CodeOpen(*s, *n), 1),
             (Unit::CodeClose(s_start, n), Some(Unit::ScopeOpen(_)), Some(Unit::Newline(s_end))) => {
-                (
-                    TTToken::CodeCloseOwningBlock(ParseSpan::new(s_start.start, s_end.end), *n),
-                    3,
-                )
+                (TTToken::CodeCloseOwningBlock(s_start.combine(s_end), *n), 3)
             }
             (
                 Unit::CodeClose(s_start, n),
                 Some(Unit::Hashes(_, n_hashes)),
                 Some(Unit::ScopeOpen(s_end)),
             ) => (
-                TTToken::CodeCloseOwningRaw(
-                    ParseSpan::new(s_start.start, s_end.end),
-                    *n,
-                    *n_hashes,
-                ),
+                TTToken::CodeCloseOwningRaw(s_start.combine(s_end), *n, *n_hashes),
                 3,
             ),
             (Unit::CodeClose(s_start, n), Some(Unit::ScopeOpen(s_end)), _) => (
-                TTToken::CodeCloseOwningInline(ParseSpan::new(s_start.start, s_end.end), *n),
+                TTToken::CodeCloseOwningInline(s_start.combine(s_end), *n),
                 2,
             ),
             (Unit::CodeClose(span, n), _, _) => (TTToken::CodeClose(*span, *n), 1),
 
             // Block Scope Open
-            (Unit::ScopeOpen(s_start), Some(Unit::Newline(s_end)), _) => (
-                TTToken::BlockScopeOpen(ParseSpan::new(s_start.start, s_end.end)),
-                2,
-            ),
+            (Unit::ScopeOpen(s_start), Some(Unit::Newline(s_end)), _) => {
+                (TTToken::BlockScopeOpen(s_start.combine(s_end)), 2)
+            }
 
             // Inline scope open
             (Unit::ScopeOpen(s), _, _) => (TTToken::InlineScopeOpen(*s), 1),
 
             // Raw scope open
-            (Unit::Hashes(s_start, n), Some(Unit::ScopeOpen(s_end)), _) => (
-                TTToken::RawScopeOpen(
-                    ParseSpan {
-                        start: s_start.start,
-                        end: s_end.end,
-                    },
-                    *n,
-                ),
-                2,
-            ),
+            (Unit::Hashes(s_start, n), Some(Unit::ScopeOpen(s_end)), _) => {
+                (TTToken::RawScopeOpen(s_start.combine(s_end), *n), 2)
+            }
 
             // Scope close
-            (Unit::ScopeClose(s_start), Some(Unit::Hashes(s_end, n)), _) => (
-                TTToken::RawScopeClose(
-                    ParseSpan {
-                        start: s_start.start,
-                        end: s_end.end,
-                    },
-                    *n,
-                ),
-                2,
-            ),
+            (Unit::ScopeClose(s_start), Some(Unit::Hashes(s_end, n)), _) => {
+                (TTToken::RawScopeClose(s_start.combine(s_end), *n), 2)
+            }
             (Unit::ScopeClose(s), _, _) => (TTToken::ScopeClose(*s), 1),
 
             // Raw scope close
             (Unit::Hashes(s, n), _, _) => (TTToken::Hashes(*s, *n), 1),
         }
     }
 
+    pub fn token_span(&self) -> ParseSpan {
+        match *self {
+            TTToken::Newline(span) => span,
+            TTToken::Escaped(span, _) => span,
+            TTToken::Backslash(span) => span,
+            TTToken::CodeOpen(span, _) => span,
+            TTToken::CodeClose(span, _) => span,
+            TTToken::CodeCloseOwningInline(span, _) => span,
+            TTToken::CodeCloseOwningRaw(span, _, _) => span,
+            TTToken::CodeCloseOwningBlock(span, _) => span,
+            TTToken::InlineScopeOpen(span) => span,
+            TTToken::BlockScopeOpen(span) => span,
+            TTToken::ScopeClose(span) => span,
+            TTToken::RawScopeOpen(span, _) => span,
+            TTToken::RawScopeClose(span, _) => span,
+            TTToken::Hashes(span, _) => span,
+            TTToken::OtherText(span) => span,
+            TTToken::Whitespace(span) => span,
+        }
+    }
+
     /// Convert a token to a [str] representation, usable for a raw-scope representation
     /// i.e. with no escaping.
     ///
     /// Newlines are converted to \n everywhere.
     pub fn stringify_raw<'a>(&self, data: &'a str) -> &'a str {
         use TTToken::*;
         match self {
```

### Comparing `turnip_text-0.0.4/src/lexer_charofs_row_col.rs` & `turnip_text-0.0.5/src/lexer/line_col_char_posn.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 //a LineColumn
 //tp LineColumn
 /// A line and column within a text stream
 ///
 /// This provides the [UserPosn] trait, which provides methods to
 /// retrieve the line and column values of the state.
-/// 
+///
 /// It also stores the char offset in the stream, not just the byte offset like lexer_rs::StreamCharPos,
 /// because this is sometimes required by e.g. error reporting libraries like annotate_snippet
 #[derive(Debug, Copy, Clone, PartialEq, Eq, Hash)]
 pub struct LineColumnChar {
     line: usize,
     column: usize,
     char_ofs: usize,
@@ -22,22 +22,30 @@
         self.char_ofs
     }
 }
 
 //ip Default for LineColumn
 impl std::default::Default for LineColumnChar {
     fn default() -> Self {
-        Self { line: 1, column: 1, char_ofs: 0, }
+        Self {
+            line: 1,
+            column: 1,
+            char_ofs: 0,
+        }
     }
 }
 
 //ip Display for LineColumn
 impl std::fmt::Display for LineColumnChar {
     fn fmt(&self, fmt: &mut std::fmt::Formatter<'_>) -> Result<(), std::fmt::Error> {
-        write!(fmt, "line {} column {} (char {})", self.line, self.column, self.char_ofs)
+        write!(
+            fmt,
+            "line {} column {} (char {})",
+            self.line, self.column, self.char_ofs
+        )
     }
 }
 
 //ip UserPosn for LineColumn
 impl UserPosn for LineColumnChar {
     fn line(&self) -> usize {
         self.line
```

### Comparing `turnip_text-0.0.4/src/python/interop.rs` & `turnip_text-0.0.5/src/interpreter/python/interop.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-use std::path::Path;
-
 use pyo3::{
-    exceptions::{PyRuntimeError, PyTypeError},
+    exceptions::{PyTypeError, PyValueError},
     intern,
     prelude::*,
     types::{PyDict, PyFloat, PyIterator, PyList, PyLong, PyString},
 };
 
-use super::typeclass::{PyInstanceList, PyTcRef, PyTypeclass, PyTypeclassList};
+use crate::{error::TurnipTextError, parser::TurnipTextParser};
+
+use super::typeclass::{PyInstanceList, PyTcRef, PyTcUnionRef, PyTypeclass, PyTypeclassList};
+
+mod error {
+    use pyo3::create_exception;
+
+    create_exception!(_native, TurnipTextError, pyo3::exceptions::PyException);
+}
 
 #[pymodule]
 #[pyo3(name = "_native")]
-pub fn turnip_text(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+pub fn turnip_text(py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(parse_file, m)?)?;
-    m.add_function(wrap_pyfunction!(parse_str, m)?)?;
     m.add_function(wrap_pyfunction!(coerce_to_inline, m)?)?;
     m.add_function(wrap_pyfunction!(coerce_to_inline_scope, m)?)?;
     m.add_function(wrap_pyfunction!(coerce_to_block, m)?)?;
     m.add_function(wrap_pyfunction!(coerce_to_block_scope, m)?)?;
 
     // Primitives
     m.add_class::<UnescapedText>()?;
     m.add_class::<RawText>()?;
     m.add_class::<Sentence>()?;
     m.add_class::<Paragraph>()?;
     m.add_class::<BlockScope>()?;
     m.add_class::<InlineScope>()?;
+    m.add_class::<DocSegment>()?;
+    m.add_class::<InsertedFile>()?;
+
+    m.add("TurnipTextError", py.get_type::<error::TurnipTextError>())?;
 
     Ok(())
 }
 
-/// Given a file path, calls [crate::cli::parse_file] (includes parsing, checking for syntax errors, evaluating python)
-#[pyfunction]
-fn parse_file<'py>(
-    py: Python<'py>,
-    path: &str,
-    locals: Option<&PyDict>,
-) -> PyResult<Py<BlockScope>> {
-    // crate::cli::parse_file already surfaces the error to the user - we can just return a generic error
-    crate::cli::parse_file(
-        py,
-        locals.unwrap_or_else(|| PyDict::new(py)),
-        Path::new(path),
-    )
-    .map_err(|_| PyRuntimeError::new_err("parse failed, see stdout"))
+impl TurnipTextError {
+    fn to_pyerr(self) -> PyErr {
+        self.display_cli_feedback();
+        error::TurnipTextError::new_err(format!("{self}"))
+    }
 }
 
 #[pyfunction]
-fn parse_str<'py>(
+fn parse_file<'py>(
     py: Python<'py>,
-    data: &str,
-    locals: Option<&PyDict>,
-) -> PyResult<Py<BlockScope>> {
-    // crate::cli::parse_str already surfaces the error to the user - we can just return a generic error
-    crate::cli::parse_str(py, locals.unwrap_or_else(|| PyDict::new(py)), data)
-        .map_err(|_| PyRuntimeError::new_err("parse failed, see stdout"))
+    file: InsertedFile,
+    py_env: &PyDict,
+) -> PyResult<Py<DocSegment>> {
+    let parser =
+        TurnipTextParser::new(py, file.name, file.contents).map_err(TurnipTextError::to_pyerr)?;
+    parser.parse(py, py_env).map_err(TurnipTextError::to_pyerr)
 }
 
 #[pyfunction]
 pub fn coerce_to_inline<'py>(py: Python<'py>, obj: &'py PyAny) -> PyResult<PyObject> {
     Ok(coerce_to_inline_pytcref(py, obj)?.unbox())
 }
 
@@ -67,15 +67,15 @@
     obj: &'py PyAny,
 ) -> PyResult<PyTcRef<Inline>> {
     // 1. if it's already Inline, return it
     if let Ok(inl) = PyTcRef::of(obj) {
         return Ok(inl);
     }
     // 2. if it's a List of Inline, return InlineScope(it)
-    // Here we first check if it's a list, then if so try to create an Inline - this will verify if it's a list of Inlines.
+    // Here we first check if it's a list, then if so try to create an InlineScope - this will verify if it's a list of Inlines.
     if let Ok(py_list) = obj.downcast::<PyList>() {
         if let Ok(inline_scope) = InlineScope::new(py, Some(py_list)) {
             let inline_scope = Py::new(py, inline_scope)?;
             return PyTcRef::of(inline_scope.as_ref(py));
         }
     }
     // 3. if it's str, return UnescapedText(it)
@@ -218,26 +218,41 @@
             obj.getattr(attr_name)?.is_true()
         } else {
             Ok(false)
         }
     }
 }
 
-/// Typeclass used internally for things that can be emitted directly from eval-brackets:
-/// i.e. an Inline or a Block.
-/// Must be one or the other - doesn't make sense for something to be both, because it doesn't know what context it would be rendered in.
-#[derive(Debug, Clone)]
-pub struct InlineXorBlock {}
-impl PyTypeclass for InlineXorBlock {
-    const NAME: &'static str = "Inline XOR Block (not both)";
+/// Typeclass representing the header for a document segment, which is rendered before any other element in the segment
+/// and defines how it interacts with other segments through the weight parameter. See [DocSegment].
+#[derive(Debug, Clone)]
+pub struct DocSegmentHeader {}
+impl DocSegmentHeader {
+    fn marker_bool_name(py: Python<'_>) -> &PyString {
+        intern!(py, "is_segment_header")
+    }
+    fn weight_field_name(py: Python<'_>) -> &PyString {
+        intern!(py, "weight")
+    }
+    pub fn get_weight(py: Python<'_>, header: &PyAny) -> PyResult<i64> {
+        header
+            .getattr(DocSegmentHeader::weight_field_name(py))?
+            .extract()
+    }
+}
+impl PyTypeclass for DocSegmentHeader {
+    const NAME: &'static str = "DocSegmentHeader";
 
     fn fits_typeclass(obj: &PyAny) -> PyResult<bool> {
-        let is_inline = Inline::fits_typeclass(obj)?;
-        let is_block = Block::fits_typeclass(obj)?;
-        Ok(is_inline ^ is_block)
+        let attr_name = Self::marker_bool_name(obj.py());
+        if matches!(obj.hasattr(attr_name), Ok(true)) {
+            obj.getattr(attr_name)?.is_true()
+        } else {
+            Ok(false)
+        }
     }
 }
 
 /// Typeclass representing the "builder" of a block scope, which may modify how that scope is rendered.
 ///
 /// Requires a method
 /// ```python
@@ -249,23 +264,23 @@
     fn marker_func_name(py: Python<'_>) -> &PyString {
         intern!(py, "build_from_blocks")
     }
     pub fn call_build_from_blocks<'py>(
         py: Python<'py>,
         builder: PyTcRef<Self>,
         blocks: Py<BlockScope>,
-    ) -> PyResult<Option<PyTcRef<Block>>> {
+    ) -> PyResult<Option<PyTcUnionRef<Block, DocSegmentHeader>>> {
         let output = builder
             .as_ref(py)
             .getattr(Self::marker_func_name(py))?
             .call1((blocks,))?;
         if output.is_none() {
             Ok(None)
         } else {
-            Ok(Some(PyTcRef::of(output)?))
+            Ok(Some(PyTcUnionRef::of(output)?))
         }
     }
 }
 impl PyTypeclass for BlockScopeBuilder {
     const NAME: &'static str = "BlockScopeBuilder";
 
     fn fits_typeclass(obj: &PyAny) -> PyResult<bool> {
@@ -281,14 +296,15 @@
 /// ```
 #[derive(Debug, Clone)]
 pub struct InlineScopeBuilder {}
 impl InlineScopeBuilder {
     fn marker_func_name(py: Python<'_>) -> &PyString {
         intern!(py, "build_from_inlines")
     }
+    // TODO: Make this return PyTcUnionRef<Inline | DocSegmentHeader>. Right now it can't because the parser can't handle it.
     pub fn call_build_from_inlines<'py>(
         py: Python<'py>,
         builder: PyTcRef<Self>,
         inlines: Py<InlineScope>,
     ) -> PyResult<PyTcRef<Inline>> {
         let output = builder
             .as_ref(py)
@@ -318,20 +334,20 @@
         intern!(py, "build_from_raw")
     }
     /// Calls builder.build_from_raw(raw), could be inline or block
     pub fn call_build_from_raw<'py>(
         py: Python<'py>,
         builder: &PyTcRef<Self>,
         raw: &String,
-    ) -> PyResult<PyTcRef<InlineXorBlock>> {
+    ) -> PyResult<PyTcUnionRef<Inline, Block>> {
         let output = builder
             .as_ref(py)
             .getattr(Self::marker_func_name(py))?
             .call1((raw,))?;
-        PyTcRef::of(output)
+        PyTcUnionRef::of(output)
     }
 }
 impl PyTypeclass for RawScopeBuilder {
     const NAME: &'static str = "RawScopeBuilder";
 
     fn fits_typeclass(obj: &PyAny) -> PyResult<bool> {
         obj.hasattr(Self::marker_func_name(obj.py()))
@@ -539,70 +555,186 @@
     }
 
     pub fn push_inline(&mut self, node: &PyAny) -> PyResult<()> {
         self.0.append_checked(node)
     }
 }
 
+// TODO Rename to TurnipTextFile, make parse a method on it? Need some warning to say "SERIOUSLY DON'T CALL .parse WHILE PARSING", or some other much simpler way to emit one than "call InsertedFile.from_blah"? Default function on DocState?
+#[pyclass]
+#[derive(Clone)]
+pub struct InsertedFile {
+    pub name: String,
+    pub contents: String,
+}
+impl InsertedFile {
+    pub fn name(&self) -> &str {
+        &self.name
+    }
+    pub fn contents(&self) -> &str {
+        &self.contents
+    }
+}
+impl std::fmt::Debug for InsertedFile {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        f.debug_struct("InsertedFile")
+            .field("name", &self.name)
+            .field("contents", &"<...>")
+            .finish()
+    }
+}
+#[pymethods]
+impl InsertedFile {
+    #[new]
+    pub fn new(name: String, contents: String) -> InsertedFile {
+        InsertedFile { name, contents }
+    }
+
+    #[staticmethod]
+    pub fn from_path(path: String) -> PyResult<InsertedFile> {
+        let name = std::fs::canonicalize(&path)?;
+        let contents = std::fs::read_to_string(&path)
+            .map_err(|e| error::TurnipTextError::new_err(format!("{e}")))?;
+        Ok(InsertedFile {
+            name: name.into_os_string().into_string().unwrap_or(path),
+            contents,
+        })
+    }
+
+    #[staticmethod]
+    pub fn from_string(contents: String) -> InsertedFile {
+        InsertedFile {
+            name: "<string>".into(),
+            contents,
+        }
+    }
+}
+
 /// This is used for implicit structure.
-/// It's created by Python code just with the Header and Weight, and the Weight is used to implicitly open and close scopes
-/// 
+/// It's created by Python code by emitting a DocSegmentHeader with some Weight, and the Weight is used to implicitly open and close scopes
+///
 /// ```text
-/// [section("Blah")] # -> ImplicitStructure(header=Section(), weight=10)
-/// 
-/// # This paragraph is implicitly included as a child of ImplicitStructure().children
+/// [heading("Blah")] # -> DocSegmentHeader(weight=0)
+///
+/// # This paragraph is implicitly included as a child of DocSegment().text
 /// some text
-/// 
-/// [subsection("Sub-Blah")] # -> ImplicitStructure(header=Subsection(), weight=20)
-/// # the weight is greater than for the Section -> the subsection is implicitly included as a child of section
-/// 
+///
+/// [subheading("Sub-Blah")] # -> DocSegmentHeader(weight=1)
+/// # the weight is greater than for the Section -> the subsection is implicitly included as a subsegment of section
+///
 /// Some other text in a subsection
-/// 
-/// [section("Blah 2")] # -> ImplicitStructure(header=Section(), weight=10)
-/// # the weight is <=subsection -> subsection 1.1 automatically ends
-/// # the weight is <=section -> section 1 automatically ends
-/// 
+///
+/// [heading("Blah 2")] # -> DocSegmentHeader(weight=0)
+/// # the weight is <=subsection -> subsection 1.1 automatically ends, subheading.build_doc_segment() called
+/// # the weight is <=section -> section 1 automatically ends, heading.build_doc_segment() called
+///
 /// Some other text in a second section
 /// ```
-/// 
+///
 /// There can be weird interactions with manual scopes.
 /// It may be confusing for a renderer to find Section containing Manual Scope containing Subsection,
 /// having the Subsection not as a direct child of the Section.
-/// Thus we allow manual scopes to be opened and closed as usual, but we don't allow ImplicitStructures *within* them.
-/// Effectively ImplicitStructure must only exist at the "top level" - they may be enclosed by ImplicitStructures, but nothing else.
-/// [TODO] this means subfiles need to emit lists of blocks directly into the enclosing BlockScope,
-/// as otherwise you couldn't have an ImplicitStructures inside them at all - they'd all be implicitly contained by a BlockScope
-/// 
+/// Thus we allow manual scopes to be opened and closed as usual, but we don't allow DocSegments *within* them.
+/// Effectively DocSegments must only exist at the "top level" - they may be enclosed by DocSegments directly, but nothing else.
+///
 /// An example error from mixing explicit and implicit scoping:
 /// ```text
 /// [section("One")]
-/// 
+///
 /// this text is clearly in section 1
-/// 
+///
 /// {
 ///     [subsection("One.One")]
-/// 
+///
 ///     this text is clearly in subsection 1.1...
 /// } # Maybe this should be an error? but then it's only a problem if there's bare text underneath...
-/// 
+///
 /// but where is this?? # This is really the error.
-/// 
+///
 /// [subsection("One.Two")]
-/// 
+///
 /// this text is clearly in subsection 1.2
 /// ```
 #[pyclass]
-#[derive(Debug,Clone)]
-pub struct ImplicitStructure {
-    pub header: Paragraph,
-    pub children: BlockScope,
-    pub weight: i64,
+#[derive(Debug, Clone)]
+pub struct DocSegment {
+    pub header: Option<PyTcRef<DocSegmentHeader>>,
+    pub contents: Py<BlockScope>,
+    pub subsegments: PyInstanceList<DocSegment>,
+}
+impl DocSegment {
+    pub fn new_no_header(
+        py: Python,
+        contents: Py<BlockScope>,
+        subsegments: PyInstanceList<DocSegment>,
+    ) -> PyResult<Self> {
+        Self::new_checked(py, None, contents, subsegments)
+    }
+    pub fn new_checked(
+        py: Python,
+        header: Option<PyTcRef<DocSegmentHeader>>,
+        contents: Py<BlockScope>,
+        subsegments: PyInstanceList<DocSegment>,
+    ) -> PyResult<Self> {
+        match &header {
+            Some(h) => {
+                let weight = DocSegmentHeader::get_weight(py, h.as_ref(py))?;
+                for subsegment in subsegments.list(py).iter() {
+                    let subsegment: Py<DocSegment> = subsegment.extract()?;
+                    match &subsegment.borrow(py).header {
+                        Some(subh) => {
+                            let subweight = DocSegmentHeader::get_weight(py, subh.as_ref(py))?;
+                            if subweight <= weight {
+                                return Err(PyValueError::new_err(format!("Trying to create a DocSegment with weight {weight} but one of the provided subsegments has weight {subweight} which is smaller. Only larger subweights are allowed.")))
+                            }
+                        }
+                        None => return Err(PyValueError::new_err(format!("Trying to create a DocSegment but a subsegement doesn't have a header. All subsegments must have headers.")))
+                    };
+                }
+            }
+            None => {}
+        }
+
+        Ok(Self {
+            header,
+            contents,
+            subsegments,
+        })
+    }
 }
 #[pymethods]
-impl ImplicitStructure {
+impl DocSegment {
+    #[new]
+    pub fn new(header: &PyAny, contents: Py<BlockScope>, subsegments: &PyList) -> PyResult<Self> {
+        Ok(Self {
+            header: Some(PyTcRef::of(header)?),
+            contents,
+            subsegments: PyInstanceList::from(subsegments)?,
+        })
+    }
     #[getter]
-    pub fn is_block(&self) -> bool {
-        true
+    pub fn header<'py>(&'py self, py: Python<'py>) -> Option<&'py PyAny> {
+        self.header.as_ref().map(|obj| obj.as_ref(py))
+    }
+    #[getter]
+    pub fn contents<'py>(&'py self, py: Python<'py>) -> &'py PyAny {
+        self.contents.as_ref(py)
+    }
+    #[getter]
+    pub fn subsegments<'py>(&'py self, py: Python<'py>) -> PyResult<&'py PyIterator> {
+        PyIterator::from_object(py, self.subsegments.list(py))
+    }
+    pub fn push_subsegment(&self, py: Python<'_>, subsegment: Py<DocSegment>) -> PyResult<()> {
+        match (&self.header, &subsegment.borrow(py).header) {
+            (Some(header), Some(subheader)) => {
+                let weight = DocSegmentHeader::get_weight(py, header.as_ref(py))?;
+                let subweight = DocSegmentHeader::get_weight(py, subheader.as_ref(py))?;
+                if subweight <= weight {
+                    return Err(PyValueError::new_err(format!("Trying to add to a DocSegment with weight {weight} but the provided subsegment has weight {subweight} which is smaller. Only larger subweights are allowed.")))
+                }
+            }
+            (_, None) => return Err(PyValueError::new_err(format!("Trying to add to a DocSegment but the subsegement doesn't have a header. All subsegments must have headers."))),
+            _ => {}
+        };
+        self.subsegments.append_checked(subsegment.as_ref(py))
     }
 }
-
-//
```

### Comparing `turnip_text-0.0.4/src/python/interp/eval_bracket.rs` & `turnip_text-0.0.5/src/interpreter/eval_bracket.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,62 @@
-use pyo3::{exceptions::PySyntaxError, ffi::Py_None, types::PyDict, Py, PyAny, PyResult, Python, intern};
+use pyo3::{
+    exceptions::PySyntaxError, ffi::Py_None, intern, types::PyDict, Py, PyAny, PyResult, Python,
+};
+
+use crate::{error::TurnipTextContextlessResult, lexer::TTToken, util::ParseSpan};
 
-use crate::{
-    lexer::TTToken,
+use super::{
     python::{
         interop::{
-            coerce_to_inline_pytcref, Block, BlockScopeBuilder, Inline, InlineScopeBuilder,
-            RawScopeBuilder,
+            coerce_to_inline_pytcref, Block, BlockScopeBuilder, DocSegmentHeader, Inline,
+            InlineScopeBuilder, InsertedFile, RawScopeBuilder,
         },
         typeclass::PyTcRef,
     },
-    util::ParseSpan,
+    MapContextlessResult,
 };
 
-use super::{InterpResult, MapInterpResult};
-
 pub enum EvalBracketContext {
     NeedBlockBuilder,
     NeedInlineBuilder,
     NeedRawBuilder { n_hashes: usize },
-    WantBlockOrInlineOrNone,
+    WantNonBuilder,
 }
 pub enum EvalBracketResult {
     /// A BlockScopeBuilder which was Needed because the final token was a [TTToken::CodeCloseOwningBlock]
     NeededBlockBuilder(PyTcRef<BlockScopeBuilder>),
     /// An InlineScopeBuilder which was Needed because the final token was a [TTToken::CodeCloseOwningInline]
     NeededInlineBuilder(PyTcRef<InlineScopeBuilder>),
     /// A RawScopeBuilder which was Needed because the final token was a [TTToken::CodeCloseOwningRaw]
     NeededRawBuilder(PyTcRef<RawScopeBuilder>, usize),
+    /// An object implementing DocSegmentHeader
+    DocSegmentHeader(PyTcRef<DocSegmentHeader>),
     /// An object implementing Block
     Block(PyTcRef<Block>),
     /// An object implementing Inline, or which was coerced to something implementing Inline
     Inline(PyTcRef<Inline>),
+    /// A InsertedFile object
+    InsertedFile(InsertedFile),
     /// None - either because it was an exec statement (e.g. `[x = 5]`) or because it genuinely was none (e.g. `[None]`)
     PyNone,
 }
 impl EvalBracketResult {
     pub fn eval_in_ctx(
         py: Python,
-        globals: &PyDict,
+        py_env: &PyDict,
         code: &str,
         ctx: EvalBracketContext,
     ) -> PyResult<EvalBracketResult> {
         // Python picks up leading whitespace as an incorrect indent
         let code = code.trim();
-        let raw_res = match py.eval(code, Some(globals), None) {
+        let raw_res = match py.eval(code, Some(py_env), None) {
             Ok(raw_res) => raw_res,
             Err(error) if error.is_instance_of::<PySyntaxError>(py) => {
                 // Try to exec() it as a statement instead of eval() it as an expression
-                py.run(code, Some(globals), None)?;
+                py.run(code, Some(py_env), None)?;
                 // Acquire a Py<PyAny> to Python None, then use into_ref() to convert it into a &PyAny.
                 // This should optimize down to `*Py_None()` because Py<T> and PyAny both boil down to *ffi::Py_Object;
                 // This is so that places that *require* non-None (e.g. NeedBlockBuilder) will always raise an error in the following match statement.
                 // This is safe because Py_None() returns a pointer-to-static.
                 unsafe { Py::<PyAny>::from_borrowed_ptr(py, Py_None()).into_ref(py) }
             }
             Err(error) => return Err(error),
@@ -59,32 +64,32 @@
         // If it has __get__, call it.
         // `property` objects and other data descriptors use this.
         let getter = intern!(py, "__get__");
         let raw_res = if raw_res.hasattr(getter)? {
             // https://docs.python.org/3.8/howto/descriptor.html
             // "For objects, the machinery is in object.__getattribute__() which transforms b.x into type(b).__dict__['x'].__get__(b, type(b))."
             //
-            // We're transforming `[x]` into (effectively) `globals.x`
-            // which should transform into (type(globals).__dict__['x']).__get__(globals, type(globals))
-            // = raw_res.__get__(globals, type(globals))
-            raw_res.call_method1(getter, (globals, globals.get_type()))?
+            // We're transforming `[x]` into (effectively) `py_env.x`
+            // which should transform into (type(py_env).__dict__['x']).__get__(py_env, type(py_env))
+            // = raw_res.__get__(py_env, type(py_env))
+            raw_res.call_method1(getter, (py_env, py_env.get_type()))?
         } else {
             raw_res
         };
         let res = match ctx {
             EvalBracketContext::NeedBlockBuilder => {
                 EvalBracketResult::NeededBlockBuilder(PyTcRef::of(raw_res)?)
             }
             EvalBracketContext::NeedInlineBuilder => {
                 EvalBracketResult::NeededInlineBuilder(PyTcRef::of(raw_res)?)
             }
             EvalBracketContext::NeedRawBuilder { n_hashes } => {
                 EvalBracketResult::NeededRawBuilder(PyTcRef::of(raw_res)?, n_hashes)
             }
-            EvalBracketContext::WantBlockOrInlineOrNone => {
+            EvalBracketContext::WantNonBuilder => {
                 if raw_res.is_none() {
                     EvalBracketResult::PyNone
                 } else {
                     // Consider: we may have an object at the very start of the line.
                     // If it's an Inline, e.g. "[virtio] is a thing..." then we want to return Inline so the rest of the line can be added.
                     // If it's a Block, e.g. [image_figure(...)], then we want to return Block.
                     // If it's neither, it needs to be *coerced*.
@@ -100,90 +105,86 @@
                     // - Sentence          -> `Paragraph([x])
                     // - CoercibleToInline -> `Paragraph([Sentence([coerce_to_inline(x)])])`
                     // I do not see the need to allow eval-brackets to directly return List[Block] or Sentence at all.
                     // Similar outcomes can be acheived by wrapping in BlockScope or Paragraph manually in the evaluated code, which better demonstrates intent.
                     // If we always coerce to inline, then the wrapping in Paragraph and Sentence happens naturally in the interpreter.
                     // => We check if it's a block, and if it isn't we try to coerce to inline.
 
-                    if let Ok(blk) = PyTcRef::of(raw_res) {
+                    // If they return an InsertedFile then just do that.
+                    if let Ok(inserted_file) = raw_res.extract::<InsertedFile>() {
+                        EvalBracketResult::InsertedFile(inserted_file)
+                    } else if let Ok(doc_seg) = PyTcRef::of(raw_res) {
+                        EvalBracketResult::DocSegmentHeader(doc_seg)
+                    } else if let Ok(blk) = PyTcRef::of(raw_res) {
                         EvalBracketResult::Block(blk)
                     } else {
                         EvalBracketResult::Inline(coerce_to_inline_pytcref(py, raw_res)?)
                     }
                 }
             }
         };
         Ok(res)
     }
 }
 
-/// If the code is closed, evaluates the result and checks it matches the type of code close:
+/// When eval-brackets are closed, evaluates the result and checks it matches the type of close:
 /// - [TTToken::CodeCloseOwningBlock] -> block builder
 /// - [TTToken::CodeCloseOwningInline] -> inline builder
 /// - [TTToken::CodeCloseOwningRaw] -> raw builder
 /// - [TTToken::CodeClose] -> block | inline | none
-pub fn handle_code_mode(
+pub fn eval_brackets(
     data: &str,
     tok: TTToken,
     code: &mut String,
     code_start: &ParseSpan,
     expected_close_len: usize,
     py: Python,
-    globals: &PyDict,
-) -> InterpResult<Option<(EvalBracketResult, ParseSpan)>> {
+    py_env: &PyDict,
+) -> TurnipTextContextlessResult<Option<(EvalBracketResult, ParseSpan)>> {
     let (code_span, eval_ctx) = match tok {
         TTToken::CodeClose(close_span, n_close_brackets)
             if n_close_brackets == expected_close_len =>
         {
             (
-                ParseSpan {
-                    start: code_start.start,
-                    end: close_span.end,
-                },
-                EvalBracketContext::WantBlockOrInlineOrNone,
+                code_start.combine(&close_span),
+                EvalBracketContext::WantNonBuilder,
             )
         }
         TTToken::CodeCloseOwningBlock(close_span, n_close_brackets)
             if n_close_brackets == expected_close_len =>
         {
             (
-                ParseSpan {
-                    start: code_start.start,
-                    end: close_span.end,
-                },
+                code_start.combine(&close_span),
                 EvalBracketContext::NeedBlockBuilder,
             )
         }
         TTToken::CodeCloseOwningInline(close_span, n_close_brackets)
             if n_close_brackets == expected_close_len =>
         {
             (
-                ParseSpan {
-                    start: code_start.start,
-                    end: close_span.end,
-                },
+                code_start.combine(&close_span),
                 EvalBracketContext::NeedInlineBuilder,
             )
         }
         TTToken::CodeCloseOwningRaw(close_span, n_close_brackets, n_hashes)
             if n_close_brackets == expected_close_len =>
         {
             (
-                ParseSpan {
-                    start: code_start.start,
-                    end: close_span.end,
-                },
+                code_start.combine(&close_span),
                 EvalBracketContext::NeedRawBuilder { n_hashes },
             )
         }
 
         _ => {
             // Code blocks use raw stringification to avoid confusion between text written and text entered
             code.push_str(tok.stringify_raw(data));
             return Ok(None);
         }
     };
 
-    let res =
-        EvalBracketResult::eval_in_ctx(py, globals, code, eval_ctx).err_as_interp(py, code_span)?;
+    let res = EvalBracketResult::eval_in_ctx(py, py_env, code, eval_ctx).err_as_interp(
+        py,
+        "Error while evaluating initial python code",
+        code_span,
+    )?;
     Ok(Some((res, code_span)))
 }
```

### Comparing `turnip_text-0.0.4/src/python/interp/para.rs` & `turnip_text-0.0.5/src/interpreter/para.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 use pyo3::{prelude::*, types::PyDict};
 
 use crate::{
+    error::TurnipTextContextlessError,
+    interpreter::{eval_brackets, EvalBracketResult, InterpError},
     lexer::{Escapable, TTToken},
-    python::{
-        interop::*,
-        interp::{handle_code_mode, EvalBracketResult, InterpError, MapInterpResult},
-        typeclass::PyTcRef,
-    },
     util::ParseSpan,
 };
 
-use super::{InlineNodeToCreate, InterpBlockTransition, InterpResult, InterpSpecialTransition};
+use super::{
+    InlineNodeToCreate, InterpBlockTransition, InterpSpecialTransition, MapContextlessResult,
+    TurnipTextContextlessResult,
+};
+
+use super::python::{
+    interop::*,
+    typeclass::{PyTcRef, PyTcUnionRef},
+};
 
 #[derive(Debug)]
 pub(crate) struct InterpParaState {
     para: Py<Paragraph>,
     sentence: Py<Sentence>,
     inline_stack: Vec<InterpInlineScopeState>,
     sentence_state: InterpSentenceState,
@@ -23,19 +28,23 @@
 #[derive(Debug)]
 struct InterpInlineScopeState {
     builder: Option<PyTcRef<InlineScopeBuilder>>,
     children: Py<InlineScope>,
     scope_start: ParseSpan,
 }
 impl InterpInlineScopeState {
-    fn build_to_inline(self, py: Python, scope_end: ParseSpan) -> InterpResult<PyTcRef<Inline>> {
-        let scope = ParseSpan::new(self.scope_start.start, scope_end.end);
+    fn build_to_inline(
+        self,
+        py: Python,
+        scope_end: ParseSpan,
+    ) -> TurnipTextContextlessResult<PyTcRef<Inline>> {
+        let scope = self.scope_start.combine(&scope_end);
         match self.builder {
             Some(builder) => InlineScopeBuilder::call_build_from_inlines(py, builder, self.children)
-                .err_as_interp(py, scope),
+                .err_as_interp(py, "Error while calling .build_from_inlines() on an object", scope),
             None => Ok(PyTcRef::of(self.children.as_ref(py)).expect("Internal error: InterpInlineScopeState::children, an InlineScope, somehow doesn't fit the Inline typeclass")),
         }
     }
 }
 
 /// Interpreter state specific to parsing paragraphs and the content within (i.e. inline content)
 #[derive(Debug)]
@@ -174,15 +183,15 @@
     pub(crate) fn para(&self) -> &Py<Paragraph> {
         &self.para
     }
 
     pub(crate) fn finalize(
         &mut self,
         py: Python,
-    ) -> InterpResult<(
+    ) -> TurnipTextContextlessResult<(
         Option<InterpBlockTransition>,
         Option<InterpSpecialTransition>,
     )> {
         match self.sentence_state {
             InterpSentenceState::SentenceStart | InterpSentenceState::MidSentence => {
                 // This will automatically check if we're inside an inline scope
                 self.handle_transition(py, Some(InterpParaTransition::EndParagraph(None)))
@@ -190,42 +199,43 @@
             InterpSentenceState::BuildingText { .. } => {
                 self.handle_transition(py, Some(InterpParaTransition::BreakSentence))?;
                 // This will automatically check if we're inside an inline scope
                 self.handle_transition(py, Some(InterpParaTransition::EndParagraph(None)))
             }
             // Error states
             InterpSentenceState::BuildingCode { code_start, .. } => {
-                return Err(InterpError::EndedInsideCode { code_start })
+                return Err(InterpError::EndedInsideCode { code_start }.into())
             }
             InterpSentenceState::BuildingRawText { raw_start, .. } => {
                 return Err(InterpError::EndedInsideRawScope {
                     raw_scope_start: raw_start,
-                })
+                }
+                .into())
             }
         }
     }
 
     pub(crate) fn handle_token(
         &mut self,
         py: Python,
-        globals: &PyDict,
+        py_env: &PyDict,
         tok: TTToken,
         data: &str,
-    ) -> InterpResult<(
+    ) -> TurnipTextContextlessResult<(
         Option<InterpBlockTransition>,
         Option<InterpSpecialTransition>,
     )> {
-        let transition = self.mutate_state_and_find_transition(py, globals, tok, data)?;
+        let transition = self.mutate_state_and_find_transition(py, py_env, tok, data)?;
         self.handle_transition(py, transition)
     }
     pub(crate) fn handle_transition(
         &mut self,
         py: Python,
         transition: Option<InterpParaTransition>,
-    ) -> InterpResult<(
+    ) -> TurnipTextContextlessResult<(
         Option<InterpBlockTransition>,
         Option<InterpSpecialTransition>,
     )> {
         if let Some(transition) = transition {
             use InterpParaTransition as T;
             use InterpSentenceState as S;
 
@@ -294,32 +304,26 @@
                     self.break_sentence(py)?;
                     (
                         S::SentenceStart,
                         (None, Some(InterpSpecialTransition::StartComment(span))),
                     )
                 }
 
-                (
-                    S::BuildingCode { .. },
-                    T::EmitNone,
-                ) => {
-                    (S::MidSentence, (None, None))
-                }
+                (S::BuildingCode { .. }, T::EmitNone) => (S::MidSentence, (None, None)),
 
                 (
                     S::SentenceStart
                     | S::MidSentence
                     | S::BuildingCode { .. }
                     | S::BuildingText { .. },
                     T::PushInlineScope(builder, span),
                 ) => {
                     let scope = InterpInlineScopeState {
                         builder,
-                        children: Py::new(py, InlineScope::new_empty(py))
-                            .err_as_interp_internal(py)?,
+                        children: Py::new(py, InlineScope::new_empty(py)).err_as_internal(py)?,
                         scope_start: span,
                     };
                     self.inline_stack.push(scope);
                     (S::MidSentence, (None, None))
                 }
                 (
                     S::SentenceStart | S::MidSentence | S::BuildingText { .. },
@@ -328,15 +332,15 @@
                     let popped_scope = self.inline_stack.pop();
                     match popped_scope {
                         Some(popped_scope) => {
                             let inline_item = popped_scope.build_to_inline(py, scope_end)?;
                             self.push_to_topmost_scope(py, inline_item.as_ref(py))?
                         },
                         None => {
-                            return Err(InterpError::InternalErr("PopInlineScope attempted with no inline scopes - should use EndParagraphAndPopBlock in this case".into()))
+                            return Err(TurnipTextContextlessError::Internal("PopInlineScope attempted with no inline scopes - should use EndParagraphAndPopBlock in this case".into()))
                         }
                     };
                     (S::MidSentence, (None, None))
                 }
 
                 (
                     S::SentenceStart
@@ -371,17 +375,18 @@
                     T::EndParagraph(para_break),
                 ) => {
                     if let Err(scope_start) = self.check_inline_scopes_closed() {
                         if let Some(para_break) = para_break {
                             return Err(InterpError::ParaBreakInInlineScope {
                                 scope_start,
                                 para_break,
-                            });
+                            }
+                            .into());
                         } else {
-                            return Err(InterpError::EndedInsideScope { scope_start });
+                            return Err(InterpError::EndedInsideScope { scope_start }.into());
                         }
                     }
                     self.break_sentence(py)?;
                     (
                         S::SentenceStart,
                         (Some(InterpBlockTransition::EndParagraph), None),
                     )
@@ -389,61 +394,64 @@
 
                 (
                     S::SentenceStart | S::MidSentence | S::BuildingText { .. },
                     T::EndParagraphAndPopBlock(scope_end_span),
                 ) => {
                     // This is only called when all inline scopes are closed - just assert they are
                     self.check_inline_scopes_closed().map_err(|_| {
-                        InterpError::InternalErr("paragraph EndParagraphAndPopBlock transition invoked when inline scopes are still on the stack".into())
+                        TurnipTextContextlessError::Internal("paragraph EndParagraphAndPopBlock transition invoked when inline scopes are still on the stack".into())
                     })?;
                     self.break_sentence(py)?;
                     (
                         S::SentenceStart,
                         (
                             Some(InterpBlockTransition::EndParagraphAndCloseManualBlockScope(
                                 scope_end_span,
                             )),
                             None,
                         ),
                     )
                 }
 
                 (_, transition) => {
-                    return Err(InterpError::InternalErr(format!(
-                        "Invalid inline state/transition pair encountered ({0:?}, {1:?})",
-                        self.sentence_state, transition
-                    )))
+                    return Err(TurnipTextContextlessError::Internal(
+                        format!(
+                            "Invalid inline state/transition pair encountered ({0:?}, {1:?})",
+                            self.sentence_state, transition
+                        )
+                        .into(),
+                    ))
                 }
             };
             self.sentence_state = new_inl_state;
             Ok(transitions)
         } else {
             Ok((None, None))
         }
     }
     /// Helper function
-    fn break_sentence(&mut self, py: Python) -> InterpResult<()> {
+    fn break_sentence(&mut self, py: Python) -> TurnipTextContextlessResult<()> {
         // If the sentence has stuff in it, push it into the paragraph and make a new one
         if self.sentence.borrow(py).__len__(py) > 0 {
             self.para
                 .borrow_mut(py)
                 .push_sentence(self.sentence.as_ref(py))
-                .err_as_interp_internal(py)?;
-            self.sentence = Py::new(py, Sentence::new_empty(py)).err_as_interp_internal(py)?;
+                .err_as_internal(py)?;
+            self.sentence = Py::new(py, Sentence::new_empty(py)).err_as_internal(py)?;
         }
         Ok(())
     }
 
     fn mutate_state_and_find_transition(
         &mut self,
         py: Python,
-        globals: &PyDict,
+        py_env: &PyDict,
         tok: TTToken,
         data: &str,
-    ) -> InterpResult<Option<InterpParaTransition>> {
+    ) -> TurnipTextContextlessResult<Option<InterpParaTransition>> {
         use InterpParaTransition::*;
         use TTToken::*;
 
         let transition = match &mut self.sentence_state {
             InterpSentenceState::SentenceStart => match tok {
                 // Escaped newline => "Continue sentence".
                 // at the start of a sentence, "Continue sentence" has no meaning
@@ -452,23 +460,23 @@
                 Whitespace(_) => None,
 
                 Newline(span) => Some(EndParagraph(Some(span))),
                 Hashes(span, _) => Some(StartComment(span)),
 
                 CodeOpen(span, n) => Some(StartInlineLevelCode(span, n)),
                 BlockScopeOpen(span) => {
-                    return Err(InterpError::BlockScopeOpenedMidPara { scope_start: span })
+                    return Err(InterpError::BlockScopeOpenedMidPara { scope_start: span }.into())
                 }
                 InlineScopeOpen(span) => Some(PushInlineScope(None, span)),
                 RawScopeOpen(span, n) => Some(StartRawScope(None, span, n)),
 
-                CodeClose(span, _) => return Err(InterpError::CodeCloseOutsideCode(span)),
+                CodeClose(span, _) => return Err(InterpError::CodeCloseOutsideCode(span).into()),
                 ScopeClose(span) => Some(self.try_pop_scope(py, span)?),
                 RawScopeClose(span, _) => {
-                    return Err(InterpError::RawScopeCloseOutsideRawScope(span))
+                    return Err(InterpError::RawScopeCloseOutsideRawScope(span).into())
                 }
 
                 _ => Some(StartText(tok.stringify_escaped(data).into())),
             },
             InterpSentenceState::MidSentence => match tok {
                 // Escaped newline => "Continue sentence" i.e. no sentence break
                 // mid-sentence, "Continue sentence" just means "do nothing"
@@ -476,23 +484,23 @@
 
                 // Newline => Sentence break
                 Newline(_) => Some(BreakSentence),
                 Hashes(span, _) => Some(StartComment(span)),
 
                 CodeOpen(span, n) => Some(StartInlineLevelCode(span, n)),
                 BlockScopeOpen(span) => {
-                    return Err(InterpError::BlockScopeOpenedMidPara { scope_start: span })
+                    return Err(InterpError::BlockScopeOpenedMidPara { scope_start: span }.into())
                 }
                 InlineScopeOpen(span) => Some(PushInlineScope(None, span)),
                 RawScopeOpen(span, n) => Some(StartRawScope(None, span, n)),
 
-                CodeClose(span, _) => return Err(InterpError::CodeCloseOutsideCode(span)),
+                CodeClose(span, _) => return Err(InterpError::CodeCloseOutsideCode(span).into()),
                 ScopeClose(span) => Some(self.try_pop_scope(py, span)?),
                 RawScopeClose(span, _) => {
-                    return Err(InterpError::RawScopeCloseOutsideRawScope(span))
+                    return Err(InterpError::RawScopeCloseOutsideRawScope(span).into())
                 }
 
                 // Whitespace is included in text
                 Whitespace(_) | _ => Some(StartText(tok.stringify_escaped(data).into())),
             },
             InterpSentenceState::BuildingText {
                 text,
@@ -504,23 +512,23 @@
 
                 // Newline => Sentence break
                 Newline(_) => Some(BreakSentence),
                 Hashes(span, _) => Some(StartComment(span)),
 
                 CodeOpen(span, n) => Some(StartInlineLevelCode(span, n)),
                 BlockScopeOpen(span) => {
-                    return Err(InterpError::BlockScopeOpenedMidPara { scope_start: span })
+                    return Err(InterpError::BlockScopeOpenedMidPara { scope_start: span }.into())
                 }
                 InlineScopeOpen(span) => Some(PushInlineScope(None, span)),
                 RawScopeOpen(span, n) => Some(StartRawScope(None, span, n)),
 
-                CodeClose(span, _) => return Err(InterpError::CodeCloseOutsideCode(span)),
+                CodeClose(span, _) => return Err(InterpError::CodeCloseOutsideCode(span).into()),
                 ScopeClose(span) => Some(self.try_pop_scope(py, span)?),
                 RawScopeClose(span, _) => {
-                    return Err(InterpError::RawScopeCloseOutsideRawScope(span))
+                    return Err(InterpError::RawScopeCloseOutsideRawScope(span).into())
                 }
 
                 // Whitespace is pushed to pending_whitespace, and no transition takes place.
                 Whitespace(_) => {
                     match pending_whitespace {
                         Some(pw) => pw.push_str(tok.stringify_escaped(data)),
                         None => *pending_whitespace = Some(tok.stringify_escaped(data).into()),
@@ -538,36 +546,40 @@
                 }
             },
             InterpSentenceState::BuildingCode {
                 code,
                 code_start,
                 expected_n_hashes,
             } => {
-                match handle_code_mode(
-                    data,
-                    tok,
-                    code,
-                    code_start,
-                    *expected_n_hashes,
-                    py,
-                    globals,
-                )? {
+                match eval_brackets(data, tok, code, code_start, *expected_n_hashes, py, py_env)? {
                     Some((res, code_span)) => {
                         // The code ended...
                         use EvalBracketResult::*;
 
                         let inl_transition = match res {
                             NeededBlockBuilder(_) => {
-                                return Err(InterpError::BlockOwnerCodeMidPara { code_span })
+                                return Err(InterpError::BlockOwnerCodeMidPara { code_span }.into())
+                            }
+                            // This is inline code because we're already deep into a paragraph at this point.
+                            // Definitely can't emit a segment here.
+                            DocSegmentHeader(_) => {
+                                return Err(
+                                    InterpError::DocSegmentHeaderMidPara { code_span }.into()
+                                )
                             }
                             Block(_) => {
-                                return Err(InterpError::BlockCodeMidPara { code_span });
+                                return Err(InterpError::BlockCodeMidPara { code_span }.into())
+                            }
+                            InsertedFile(_) => {
+                                return Err(InterpError::InsertedFileMidPara { code_span }.into())
                             }
                             NeededInlineBuilder(i) => PushInlineScope(Some(i), code_span),
-                            NeededRawBuilder(r, n_hashes) => StartRawScope(Some(r), code_span, n_hashes),
+                            NeededRawBuilder(r, n_hashes) => {
+                                StartRawScope(Some(r), code_span, n_hashes)
+                            }
                             // This includes coerced objects - e.g. eval bracket returning a string gets wrapped in UnescapedText automatically
                             Inline(i) => PushInlineContent(InlineNodeToCreate::PythonObject(i)),
                             PyNone => EmitNone,
                         };
                         Some(inl_transition)
                     }
                     None => None,
@@ -577,57 +589,62 @@
                 builder,
                 text,
                 expected_n_hashes,
                 raw_start,
             } => match tok {
                 RawScopeClose(_, n_hashes) if n_hashes == *expected_n_hashes => match builder {
                     Some(builder) => {
-                        let to_emit = RawScopeBuilder::call_build_from_raw(py, builder, text).err_as_interp(py, *raw_start)?;
-                    
-                        let to_emit_as_py = to_emit.as_ref(py);
-                        if let Ok(_) = PyTcRef::<Block>::of(to_emit_as_py) {
-                            return Err(InterpError::BlockCodeFromRawScopeMidPara{ code_span: *raw_start })
-                        } else if let Ok(inl) = PyTcRef::of(to_emit_as_py) {
-                            Some(PushInlineContent(InlineNodeToCreate::PythonObject(inl)))
-                        } else {
-                            unreachable!()
+                        let to_emit = RawScopeBuilder::call_build_from_raw(py, builder, text)
+                            .err_as_interp(
+                                py,
+                                "Error while calling .build_from_raw() on an object",
+                                *raw_start,
+                            )?;
+
+                        match to_emit {
+                            PyTcUnionRef::A(inl) => {
+                                Some(PushInlineContent(InlineNodeToCreate::PythonObject(inl)))
+                            }
+                            PyTcUnionRef::B(_) => {
+                                return Err(InterpError::BlockCodeFromRawScopeMidPara {
+                                    code_span: *raw_start,
+                                }
+                                .into())
+                            }
                         }
-                    },
-                    None => Some(
-                        PushInlineContent(InlineNodeToCreate::RawText(text.clone())),
-                    ),
-                }
-                    
+                    }
+                    None => Some(PushInlineContent(InlineNodeToCreate::RawText(text.clone()))),
+                },
+
                 _ => {
                     text.push_str(tok.stringify_raw(data));
                     None
                 }
             },
         };
         Ok(transition)
     }
 
     fn try_pop_scope(
         &mut self,
         py: Python,
         scope_close_span: ParseSpan,
-    ) -> InterpResult<InterpParaTransition> {
+    ) -> TurnipTextContextlessResult<InterpParaTransition> {
         match self.inline_stack.last() {
             Some(InterpInlineScopeState { .. }) => {
                 Ok(InterpParaTransition::PopInlineScope(scope_close_span))
             }
             None => {
                 // If the sentence has stuff in it, push it into the paragraph and make a new one
                 if self.sentence.borrow(py).__len__(py) > 0 {
                     self.para
                         .borrow_mut(py)
                         .push_sentence(self.sentence.as_ref(py))
-                        .err_as_interp_internal(py)?;
-                    self.sentence =
-                        Py::new(py, Sentence::new_empty(py)).err_as_interp_internal(py)?;
+                        .err_as_internal(py)?;
+                    self.sentence = Py::new(py, Sentence::new_empty(py)).err_as_internal(py)?;
                 }
                 Ok(InterpParaTransition::EndParagraphAndPopBlock(
                     scope_close_span,
                 ))
             }
         }
     }
@@ -637,15 +654,15 @@
         if let Some(i) = self.inline_stack.last() {
             Err(i.scope_start)
         } else {
             Ok(())
         }
     }
 
-    fn push_to_topmost_scope(&self, py: Python, node: &PyAny) -> InterpResult<()> {
+    fn push_to_topmost_scope(&self, py: Python, node: &PyAny) -> TurnipTextContextlessResult<()> {
         match self.inline_stack.last() {
             Some(i) => i.children.borrow_mut(py).push_inline(node),
             None => self.sentence.borrow_mut(py).push_inline(node),
         }
-        .err_as_interp_internal(py)
+        .err_as_internal(py)
     }
 }
```

### Comparing `turnip_text-0.0.4/src/tests/mod.rs` & `turnip_text-0.0.5/src/tests/mod.rs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 //! All tests are disabled unless compiled without the feature to make it clear that's necessary.
 #![cfg(all(test, not(feature = "extension-module")))]
 
 mod test_lexer;
 mod test_lexer_parser;
 mod test_parser;
 
-// TODO tests for coercion?
+// TODO tests for coercion?
```

### Comparing `turnip_text-0.0.4/src/tests/test_lexer.rs` & `turnip_text-0.0.5/src/tests/test_lexer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-use crate::lexer::{units_to_tokens, Unit};
+use crate::lexer::lex;
 
-use crate::lexer::{Escapable, LexError, LexPosn, LexToken, TTToken};
-use lexer_rs::{Lexer, LexerOfStr};
-
-pub type TextStream<'stream> = LexerOfStr<'stream, LexPosn, LexToken, LexError>;
+use crate::lexer::{Escapable, TTToken};
 
 /// A type mimicking [TTToken] for test purposes
 #[derive(Debug, Copy, Clone, PartialEq, Eq)]
 pub enum TestTTToken<'a> {
     Newline,
     Escaped(Escapable),
     Backslash,
@@ -47,24 +44,19 @@
             TTToken::OtherText(span) => Self::OtherText(data[span.byte_range()].into()),
             TTToken::Whitespace(span) => Self::Whitespace(data[span.byte_range()].into()),
         }
     }
 }
 
 /// Run the lexer on a given piece of text, convert the lexed tokens to our test versions, and compare with the expected result.
-fn expect_lex<'a>(data: &str, expected_stok_types: Vec<TestTTToken<'a>>) {
+pub fn expect_lex<'a>(data: &str, expected_stok_types: Vec<TestTTToken<'a>>) {
     println!("{:?}", data);
 
     // First step: lex
-    let l = TextStream::new(data);
-    let units: Vec<Unit> = l
-        .iter(&[Box::new(Unit::parse_special), Box::new(Unit::parse_other)])
-        .scan((), |_, x| x.ok())
-        .collect();
-    let stoks = units_to_tokens(units);
+    let stoks: Vec<TTToken> = lex(0, data).scan((), |_, x| x.ok()).collect();
     let stok_types: Vec<TestTTToken> = stoks
         .iter()
         .map(|stok| TestTTToken::from_str_tok(data, *stok))
         .collect();
 
     assert_eq!(stok_types, expected_stok_types);
 }
@@ -540,8 +532,8 @@
 }
 #[test]
 pub fn test_crlf() {
     // '\r' + '\n'
     expect_lex("\r\ncontent", vec![Newline, OtherText("content")])
 }
 
-// TODO test error messages for multibyte?
+// TODO test error messages for multibyte?
```

### Comparing `turnip_text-0.0.4/src/tests/test_lexer_parser.rs` & `turnip_text-0.0.5/src/tests/test_lexer_parser.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,22 @@
-use crate::lexer::{units_to_tokens, Unit};
-
 use crate::lexer::Escapable;
-use lexer_rs::Lexer;
 
 use super::test_lexer::*;
 use super::test_parser::*;
 
 /// Run the lexer AND parser on given data, checking the results of both against expected versions as specified in [super::test_lexer::expect_lex] and [super::test_parser::expect_parse]
 fn expect_lex_parse<'a>(
     data: &str,
     expected_stok_types: Vec<TestTTToken<'a>>,
-    expected_parse: Result<TestBlock, TestInterpError>,
+    expected_parse: Result<TestDocSegment, TestTurnipError>,
 ) {
     println!("{:?}", data);
 
-    // First step: lex
-    let l = TextStream::new(data);
-    let units: Vec<Unit> = l
-        .iter(&[Box::new(Unit::parse_special), Box::new(Unit::parse_other)])
-        .scan((), |_, x| x.ok())
-        .collect();
-    let stoks = units_to_tokens(units);
-    let stok_types: Vec<TestTTToken> = stoks
-        .iter()
-        .map(|stok| TestTTToken::from_str_tok(data, *stok))
-        .collect();
-
-    assert_eq!(stok_types, expected_stok_types);
-
-    expect_parse_tokens(data, stoks, expected_parse)
+    expect_lex(data, expected_stok_types);
+    expect_parse(data, expected_parse)
 }
 
 use TestTTToken::*;
 
 // These tests are condensed versions of the tests in [test_parser] that also sanity-check the tokens generated.
 
 #[test]
@@ -335,21 +319,18 @@
     )
 }
 
 #[test]
 pub fn test_special_with_escaped_backslash() {
     expect_lex_parse(
         r#"\\#"#,
-        vec![
-            Escaped(Escapable::Backslash),
-            Hashes(1),
-        ],
-        Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![
-            test_text("\\"),
-        ]])])),
+        vec![Escaped(Escapable::Backslash), Hashes(1)],
+        Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![test_text(
+            "\\",
+        )]])])),
     )
 }
 
 #[test]
 pub fn test_escaped_special_with_escaped_backslash() {
     expect_lex_parse(
         r#"\\\[not code"#,
```

### Comparing `turnip_text-0.0.4/src/tests/test_parser.rs` & `turnip_text-0.0.5/src/tests/test_parser.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,70 @@
-use crate::lexer::{units_to_tokens, TTToken, Unit};
-use crate::tests::test_lexer::TextStream;
-
-use lexer_rs::Lexer;
+use crate::error::{TurnipTextError, TurnipTextResult};
+use crate::interpreter::InterpError;
+use crate::parser::{ParsingFile, TurnipTextParser};
 use regex::Regex;
 
-use crate::python::interop::{
-    BlockScope, InlineScope, Paragraph, RawText, Sentence, UnescapedText,
+use crate::interpreter::python::{
+    interop::{
+        BlockScope, DocSegment, DocSegmentHeader, InlineScope, Paragraph, RawText, Sentence,
+        UnescapedText,
+    },
+    prepare_freethreaded_turniptext_python,
 };
-use crate::python::{interp_data, prepare_freethreaded_turniptext_python, InterpError};
 use crate::util::ParseSpan;
 
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 
 use std::panic;
 // We need to initialize Python the first time we test
 use std::sync::Once;
 static INIT_PYTHON: Once = Once::new();
 
 /// A type mimicking [ParserSpan] for test purposes
 #[derive(Debug, Clone, PartialEq, Eq)]
-pub struct TestParserSpan {
-    pub start: (usize, usize),
-    pub end: (usize, usize),
-}
-impl From<ParseSpan> for TestParserSpan {
-    fn from(p: ParseSpan) -> Self {
-        Self {
-            start: (p.start.line, p.start.column),
-            end: (p.end.line, p.end.column),
+pub struct TestParserSpan(&'static str);
+impl TestParserSpan {
+    fn same_text(&self, other: &ParseSpan, data: &Vec<ParsingFile>) -> bool {
+        let other_str = unsafe {
+            data[other.file_idx()]
+                .contents()
+                .get_unchecked(other.byte_range())
+        };
+        dbg!(self.0) == dbg!(other_str)
+    }
+}
+
+/// A type mimicking [TurnipTextError] for test purposes
+#[derive(Debug, Clone)]
+pub enum TestTurnipError {
+    Lex(char),
+    Interp(TestInterpError),
+    Internal(Regex),
+    InternalPython(Regex),
+}
+impl From<TestInterpError> for TestTurnipError {
+    fn from(value: TestInterpError) -> Self {
+        Self::Interp(value)
+    }
+}
+impl PartialEq<TurnipTextError> for TestTurnipError {
+    fn eq(&self, other: &TurnipTextError) -> bool {
+        match (self, other) {
+            (Self::Lex(l_ch), TurnipTextError::Lex(_, _, r_err)) => *l_ch == r_err.ch,
+            (Self::Interp(l_interp), TurnipTextError::Interp(sources, r_interp)) => {
+                l_interp.effectively_eq(r_interp, sources)
+            }
+            (Self::InternalPython(l_pyerr), TurnipTextError::InternalPython(r_pyerr)) => {
+                l_pyerr.is_match(&r_pyerr)
+            }
+            (Self::Internal(l_pyerr), TurnipTextError::Internal(r_pyerr)) => {
+                l_pyerr.is_match(&r_pyerr)
+            }
+            _ => false,
         }
     }
 }
 
 /// A type mimicking [InterpError] for test purposes
 #[derive(Debug, Clone)]
 pub enum TestInterpError {
@@ -79,144 +111,245 @@
     InternalPythonErr {
         pyerr: Regex,
     },
     InternalErr(Regex),
     EscapedNewlineOutsideParagraph {
         newline: TestParserSpan,
     },
+
+    DocSegmentHeaderMidPara {
+        code_span: TestParserSpan,
+    },
+
+    DocSegmentHeaderMidScope {
+        code_span: TestParserSpan,
+        block_close_span: Option<TestParserSpan>,
+        enclosing_scope_start: TestParserSpan,
+    },
 }
-impl PartialEq<InterpError> for TestInterpError {
-    fn eq(&self, other: &InterpError) -> bool {
+impl TestInterpError {
+    fn effectively_eq(&self, other: &InterpError, data: &Vec<ParsingFile>) -> bool {
         match (self, other) {
             (Self::CodeCloseOutsideCode(l0), InterpError::CodeCloseOutsideCode(r0)) => {
-                (*l0) == (*r0).into()
+                l0.same_text(r0, data)
             }
             (Self::ScopeCloseOutsideScope(l0), InterpError::ScopeCloseOutsideScope(r0)) => {
-                (*l0) == (*r0).into()
+                l0.same_text(r0, data)
             }
             (
                 Self::RawScopeCloseOutsideRawScope(l0),
                 InterpError::RawScopeCloseOutsideRawScope(r0),
-            ) => (*l0) == (*r0).into(),
+            ) => l0.same_text(r0, data),
             (
                 Self::EndedInsideCode {
                     code_start: l_code_start,
                 },
                 InterpError::EndedInsideCode {
                     code_start: r_code_start,
                 },
-            ) => (*l_code_start) == (*r_code_start).into(),
+            ) => l_code_start.same_text(r_code_start, data),
             (
                 Self::EndedInsideRawScope {
                     raw_scope_start: l_raw_scope_start,
                 },
                 InterpError::EndedInsideRawScope {
                     raw_scope_start: r_raw_scope_start,
                 },
-            ) => (*l_raw_scope_start) == (*r_raw_scope_start).into(),
+            ) => l_raw_scope_start.same_text(r_raw_scope_start, data),
             (
                 Self::EndedInsideScope {
                     scope_start: l_scope_start,
                 },
                 InterpError::EndedInsideScope {
                     scope_start: r_scope_start,
                 },
-            ) => (*l_scope_start) == (*r_scope_start).into(),
+            ) => l_scope_start.same_text(r_scope_start, data),
             (
                 Self::BlockScopeOpenedMidPara {
                     scope_start: l_scope_start,
                 },
                 InterpError::BlockScopeOpenedMidPara {
                     scope_start: r_scope_start,
                 },
-            ) => (*l_scope_start) == (*r_scope_start).into(),
+            ) => l_scope_start.same_text(r_scope_start, data),
             (
                 Self::BlockOwnerCodeMidPara {
                     code_span: l_code_span,
                 },
                 InterpError::BlockOwnerCodeMidPara {
                     code_span: r_code_span,
                 },
-            ) => (*l_code_span) == (*r_code_span).into(),
+            ) => l_code_span.same_text(r_code_span, data),
             (
                 Self::BlockCodeMidPara {
                     code_span: l_code_span,
                 },
                 InterpError::BlockCodeMidPara {
                     code_span: r_code_span,
                 },
-            ) => (*l_code_span) == (*r_code_span).into(),
+            ) => l_code_span.same_text(r_code_span, data),
             (
                 Self::BlockCodeFromRawScopeMidPara {
                     code_span: l_code_span,
                 },
                 InterpError::BlockCodeFromRawScopeMidPara {
                     code_span: r_code_span,
                 },
-            ) => (*l_code_span) == (*r_code_span).into(),
+            ) => l_code_span.same_text(r_code_span, data),
             (
                 Self::SentenceBreakInInlineScope {
                     scope_start: l_scope_start,
                 },
                 InterpError::SentenceBreakInInlineScope {
                     scope_start: r_scope_start,
                 },
-            ) => (*l_scope_start) == (*r_scope_start).into(),
+            ) => l_scope_start.same_text(r_scope_start, data),
             (
                 Self::ParaBreakInInlineScope {
                     scope_start: l_scope_start,
                 },
                 InterpError::ParaBreakInInlineScope {
                     scope_start: r_scope_start,
                     ..
                 },
-            ) => (*l_scope_start) == (*r_scope_start).into(),
+            ) => l_scope_start.same_text(r_scope_start, data),
             (
                 Self::BlockOwnerCodeHasNoScope {
                     code_span: l_code_span,
                 },
                 InterpError::BlockOwnerCodeHasNoScope {
                     code_span: r_code_span,
                 },
-            ) => (*l_code_span) == (*r_code_span).into(),
+            ) => l_code_span.same_text(r_code_span, data),
             (
                 Self::InlineOwnerCodeHasNoScope {
                     code_span: l_code_span,
                 },
                 InterpError::InlineOwnerCodeHasNoScope {
                     code_span: r_code_span,
                 },
-            ) => (*l_code_span) == (*r_code_span).into(),
+            ) => l_code_span.same_text(r_code_span, data),
 
             (
                 Self::PythonErr {
                     pyerr: l_pyerr,
                     code_span: l_code_span,
                 },
                 InterpError::PythonErr {
+                    ctx: _, // TODO this is user-facing - do we need to test it?
                     pyerr: r_pyerr,
                     code_span: r_code_span,
                 },
-            ) => dbg!(l_pyerr).is_match(&dbg!(r_pyerr)) && (*l_code_span) == (*r_code_span).into(),
-            (
-                Self::InternalPythonErr { pyerr: l_pyerr },
-                InterpError::InternalPythonErr { pyerr: r_pyerr },
-            ) => l_pyerr.is_match(&r_pyerr),
-
-            (Self::InternalErr(l0), InterpError::InternalErr(r0)) => l0.is_match(&r0),
+            ) => dbg!(l_pyerr).is_match(&dbg!(r_pyerr)) && l_code_span.same_text(r_code_span, data),
 
             (
                 Self::EscapedNewlineOutsideParagraph { newline: l_newline },
                 InterpError::EscapedNewlineOutsideParagraph { newline: r_newline },
-            ) => (*l_newline) == (*r_newline).into(),
+            ) => l_newline.same_text(r_newline, data),
+
+            (
+                Self::DocSegmentHeaderMidPara {
+                    code_span: l_code_span,
+                },
+                InterpError::DocSegmentHeaderMidPara {
+                    code_span: r_code_span,
+                },
+            ) => l_code_span.same_text(r_code_span, data),
+
+            (
+                Self::DocSegmentHeaderMidScope {
+                    code_span: l_code_span,
+                    block_close_span: l_block_close_span,
+                    enclosing_scope_start: l_enclosing_scope_start,
+                },
+                InterpError::DocSegmentHeaderMidScope {
+                    code_span: r_code_span,
+                    block_close_span: r_block_close_span,
+                    enclosing_scope_start: r_enclosing_scope_start,
+                },
+            ) => {
+                (l_code_span.same_text(r_code_span, data))
+                    && (match (l_block_close_span, r_block_close_span) {
+                        (Some(l), Some(r)) => l.same_text(r, data),
+                        (None, None) => true,
+                        _ => false,
+                    })
+                    && (l_enclosing_scope_start.same_text(r_enclosing_scope_start, data))
+            }
             _ => false,
         }
     }
 }
 
+const GLOBALS_CODE: &'static str = r#"
+# The Rust module name is _native, which is included under turnip_text, so Python IDEs don't try to import directly from it.
+# This means we use _native instead of turnip_text as the module name here.
+from _native import InlineScope, UnescapedText, BlockScope
+
+class FauxBlock:
+    is_block = True
+    def __init__(self, contents):
+        self.test_block = contents
+
+class FauxInline:
+    is_inline = True
+    def __init__(self, contents):
+        self.test_inline = contents
+
+class FauxInlineRaw:
+    is_inline = True
+    def __init__(self, raw_str):
+        self.test_raw_str = str(raw_str)
+
+class TestBuilder:
+    def build_from_blocks(self, contents):
+        return FauxBlock(contents)
+    def build_from_inlines(self, contents):
+        return FauxInline(contents)
+
+class TestRawInlineBuilder:
+    def build_from_raw(self, raw_str):
+        return FauxInlineRaw(raw_str)
+
+TEST_BLOCK = FauxBlock(BlockScope([]))
+
+class TestRawBlockBuilder:
+    def build_from_raw(self, raw_str):
+        return TEST_BLOCK
+
+class TestBlockSwallower():
+    def build_from_blocks(self, contents):
+        return None
+
+TEST_BLOCK_BUILDER = TestBuilder()
+TEST_INLINE_BUILDER = TestBuilder()
+TEST_RAW_INLINE_BUILDER = TestRawInlineBuilder()
+TEST_RAW_BLOCK_BUILDER = TestRawBlockBuilder()
+
+TEST_BLOCK_SWALLOWER = TestBlockSwallower()
+
+TEST_PROPERTY = property(lambda x: 5)
+
+class TestDocSegmentHeader:
+    is_segment_header = True
+    weight = 0
+    def __init__(self, test_block=None):
+        self.test_block = test_block
+
+class TestDocSegmentBuilder:
+    def build_from_blocks(self, contents):
+        return TestDocSegmentHeader(contents)
+"#;
+
+#[derive(Debug, PartialEq, Eq)]
+pub struct TestDocSegment {
+    header: Option<(i64, Option<TestBlock>)>,
+    contents: TestBlock,
+    subsegments: Vec<TestDocSegment>,
+}
 #[derive(Debug, PartialEq, Eq)]
 pub enum TestBlock {
     BlockScope(Vec<TestBlock>),
     Paragraph(Vec<Vec<TestInline>>),
 
     TestOwnedBlock(Vec<TestBlock>),
 }
@@ -227,30 +360,70 @@
     RawText(String),
 
     /// Test-only - a Python object built from an inline scope with test_inline: List[Inline] = the contents of that scope
     TestOwnedInline(Vec<TestInline>),
     /// Test-only - a Python object built from raw text with test_raw_str: str = the raw text
     TestOwnedRaw(String),
 }
-pub fn test_doc(contents: Vec<TestBlock>) -> TestBlock {
-    TestBlock::BlockScope(contents)
+pub fn test_doc(contents: Vec<TestBlock>) -> TestDocSegment {
+    TestDocSegment {
+        header: None,
+        contents: TestBlock::BlockScope(contents),
+        subsegments: vec![],
+    }
 }
 pub fn test_sentence(s: impl Into<String>) -> Vec<TestInline> {
     vec![TestInline::UnescapedText(s.into())]
 }
 pub fn test_text(s: impl Into<String>) -> TestInline {
     TestInline::UnescapedText(s.into())
 }
 pub fn test_raw_text(s: impl Into<String>) -> TestInline {
     TestInline::RawText(s.into())
 }
 
 pub trait PyToTest<T> {
     fn as_test(&self, py: Python) -> T;
 }
+impl PyToTest<TestDocSegment> for PyAny {
+    fn as_test(&self, py: Python) -> TestDocSegment {
+        if let Ok(doc_segment) = self.extract::<DocSegment>() {
+            TestDocSegment {
+                header: doc_segment.header.map(|header| {
+                    let weight = DocSegmentHeader::get_weight(py, header.as_ref(py))
+                        .expect("Couldn't get_weight of header");
+                    let contents = match header.as_ref(py).getattr("test_block") {
+                        Ok(test_block) => {
+                            if test_block.is_none() {
+                                None
+                            } else {
+                                Some(test_block.as_test(py))
+                            }
+                        }
+                        Err(_) => None,
+                    };
+                    (weight, contents)
+                }),
+                contents: doc_segment.contents.as_ref(py).as_test(py),
+                subsegments: doc_segment
+                    .subsegments
+                    .list(py)
+                    .iter()
+                    .map(|subseg| subseg.as_test(py))
+                    .collect(),
+            }
+        } else {
+            let repr = match self.repr() {
+                Ok(py_str) => py_str.to_string(),
+                Err(_) => "<couldn't call __repr__>".to_owned(),
+            };
+            panic!("Expected DocSegment, got {repr}")
+        }
+    }
+}
 impl PyToTest<TestBlock> for PyAny {
     fn as_test(&self, py: Python) -> TestBlock {
         if let Ok(block) = self.extract::<BlockScope>() {
             TestBlock::BlockScope(
                 block
                     .0
                     .list(py)
@@ -273,29 +446,37 @@
                     .0
                     .list(py)
                     .iter()
                     .map(|obj| PyToTest::as_test(obj, py))
                     .collect(),
             )
         } else {
-            panic!("Python BlockNode-like is neither BlockScope or Paragraph")
+            let repr = match self.repr() {
+                Ok(py_str) => py_str.to_string(),
+                Err(_) => "<couldn't call __repr__>".to_owned(),
+            };
+            panic!("Expected BlockNode-like, got {repr}")
         }
     }
 }
 impl PyToTest<Vec<TestInline>> for PyAny {
     fn as_test(&self, py: Python) -> Vec<TestInline> {
         if let Ok(sentence) = self.extract::<Sentence>() {
             sentence
                 .0
                 .list(py)
                 .iter()
                 .map(|obj| PyToTest::as_test(obj, py))
                 .collect()
         } else {
-            panic!("Python Sentence-like is not Sentence")
+            let repr = match self.repr() {
+                Ok(py_str) => py_str.to_string(),
+                Err(_) => "<couldn't call __repr__>".to_owned(),
+            };
+            panic!("Expected Sentence, got {repr}")
         }
     }
 }
 impl PyToTest<TestInline> for PyAny {
     fn as_test(&self, py: Python) -> TestInline {
         if let Ok(inl) = self.extract::<InlineScope>() {
             TestInline::InlineScope(
@@ -318,134 +499,67 @@
                     .iter()
                     .map(|obj| PyToTest::as_test(obj, py))
                     .collect(),
             )
         } else if let Ok(text) = dbg!(self.getattr("test_raw_str")) {
             TestInline::TestOwnedRaw(text.to_string())
         } else {
-            TestInline::UnescapedText(
-                self.str()
-                    .expect("Failed to stringify output Python object")
-                    .to_string(),
-            )
+            let repr = match self.repr() {
+                Ok(py_str) => py_str.to_string(),
+                Err(_) => "<couldn't call __repr__>".to_owned(),
+            };
+            panic!("Expected Inline, got {repr}")
         }
     }
 }
 
 /// Generate a set of local Python variables used in each test case
 ///
 /// Provides `TEST_BLOCK_BUILDER`, `TEST_INLINE_BUILDER`, `TEST_RAW_BUILDER` objects
 /// that can own block, inline, and raw scopes respectively.
 pub fn generate_globals<'interp>(py: Python<'interp>) -> Option<&'interp PyDict> {
     let globals = PyDict::new(py);
 
-    let result = py.run(
-        r#"
-# The Rust module name is _native, which is included under turnip_text, so Python IDEs don't try to import directly from it.
-# This means we use _native instead of turnip_text as the module name here.
-from _native import InlineScope, UnescapedText, BlockScope
-
-class FauxBlock:
-    is_block = True
-    def __init__(self, contents):
-        self.test_block = contents
-
-class FauxInline:
-    is_inline = True
-    def __init__(self, contents):
-        self.test_inline = contents
-
-class FauxInlineRaw:
-    is_inline = True
-    def __init__(self, raw_str):
-        self.test_raw_str = str(raw_str)
-
-class TestBuilder:
-    def build_from_blocks(self, contents):
-        return FauxBlock(contents)
-    def build_from_inlines(self, contents):
-        return FauxInline(contents)
-
-class TestRawInlineBuilder:
-    def build_from_raw(self, raw_str):
-        return FauxInlineRaw(raw_str)
-
-TEST_BLOCK = FauxBlock(BlockScope([]))
-
-class TestRawBlockBuilder:
-    def build_from_raw(self, raw_str):
-        return TEST_BLOCK
-
-class TestBlockSwallower():
-    def build_from_blocks(self, contents):
-        return None
-
-TEST_BLOCK_BUILDER = TestBuilder()
-TEST_INLINE_BUILDER = TestBuilder()
-TEST_RAW_INLINE_BUILDER = TestRawInlineBuilder()
-TEST_RAW_BLOCK_BUILDER = TestRawBlockBuilder()
-
-TEST_BLOCK_SWALLOWER = TestBlockSwallower()
-
-TEST_PROPERTY = property(lambda x: 5)
-
-"#,
-        Some(globals),
-        Some(globals),
-    );
+    let result = py.run(GLOBALS_CODE, Some(globals), Some(globals));
 
     match result {
         Err(pyerr) => {
             pyerr.print(py);
             return None;
         }
         Ok(_) => {}
     };
 
     Some(globals)
 }
 
 /// Run the lexer and parser on a given piece of text, convert the parsed result to our test versions, and compare with the expected result.
-fn expect_parse<'a>(data: &str, expected_parse: Result<TestBlock, TestInterpError>) {
-    println!("{:?}", data);
 
-    // First step: lex
-    let l = TextStream::new(data);
-    let units: Vec<Unit> = l
-        .iter(&[Box::new(Unit::parse_special), Box::new(Unit::parse_other)])
-        .scan((), |_, x| x.ok())
-        .collect();
-    let stoks = units_to_tokens(units);
-
-    expect_parse_tokens(data, stoks, expected_parse)
-}
-
-pub fn expect_parse_tokens(
-    data: &str,
-    stoks: Vec<TTToken>,
-    expected_parse: Result<TestBlock, TestInterpError>,
-) {
+fn expect_parse_err<T: Into<TestTurnipError>>(data: &str, expected_err: T) {
+    expect_parse(data, Err(expected_err.into()))
+}
+
+pub fn expect_parse(data: &str, expected_parse: Result<TestDocSegment, TestTurnipError>) {
     // Make sure Python has been set up
     INIT_PYTHON.call_once(prepare_freethreaded_turniptext_python);
 
     // Second step: parse
     // Need to do this safely so that we don't panic inside Python::with_gil.
     // I'm not 100% sure but I'm afraid it will poison the GIL and break subsequent tests.
-    let root: Result<Result<TestBlock, InterpError>, _> = {
+    let root: Result<TurnipTextResult<TestDocSegment>, _> = {
         // Catch all non-abort panics while running the interpreter
         // and handling the output
         panic::catch_unwind(|| {
             Python::with_gil(|py| {
-                let globals = generate_globals(py).expect("Couldn't generate globals dict");
-                let root = interp_data(py, globals, data, stoks.into_iter());
-                root.map(|bs| {
-                    let bs_obj = bs.to_object(py);
-                    let bs: &PyAny = bs_obj.as_ref(py);
-                    (bs as &dyn PyToTest<TestBlock>).as_test(py)
-                })
+                let py_env = generate_globals(py).expect("Couldn't generate globals dict");
+                let parser = TurnipTextParser::new(py, "<test>".into(), data.into())?;
+                let root = parser.parse(py, py_env)?;
+                let doc_obj = root.to_object(py);
+                let doc: &PyAny = doc_obj.as_ref(py);
+                Ok(doc.as_test(py))
             })
         })
         // Unlock mutex
     };
     // If any of the python-related code tried to panic, re-panic here now the mutex is unlocked
     match root {
         Ok(root) => {
@@ -647,26 +761,23 @@
             )]),
         ])])),
     )
 }
 
 #[test]
 pub fn test_owned_block_scope_with_non_block_builder() {
-    expect_parse(
+    expect_parse_err(
         r#"[None]{
 It was the best of the times, it was the blurst of times
 }
 "#,
-        Err(TestInterpError::PythonErr {
+        TestInterpError::PythonErr {
             pyerr: Regex::new(r"TypeError : Expected object fitting typeclass BlockScopeBuilder, didn't get it. Got None").unwrap(),
-            code_span: TestParserSpan {
-                start: (1, 1),
-                end: (2, 1),
-            },
-        }),
+            code_span: TestParserSpan("[None]{\n"),
+        },
     )
 }
 
 #[test]
 pub fn test_owned_inline_scope() {
     expect_parse(
         r"[TEST_INLINE_BUILDER]{special text}",
@@ -674,25 +785,22 @@
             TestInline::TestOwnedInline(vec![test_text("special text")]),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_owned_inline_scope_with_non_inline_builder() {
-    expect_parse(
+    expect_parse_err(
         r"[None]{special text}",
-        Err(TestInterpError::PythonErr {
+        TestInterpError::PythonErr {
             pyerr:
                 Regex::new("TypeError : Expected object fitting typeclass InlineScopeBuilder, didn't get it. Got None"
                     ).unwrap(),
-            code_span: TestParserSpan {
-                start: (1, 1),
-                end: (1, 8),
-            },
-        }),
+            code_span: TestParserSpan("[None]{"),
+        },
     )
 }
 
 #[test]
 pub fn test_owned_inline_raw_scope_with_newline() {
     expect_parse(
         r#"[TEST_RAW_INLINE_BUILDER]#{
@@ -707,26 +815,23 @@
             ),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_owned_inline_raw_scope_with_non_raw_builder() {
-    expect_parse(
+    expect_parse_err(
         r#"[None]#{
 import os
 }#"#,
-        Err(TestInterpError::PythonErr {
+        TestInterpError::PythonErr {
             pyerr: Regex::new("TypeError : Expected object fitting typeclass RawScopeBuilder, didn't get it. Got None"
         ).unwrap(),
-            code_span: TestParserSpan {
-                start: (1, 1),
-                end: (1, 9),
-            },
-        }),
+            code_span: TestParserSpan("[None]#{"),
+        },
     )
 }
 
 #[test]
 pub fn test_inline_raw_escaped_scope() {
     expect_parse(
         r#"Outside the scope \#\{not inside a scope\}"#,
@@ -806,78 +911,60 @@
         Ok(test_doc(vec![TestBlock::Paragraph(vec![test_sentence(
             "2",
         )])])),
     )
 }
 #[test]
 pub fn test_code_close_in_text() {
-    expect_parse(
+    expect_parse_err(
         "not code ] but closed code",
-        Err(TestInterpError::CodeCloseOutsideCode(TestParserSpan {
-            start: (1, 10),
-            end: (1, 11),
-        })),
+        TestInterpError::CodeCloseOutsideCode(TestParserSpan("]")),
     )
 }
 #[test]
 pub fn test_scope_close_outside_scope() {
-    expect_parse(
+    expect_parse_err(
         "not in a scope } but closed scope",
-        Err(TestInterpError::ScopeCloseOutsideScope(TestParserSpan {
-            start: (1, 16),
-            end: (1, 17),
-        })),
+        TestInterpError::ScopeCloseOutsideScope(TestParserSpan("}")),
     )
 }
 #[test]
 pub fn test_mismatching_raw_scope_close() {
-    expect_parse(
+    expect_parse_err(
         "##{ text in a scope with a }#",
-        Err(TestInterpError::EndedInsideRawScope {
-            raw_scope_start: TestParserSpan {
-                start: (1, 1),
-                end: (1, 4),
-            },
-        }),
+        TestInterpError::EndedInsideRawScope {
+            raw_scope_start: TestParserSpan("##{"),
+        },
     )
 }
 #[test]
 pub fn test_ended_inside_code() {
-    expect_parse(
+    expect_parse_err(
         "text [code",
-        Err(TestInterpError::EndedInsideCode {
-            code_start: TestParserSpan {
-                start: (1, 6),
-                end: (1, 7),
-            },
-        }),
+        TestInterpError::EndedInsideCode {
+            code_start: TestParserSpan("["),
+        },
     )
 }
 #[test]
 pub fn test_ended_inside_raw_scope() {
-    expect_parse(
+    expect_parse_err(
         "text #{raw",
-        Err(TestInterpError::EndedInsideRawScope {
-            raw_scope_start: TestParserSpan {
-                start: (1, 6),
-                end: (1, 8),
-            },
-        }),
+        TestInterpError::EndedInsideRawScope {
+            raw_scope_start: TestParserSpan("#{"),
+        },
     )
 }
 #[test]
 pub fn test_ended_inside_scope() {
-    expect_parse(
+    expect_parse_err(
         "text {scope",
-        Err(TestInterpError::SentenceBreakInInlineScope {
-            scope_start: TestParserSpan {
-                start: (1, 6),
-                end: (1, 7),
-            },
-        }),
+        TestInterpError::SentenceBreakInInlineScope {
+            scope_start: TestParserSpan("{"),
+        },
     )
 }
 
 #[test]
 pub fn test_block_scope_vs_inline_scope() {
     expect_parse(
         r#"{
@@ -957,23 +1044,20 @@
         "[TEST_BLOCK]",
         Ok(test_doc(vec![TestBlock::TestOwnedBlock(vec![])])),
     )
 }
 
 #[test]
 pub fn test_cant_emit_block_from_code_inside_paragraph() {
-    expect_parse(
+    expect_parse_err(
         "Lorem ipsum!
 I'm in a [TEST_BLOCK]",
-        Err(TestInterpError::BlockCodeMidPara {
-            code_span: TestParserSpan {
-                start: (2, 10),
-                end: (2, 22),
-            },
-        }),
+        TestInterpError::BlockCodeMidPara {
+            code_span: TestParserSpan("[TEST_BLOCK]"),
+        },
     )
 }
 
 #[test]
 pub fn test_raw_scope_emitting_block_from_block_level() {
     expect_parse(
         "[TEST_RAW_BLOCK_BUILDER]#{some raw stuff that goes in a block!}#",
@@ -989,17 +1073,17 @@
             TestInline::TestOwnedRaw("some raw stuff that goes in a block!".into()),
         ]])])),
     )
 }
 
 #[test]
 pub fn test_raw_scope_cant_emit_block_inside_paragraph() {
-    expect_parse(
+    expect_parse_err(
         "Inside a paragraph, you can't [TEST_RAW_BLOCK_BUILDER]#{some raw stuff that goes in a block!}#",
-        Err(TestInterpError::BlockCodeFromRawScopeMidPara { code_span: TestParserSpan { start: (1, 31), end: (1, 57) } })
+        TestInterpError::BlockCodeFromRawScopeMidPara { code_span: TestParserSpan("[TEST_RAW_BLOCK_BUILDER]#{") }
     )
 }
 
 #[test]
 pub fn test_raw_scope_emitting_inline_inside_paragraph() {
     expect_parse(
         "Inside a paragraph, you can [TEST_RAW_INLINE_BUILDER]#{insert an inline raw!}#",
@@ -1046,85 +1130,70 @@
 #[test]
 pub fn test_emit_none() {
     expect_parse("[None]", Ok(test_doc(vec![])))
 }
 
 #[test]
 pub fn test_cant_eval_none_for_block_builder() {
-    expect_parse(
+    expect_parse_err(
         "[None]{
     That doesn't make any sense! The owner can't be None
 }",
-        Err(TestInterpError::PythonErr {
+        TestInterpError::PythonErr {
             pyerr: Regex::new("TypeError : Expected object fitting typeclass BlockScopeBuilder, didn't get it. Got None").unwrap(),
-            code_span: TestParserSpan {
-                start: (1, 1),
-                end: (2, 1),
-            },
-        }),
+            code_span: TestParserSpan("[None]{\n"),
+        },
     )
 }
 
 #[test]
 pub fn test_cant_assign_for_block_builder() {
-    expect_parse(
+    expect_parse_err(
         "[x = 5]{
     That doesn't make any sense! The owner can't be an abstract concept of x being something
 }",
-        Err(TestInterpError::PythonErr {
+        TestInterpError::PythonErr {
             pyerr: Regex::new("TypeError : Expected object fitting typeclass BlockScopeBuilder, didn't get it. Got None").unwrap(),
-            code_span: TestParserSpan {
-                start: (1, 1),
-                end: (2, 1),
-            },
-        }),
+            code_span: TestParserSpan("[x = 5]{\n"),
+        },
     )
 }
 
 #[test]
 pub fn test_cant_assign_for_raw_builder() {
-    expect_parse(
+    expect_parse_err(
         "[x = 5]#{That doesn't make any sense! The owner can't be an abstract concept of x being something}#",
-        Err(TestInterpError::PythonErr {
+        TestInterpError::PythonErr {
             pyerr: Regex::new("TypeError : Expected object fitting typeclass RawScopeBuilder, didn't get it. Got None").unwrap(),
-            code_span: TestParserSpan {
-                start: (1, 1),
-                end: (1, 10),
-            },
-        }),
+            code_span: TestParserSpan("[x = 5]#{"),
+        },
     )
 }
 
 #[test]
 pub fn test_cant_assign_for_inline_builder() {
-    expect_parse(
+    expect_parse_err(
         "[x = 5]{That doesn't make any sense! The owner can't be an abstract concept of x being something}",
-        Err(TestInterpError::PythonErr {
+        TestInterpError::PythonErr {
             pyerr: Regex::new("TypeError : Expected object fitting typeclass InlineScopeBuilder, didn't get it. Got None").unwrap(),
-            code_span: TestParserSpan {
-                start: (1, 1),
-                end: (1, 9),
-            },
-        }),
+            code_span: TestParserSpan ("[x = 5]{"),
+        },
     )
 }
 
 #[test]
 pub fn test_syntax_errs_passed_thru() {
     // The assignment support depends on trying to eval() the expression, that failing with a SyntaxError, and then trying to exec() it.
     // Make sure that something invalid as both still returns a SyntaxError
-    expect_parse(
+    expect_parse_err(
         "[1invalid]",
-        Err(TestInterpError::PythonErr {
+        TestInterpError::PythonErr {
             pyerr: Regex::new("^SyntaxError : invalid syntax").unwrap(),
-            code_span: TestParserSpan {
-                start: (1, 1),
-                end: (1, 11),
-            },
-        }),
+            code_span: TestParserSpan("[1invalid]"),
+        },
     )
 }
 
 #[test]
 pub fn test_block_scope_builder_return_none() {
     expect_parse(
         "[TEST_BLOCK_SWALLOWER]{
@@ -1148,7 +1217,51 @@
     expect_parse(
         "[TEST_PROPERTY]",
         Ok(test_doc(vec![TestBlock::Paragraph(vec![vec![test_text(
             "5",
         )]])])),
     )
 }
+
+#[test]
+pub fn test_no_emit_doc_segment_header_in_block_scope() {
+    expect_parse_err(
+        "{
+[TestDocSegmentHeader()]
+}",
+        TestInterpError::DocSegmentHeaderMidScope {
+            code_span: TestParserSpan("[TestDocSegmentHeader()]"),
+            block_close_span: None,
+            enclosing_scope_start: TestParserSpan("{\n"),
+        },
+    )
+}
+
+#[test]
+pub fn test_no_build_doc_segment_header_in_block_scope() {
+    expect_parse_err(
+        "{
+[TestDocSegmentBuilder()]{
+    Sometimes docsegmentheaders can be built, too!
+    But if they're in a block scope it shouldn't be allowed :(
+}
+}",
+        TestInterpError::DocSegmentHeaderMidScope {
+            code_span: TestParserSpan("[TestDocSegmentBuilder()]{\n"),
+            block_close_span: Some(TestParserSpan("}")),
+            enclosing_scope_start: TestParserSpan("{\n"),
+        },
+    )
+}
+
+#[test]
+pub fn test_no_emit_doc_segment_header_in_para() {
+    expect_parse_err(
+        "And as I was saying [TestDocSegmentHeader()]",
+        TestInterpError::DocSegmentHeaderMidPara {
+            code_span: TestParserSpan("[TestDocSegmentHeader()]"),
+        },
+    )
+}
+
+// TODO MORE TESTS FOR DOC STURCURE. OH FUCK I NEED TO CHANGE THE TEST HARNESS
+// TODO tests for inserted files. Are they exclusively on block boundaries?
```

### Comparing `turnip_text-0.0.4/src/util.rs` & `turnip_text-0.0.5/src/util.rs`

 * *Files 26% similar despite different names*

```diff
@@ -24,24 +24,52 @@
         }
     }
 }
 
 /// Helper struct representing a span of characters between `start` (inclusive) and `end` (exclusive) in a file
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
 pub struct ParseSpan {
-    pub start: ParsePosn,
-    pub end: ParsePosn,
+    file_idx: usize,
+    start: ParsePosn,
+    end: ParsePosn,
 }
 impl ParseSpan {
-    pub fn from_lex(start: LexPosn, end: LexPosn) -> Self {
+    pub fn single_char(file_idx: usize, start: LexPosn, c: char) -> Self {
         Self {
+            file_idx,
+            start: start.clone().into(),
+            end: start.advance_cols(c.len_utf8(), 1).into(),
+        }
+    }
+    pub fn from_lex(file_idx: usize, start: LexPosn, end: LexPosn) -> Self {
+        Self {
+            file_idx,
             start: start.into(),
             end: end.into(),
         }
     }
-    pub fn new(start: ParsePosn, end: ParsePosn) -> Self {
-        Self { start, end }
+    pub fn new(file_idx: usize, start: ParsePosn, end: ParsePosn) -> Self {
+        Self {
+            file_idx,
+            start,
+            end,
+        }
     }
     pub fn byte_range(&self) -> Range<usize> {
         self.start.byte_ofs..self.end.byte_ofs
     }
+    pub fn combine(&self, other: &ParseSpan) -> ParseSpan {
+        assert_eq!(self.file_idx, other.file_idx);
+        assert!(self.start.byte_ofs < other.end.byte_ofs);
+        ParseSpan {
+            file_idx: self.file_idx,
+            start: self.start,
+            end: other.end,
+        }
+    }
+    pub fn annotate_snippets_range(&self) -> (usize, usize) {
+        (self.start.char_ofs, self.end.char_ofs)
+    }
+    pub fn file_idx(&self) -> usize {
+        self.file_idx
+    }
 }
```

### Comparing `turnip_text-0.0.4/turnip_text.pyi` & `turnip_text-0.0.5/python/turnip_text/__init__.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,57 @@
+import abc
 from typing import (
     Any,
     Dict,
+    Iterable,
     Iterator,
     List,
     Optional,
     Protocol,
+    Sequence,
+    Tuple,
     Union,
     runtime_checkable,
 )
 
 @runtime_checkable
 class Inline(Protocol):
     is_inline: bool = True
 
-
 @runtime_checkable
 class Block(Protocol):
     is_block: bool = True
 
+@runtime_checkable
+class DocSegmentHeader(Protocol):
+    is_segment_header: bool = True
+    weight: int = 0
+
+class BlockScopeBuilder(abc.ABC):
+    @abc.abstractmethod
+    def build_from_blocks(
+        self, bs: BlockScope
+    ) -> Optional[Block | DocSegmentHeader]: ...
+    def __matmul__(
+        self, maybe_b: "CoercibleToBlockScope"
+    ) -> Optional[Block | DocSegmentHeader]:
+        bs = coerce_to_block_scope(maybe_b)
+        return self.build_from_blocks(bs)
+
+class InlineScopeBuilder(abc.ABC):
+    @abc.abstractmethod
+    def build_from_inlines(self, inls: InlineScope) -> Inline: ...
+    def __matmul__(self, maybe_inls: "CoercibleToInlineScope") -> Inline:
+        inls = coerce_to_inline_scope(maybe_inls)
+        return self.build_from_inlines(inls)
+
+@runtime_checkable
+class RawScopeBuilder(Protocol):
+    def build_from_raw(self, raw: str) -> Union[Inline, Block]: ...
+
 # The types that can be coerced into an Inline, in the order they are checked and attempted.
 # List[Inline] is coerced by wrapping it in an InlineScope
 CoercibleToInline = Union[Inline, List[Inline], str, int, float]
 
 # The types that can be coerced into an InlineScope, in the order they are checked and attempted.
 # 1. InlineScopes are passed through.
 # 2. Coercion to Inline is attempted, and must succeed.
@@ -34,16 +64,20 @@
 CoercibleToBlock = Union[
     List[Block], Block, Paragraph, Sentence, CoercibleToInlineScope
 ]
 
 # The types that can be coerced into a BlockScope, in the order they are checked and attempted
 CoercibleToBlockScope = Union[BlockScope, CoercibleToBlock]
 
-def parse_file_native(path: str, locals: Dict[str, Any]) -> BlockScope: ...
-def parse_str_native(data: str, locals: Dict[str, Any]) -> BlockScope: ...
+def join_inlines(inlines: Iterable[Inline], joiner: Inline) -> InlineScope:
+    """Equivalent of string.join, but for joining any set of Inlines with a joiner Inline"""
+    ...
+
+# Parsers return a BlockScope of the top-level content, then a DocSegment tree
+def parse_file_native(file: InsertedFile, locals: Dict[str, Any]) -> DocSegment: ...
 def coerce_to_inline(obj: CoercibleToInline) -> Inline: ...
 def coerce_to_inline_scope(obj: CoercibleToInlineScope) -> InlineScope: ...
 def coerce_to_block(obj: CoercibleToBlock) -> Block: ...
 def coerce_to_block_scope(obj: CoercibleToBlockScope) -> BlockScope: ...
 
 class UnescapedText(Inline):
     def __init__(self, text: str) -> None: ...
@@ -84,7 +118,34 @@
 class InlineScope(Inline):
     def __init__(self, list: Optional[List[Inline]] = None): ...
     def __len__(self) -> int: ...
     # Iterate over the inline items in the InlineScope
     def __iter__(self) -> Iterator[Inline]: ...
     # Push an inline item into the InlineScope
     def push_inline(self, b: Inline) -> None: ...
+
+class DocSegment:
+    def __init__(
+        self,
+        header: DocSegmentHeader,
+        contents: BlockScope,
+        subsegments: List[DocSegment],
+    ): ...
+    @property
+    def header(self) -> DocSegmentHeader: ...
+    @property
+    def contents(self) -> BlockScope: ...
+    @property
+    def subsegments(self) -> Iterator["DocSegment"]: ...
+    # TODO make something that does correct weight checking??
+    def push_subsegment(self, d: DocSegment) -> None: ...
+
+class InsertedFile:
+    """
+    Emit an instance of this class from eval-brackets in a Block context to start parsing its contents instead.
+    """
+
+    def __init__(self, name: str, contents: str) -> None: ...
+    @staticmethod
+    def from_path(path: str) -> InsertedFile: ...
+    @staticmethod
+    def from_string(contents: str) -> InsertedFile: ...
```

### Comparing `turnip_text-0.0.4/Cargo.lock` & `turnip_text-0.0.5/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,15 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "turnip_text"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
  "annotate-snippets",
  "anyhow",
  "argh",
  "lexer-rs",
  "pyo3",
  "regex",
```

### Comparing `turnip_text-0.0.4/PKG-INFO` & `turnip_text-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: turnip_text
-Version: 0.0.4
+Version: 0.0.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Dist: mypy ; extra == 'typing'
 Requires-Dist: black ; extra == 'fmt'
 Requires-Dist: pytest ; extra == 'test'
```

