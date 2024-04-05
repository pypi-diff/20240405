# Comparing `tmp/pyscal_rdf-0.2.3.tar.gz` & `tmp/pyscal_rdf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal_rdf-0.2.3.tar", last modified: Thu Apr  4 10:44:37 2024, max compression
+gzip compressed data, was "pyscal_rdf-0.2.5.tar", last modified: Fri Apr  5 09:14:49 2024, max compression
```

## Comparing `pyscal_rdf-0.2.3.tar` & `pyscal_rdf-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.357071 pyscal_rdf-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.349072 pyscal_rdf-0.2.3/pyscal_rdf/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/pyscal_rdf/data/
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/asmo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/cmso.owl
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/element.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/pldo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/data/podo.owl
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18815 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/json_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/pyscal_rdf/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/network/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    27466 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/pyscal_rdf/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/pyscal_rdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:44:37.357071 pyscal_rdf-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-04 10:44:37.000000 pyscal_rdf-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:44:37.353072 pyscal_rdf-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-04 10:44:35.000000 pyscal_rdf-0.2.3/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:14:49.499513 pyscal_rdf-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-05 09:14:49.495513 pyscal_rdf-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:14:49.491513 pyscal_rdf-0.2.5/pyscal_rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:14:49.495513 pyscal_rdf-0.2.5/pyscal_rdf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/data/asmo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/data/cmso.owl
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/data/element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/data/pldo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/data/podo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18815 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/json_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:14:49.495513 pyscal_rdf-0.2.5/pyscal_rdf/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/network/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/network/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/network/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28790 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/pyscal_rdf/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:14:49.495513 pyscal_rdf-0.2.5/pyscal_rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-05 09:14:49.000000 pyscal_rdf-0.2.5/pyscal_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-05 09:14:49.000000 pyscal_rdf-0.2.5/pyscal_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:14:49.000000 pyscal_rdf-0.2.5/pyscal_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:14:49.000000 pyscal_rdf-0.2.5/pyscal_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 09:14:49.000000 pyscal_rdf-0.2.5/pyscal_rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 09:14:49.000000 pyscal_rdf-0.2.5/pyscal_rdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:14:49.499513 pyscal_rdf-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-05 09:14:49.000000 pyscal_rdf-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:14:49.495513 pyscal_rdf-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-05 09:14:44.000000 pyscal_rdf-0.2.5/tests/test_structuregraph.py
```

### Comparing `pyscal_rdf-0.2.3/LICENSE` & `pyscal_rdf-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/PKG-INFO` & `pyscal_rdf-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pyscal_rdf
-Version: 0.2.3
+Version: 0.2.5
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ase
 Requires-Dist: rdflib
 Requires-Dist: pyyaml
 Requires-Dist: graphviz
 Requires-Dist: networkx
-Requires-Dist: ipycytoscape
 Requires-Dist: pyscal3
 Requires-Dist: spglib
 Requires-Dist: pandas
 Requires-Dist: owlready2
 
 # pyscal_rdf
```

### Comparing `pyscal_rdf-0.2.3/README.md` & `pyscal_rdf-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/data/asmo.owl` & `pyscal_rdf-0.2.5/pyscal_rdf/data/asmo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/data/cmso.owl` & `pyscal_rdf-0.2.5/pyscal_rdf/data/cmso.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/data/element.yml` & `pyscal_rdf-0.2.5/pyscal_rdf/data/element.yml`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/data/pldo.owl` & `pyscal_rdf-0.2.5/pyscal_rdf/data/pldo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/data/podo.owl` & `pyscal_rdf-0.2.5/pyscal_rdf/data/podo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/graph.py` & `pyscal_rdf-0.2.5/pyscal_rdf/graph.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/json_io.py` & `pyscal_rdf-0.2.5/pyscal_rdf/json_io.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/network/network.py` & `pyscal_rdf-0.2.5/pyscal_rdf/network/network.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/network/ontology.py` & `pyscal_rdf-0.2.5/pyscal_rdf/network/ontology.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/network/parser.py` & `pyscal_rdf-0.2.5/pyscal_rdf/network/parser.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/network/patch.py` & `pyscal_rdf-0.2.5/pyscal_rdf/network/patch.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/network/term.py` & `pyscal_rdf-0.2.5/pyscal_rdf/network/term.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/properties.py` & `pyscal_rdf-0.2.5/pyscal_rdf/properties.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/structure.py` & `pyscal_rdf-0.2.5/pyscal_rdf/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,43 @@
 
             for e, r in composition.items():
                 if e in element_indetifiers.keys():
                     element = URIRef(element_indetifiers[e])
                     self.graph.add((chemical_species, CMSO.hasElement, element))
                     self.graph.add((element, RDF.type, CMSO.Element))
                     self.graph.add((element, CMSO.hasSymbol, Literal(e, datatype=XSD.string)))
-                    self.graph.add((element, CMSO.hasElementRatio, Literal(r, datatype=XSD.float)))        
+                    self.graph.add((element, CMSO.hasElementRatio, Literal(r, datatype=XSD.float)))
+
+            #we also have to read in file and clean it up
+            filepath = self.graph.graph.value(URIRef(f'{self.sample}_Position'), CMSO.hasPath).toPython()
+            position_identifier = self.graph.graph.value(URIRef(f'{self.sample}_Position'), CMSO.hasIdentifier).toPython()
+            species_identifier = self.graph.graph.value(URIRef(f'{self.sample}_Species'), CMSO.hasIdentifier).toPython()
+
+            #open the file for reading
+            with open(filepath, 'r') as fin:
+                data = json.load(fin)
+                positions = data[position_identifier]['value']
+                species = data[species_identifier]['value']
+
+            #clean up items
+            positions = [pos for count, pos in enumerate(positions) if count not in delete_ids]
+            species = [pos for count, pos in enumerate(species) if count not in delete_ids]
+
+            datadict = {
+                position_identifier:{
+                    "value": positions,
+                    "label": "position", 
+                },
+                species_identifier:{
+                    "value": species,
+                    "label": "species", 
+                },
+            }
+            outfile = os.path.join(self.graph.structure_store, str(self._name).split(':')[-1])
+            json_io.write_file(outfile,  datadict)
 
 
     def __delitem__(self, val):
         if isinstance(val, int):
             val = [val]
         #now the graph has to be updated accordingly
         self.delete(indices=list(val))
```

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/visualize.py` & `pyscal_rdf-0.2.5/pyscal_rdf/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import graphviz
 import os
 from rdflib import BNode, URIRef, Literal, Namespace
 import uuid
 import json
-import ipycytoscape
 
 
 def get_title_from_BNode(x):
     return x.toPython()
 
 def get_string_from_URI(x):
     """
```

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf/workflow.py` & `pyscal_rdf-0.2.5/pyscal_rdf/workflow.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf.egg-info/PKG-INFO` & `pyscal_rdf-0.2.5/pyscal_rdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pyscal_rdf
-Version: 0.2.3
+Version: 0.2.5
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/pyscal_rdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ase
 Requires-Dist: rdflib
 Requires-Dist: pyyaml
 Requires-Dist: graphviz
 Requires-Dist: networkx
-Requires-Dist: ipycytoscape
 Requires-Dist: pyscal3
 Requires-Dist: spglib
 Requires-Dist: pandas
 Requires-Dist: owlready2
 
 # pyscal_rdf
```

### Comparing `pyscal_rdf-0.2.3/pyscal_rdf.egg-info/SOURCES.txt` & `pyscal_rdf-0.2.5/pyscal_rdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/setup.py` & `pyscal_rdf-0.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='pyscal_rdf',
-    version='0.2.3',
+    version='0.2.5',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['pyscal_rdf', 'pyscal_rdf.*']),
     zip_safe=False,
     download_url = 'https://github.com/pyscal/pyscal_rdf',
     url = 'https://pyscal.org',
     install_requires=['numpy', 'ase', 'rdflib', 
     'pyyaml', 'graphviz', 'networkx', 
-    'ipycytoscape', 'pyscal3', 'spglib', 'pandas', 'owlready2'],
+    'pyscal3', 'spglib', 'pandas', 'owlready2'],
     classifiers=[
         'Programming Language :: Python :: 3'
     ],
     include_package_data=True,
 )
```

### Comparing `pyscal_rdf-0.2.3/tests/test_encoder_and_write.py` & `pyscal_rdf-0.2.5/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/tests/test_graph.py` & `pyscal_rdf-0.2.5/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.2.3/tests/test_structuregraph.py` & `pyscal_rdf-0.2.5/tests/test_structuregraph.py`

 * *Files identical despite different names*

