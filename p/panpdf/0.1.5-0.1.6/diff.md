# Comparing `tmp/panpdf-0.1.5.tar.gz` & `tmp/panpdf-0.1.6.tar.gz`

## Comparing `panpdf-0.1.5.tar` & `panpdf-0.1.6.tar`

### file list

```diff
@@ -1,69 +1,67 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.1.5/.gitattributes
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 panpdf-0.1.5/mkdocs.yml
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.1.5/ruff_defaults.toml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 panpdf-0.1.5/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 panpdf-0.1.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 panpdf-0.1.5/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 panpdf-0.1.5/.devcontainer/postCreateCommand.sh
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 panpdf-0.1.5/.devcontainer/vscode_extensions_install.sh
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/defaults.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/include-after-body.tex
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/include-before-body.tex
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/include-in-header.tex
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/images/figure.pdf
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/images/figure.tex
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/images/header.pdf
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/images/header.tex
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/src/1.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 panpdf-0.1.5/examples/src/2.md
--rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.1.5/notebooks/pdf.ipynb
--rw-r--r--   0        0        0    60992 2020-02-02 00:00:00.000000 panpdf-0.1.5/notebooks/pgf.ipynb
--rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.1.5/notebooks/png.ipynb
--rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.1.5/notebooks/svg.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/formatters.py
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/main.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/stores.py
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/filters/__init__.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/filters/attribute.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/filters/crossref.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/filters/filter.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/filters/jupyter.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/filters/layout.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/filters/verbatim.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 panpdf-0.1.5/src/panpdf/filters/zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/test_converters.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/test_formatters.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/test_main.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/test_stores.py
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/test_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/conftest.py
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/test_attribute.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/test_crossref.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/test_filter.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/test_jupyter.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/test_layout.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/test_verbatim.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/filters/test_zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/test_nbformat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_cite.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_code.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_figure.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_math.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_metadata.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_raw.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_section.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_table.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.1.5/tests/libraries/panflute/test_tex.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 panpdf-0.1.5/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.1.5/README.md
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 panpdf-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.1.6/.gitattributes
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 panpdf-0.1.6/mkdocs.yml
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.1.6/ruff_defaults.toml
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 panpdf-0.1.6/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 panpdf-0.1.6/.devcontainer/postCreate.sh
+-rw-r--r--   0        0        0   118258 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/a.pdf
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/defaults.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/include-after-body.tex
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/include-before-body.tex
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/include-in-header.tex
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/images/figure.pdf
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/images/figure.tex
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/images/header.pdf
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/images/header.tex
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/src/1.md
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/src/2.md
+-rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.1.6/notebooks/pdf.ipynb
+-rw-r--r--   0        0        0    60992 2020-02-02 00:00:00.000000 panpdf-0.1.6/notebooks/pgf.ipynb
+-rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.1.6/notebooks/png.ipynb
+-rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.1.6/notebooks/svg.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/__init__.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/formatters.py
+-rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/main.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/stores.py
+-rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/__init__.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/attribute.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/crossref.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/filter.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/jupyter.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/layout.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/verbatim.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_converters.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_formatters.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_main.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_stores.py
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/conftest.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_attribute.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_crossref.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_filter.py
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_jupyter.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_layout.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_verbatim.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/test_nbformat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_cite.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_code.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_figure.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_math.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_metadata.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_raw.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_section.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_table.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_tex.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 panpdf-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.1.6/README.md
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 panpdf-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.1.6/PKG-INFO
```

### Comparing `panpdf-0.1.5/mkdocs.yml` & `panpdf-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/ruff_defaults.toml` & `panpdf-0.1.6/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/.devcontainer/devcontainer.json` & `panpdf-0.1.6/.devcontainer/devcontainer.json`

 * *Files 8% similar despite different names*

```diff
@@ -32,12 +32,12 @@
         "github.vscode-github-actions",
         "ms-python.python",
         "ms-python.vscode-pylance",
         "ms-toolsai.jupyter"
       ]
     }
   },
-  "postCreateCommand": ".devcontainer/postCreateCommand.sh"
+  "postCreateCommand": ".devcontainer/postCreate.sh"
 
   // Use 'forwardPorts' to make a list of ports inside the container available locally.
   // "forwardPorts": [],
 }
```

### Comparing `panpdf-0.1.5/examples/defaults.yaml` & `panpdf-0.1.6/examples/defaults.yaml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/examples/include-in-header.tex` & `panpdf-0.1.6/examples/include-in-header.tex`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/examples/images/figure.pdf` & `panpdf-0.1.6/examples/images/figure.pdf`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/examples/images/header.pdf` & `panpdf-0.1.6/examples/images/header.pdf`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/examples/src/1.md` & `panpdf-0.1.6/examples/src/1.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/notebooks/pdf.ipynb` & `panpdf-0.1.6/notebooks/pdf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/notebooks/pgf.ipynb` & `panpdf-0.1.6/notebooks/pgf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/notebooks/png.ipynb` & `panpdf-0.1.6/notebooks/png.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/notebooks/svg.ipynb` & `panpdf-0.1.6/notebooks/svg.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/formatters.py` & `panpdf-0.1.6/src/panpdf/formatters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/main.py` & `panpdf-0.1.6/src/panpdf/main.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/stores.py` & `panpdf-0.1.6/src/panpdf/stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/tools.py` & `panpdf-0.1.6/src/panpdf/tools.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/filters/attribute.py` & `panpdf-0.1.6/src/panpdf/filters/attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/filters/crossref.py` & `panpdf-0.1.6/src/panpdf/filters/crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/filters/filter.py` & `panpdf-0.1.6/src/panpdf/filters/filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/filters/jupyter.py` & `panpdf-0.1.6/src/panpdf/filters/jupyter.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 class Jupyter(Filter):
     types: ClassVar[type[Image]] = Image
     defaults: Path | None = None
     standalone: bool = False
     pandoc_path: Path | None = None
     store: Store = field(default_factory=Store)
 
-    def set_notebooks_dir(self, notebooks_dir: list[Path]):
-        self.store.set_notebooks_dir(notebooks_dir)
+    # def set_notebooks_dir(self, notebooks_dir: list[Path]):
+    #     self.store.set_notebooks_dir(notebooks_dir)
 
     def action(self, image: Image, doc: Doc) -> Image:
         url = image.url
         identifier = image.identifier
 
         if not identifier or (url and not url.endswith(".ipynb")):
             return image
```

### Comparing `panpdf-0.1.5/src/panpdf/filters/layout.py` & `panpdf-0.1.6/src/panpdf/filters/layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/src/panpdf/filters/zotero.py` & `panpdf-0.1.6/src/panpdf/filters/zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/conftest.py` & `panpdf-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/test_converters.py` & `panpdf-0.1.6/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/test_formatters.py` & `panpdf-0.1.6/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/test_main.py` & `panpdf-0.1.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/test_stores.py` & `panpdf-0.1.6/tests/test_stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/test_tools.py` & `panpdf-0.1.6/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/filters/test_attribute.py` & `panpdf-0.1.6/tests/filters/test_attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/filters/test_crossref.py` & `panpdf-0.1.6/tests/filters/test_crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/filters/test_filter.py` & `panpdf-0.1.6/tests/filters/test_filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/filters/test_jupyter.py` & `panpdf-0.1.6/tests/filters/test_jupyter.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import platform
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 import yaml
-from panflute import Doc, Image
+from panflute import Doc, Image, Str
 
 from panpdf.filters.jupyter import Jupyter
 
 if TYPE_CHECKING:
     from panpdf.stores import Store
 
 
@@ -40,14 +40,20 @@
 
     path = Path(url)
     assert path.exists()
     assert path.stat().st_size
     assert text.startswith("JVBER")
 
 
+def test_create_image_file_none():
+    from panpdf.filters.jupyter import create_image_file
+
+    assert create_image_file({}) is None
+
+
 def test_create_defaults_for_standalone(defaults):
     from panpdf.filters.jupyter import create_defaults_for_standalone
 
     path = create_defaults_for_standalone(defaults)
     assert path.exists()
 
     with path.open(encoding="utf8") as f:
@@ -136,7 +142,26 @@
 
         store.delete_data(f"{fmt}.ipynb", f"fig:{fmt}", "application/pdf")
 
         data = store.get_data(f"{fmt}.ipynb", f"fig:{fmt}")
         assert "image/png" in data
         assert "text/plain" in data
         assert "application/pdf" not in data
+
+
+def test_jupyter_action():
+    from panpdf.filters.jupyter import Jupyter
+
+    doc = Doc()
+    jupyter = Jupyter()
+    image = Image(Str("a"), url="a.png")
+    assert jupyter.action(image, doc) is image
+
+
+def test_jupyter_action_error():
+    from panpdf.filters.jupyter import Jupyter
+
+    doc = Doc()
+    jupyter = Jupyter()
+    image = Image(Str("a"), url="a.ipynb", identifier="a")
+    with pytest.raises(ValueError, match=r"\[panpdf\] Unknown"):
+        jupyter.action(image, doc)
```

### Comparing `panpdf-0.1.5/tests/filters/test_layout.py` & `panpdf-0.1.6/tests/filters/test_layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import platform
 from pathlib import Path
 
 import panflute as pf
 import pytest
-from panflute import Doc, Figure, Para, RawInline, Span, Table
+from panflute import Doc, Figure, Image, Para, RawInline, Span, Str, Table
 
 from panpdf.filters.attribute import Attribute
 from panpdf.filters.jupyter import Jupyter
 
 
 def _prepare(text: str):
     return Attribute().run(text).content[0]  # type:ignore
@@ -149,7 +149,14 @@
     layout.run(doc)
 
     assert "__subcaption__" not in doc.metadata
     x = doc.metadata["include-in-header"]
     assert isinstance(x, pf.MetaList)
     f = Path(pf.stringify(x[0]))
     assert f.exists()
+
+
+def test_get_width():
+    from panpdf.filters.layout import get_width
+
+    image = Image(Str("a"), attributes={"width": "50%"})
+    assert get_width(image, "width") == "0.5\\columnwidth"
```

### Comparing `panpdf-0.1.5/tests/filters/test_verbatim.py` & `panpdf-0.1.6/tests/filters/test_verbatim.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 
 def test_create_header():
     from panpdf.filters.verbatim import create_header
 
     path = create_header()
     assert path.exists()
-    path.read_text("utf-8").startswith("\\ifdefined\\Shaded")
+    text = path.read_text("utf-8")
+    assert text.startswith("\\ifdefined\\Shaded")
 
 
 def test_verbatim():
     from panpdf.filters.verbatim import Verbatim
 
     verbatim = Verbatim()
     assert not verbatim.shaded
```

### Comparing `panpdf-0.1.5/tests/filters/test_zotero.py` & `panpdf-0.1.6/tests/filters/test_zotero.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,9 +93,9 @@
     assert "\\url{https://github.com/daizutabi/panpdf}}" in tex
 
 
 def test_zotero_nokey():
     from panpdf.filters.zotero import Zotero
 
     doc = Doc()
-    doc = Zotero().run(doc)
+    Zotero().finalize(doc)
     assert not doc.metadata
```

### Comparing `panpdf-0.1.5/tests/libraries/test_nbformat.py` & `panpdf-0.1.6/tests/libraries/test_nbformat.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_cite.py` & `panpdf-0.1.6/tests/libraries/panflute/test_cite.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_code.py` & `panpdf-0.1.6/tests/libraries/panflute/test_code.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_figure.py` & `panpdf-0.1.6/tests/libraries/panflute/test_figure.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_math.py` & `panpdf-0.1.6/tests/libraries/panflute/test_math.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_metadata.py` & `panpdf-0.1.6/tests/libraries/panflute/test_metadata.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_raw.py` & `panpdf-0.1.6/tests/libraries/panflute/test_raw.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_section.py` & `panpdf-0.1.6/tests/libraries/panflute/test_section.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_table.py` & `panpdf-0.1.6/tests/libraries/panflute/test_table.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/tests/libraries/panflute/test_tex.py` & `panpdf-0.1.6/tests/libraries/panflute/test_tex.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/LICENSE.txt` & `panpdf-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/README.md` & `panpdf-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/pyproject.toml` & `panpdf-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.5/PKG-INFO` & `panpdf-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpdf
-Version: 0.1.5
+Version: 0.1.6
 Summary: PDF documentation generator
 Project-URL: Documentation, https://daizutabi.github.io/panpdf
 Project-URL: Source, https://github.com/daizutabi/panpdf
 Project-URL: Issues, https://github.com/daizutabi/panpdf/issues
 Author-email: daizutabi <daizutabi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

