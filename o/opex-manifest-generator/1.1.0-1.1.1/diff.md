# Comparing `tmp/opex_manifest_generator-1.1.0.tar.gz` & `tmp/opex_manifest_generator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opex_manifest_generator-1.1.0.tar", last modified: Thu Apr  4 10:05:15 2024, max compression
+gzip compressed data, was "opex_manifest_generator-1.1.1.tar", last modified: Fri Apr  5 13:57:01 2024, max compression
```

## Comparing `opex_manifest_generator-1.1.0.tar` & `opex_manifest_generator-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:05:15.988477 opex_manifest_generator-1.1.0/
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.0/LICENSE.md
--rw-rw-rw-   0        0        0      701 2024-04-04 10:05:15.985465 opex_manifest_generator-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    19695 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 10:05:15.933873 opex_manifest_generator-1.1.0/opex_manifest_generator/
--rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/__init__.py
--rw-rw-rw-   0        0        0     6190 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/cli.py
--rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/common.py
--rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/hash.py
--rw-rw-rw-   0        0        0    23661 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/opex_manifest.py
--rw-rw-rw-   0        0        0    20008 2024-03-26 21:35:58.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/opex_manifest_v1.py
--rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/test_cli.py
--rw-rw-rw-   0        0        0       21 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.0/opex_manifest_generator/version.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:05:15.974175 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-04 10:05:15.000000 opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      819 2024-04-04 10:00:33.000000 opex_manifest_generator-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 10:05:15.989475 opex_manifest_generator-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.642300 opex_manifest_generator-1.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      701 2024-04-05 13:57:01.642300 opex_manifest_generator-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    19695 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.595410 opex_manifest_generator-1.1.1/opex_manifest_generator/
+-rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/__init__.py
+-rw-rw-rw-   0        0        0     6190 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/cli.py
+-rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/common.py
+-rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/hash.py
+-rw-rw-rw-   0        0        0    25427 2024-04-05 13:55:47.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/opex_manifest.py
+-rw-rw-rw-   0        0        0    20008 2024-03-26 21:35:58.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/opex_manifest_reference.py
+-rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/test_cli.py
+-rw-rw-rw-   0        0        0       21 2024-04-05 08:23:42.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/version.py
+drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.642300 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      819 2024-04-05 08:25:10.000000 opex_manifest_generator-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 13:57:01.642300 opex_manifest_generator-1.1.1/setup.cfg
```

### Comparing `opex_manifest_generator-1.1.0/LICENSE.md` & `opex_manifest_generator-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.0/PKG-INFO` & `opex_manifest_generator-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.0/README.md` & `opex_manifest_generator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.0/opex_manifest_generator/cli.py` & `opex_manifest_generator-1.1.1/opex_manifest_generator/cli.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.0/opex_manifest_generator/common.py` & `opex_manifest_generator-1.1.1/opex_manifest_generator/common.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.0/opex_manifest_generator/hash.py` & `opex_manifest_generator-1.1.1/opex_manifest_generator/hash.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.0/opex_manifest_generator/opex_manifest.py` & `opex_manifest_generator-1.1.1/opex_manifest_generator/opex_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         self.acc_prefix = acc_prefix
         self.input = input
         self.title_flag = False
         self.description_flag = False
         self.security_flag = False
         self.ignore_flag = False
         self.sourceid_flag = False
+        self.hash_from_spread = False        
         self.hidden_flag = hidden_flag
         self.zip_flag = zip_flag
         self.output_format = output_format
         self.metadata_flag = metadata_flag
         self.metadata_dir = metadata_dir
         
     def print_running_time(self):
@@ -109,15 +110,15 @@
             elif bool(remove):
                 print(f"Removing: {file_path}")
                 # Not functioning correctly
                 if os.path.isdir(file_path): shutil.rmtree(dir)
                 else: os.remove(file_path)
                 return True
             else: return False
-    
+                
     def ignore_df_lookup(self,file_path: str):
         idx = self.df.index[self.df['FullName'] == file_path]
         if idx.empty: return False
         else: ignore = self.df['Ignore'].loc[idx].item()
         if str(ignore).lower() in {"nan","nat"}: return False
         elif str(ignore).lower() in {"true"}: return True
         else: return False
@@ -128,14 +129,27 @@
         else:
             sourceid = self.df['SourceID'].loc[idx].item()
             if str(sourceid) in {"nan","nat"}: pass
             else:
                 source_xml = ET.SubElement(xml_element,f"{{{self.opexns}}}SourceID")
                 source_xml.text = str(sourceid)
 
+    def hash_df_lookup(self,file_path,xml_fixities):
+        idx = self.df.index[self.df['FullName'] == file_path]
+        if idx.empty: pass
+        else:
+            if "Hash" in self.column_headers and "Algorithm" in self.column_headers:
+                self.fixity = ET.SubElement(xml_fixities,f"{{{self.opexns}}}Fixity")        
+                self.hash = self.df["Hash"].loc[idx].item()
+                self.algorithm = self.df["Algorithm"].loc[idx].item()
+                self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
+                self.fixity.set("type", self.algorithm)
+                self.fixity.set("value",self.hash)
+            else: pass
+
     def ident_df_lookup(self,file_path):
         idx = self.df.index[self.df['FullName'] == file_path]
         if idx.empty:
             ident = "ERROR"
             self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
             self.identifier.set("type","code")
             self.identifier.text = ident
@@ -193,23 +207,39 @@
     def clear_opex(self):
         walk = list(os.walk(self.root))
         for dir,_,files in walk[::-1]:
             for file in files:
                 file_path = win_256_check(os.path.join(dir,file))   
                 if str(file_path).endswith('.opex'):
                     os.remove(file_path)
-                    print(f'Cleared Opex: {file_path}') #fileprint(os.path.join(d,sd,f))
+                    print(f'Cleared Opex: {file_path}')
     
     def set_flags(self):
         if 'Title' in self.df: self.title_flag = True
         if 'Description' in self.df: self.description_flag = True
         if 'Security' in self.df: self.security_flag = True
         if 'SourceID' in self.df: self.sourceid_flag = True
         if 'Ignore' in self.df: self.ignore_flag = True
-        
+        if 'Hash' in self.df and 'Algorithm' in self.df:
+            self.hash_from_spread = True
+            print("Hash detected in Spreadsheet; taking hashes from spreadsheet");time.sleep(3)
+
+    def print_descriptive_xmls(self):
+        for file in os.listdir(self.metadata_dir):
+            path = os.path.join(self.metadata_dir,file)
+            print(path)
+            xml_file = ET.parse(path)
+            root_element = ET.QName(xml_file.find('.'))
+            root_element_ln = root_element.localname
+            for elem in xml_file.findall(".//"):
+                elem_path = xml_file.getelementpath(elem)
+                elem = ET.QName(elem)
+                elem_lnpath = elem_path.replace(f"{{{elem.namespace}}}",root_element_ln + ":")
+                print(elem_lnpath)
+
     def init_generate_descriptive_metadata(self):
         self.xml_files = []
         for file in os.listdir(self.metadata_dir):
             if file.endswith('xml'):
                 """
                 Generates info on the elements of the XML Files placed in the Metadata directory.
                 Composed as a list of dictionaries.
@@ -298,23 +328,25 @@
         if security:
             self.securityxml = ET.SubElement(self.properties,f"{{{self.opexns}}}SecurityDescriptor")
             self.securityxml.text = str(security)
         if self.autoclass_flag in {"generic","g"}:
             self.properties.remove(self.identifiers)
         elif self.autoclass_flag or self.input:
             self.ident_df_lookup(file_path)
+        if self.identifiers is None: self.properties.remove(self.identifiers)
+        if self.properties is None: xmlroot.remove(self.properties)
 
 
-    def genererate_opex_fixity(self):
+    def genererate_opex_fixity(self,file_path):
         self.fixity = ET.SubElement(self.fixities,f"{{{self.opexns}}}Fixity")        
-        self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(self.file_path) # Double Check...
+        self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
         self.fixity.set("type", self.algorithm)
         self.fixity.set("value",self.hash)
-        self.OMG.list_fixity.append([self.algorithm,self.hash,self.file_path])
-        self.OMG.list_path.append(self.file_path)        
+        self.OMG.list_fixity.append([self.algorithm,self.hash,file_path])
+        self.OMG.list_path.append(file_path)
 
     def main(self):
         print(f"Start time: {self.start_time}")        
         if self.clear_opex_flag:
             self.clear_opex()
             if self.autoclass_flag or self.algorithm or self.input: pass
             else: 
@@ -431,15 +463,16 @@
             self.xmlroot = ET.Element(f"{{{self.opexns}}}OPEXMetadata",nsmap={"opex":self.opexns})
             if self.OMG.algorithm or self.OMG.sourceid_flag:
                 self.transfer = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}Transfer")
                 if self.OMG.sourceid_flag:
                     self.OMG.sourceid_df_lookup(self.transfer,self.file_path)
                 if self.OMG.algorithm:
                     self.fixities = ET.SubElement(self.transfer,f"{{{self.opexns}}}Fixities")
-                    self.genererate_opex_fixity()            
+                    if self.OMG.hash_from_spread: self.OMG.hash_df_lookup(self.file_path,self.fixities)  
+                    else: self.genererate_opex_fixity(self.file_path)            
             if self.OMG.autoclass_flag or self.OMG.input:
                 if self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag: self.title,self.description,self.security = self.OMG.meta_df_lookup(file_path) 
                 self.OMG.generate_opex_properties(self.xmlroot,self.file_path,title=self.title,description=self.description,security=self.security)
                 if not self.OMG.metadata_flag in {'none','n'}:
                     self.xml_descmeta = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}DescriptiveMetadata")
                     self.OMG.generate_descriptive_metadata(self.xml_descmeta,self.file_path)
             opex_path = self.OMG.write_opex(self.file_path,self.xmlroot)
```

### Comparing `opex_manifest_generator-1.1.0/opex_manifest_generator/opex_manifest_v1.py` & `opex_manifest_generator-1.1.1/opex_manifest_generator/opex_manifest_reference.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/PKG-INFO` & `opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.0/opex_manifest_generator.egg-info/SOURCES.txt` & `opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 README.md
 pyproject.toml
 opex_manifest_generator/__init__.py
 opex_manifest_generator/cli.py
 opex_manifest_generator/common.py
 opex_manifest_generator/hash.py
 opex_manifest_generator/opex_manifest.py
-opex_manifest_generator/opex_manifest_v1.py
+opex_manifest_generator/opex_manifest_reference.py
 opex_manifest_generator/test_cli.py
 opex_manifest_generator/version.py
 opex_manifest_generator.egg-info/PKG-INFO
 opex_manifest_generator.egg-info/SOURCES.txt
 opex_manifest_generator.egg-info/dependency_links.txt
 opex_manifest_generator.egg-info/entry_points.txt
 opex_manifest_generator.egg-info/requires.txt
```

### Comparing `opex_manifest_generator-1.1.0/pyproject.toml` & `opex_manifest_generator-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 226f 7065 785f 6d61  .name = "opex_ma
 00000070: 6e69 6665 7374 5f67 656e 6572 6174 6f72  nifest_generator
 00000080: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000090: 312e 3022 0d0a 6175 7468 6f72 7320 3d20  1.0"..authors = 
+00000090: 312e 3122 0d0a 6175 7468 6f72 7320 3d20  1.1"..authors = 
 000000a0: 5b0d 0a20 2020 207b 6e61 6d65 3d22 4368  [..    {name="Ch
 000000b0: 7269 7374 6f70 6865 7220 5072 696e 6365  ristopher Prince
 000000c0: 222c 2065 6d61 696c 3d22 632e 706a 2e70  ", email="c.pj.p
 000000d0: 7269 6e63 6540 676d 6169 6c2e 636f 6d22  rince@gmail.com"
 000000e0: 7d0d 0a20 2020 205d 0d0a 6465 7363 7269  }..    ]..descri
 000000f0: 7074 696f 6e20 3d20 224f 7065 7820 4d61  ption = "Opex Ma
 00000100: 6e69 6665 7374 2047 656e 6572 6174 6f72  nifest Generator
```

