# Comparing `tmp/gasm-1.1.5.tar.gz` & `tmp/gasm-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gasm-1.1.5.tar", last modified: Sun Mar 31 22:41:30 2024, max compression
+gzip compressed data, was "gasm-1.1.6.tar", last modified: Fri Apr  5 21:10:44 2024, max compression
```

## Comparing `gasm-1.1.5.tar` & `gasm-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 goppert  (44650) under       (21)        0 2024-03-31 22:41:30.502818 gasm-1.1.5/
--rw-------   0 goppert  (44650) under       (21)     1072 2024-03-21 04:26:15.000000 gasm-1.1.5/LICENSE
--rw-r--r--   0 goppert  (44650) under       (21)     6092 2024-03-31 22:41:30.487820 gasm-1.1.5/PKG-INFO
--rw-------   0 goppert  (44650) under       (21)     4497 2024-03-31 05:34:29.000000 gasm-1.1.5/README.md
--rw-------   0 goppert  (44650) under       (21)      525 2024-03-31 22:41:20.000000 gasm-1.1.5/pyproject.toml
--rw-------   0 goppert  (44650) under       (21)       38 2024-03-31 22:41:30.503821 gasm-1.1.5/setup.cfg
-drwx------   0 goppert  (44650) under       (21)        0 2024-03-31 22:41:30.374817 gasm-1.1.5/src/
--rw-------   0 goppert  (44650) under       (21)        0 2024-03-21 04:22:58.000000 gasm-1.1.5/src/__init__.py
--rw-------   0 goppert  (44650) under       (21)     4708 2024-03-31 16:38:30.000000 gasm-1.1.5/src/dasm.py
-drwx------   0 goppert  (44650) under       (21)        0 2024-03-31 22:41:30.472818 gasm-1.1.5/src/gasm.egg-info/
--rw-r--r--   0 goppert  (44650) under       (21)     6092 2024-03-31 22:41:30.000000 gasm-1.1.5/src/gasm.egg-info/PKG-INFO
--rw-------   0 goppert  (44650) under       (21)      235 2024-03-31 22:41:30.000000 gasm-1.1.5/src/gasm.egg-info/SOURCES.txt
--rw-------   0 goppert  (44650) under       (21)        1 2024-03-31 22:41:30.000000 gasm-1.1.5/src/gasm.egg-info/dependency_links.txt
--rw-------   0 goppert  (44650) under       (21)       52 2024-03-31 22:41:30.000000 gasm-1.1.5/src/gasm.egg-info/entry_points.txt
--rw-------   0 goppert  (44650) under       (21)       19 2024-03-31 22:41:30.000000 gasm-1.1.5/src/gasm.egg-info/top_level.txt
--rw-------   0 goppert  (44650) under       (21)     7742 2024-03-31 22:39:00.000000 gasm-1.1.5/src/gasm.py
+drwx------   0 goppert  (44650) under       (21)        0 2024-04-05 21:10:44.289517 gasm-1.1.6/
+-rw-------   0 goppert  (44650) under       (21)     1072 2024-03-21 04:26:15.000000 gasm-1.1.6/LICENSE
+-rw-r--r--   0 goppert  (44650) under       (21)     6092 2024-04-05 21:10:44.278493 gasm-1.1.6/PKG-INFO
+-rw-------   0 goppert  (44650) under       (21)     4497 2024-03-31 05:34:29.000000 gasm-1.1.6/README.md
+-rw-------   0 goppert  (44650) under       (21)      525 2024-04-05 21:10:26.000000 gasm-1.1.6/pyproject.toml
+-rw-------   0 goppert  (44650) under       (21)       38 2024-04-05 21:10:44.290514 gasm-1.1.6/setup.cfg
+drwx------   0 goppert  (44650) under       (21)        0 2024-04-05 21:10:44.190505 gasm-1.1.6/src/
+-rw-------   0 goppert  (44650) under       (21)        0 2024-03-21 04:22:58.000000 gasm-1.1.6/src/__init__.py
+-rw-------   0 goppert  (44650) under       (21)     4708 2024-03-31 16:38:30.000000 gasm-1.1.6/src/dasm.py
+drwx------   0 goppert  (44650) under       (21)        0 2024-04-05 21:10:44.265507 gasm-1.1.6/src/gasm.egg-info/
+-rw-r--r--   0 goppert  (44650) under       (21)     6092 2024-04-05 21:10:44.000000 gasm-1.1.6/src/gasm.egg-info/PKG-INFO
+-rw-------   0 goppert  (44650) under       (21)      235 2024-04-05 21:10:44.000000 gasm-1.1.6/src/gasm.egg-info/SOURCES.txt
+-rw-------   0 goppert  (44650) under       (21)        1 2024-04-05 21:10:44.000000 gasm-1.1.6/src/gasm.egg-info/dependency_links.txt
+-rw-------   0 goppert  (44650) under       (21)       52 2024-04-05 21:10:44.000000 gasm-1.1.6/src/gasm.egg-info/entry_points.txt
+-rw-------   0 goppert  (44650) under       (21)       19 2024-04-05 21:10:44.000000 gasm-1.1.6/src/gasm.egg-info/top_level.txt
+-rw-------   0 goppert  (44650) under       (21)     7737 2024-04-05 21:10:05.000000 gasm-1.1.6/src/gasm.py
```

### Comparing `gasm-1.1.5/LICENSE` & `gasm-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gasm-1.1.5/PKG-INFO` & `gasm-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasm
-Version: 1.1.5
+Version: 1.1.6
 Summary: An assembler/dissassembler for the Gheith ISA
 Author-email: Michael Goppert <goppert@cs.utexas.edu>
 License: MIT License
         
         Copyright (c) 2024 Michael Goppert
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gasm-1.1.5/README.md` & `gasm-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gasm-1.1.5/pyproject.toml` & `gasm-1.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gasm"
-version = "1.1.5"
+version = "1.1.6"
 requires-python = ">=3.8"
 authors = [
      { name="Michael Goppert", email="goppert@cs.utexas.edu"},
 ]
 description = "An assembler/dissassembler for the Gheith ISA"
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `gasm-1.1.5/src/dasm.py` & `gasm-1.1.6/src/dasm.py`

 * *Files identical despite different names*

### Comparing `gasm-1.1.5/src/gasm.egg-info/PKG-INFO` & `gasm-1.1.6/src/gasm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasm
-Version: 1.1.5
+Version: 1.1.6
 Summary: An assembler/dissassembler for the Gheith ISA
 Author-email: Michael Goppert <goppert@cs.utexas.edu>
 License: MIT License
         
         Copyright (c) 2024 Michael Goppert
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gasm-1.1.5/src/gasm.py` & `gasm-1.1.6/src/gasm.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     source = sys.argv[1]
 
     if (len(sys.argv) > 2):
         dest = sys.argv[2]
     else:
         # version command
         if sys.argv[1] in ['-v', '-V', '--version']:
-            print('gasm by Michael Goppert\n1.1.4')
+            print('gasm by Michael Goppert\n1.1.6')
             exit(0)
 
         # deduce dest
         path = source.split('/')
         source_name = os.path.splitext(path[len(path) - 1])[0]
         dest = f'{source_name}.hex'
 
@@ -37,45 +37,30 @@
                 if line_is_label:
                     label, _ = line.split(':')
                     if label.lower() in ['end', 'sub', 'movl', 'movh', 'jz', 'jnz', 'js', 'jns', 'ld', 'st']:
                         print(f'INVALID LABEL ({label}) AT LINE {len(resolved_lines)}')
                         exit(1)
                     mem_word_loc = (len(resolved_lines) - ignored_lines + offset_lines) * 2
                     mem_loc = mem_word_loc + 1 if label.startswith('!mis_') else mem_word_loc
-                    if not label.startswith('!mis_'):
-                        resolved_lines.append(f'// [PC: {hex(mem_loc)}] <{label}>:')
-                        ignored_lines += 1
+                    #if not label.startswith('!mis_'):
+                    resolved_lines.append(f'// [PC: {hex(mem_loc)}] <{label}>:')
+                    ignored_lines += 1
                     labels[label] =  mem_loc
                 else:
                     if (not line) or line.strip().startswith('//') or line.strip().startswith('@'):
                         ignored_lines += 1
                     if '@END MISALIGNED' in line:
                         offset_lines += 1
                     resolved_lines.append(line)
 
             # update lines
             lines = resolved_lines
 
             # assemble
             for line_num, line in enumerate(lines):
-                # print data
-                if in_data_block:
-                    o.write(f'{line}\n')
-                    continue
-
-                # empty line
-                if not line.strip():
-                    if not in_mis_block:
-                        o.write('\n')
-                    continue
-
-                # mem directive
-                if line.startswith('@'):
-                    o.write(f'{line}\n')
-                    continue
 
                 # comment
                 comment = ''
                 if line.strip().startswith('//'):
                     if '@BEGIN' in line or '@END' in line:
                         if 'DATA' in line:
                             in_data_block = not in_data_block
@@ -84,25 +69,42 @@
                             mis_block_ins += 'ff'
 
                             # print result if no longer in block
                             if not in_mis_block:
                                 for i in range(int(len(mis_block_ins) / 4)):
                                     o.write(f'{mis_block_ins[i * 4 : i * 4 + 4][::-1]}\n')
                                 mis_block_ins = ''
+
                         o.write(f'{line}\n')
                     elif (line.startswith(' ' or line.startswith('\t'))):
                         o.write(f'        {line.strip()}\n')
                     else:
                         o.write(f'{line}\n')
                     continue
                 elif '//' in line:
                     comment_index = line.index('//')
                     comment = line[comment_index:]
                     line = line[:comment_index].strip()
 
+                # print data
+                if in_data_block:
+                    o.write(f'{line}\n')
+                    continue
+
+                # empty line
+                if not line.strip():
+                    if not in_mis_block:
+                        o.write('\n')
+                    continue
+
+                # mem directive
+                if line.startswith('@'):
+                    o.write(f'{line}\n')
+                    continue
+
                 # remove extra symbols
                 line = line.replace(',', '')
 
                 # filter out whitespace
                 u_comps = line.split(' ')
                 comps = list(filter(lambda c: c != '' and c != ' ' and c != '\t', u_comps))
```

