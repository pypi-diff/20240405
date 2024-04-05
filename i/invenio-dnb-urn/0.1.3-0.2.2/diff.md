# Comparing `tmp/invenio-dnb-urn-0.1.3.tar.gz` & `tmp/invenio-dnb-urn-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-dnb-urn-0.1.3.tar", last modified: Fri Feb 17 13:29:34 2023, max compression
+gzip compressed data, was "invenio-dnb-urn-0.2.2.tar", last modified: Fri Apr  5 15:15:46 2024, max compression
```

## Comparing `invenio-dnb-urn-0.1.3.tar` & `invenio-dnb-urn-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,36 @@
-drwxr-xr-x   0 gressho   (1000) gressho   (1000)        0 2023-02-17 13:29:34.546037 invenio-dnb-urn-0.1.3/
--rw-r--r--   0 gressho   (1000) gressho   (1000)      296 2022-07-29 13:30:54.000000 invenio-dnb-urn-0.1.3/AUTHORS.rst
--rw-r--r--   0 gressho   (1000) gressho   (1000)     1080 2022-05-04 14:57:50.000000 invenio-dnb-urn-0.1.3/LICENSE
--rw-r--r--   0 gressho   (1000) gressho   (1000)     5898 2023-02-17 13:29:34.546037 invenio-dnb-urn-0.1.3/PKG-INFO
--rw-r--r--   0 gressho   (1000) gressho   (1000)     5356 2023-02-17 09:39:19.000000 invenio-dnb-urn-0.1.3/README.md
-drwxr-xr-x   0 gressho   (1000) gressho   (1000)        0 2023-02-17 13:29:34.533037 invenio-dnb-urn-0.1.3/invenio_dnb_urn/
--rw-r--r--   0 gressho   (1000) gressho   (1000)      517 2023-02-17 13:26:38.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/__init__.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)     1190 2022-08-26 10:23:58.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/cli.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)      821 2023-02-01 08:58:00.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/config.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)      450 2023-02-01 08:58:10.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/errors.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)    20011 2023-02-06 12:49:05.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/oai.py
-drwxr-xr-x   0 gressho   (1000) gressho   (1000)        0 2023-02-17 13:29:34.535037 invenio-dnb-urn-0.1.3/invenio_dnb_urn/provider/
--rw-r--r--   0 gressho   (1000) gressho   (1000)      355 2023-02-01 11:29:18.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/provider/__init__.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)     6061 2023-02-01 14:40:47.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/provider/dnburn.py
-drwxr-xr-x   0 gressho   (1000) gressho   (1000)        0 2023-02-17 13:29:34.546037 invenio-dnb-urn-0.1.3/invenio_dnb_urn/serialize/
--rw-r--r--   0 gressho   (1000) gressho   (1000)      337 2023-02-17 09:40:39.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/serialize/__init__.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)     1842 2023-02-01 08:57:12.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/serialize/xmetadiss.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)     1033 2023-02-01 08:58:43.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/utils.py
--rw-r--r--   0 gressho   (1000) gressho   (1000)     1052 2023-02-01 08:59:09.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn/views.py
-drwxr-xr-x   0 gressho   (1000) gressho   (1000)        0 2023-02-17 13:29:34.535037 invenio-dnb-urn-0.1.3/invenio_dnb_urn.egg-info/
--rw-r--r--   0 gressho   (1000) gressho   (1000)     5898 2023-02-17 13:29:34.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn.egg-info/PKG-INFO
--rw-r--r--   0 gressho   (1000) gressho   (1000)      647 2023-02-17 13:29:34.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn.egg-info/SOURCES.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)        1 2023-02-17 13:29:34.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn.egg-info/dependency_links.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)      238 2023-02-17 13:29:34.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn.egg-info/entry_points.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)        1 2022-08-29 14:08:32.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn.egg-info/not-zip-safe
--rw-r--r--   0 gressho   (1000) gressho   (1000)      630 2023-02-17 13:29:34.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn.egg-info/requires.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)       16 2023-02-17 13:29:34.000000 invenio-dnb-urn-0.1.3/invenio_dnb_urn.egg-info/top_level.txt
--rw-r--r--   0 gressho   (1000) gressho   (1000)     2379 2023-02-17 13:29:34.547037 invenio-dnb-urn-0.1.3/setup.cfg
--rw-r--r--   0 gressho   (1000) gressho   (1000)      316 2022-07-29 13:30:32.000000 invenio-dnb-urn-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:15:46.085698 invenio-dnb-urn-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/.editorconfig
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:15:46.077698 invenio-dnb-urn-0.2.2/.tx/
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/.tx/config
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      564 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2432 2024-04-05 15:15:46.085698 invenio-dnb-urn-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:15:46.081698 invenio-dnb-urn-0.2.2/invenio_dnb_urn/
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    22047 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/oai.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:15:46.081698 invenio-dnb-urn-0.2.2/invenio_dnb_urn/provider/
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6116 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/provider/dnburn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:15:46.081698 invenio-dnb-urn-0.2.2/invenio_dnb_urn/serialize/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/serialize/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/serialize/xmetadiss.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:15:46.081698 invenio-dnb-urn-0.2.2/invenio_dnb_urn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2432 2024-04-05 15:15:46.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-05 15:15:46.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 15:15:46.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      175 2024-04-05 15:15:46.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 15:15:46.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      548 2024-04-05 15:15:46.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-05 15:15:46.000000 invenio-dnb-urn-0.2.2/invenio_dnb_urn.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-04-05 15:15:46.085698 invenio-dnb-urn-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 15:15:46.081698 invenio-dnb-urn-0.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      365 2024-04-05 15:15:40.000000 invenio-dnb-urn-0.2.2/tests/test_invenio_dnb_urn.py
```

### Comparing `invenio-dnb-urn-0.1.3/LICENSE` & `invenio-dnb-urn-0.2.2/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 MIT License
 
-Copyright (C) 2022 University of Münster.
+Copyright (C) 2022-2024 University of Münster.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `invenio-dnb-urn-0.1.3/invenio_dnb_urn/config.py` & `invenio-dnb-urn-0.2.2/invenio_dnb_urn/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022, 2023 University of Münster.
+# Copyright (C) 2022-2024 University of Münster.
 #
-# Invenio-Dnb-Urn is free software; you can redistribute it and/or modify
+# invenio-dnb-urn is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Epicur-based data model for Invenio."""
 
 EPICUR_NBN_SCHEME = "urn:nbn:de"
 
 """URN-PIDStore configuration used by the DnbUrnProvider."""
```

### Comparing `invenio-dnb-urn-0.1.3/invenio_dnb_urn/oai.py` & `invenio-dnb-urn-0.2.2/invenio_dnb_urn/oai.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022, 2023 University Münster.
+# Copyright (C) 2022-2024 University of Münster.
 #
-# Invenio-Dnb-Urn is free software; you can redistribute it and/or modify
+# invenio-dnb-urn is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
-""" InvenioRDM additional metadata output format for OAI DataProvider. """
+"""InvenioRDM additional metadata output format for OAI DataProvider."""
 
 from flask import current_app
 from lxml import etree
 
 from .utils import get_vocabulary_props
 
 
@@ -32,363 +32,517 @@
     attribs = {
         f"{{{nsmap['xsi']}}}schemaLocation": (
             "http://www.d-nb.de/standards/xmetadissplus/ "
             "http://www.d-nb.de/standards/xmetadissplus/xmetadissplus.xsd"
         ),
     }
 
-    source = record['_source']
-    metadata = source['metadata']
+    source = record["_source"]
+    metadata = source["metadata"]
     print(record)
     # prepare the structure required by the 'xMetaDissPlus' metadataPrefix
-    xmetadiss = etree.Element("{http://www.d-nb.de/standards/xmetadissplus/}xMetaDiss", nsmap=nsmap, attrib=attribs)
+    xmetadiss = etree.Element(
+        "{http://www.d-nb.de/standards/xmetadissplus/}xMetaDiss",
+        nsmap=nsmap,
+        attrib=attribs,
+    )
     title = etree.SubElement(
-        xmetadiss, "{http://purl.org/dc/elements/1.1/}title",
-        nsmap=nsmap)
+        xmetadiss, "{http://purl.org/dc/elements/1.1/}title", nsmap=nsmap
+    )
     lang = None
-    if 'languages' in metadata:
-        lang = metadata['languages'][0]['id']
+    if "languages" in metadata:
+        lang = metadata["languages"][0]["id"]
         if lang == "deu":
             lang = "ger"
-        title.attrib['lang'] = lang
-        title.attrib['{http://www.w3.org/2001/XMLSchema-instance}type'] = 'ddb:titleISO639-2'
-    title.text = metadata['title']
-    if 'additional_titles' in metadata:
-        for additionaltitle in metadata['additional_titles']:
-            if additionaltitle['type']['id'] == 'translated-title' or additionaltitle['type']['id'] == 'subtitle':
+        title.attrib["lang"] = lang
+        title.attrib["{http://www.w3.org/2001/XMLSchema-instance}type"] = (
+            "ddb:titleISO639-2"
+        )
+    title.text = metadata["title"]
+    if "additional_titles" in metadata:
+        for additionaltitle in metadata["additional_titles"]:
+            if (
+                additionaltitle["type"]["id"] == "translated-title"
+                or additionaltitle["type"]["id"] == "subtitle"
+            ):
                 alternativetitle = etree.SubElement(
-                    xmetadiss, "{http://purl.org/dc/terms/}alternative",
+                    xmetadiss,
+                    "{http://purl.org/dc/terms/}alternative",
                     nsmap=nsmap,
-                    attrib={'{http://www.w3.org/2001/XMLSchema-instance}type': 'ddb:talternativeISO639-2'})
-                if additionaltitle['type']['id'] == 'translated-title':
-                    alternativetitle.attrib['{http://www.d-nb.de/standards/ddb/}type'] = 'translated'
-                if 'lang' in additionaltitle:
-                    additionaltitle_lang = additionaltitle['lang']['id']
+                    attrib={
+                        "{http://www.w3.org/2001/XMLSchema-instance}type": "ddb:talternativeISO639-2"
+                    },
+                )
+                if additionaltitle["type"]["id"] == "translated-title":
+                    alternativetitle.attrib[
+                        "{http://www.d-nb.de/standards/ddb/}type"
+                    ] = "translated"
+                if "lang" in additionaltitle:
+                    additionaltitle_lang = additionaltitle["lang"]["id"]
                     if additionaltitle_lang == "deu":
                         additionaltitle_lang = "ger"
-                    alternativetitle.attrib['lang'] = additionaltitle_lang
-                alternativetitle.text = additionaltitle['title']
-    for mcreator in metadata['creators']:
-        creator = etree.SubElement(xmetadiss, "{http://purl.org/dc/elements/1.1/}creator",
-                                   nsmap=nsmap,
-                                   attrib={'{http://www.w3.org/2001/XMLSchema-instance}type': 'pc:MetaPers'})
-        person = etree.SubElement(creator, "{http://www.d-nb.de/standards/pc/}person", nsmap=nsmap)
-        mperson = mcreator['person_or_org']
-        if 'identifiers' in mperson:
-            for midentifier in mperson['identifiers']:
-                mscheme = midentifier['scheme']
+                    alternativetitle.attrib["lang"] = additionaltitle_lang
+                alternativetitle.text = additionaltitle["title"]
+    for mcreator in metadata["creators"]:
+        creator = etree.SubElement(
+            xmetadiss,
+            "{http://purl.org/dc/elements/1.1/}creator",
+            nsmap=nsmap,
+            attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "pc:MetaPers"},
+        )
+        person = etree.SubElement(
+            creator, "{http://www.d-nb.de/standards/pc/}person", nsmap=nsmap
+        )
+        mperson = mcreator["person_or_org"]
+        if "identifiers" in mperson:
+            for midentifier in mperson["identifiers"]:
+                mscheme = midentifier["scheme"]
                 if mscheme == "orcid":
-                    id = etree.SubElement(person, "{http://www.d-nb.de/standards/ddb/}ORCID")
-                    id.text = midentifier['identifier']
+                    id = etree.SubElement(
+                        person, "{http://www.d-nb.de/standards/ddb/}ORCID"
+                    )
+                    id.text = midentifier["identifier"]
                 elif mscheme == "gnd":
-                    person.attrib['{http://www.d-nb.de/standards/ddb/}GND-Nr'] = midentifier['identifier']
+                    person.attrib["{http://www.d-nb.de/standards/ddb/}GND-Nr"] = (
+                        midentifier["identifier"]
+                    )
                 elif mscheme == "isni":
-                    id = etree.SubElement(person, "{http://www.d-nb.de/standards/ddb/}ISNI")
-                    id.text = midentifier['identifier']
+                    id = etree.SubElement(
+                        person, "{http://www.d-nb.de/standards/ddb/}ISNI"
+                    )
+                    id.text = midentifier["identifier"]
                 elif mscheme == "ror":
-                    id = etree.SubElement(person, "{http://www.d-nb.de/standards/ddb/}OtherId")
-                    id.text = "(ror)" + midentifier['identifier']
-        name = etree.SubElement(person, "{http://www.d-nb.de/standards/pc/}name", nsmap=nsmap)
-        if mperson['type'] == 'personal':
-            name.attrib['type'] = "nameUsedByThePerson"
-            foreName = etree.SubElement(name, "{http://www.d-nb.de/standards/pc/}foreName", nsmap=nsmap)
-            foreName.text = mperson['given_name']
-            surName = etree.SubElement(name, "{http://www.d-nb.de/standards/pc/}surName", nsmap=nsmap)
-            surName.text = mperson['family_name']
-            if 'affiliations' in mcreator:
-                maffiliation = mcreator['affiliations'][0]
-                affiliation = etree.SubElement(person, "{http://www.d-nb.de/standards/pc/}affiliation", nsmap=nsmap)
-                institution = etree.SubElement(affiliation,
-                                               "{http://www.d-nb.de/standards/cc/}universityOrInstitution",
-                                               nsmap=nsmap)
-                ccname = etree.SubElement(institution, "{http://www.d-nb.de/standards/cc/}name", nsmap=nsmap)
-                ccname.text = maffiliation['name']
+                    id = etree.SubElement(
+                        person, "{http://www.d-nb.de/standards/ddb/}OtherId"
+                    )
+                    id.text = "(ror)" + midentifier["identifier"]
+        name = etree.SubElement(
+            person, "{http://www.d-nb.de/standards/pc/}name", nsmap=nsmap
+        )
+        if mperson["type"] == "personal":
+            name.attrib["type"] = "nameUsedByThePerson"
+            foreName = etree.SubElement(
+                name, "{http://www.d-nb.de/standards/pc/}foreName", nsmap=nsmap
+            )
+            foreName.text = mperson["given_name"]
+            surName = etree.SubElement(
+                name, "{http://www.d-nb.de/standards/pc/}surName", nsmap=nsmap
+            )
+            surName.text = mperson["family_name"]
+            if "affiliations" in mcreator:
+                maffiliation = mcreator["affiliations"][0]
+                affiliation = etree.SubElement(
+                    person, "{http://www.d-nb.de/standards/pc/}affiliation", nsmap=nsmap
+                )
+                institution = etree.SubElement(
+                    affiliation,
+                    "{http://www.d-nb.de/standards/cc/}universityOrInstitution",
+                    nsmap=nsmap,
+                )
+                ccname = etree.SubElement(
+                    institution, "{http://www.d-nb.de/standards/cc/}name", nsmap=nsmap
+                )
+                ccname.text = maffiliation["name"]
         else:
-            name.attrib['type'] = "otherName"
-            name.attrib['otherNameType'] = "organisation"
-            organisationName = etree.SubElement(name, "{http://www.d-nb.de/standards/pc/}organisationName", nsmap=nsmap)
-            organisationName.text = mperson['name']
-    if 'subjects' in metadata:
-        for msubject in metadata['subjects']:
-            subject = etree.SubElement(xmetadiss, "{http://purl.org/dc/elements/1.1/}subject", nsmap=nsmap)
-            if 'scheme' in msubject:
-                if msubject['scheme'] == 'FOS':
-                    subject.attrib['{http://www.w3.org/2001/XMLSchema-instance}type'] = "xMetaDiss:noScheme"
-                    subject.text = msubject['subject']
-                elif 'DDC' in msubject['scheme']:
-                    subject.attrib['{http://www.w3.org/2001/XMLSchema-instance}type'] = "dcterms:DDC"
-                    id = msubject['id']
+            name.attrib["type"] = "otherName"
+            name.attrib["otherNameType"] = "organisation"
+            organisationName = etree.SubElement(
+                name, "{http://www.d-nb.de/standards/pc/}organisationName", nsmap=nsmap
+            )
+            organisationName.text = mperson["name"]
+    if "subjects" in metadata:
+        for msubject in metadata["subjects"]:
+            subject = etree.SubElement(
+                xmetadiss, "{http://purl.org/dc/elements/1.1/}subject", nsmap=nsmap
+            )
+            if "scheme" in msubject:
+                if msubject["scheme"] == "FOS":
+                    subject.attrib[
+                        "{http://www.w3.org/2001/XMLSchema-instance}type"
+                    ] = "xMetaDiss:noScheme"
+                    subject.text = msubject["subject"]
+                elif "DDC" in msubject["scheme"]:
+                    subject.attrib[
+                        "{http://www.w3.org/2001/XMLSchema-instance}type"
+                    ] = "dcterms:DDC"
+                    id = msubject["id"]
                     reversed_id = "".join(reversed(id))
                     last_slash = len(id) - reversed_id.index("/") - 1
-                    subject.text = id[last_slash + 1:]
+                    subject.text = id[last_slash + 1 :]
                 else:
-                    subject.attrib['{http://www.w3.org/2001/XMLSchema-instance}type'] = "xMetaDiss:noScheme"
-                    subject.text = msubject['subject']
-    mpublisher = metadata['publisher']
-    if '/' in mpublisher:
+                    subject.attrib[
+                        "{http://www.w3.org/2001/XMLSchema-instance}type"
+                    ] = "xMetaDiss:noScheme"
+                    subject.text = msubject["subject"]
+    mpublisher = metadata["publisher"]
+    if "/" in mpublisher:
         reversed_mpublisher = "".join(reversed(mpublisher))
         first_slash = mpublisher.index("/")
         last_slash = len(mpublisher) - reversed_mpublisher.index("/") - 1
         sinstitution = mpublisher[:first_slash].rstrip()
-        splace = mpublisher[last_slash + 1:].lstrip()
+        splace = mpublisher[last_slash + 1 :].lstrip()
     else:
         sinstitution = mpublisher
         splace = "..."
-    publisher = etree.SubElement(xmetadiss, "{http://purl.org/dc/elements/1.1/}publisher", nsmap=nsmap,
-                                 attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "cc:Publisher"})
-    institution = etree.SubElement(publisher,
-                                   "{http://www.d-nb.de/standards/cc/}universityOrInstitution",
-                                   nsmap=nsmap)
-    ccname = etree.SubElement(institution, "{http://www.d-nb.de/standards/cc/}name", nsmap=nsmap)
+    publisher = etree.SubElement(
+        xmetadiss,
+        "{http://purl.org/dc/elements/1.1/}publisher",
+        nsmap=nsmap,
+        attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "cc:Publisher"},
+    )
+    institution = etree.SubElement(
+        publisher,
+        "{http://www.d-nb.de/standards/cc/}universityOrInstitution",
+        nsmap=nsmap,
+    )
+    ccname = etree.SubElement(
+        institution, "{http://www.d-nb.de/standards/cc/}name", nsmap=nsmap
+    )
     ccname.text = sinstitution
-    ccplace = etree.SubElement(institution, "{http://www.d-nb.de/standards/cc/}place", nsmap=nsmap)
+    ccplace = etree.SubElement(
+        institution, "{http://www.d-nb.de/standards/cc/}place", nsmap=nsmap
+    )
     ccplace.text = splace
-    if 'contributors' in metadata:
-        for mcontributor in metadata['contributors']:
-            contributor = etree.SubElement(xmetadiss, "{http://purl.org/dc/elements/1.1/}contributor", nsmap=nsmap,
-                                   attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "pc:Contributor"})
-            person = etree.SubElement(contributor, "{http://www.d-nb.de/standards/pc/}person", nsmap=nsmap)
-            mperson = mcontributor['person_or_org']
-            if 'identifiers' in mperson:
-                for midentifier in mperson['identifiers']:
-                    mscheme = midentifier['scheme']
+    if "contributors" in metadata:
+        for mcontributor in metadata["contributors"]:
+            contributor = etree.SubElement(
+                xmetadiss,
+                "{http://purl.org/dc/elements/1.1/}contributor",
+                nsmap=nsmap,
+                attrib={
+                    "{http://www.w3.org/2001/XMLSchema-instance}type": "pc:Contributor"
+                },
+            )
+            person = etree.SubElement(
+                contributor, "{http://www.d-nb.de/standards/pc/}person", nsmap=nsmap
+            )
+            mperson = mcontributor["person_or_org"]
+            if "identifiers" in mperson:
+                for midentifier in mperson["identifiers"]:
+                    mscheme = midentifier["scheme"]
                     if mscheme == "orcid":
-                        id = etree.SubElement(person, "{http://www.d-nb.de/standards/ddb/}ORCID")
-                        id.text = midentifier['identifier']
+                        id = etree.SubElement(
+                            person, "{http://www.d-nb.de/standards/ddb/}ORCID"
+                        )
+                        id.text = midentifier["identifier"]
                     elif mscheme == "gnd":
-                        person.attrib['{http://www.d-nb.de/standards/ddb/}GND-Nr'] = midentifier['identifier']
+                        person.attrib["{http://www.d-nb.de/standards/ddb/}GND-Nr"] = (
+                            midentifier["identifier"]
+                        )
                     elif mscheme == "isni":
-                        id = etree.SubElement(person, "{http://www.d-nb.de/standards/ddb/}ISNI")
-                        id.text = midentifier['identifier']
+                        id = etree.SubElement(
+                            person, "{http://www.d-nb.de/standards/ddb/}ISNI"
+                        )
+                        id.text = midentifier["identifier"]
                     elif mscheme == "ror":
-                        id = etree.SubElement(person, "{http://www.d-nb.de/standards/ddb/}OtherId")
-                        id.text = "(ror)" + midentifier['identifier']
-            name = etree.SubElement(person, "{http://www.d-nb.de/standards/pc/}name", nsmap=nsmap)
-            if mperson['type'] == 'personal':
-                name.attrib['type'] = "nameUsedByThePerson"
-                foreName = etree.SubElement(name, "{http://www.d-nb.de/standards/pc/}foreName", nsmap=nsmap)
-                foreName.text = mperson['given_name']
-                surName = etree.SubElement(name, "{http://www.d-nb.de/standards/pc/}surName", nsmap=nsmap)
-                surName.text = mperson['family_name']
-                if 'affiliations' in mcreator:
-                    maffiliation = mcreator['affiliations'][0]
-                    affiliation = etree.SubElement(person, "{http://www.d-nb.de/standards/pc/}affiliation", nsmap=nsmap)
-                    institution = etree.SubElement(affiliation,
-                                                   "{http://www.d-nb.de/standards/cc/}universityOrInstitution",
-                                                   nsmap=nsmap)
-                    ccname = etree.SubElement(institution, "{http://www.d-nb.de/standards/cc/}name", nsmap=nsmap)
-                    ccname.text = maffiliation['name']
+                        id = etree.SubElement(
+                            person, "{http://www.d-nb.de/standards/ddb/}OtherId"
+                        )
+                        id.text = "(ror)" + midentifier["identifier"]
+            name = etree.SubElement(
+                person, "{http://www.d-nb.de/standards/pc/}name", nsmap=nsmap
+            )
+            if mperson["type"] == "personal":
+                name.attrib["type"] = "nameUsedByThePerson"
+                foreName = etree.SubElement(
+                    name, "{http://www.d-nb.de/standards/pc/}foreName", nsmap=nsmap
+                )
+                foreName.text = mperson["given_name"]
+                surName = etree.SubElement(
+                    name, "{http://www.d-nb.de/standards/pc/}surName", nsmap=nsmap
+                )
+                surName.text = mperson["family_name"]
+                if "affiliations" in mcreator:
+                    maffiliation = mcreator["affiliations"][0]
+                    affiliation = etree.SubElement(
+                        person,
+                        "{http://www.d-nb.de/standards/pc/}affiliation",
+                        nsmap=nsmap,
+                    )
+                    institution = etree.SubElement(
+                        affiliation,
+                        "{http://www.d-nb.de/standards/cc/}universityOrInstitution",
+                        nsmap=nsmap,
+                    )
+                    ccname = etree.SubElement(
+                        institution,
+                        "{http://www.d-nb.de/standards/cc/}name",
+                        nsmap=nsmap,
+                    )
+                    ccname.text = maffiliation["name"]
             else:
-                name.attrib['type'] = "otherName"
-                name.attrib['otherNameType'] = "organisation"
-                organisationName = etree.SubElement(name, "{http://www.d-nb.de/standards/pc/}organisationName", nsmap=nsmap)
-                organisationName.text = mperson['name']
+                name.attrib["type"] = "otherName"
+                name.attrib["otherNameType"] = "organisation"
+                organisationName = etree.SubElement(
+                    name,
+                    "{http://www.d-nb.de/standards/pc/}organisationName",
+                    nsmap=nsmap,
+                )
+                organisationName.text = mperson["name"]
     mdate_issued = None
-    if 'dates' in metadata:
-        for mdate in metadata['dates']:
-            if mdate['type']['id'] == 'issued':
-                mdate_issued = mdate['date']
+    if "dates" in metadata:
+        for mdate in metadata["dates"]:
+            if mdate["type"]["id"] == "issued":
+                mdate_issued = mdate["date"]
     if mdate_issued == None:
-        mdate_issued = metadata['publication_date']
-    date_issued = etree.SubElement(xmetadiss, "{http://purl.org/dc/terms/}issued", nsmap=nsmap,
-                                   attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "dcterms:W3CDTF"})
+        mdate_issued = metadata["publication_date"]
+    date_issued = etree.SubElement(
+        xmetadiss,
+        "{http://purl.org/dc/terms/}issued",
+        nsmap=nsmap,
+        attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "dcterms:W3CDTF"},
+    )
     date_issued.text = mdate_issued
     dini_mapping = current_app.config.get("XMETADISS_TYPE_DINI_PUBLTYPE")
     dcterms_mapping = current_app.config.get("XMETADISS_TYPE_DCTERMS_DCMITYPE")
-    xmetadiss = add_dctype(xmetadiss, nsmap, metadata, dini_mapping, 'dini:publType')
-    xmetadiss = add_dctype(xmetadiss, nsmap, metadata, dcterms_mapping, 'dcterms:DCMIType')
+    xmetadiss = add_dctype(xmetadiss, nsmap, metadata, dini_mapping, "dini:publType")
+    xmetadiss = add_dctype(
+        xmetadiss, nsmap, metadata, dcterms_mapping, "dcterms:DCMIType"
+    )
 
-    pids = record['_source']['pids']
+    pids = record["_source"]["pids"]
     urn = None
     doi = None
     for mpid in pids:
-        if 'urn' in mpid:
-            urn = pids['urn']['identifier']
-        if 'doi' in mpid:
-            doi = pids['doi']['identifier']
+        if "urn" in mpid:
+            urn = pids["urn"]["identifier"]
+        if "doi" in mpid:
+            doi = pids["doi"]["identifier"]
     if urn is not None:
         dcidentifier = etree.SubElement(
-            xmetadiss, "{http://purl.org/dc/elements/1.1/}identifier",
+            xmetadiss,
+            "{http://purl.org/dc/elements/1.1/}identifier",
             nsmap=nsmap,
-            attrib={'{http://www.w3.org/2001/XMLSchema-instance}type': 'urn:nbn'})
+            attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "urn:nbn"},
+        )
         dcidentifier.text = urn
     elif doi is not None:
         dcidentifier = etree.SubElement(
-            xmetadiss, "{http://purl.org/dc/elements/1.1/}identifier",
+            xmetadiss,
+            "{http://purl.org/dc/elements/1.1/}identifier",
             nsmap=nsmap,
-            attrib={'{http://www.w3.org/2001/XMLSchema-instance}type': 'doi:doi'})
+            attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "doi:doi"},
+        )
         dcidentifier.text = doi
 
-    if 'sizes' in metadata:
-        for size in metadata['sizes']:
+    if "sizes" in metadata:
+        for size in metadata["sizes"]:
             dcterms_extent = etree.SubElement(
-                xmetadiss, "{http://purl.org/dc/terms/}extent",
-                nsmap=nsmap)
+                xmetadiss, "{http://purl.org/dc/terms/}extent", nsmap=nsmap
+            )
             dcterms_extent.text = size
     dcterms_medium = etree.SubElement(
-        xmetadiss, "{http://purl.org/dc/terms/}medium",
+        xmetadiss,
+        "{http://purl.org/dc/terms/}medium",
         nsmap=nsmap,
-        attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "dcterms:IMT"})
+        attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": "dcterms:IMT"},
+    )
     dcterms_medium.text = "application/zip"
     if lang is not None:
         language = etree.SubElement(
-            xmetadiss, "{http://purl.org/dc/elements/1.1/}language",
+            xmetadiss,
+            "{http://purl.org/dc/elements/1.1/}language",
             nsmap=nsmap,
-            attrib={'{http://www.w3.org/2001/XMLSchema-instance}type': 'ddb:titleISO639-2'})
+            attrib={
+                "{http://www.w3.org/2001/XMLSchema-instance}type": "ddb:titleISO639-2"
+            },
+        )
         language.text = lang
-    if 'additional_descriptions' in metadata:
-        for additional_description in metadata['additional_descriptions']:
-            if additional_description['type']['id'] == 'series-information':
+    if "additional_descriptions" in metadata:
+        for additional_description in metadata["additional_descriptions"]:
+            if additional_description["type"]["id"] == "series-information":
                 isPartOf = etree.SubElement(
-                    xmetadiss, "{http://purl.org/dc/terms/}isPartOf",
+                    xmetadiss,
+                    "{http://purl.org/dc/terms/}isPartOf",
                     nsmap=nsmap,
-                    attrib={'{http://www.w3.org/2001/XMLSchema-instance}type': 'ddb:noScheme'})
-                mIsPartOf = additional_description['description'].replace("<p>", "")
+                    attrib={
+                        "{http://www.w3.org/2001/XMLSchema-instance}type": "ddb:noScheme"
+                    },
+                )
+                mIsPartOf = additional_description["description"].replace("<p>", "")
                 mIsPartOf = mIsPartOf.replace("</p>", "")
                 isPartOf.text = mIsPartOf
-    if 'custom_fields' in source:
-        custom_fields = source['custom_fields']
-        if 'thesis:level' in custom_fields \
-            and 'thesis:organisation' in custom_fields \
-            and 'thesis:place' in custom_fields:
+    if "custom_fields" in source:
+        custom_fields = source["custom_fields"]
+        if (
+            "thesis:level" in custom_fields
+            and "thesis:organisation" in custom_fields
+            and "thesis:place" in custom_fields
+        ):
             thesis_degree = etree.SubElement(
-                xmetadiss, "{http://www.ndltd.org/standards/metadata/etdms/1.0/}degree",
-                nsmap=nsmap)
+                xmetadiss,
+                "{http://www.ndltd.org/standards/metadata/etdms/1.0/}degree",
+                nsmap=nsmap,
+            )
             thesis_level = etree.SubElement(
-                thesis_degree, "{http://www.ndltd.org/standards/metadata/etdms/1.0/}level",
-                nsmap=nsmap
+                thesis_degree,
+                "{http://www.ndltd.org/standards/metadata/etdms/1.0/}level",
+                nsmap=nsmap,
             )
-            thesis_level.text = custom_fields['thesis:level']['id']
+            thesis_level.text = custom_fields["thesis:level"]["id"]
             thesis_grantor = etree.SubElement(
-                thesis_degree, "{http://www.ndltd.org/standards/metadata/etdms/1.0/}grantor",
-                nsmap=nsmap
+                thesis_degree,
+                "{http://www.ndltd.org/standards/metadata/etdms/1.0/}grantor",
+                nsmap=nsmap,
+            )
+            grantor_institution = etree.SubElement(
+                thesis_grantor,
+                "{http://www.d-nb.de/standards/cc/}universityOrInstitution",
+                nsmap=nsmap,
             )
-            grantor_institution = etree.SubElement(thesis_grantor,
-                                           "{http://www.d-nb.de/standards/cc/}universityOrInstitution",
-                                           nsmap=nsmap)
             grantor_ccname = etree.SubElement(
-                grantor_institution, "{http://www.d-nb.de/standards/cc/}name",
-                nsmap=nsmap)
-            grantor_ccname.text = custom_fields['thesis:organisation']
+                grantor_institution,
+                "{http://www.d-nb.de/standards/cc/}name",
+                nsmap=nsmap,
+            )
+            grantor_ccname.text = custom_fields["thesis:organisation"]
             grantor_ccplace = etree.SubElement(
-                grantor_institution, "{http://www.d-nb.de/standards/cc/}place",
-                nsmap=nsmap)
-            grantor_ccplace.text = custom_fields['thesis:place']
+                grantor_institution,
+                "{http://www.d-nb.de/standards/cc/}place",
+                nsmap=nsmap,
+            )
+            grantor_ccplace.text = custom_fields["thesis:place"]
 
     ddbtransfer = etree.SubElement(
-        xmetadiss, "{http://www.d-nb.de/standards/ddb/}transfer",
+        xmetadiss,
+        "{http://www.d-nb.de/standards/ddb/}transfer",
         nsmap=nsmap,
-        attrib={'{http://www.d-nb.de/standards/ddb/}type': 'dcterms:URI'})
-    ddbtransfer.text = current_app.config.get("SITE_API_URL") + "/records/" \
-                           + record['_source']['id'] + "/files-archive"
+        attrib={"{http://www.d-nb.de/standards/ddb/}type": "dcterms:URI"},
+    )
+    ddbtransfer.text = (
+        current_app.config.get("SITE_API_URL")
+        + "/records/"
+        + record["_source"]["id"]
+        + "/files-archive"
+    )
 
     ddbidentifier = etree.SubElement(
-        xmetadiss, "{http://www.d-nb.de/standards/ddb/}identifier",
+        xmetadiss,
+        "{http://www.d-nb.de/standards/ddb/}identifier",
         nsmap=nsmap,
-        attrib={'{http://www.d-nb.de/standards/ddb/}type': 'URL'})
-    ddbidentifier.text = current_app.config.get("SITE_UI_URL") + "/records/" \
-                           + record['_source']['id']
+        attrib={"{http://www.d-nb.de/standards/ddb/}type": "URL"},
+    )
+    ddbidentifier.text = (
+        current_app.config.get("SITE_UI_URL") + "/records/" + record["_source"]["id"]
+    )
     if urn is not None and doi is not None:
         ddbidentifier = etree.SubElement(
-            xmetadiss, "{http://www.d-nb.de/standards/ddb/}identifier",
+            xmetadiss,
+            "{http://www.d-nb.de/standards/ddb/}identifier",
             nsmap=nsmap,
-            attrib={'{http://www.d-nb.de/standards/ddb/}type': 'DOI'})
+            attrib={"{http://www.d-nb.de/standards/ddb/}type": "DOI"},
+        )
         ddbidentifier.text = doi
 
-    if 'identifiers' in metadata:
-        for midentifier in metadata['identifiers']:
-            identifier = midentifier['identifier']
-            scheme = 'other'
-            if midentifier['scheme'] == 'url':
-                scheme = 'URL'
-            elif midentifier['scheme'] == 'urn':
-                scheme = 'URN'
-            elif midentifier['scheme'] == 'doi':
-                scheme = 'DOI'
-            elif midentifier['scheme'] == 'handle':
-                scheme = 'handle'
-            elif midentifier['scheme'] == 'isbn':
-                scheme = 'ISBN'
+    if "identifiers" in metadata:
+        for midentifier in metadata["identifiers"]:
+            identifier = midentifier["identifier"]
+            scheme = "other"
+            if midentifier["scheme"] == "url":
+                scheme = "URL"
+            elif midentifier["scheme"] == "urn":
+                scheme = "URN"
+            elif midentifier["scheme"] == "doi":
+                scheme = "DOI"
+            elif midentifier["scheme"] == "handle":
+                scheme = "handle"
+            elif midentifier["scheme"] == "isbn":
+                scheme = "ISBN"
             ddbidentifier = etree.SubElement(
-                xmetadiss, "{http://www.d-nb.de/standards/ddb/}identifier",
+                xmetadiss,
+                "{http://www.d-nb.de/standards/ddb/}identifier",
                 nsmap=nsmap,
-                attrib={'{http://www.d-nb.de/standards/ddb/}type': scheme})
+                attrib={"{http://www.d-nb.de/standards/ddb/}type": scheme},
+            )
             ddbidentifier.text = identifier
 
-    maccess = record['_source']['access']
-    kind = 'free'
-    if maccess['files'] == 'restricted':
-        kind = 'domain'
+    maccess = record["_source"]["access"]
+    kind = "free"
+    if maccess["files"] == "restricted":
+        kind = "domain"
     ddbrights = etree.SubElement(
-        xmetadiss, "{http://www.d-nb.de/standards/ddb/}rights",
+        xmetadiss,
+        "{http://www.d-nb.de/standards/ddb/}rights",
         nsmap=nsmap,
-        attrib={'{http://www.d-nb.de/standards/ddb/}kind': kind})
-    if 'rights' in metadata:
-        for mright in metadata['rights']:
+        attrib={"{http://www.d-nb.de/standards/ddb/}kind": kind},
+    )
+    if "rights" in metadata:
+        for mright in metadata["rights"]:
             access = etree.SubElement(
                 xmetadiss,
                 "{http://www.d-nb.de/standards/ddb/}licence",
                 nsmap=nsmap,
-                attrib={'{http://www.d-nb.de/standards/ddb/}licenceType': 'access'})
-            access.text = 'OA'
-            if 'cc' in mright['id']:
+                attrib={"{http://www.d-nb.de/standards/ddb/}licenceType": "access"},
+            )
+            access.text = "OA"
+            if "cc" in mright["id"]:
                 cc = etree.SubElement(
                     xmetadiss,
                     "{http://www.d-nb.de/standards/ddb/}licence",
                     nsmap=nsmap,
-                    attrib={'{http://www.d-nb.de/standards/ddb/}licenceType': 'cc'})
-                cc.text = mright['id']
+                    attrib={"{http://www.d-nb.de/standards/ddb/}licenceType": "cc"},
+                )
+                cc.text = mright["id"]
             else:
                 other_scheme = etree.SubElement(
                     xmetadiss,
                     "{http://www.d-nb.de/standards/ddb/}licence",
                     nsmap=nsmap,
-                    attrib={'{http://www.d-nb.de/standards/ddb/}licenceType': 'noScheme'})
-                if 'de' in mright['title']:
-                    other_scheme.text = mright['title']['de']
+                    attrib={
+                        "{http://www.d-nb.de/standards/ddb/}licenceType": "noScheme"
+                    },
+                )
+                if "de" in mright["title"]:
+                    other_scheme.text = mright["title"]["de"]
                 else:
-                    other_scheme.text = mright['title']['en']
+                    other_scheme.text = mright["title"]["en"]
             lic_url = etree.SubElement(
-                    xmetadiss,
-                    "{http://www.d-nb.de/standards/ddb/}licence",
-                    nsmap=nsmap,
-                    attrib={'{http://www.d-nb.de/standards/ddb/}licenceType': 'URL'})
-            lic_url.text = mright['props']['url']
+                xmetadiss,
+                "{http://www.d-nb.de/standards/ddb/}licence",
+                nsmap=nsmap,
+                attrib={"{http://www.d-nb.de/standards/ddb/}licenceType": "URL"},
+            )
+            lic_url.text = mright["props"]["url"]
     else:
         access = etree.SubElement(
             xmetadiss,
             "{http://www.d-nb.de/standards/ddb/}licence",
             nsmap=nsmap,
-            attrib={'{http://www.d-nb.de/standards/ddb/}licenceType': 'access'})
-        access.text = 'nOA'
+            attrib={"{http://www.d-nb.de/standards/ddb/}licenceType": "access"},
+        )
+        access.text = "nOA"
         other_scheme = etree.SubElement(
             xmetadiss,
             "{http://www.d-nb.de/standards/ddb/}licence",
             nsmap=nsmap,
-            attrib={'{http://www.d-nb.de/standards/ddb/}licenceType': 'otherScheme'})
-        other_scheme.text = 'Keine Angabe'
+            attrib={"{http://www.d-nb.de/standards/ddb/}licenceType": "otherScheme"},
+        )
+        other_scheme.text = "Keine Angabe"
         lic_url = etree.SubElement(
             xmetadiss,
             "{http://www.d-nb.de/standards/ddb/}licence",
             nsmap=nsmap,
-            attrib={'{http://www.d-nb.de/standards/ddb/}licenceType': 'URL'})
-        lic_url.text = 'Keine Angabe'
+            attrib={"{http://www.d-nb.de/standards/ddb/}licenceType": "URL"},
+        )
+        lic_url.text = "Keine Angabe"
 
     return xmetadiss
 
 
 def add_dctype(parent, nsmap, metadata, mapping, type):
-    print(mapping)
+    """Add a DCType element."""
     props = get_vocabulary_props(
         "resourcetypes",
         [
             "props." + mapping,
         ],
         metadata["resource_type"]["id"],
     )
     dctype = etree.SubElement(
-        parent, "{http://purl.org/dc/elements/1.1/}type",
+        parent,
+        "{http://purl.org/dc/elements/1.1/}type",
         nsmap=nsmap,
-        attrib={'{http://www.w3.org/2001/XMLSchema-instance}type': type})
+        attrib={"{http://www.w3.org/2001/XMLSchema-instance}type": type},
+    )
     mapped_type = props.get(mapping)
     dctype.text = mapped_type
     return parent
```

### Comparing `invenio-dnb-urn-0.1.3/invenio_dnb_urn/provider/dnburn.py` & `invenio-dnb-urn-0.2.2/invenio_dnb_urn/provider/dnburn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022, 2023 University of Münster.
+# Copyright (C) 2022-2024 University of Münster.
 #
-# Invenio-Dnb-Urn is free software; you can redistribute it and/or modify it
+# invenio-dnb-urn is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
+"""DNB urn client and provider to use the dnb-urn-service API wrapper."""
+
 import json
 import warnings
 
 from dnb_urn_service import DNBUrnServiceRESTClient
 from dnb_urn_service.errors import DNBURNServiceError
 from flask import current_app
 from invenio_pidstore.models import PIDStatus
@@ -39,17 +41,20 @@
         if not prefix:
             raise RuntimeError("Invalid URN prefix configured.")
         urn_format = self.cfg("format", "{prefix}-{id}")
         return urn_format.format(prefix=prefix, id=record.pid.pid_value)
 
     def check_credentials(self, **kwargs):
         """Returns if the client has the credentials properly set up.
+
         If the client is running on test mode the credentials are required, too.
         """
-        if not (self.cfg("username") and self.cfg("password") and self.cfg("id_prefix")):
+        if not (
+            self.cfg("username") and self.cfg("password") and self.cfg("id_prefix")
+        ):
             warnings.warn(
                 f"The {self.__class__.__name__} is misconfigured. Please "
                 f"set {self.cfgkey('username')}, {self.cfgkey('password')}"
                 f" and {self.cfgkey('id_prefix')} in your configuration.",
                 UserWarning,
             )
 
@@ -68,20 +73,15 @@
 
 
 class DnbUrnProvider(PIDProvider):
     """URN provider."""
 
     name = "urn"
 
-    def __init__(
-        self,
-        id_,
-        client=None,
-        pid_type="urn",
-        **kwargs):
+    def __init__(self, id_, client=None, pid_type="urn", **kwargs):
         """Constructor."""
         super().__init__(
             id_,
             client=(client or DNBUrnClient("dnb", config_prefix="URN_DNB")),
             pid_type=pid_type,
             default_status=PIDStatus.NEW,
             managed=True,
@@ -155,15 +155,14 @@
     def delete(self, pid, **kwargs):
         """Delete/unregister a registered URN.
 
         If the PID has not been reserved then it's deleted only locally.
         Otherwise, there is a problem: a URN can't be deleted remotely.
         :returns: `True` if is deleted successfully.
         """
-
         return super().delete(pid, **kwargs)
 
     def validate(self, record, identifier=None, provider=None, **kwargs):
         """Validate the attributes of the identifier.
 
         :returns: A tuple (success, errors). The first specifies if the
                   validation was passed successfully. The second one is an
```

### Comparing `invenio-dnb-urn-0.1.3/invenio_dnb_urn/serialize/xmetadiss.py` & `invenio-dnb-urn-0.2.2/invenio_dnb_urn/serialize/xmetadiss.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022, 2023 University of Münster.
+# Copyright (C) 2022-2024 University of Münster.
 #
 # Invenio-Dnb-Urn is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """xMetaDissPlus-based data model for Invenio."""
 
 from invenio_rdm_records.oaiserver.resources.config import OAIPMHServerResourceConfig
@@ -18,42 +18,39 @@
 
     def __init__(self, app=None):
         """Extension initialization."""
         if app:
             self.init_app(app)
 
     def init_app(self, app):
+        """Flask application initialization."""
         self.init_config(app)
         self.init_services(app)
         self.init_resource(app)
         app.extensions["invenio_dnb_urn"] = self
 
     def init_config(self, app):
         """Initialize configuration."""
 
-    def init_config(self, app):
-        """Initialize configuration."""
-
     def service_configs(self, app):
         """Customized service configs."""
 
         class ServiceConfigs:
             oaipmh_server = OAIPMHServerServiceConfig
 
         return ServiceConfigs
 
     def init_services(self, app):
-        """Initialize services"""
+        """Initialize services."""
         service_configs = self.service_configs(app)
 
         self.oaipmh_server_service = OAIPMHServerService(
             config=service_configs.oaipmh_server,
         )
 
     def init_resource(self, app):
-        """Initialize resources"""
-
+        """Initialize resources."""
         # OAI-PMH
         self.oaipmh_server_resource = OAIPMHServerResource(
             service=self.oaipmh_server_service,
             config=OAIPMHServerResourceConfig,
         )
```

### Comparing `invenio-dnb-urn-0.1.3/invenio_dnb_urn/utils.py` & `invenio-dnb-urn-0.2.2/invenio_dnb_urn/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022, 2023 University of Münster.
+# Copyright (C) 2022-2024 University of Münster.
 #
-# Invenio-Dnb-Urn is free software; you can redistribute it and/or modify
+# invenio-dnb-urn is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Helpers for serializers."""
 
 from invenio_access.permissions import system_identity
 from invenio_search.engine import dsl
 from invenio_vocabularies.proxies import current_service as vocabulary_service
```

### Comparing `invenio-dnb-urn-0.1.3/invenio_dnb_urn/views.py` & `invenio-dnb-urn-0.2.2/invenio_dnb_urn/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2022, 2023 University of Münster.
+# Copyright (C) 2022-2024 University of Münster.
 #
-# Invenio-Dnb-Urn is free software; you can redistribute it and/or modify
-# it under the terms of the MIT License; see LICENSE file for more details.
+# invenio-dnb-urn is free software; you can redistribute it and/or modify it
+# under the terms of the MIT License; see LICENSE file for more details.
 
 """Views."""
 
 from flask import Blueprint
 
 blueprint = Blueprint("invenio_dnb_urn_ext", __name__)
```

### Comparing `invenio-dnb-urn-0.1.3/setup.cfg` & `invenio-dnb-urn-0.2.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,90 @@
 [metadata]
 name = invenio-dnb-urn
 version = attr: invenio_dnb_urn.__version__
 description = "InvenioRDM module so support DNB urn registration."
-long_description = file: README.md
-long_description_content_type = text/markdown
-keywords = invenio rdm data model
+long_description = file: README.rst, CHANGES.rst
+keywords = invenio TODO
 license = MIT
 author = University of Münster
-author_email = gressho@uni-muenster.de
+author_email = forschungsdaten@uni-muenster.de
 platforms = any
 url = https://github.com/ulbmuenster/invenio-dnb-urn
 classifiers = 
 	Development Status :: 3 - Alpha
 
 [options]
 include_package_data = True
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.9
 zip_safe = False
 install_requires = 
-	arrow>=0.17.0
-	citeproc-py-styles>=0.1.2
-	citeproc-py>=0.6.0
-	dcxml>=0.1.2
-	dnb-urn-service>=0.1.5,<1.0.0
-	Faker>=2.0.3
+	dnb-urn-service>=0.1.6
 	Flask>=2.2.0,<2.3.0
-	flask-iiif>=0.6.2
-	ftfy>=4.4.3,<5.0.0
+	lxml>=5.2.1
+	invenio-access>=1.4.4,<1.5.0
 	invenio-drafts-resources>=0.18.2
 	invenio-oaiserver>=2.1.0,<2.2.0
 	invenio-pidstore>=1.2.3,<1.3.0
 	invenio-rdm-records>=2.1.0,<3.0.0
-	pytz>=2020.4
-	pyyaml>=5.4.0
+	invenio-search[opensearch2]>=2.3.1
+	invenio-vocabularies>=1.0.4,<1.1.0
 
 [options.extras_require]
 tests = 
-	pytest-black>=0.3.0
 	invenio-app>=1.3.4,<2.0.0
-	invenio-db[postgresql,mysql,versioning]>=1.0.14,<2.0.0
 	pytest-invenio>=2.1.0,<3.0.0
+	pytest-black>=0.3.0
+	invenio-app>=1.3.4
+	invenio-db[postgresql,mysql,versioning]>=1.0.14,<2.0
 	pytest-mock>=1.6.0
-	sphinx>=4.5.0
+	sphinx>=4.2.0,<5
 	tripoli~=2.0.0
-opensearch1 = 
-	invenio-search[opensearch1]>=2.1.0,<3.0.0
 opensearch2 = 
 	invenio-search[opensearch2]>=2.1.0,<3.0.0
 
 [options.entry_points]
 invenio_base.apps = 
 	invenio_dnb_urn = invenio_dnb_urn:InvenioSerializerXMetaDissPlus
 invenio_base.api_apps = 
 	invenio_dnb_urn = invenio_dnb_urn:InvenioSerializerXMetaDissPlus
-invenio_i18n.translations = 
-	invenio_dnb_urn = invenio_dnb_urn
-
-[build_sphinx]
-source-dir = docs/
-build-dir = docs/_build
-all_files = 1
 
 [bdist_wheel]
 universal = 1
 
 [pydocstyle]
 add_ignore = D401,D403
 
+[isort]
+profile = black
+
+[check-manifest]
+ignore = 
+	*-requirements.txt
+
+[tool:pytest]
+addopts = --black --isort --pydocstyle --cov=invenio_dnb_urn --cov-report term --cov-report xml:coverage.xml --junitxml=report.xml
+testpaths = tests invenio_dnb_urn
+
+[compile_catalog]
+directory = invenio_dnb_urn/translations/
+use-fuzzy = True
+
 [extract_messages]
-copyright_holder = CERN
-msgid_bugs_address = info@inveniosoftware.org
+copyright_holder = University of Münster
+msgid_bugs_address = forschungsdaten@uni-muenster.de
 mapping-file = babel.ini
 output-file = invenio_dnb_urn/translations/messages.pot
 add-comments = NOTE
 
 [init_catalog]
 input-file = invenio_dnb_urn/translations/messages.pot
 output-dir = invenio_dnb_urn/translations/
 
 [update_catalog]
 input-file = invenio_dnb_urn/translations/messages.pot
 output-dir = invenio_dnb_urn/translations/
 
-[isort]
-profile = black
-
-[check-manifest]
-ignore = 
-	*-requirements.txt
-
-[tool:pytest]
-addopts = --black --isort --pydocstyle --doctest-glob="*.rst" --doctest-modules --cov=invenio_dnb_urn --cov-report=term-missing
-testpaths = docs tests invenio_dnb_urn
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

