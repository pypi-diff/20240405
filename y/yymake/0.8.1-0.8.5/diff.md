# Comparing `tmp/yymake-0.8.1.tar.gz` & `tmp/yymake-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yymake-0.8.1.tar", last modified: Sun Jan 21 13:55:30 2024, max compression
+gzip compressed data, was "yymake-0.8.5.tar", last modified: Fri Apr  5 02:29:16 2024, max compression
```

## Comparing `yymake-0.8.1.tar` & `yymake-0.8.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-01-21 13:55:30.641680 yymake-0.8.1/
--rw-r--r--   0 evil       (501) staff       (20)     1067 2023-09-22 13:25:57.000000 yymake-0.8.1/LICENSE
--rw-r--r--   0 evil       (501) staff       (20)      886 2024-01-21 13:55:30.641180 yymake-0.8.1/PKG-INFO
--rw-r--r--   0 evil       (501) staff       (20)      279 2023-10-10 14:20:53.000000 yymake-0.8.1/README.md
--rw-r--r--   0 evil       (501) staff       (20)       38 2024-01-21 13:55:30.641789 yymake-0.8.1/setup.cfg
--rw-r--r--   0 evil       (501) staff       (20)     1112 2024-01-21 13:54:59.000000 yymake-0.8.1/setup.py
-drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-01-21 13:55:30.634132 yymake-0.8.1/ymake/
--rw-r--r--   0 evil       (501) staff       (20)        0 2023-09-29 15:05:14.000000 yymake-0.8.1/ymake/__init__.py
--rw-r--r--   0 evil       (501) staff       (20)     3069 2023-11-04 13:14:41.000000 yymake-0.8.1/ymake/automake.py
--rw-r--r--   0 evil       (501) staff       (20)    16827 2024-01-21 13:55:17.000000 yymake-0.8.1/ymake/builder.py
--rw-r--r--   0 evil       (501) staff       (20)      830 2023-09-29 15:57:02.000000 yymake-0.8.1/ymake/cmake.py
--rw-r--r--   0 evil       (501) staff       (20)     1091 2023-10-08 14:34:08.000000 yymake-0.8.1/ymake/detect.py
--rw-r--r--   0 evil       (501) staff       (20)    19464 2024-01-21 13:53:21.000000 yymake-0.8.1/ymake/function.py
--rw-r--r--   0 evil       (501) staff       (20)      333 2023-11-04 13:27:31.000000 yymake-0.8.1/ymake/globa.py
--rw-r--r--   0 evil       (501) staff       (20)     2151 2024-01-21 12:58:43.000000 yymake-0.8.1/ymake/graph.py
--rw-r--r--   0 evil       (501) staff       (20)     1057 2023-09-24 16:51:29.000000 yymake-0.8.1/ymake/log.py
--rw-r--r--   0 evil       (501) staff       (20)     8076 2024-01-21 12:39:16.000000 yymake-0.8.1/ymake/node.py
--rw-r--r--   0 evil       (501) staff       (20)     3575 2023-11-04 07:58:55.000000 yymake-0.8.1/ymake/op.py
--rw-r--r--   0 evil       (501) staff       (20)      400 2023-09-29 15:56:48.000000 yymake-0.8.1/ymake/toolchain.py
--rw-r--r--   0 evil       (501) staff       (20)      336 2023-09-29 15:19:38.000000 yymake-0.8.1/ymake/version.py
--rw-r--r--   0 evil       (501) staff       (20)    10782 2024-01-21 12:58:43.000000 yymake-0.8.1/ymake/yaya.py
-drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-01-21 13:55:30.640442 yymake-0.8.1/ymake/yymake.egg-info/
--rw-r--r--   0 evil       (501) staff       (20)      886 2024-01-21 13:55:30.000000 yymake-0.8.1/ymake/yymake.egg-info/PKG-INFO
--rw-r--r--   0 evil       (501) staff       (20)      465 2024-01-21 13:55:30.000000 yymake-0.8.1/ymake/yymake.egg-info/SOURCES.txt
--rw-r--r--   0 evil       (501) staff       (20)        1 2024-01-21 13:55:30.000000 yymake-0.8.1/ymake/yymake.egg-info/dependency_links.txt
--rw-r--r--   0 evil       (501) staff       (20)       99 2024-01-21 13:55:30.000000 yymake-0.8.1/ymake/yymake.egg-info/entry_points.txt
--rw-r--r--   0 evil       (501) staff       (20)       44 2024-01-21 13:55:30.000000 yymake-0.8.1/ymake/yymake.egg-info/requires.txt
--rw-r--r--   0 evil       (501) staff       (20)        1 2024-01-21 13:55:30.000000 yymake-0.8.1/ymake/yymake.egg-info/top_level.txt
+drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-04-05 02:29:16.185274 yymake-0.8.5/
+-rw-r--r--   0 evil       (501) staff       (20)     1067 2023-09-22 13:25:57.000000 yymake-0.8.5/LICENSE
+-rw-r--r--   0 evil       (501) staff       (20)      886 2024-04-05 02:29:16.184400 yymake-0.8.5/PKG-INFO
+-rw-r--r--   0 evil       (501) staff       (20)      279 2023-10-10 14:20:53.000000 yymake-0.8.5/README.md
+-rw-r--r--   0 evil       (501) staff       (20)       38 2024-04-05 02:29:16.185440 yymake-0.8.5/setup.cfg
+-rw-r--r--   0 evil       (501) staff       (20)     1112 2024-03-31 02:31:09.000000 yymake-0.8.5/setup.py
+drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-04-05 02:29:16.175643 yymake-0.8.5/ymake/
+-rw-r--r--   0 evil       (501) staff       (20)        0 2023-09-29 15:05:14.000000 yymake-0.8.5/ymake/__init__.py
+-rw-r--r--   0 evil       (501) staff       (20)     3186 2024-03-24 17:42:02.000000 yymake-0.8.5/ymake/automake.py
+-rw-r--r--   0 evil       (501) staff       (20)    17474 2024-03-25 14:05:53.000000 yymake-0.8.5/ymake/builder.py
+-rw-r--r--   0 evil       (501) staff       (20)      830 2023-09-29 15:57:02.000000 yymake-0.8.5/ymake/cmake.py
+-rw-r--r--   0 evil       (501) staff       (20)     1091 2023-10-08 14:34:08.000000 yymake-0.8.5/ymake/detect.py
+-rw-r--r--   0 evil       (501) staff       (20)    19584 2024-03-30 06:14:38.000000 yymake-0.8.5/ymake/function.py
+-rw-r--r--   0 evil       (501) staff       (20)      333 2023-11-04 13:27:31.000000 yymake-0.8.5/ymake/globa.py
+-rw-r--r--   0 evil       (501) staff       (20)     2615 2024-04-05 01:54:59.000000 yymake-0.8.5/ymake/graph.py
+-rw-r--r--   0 evil       (501) staff       (20)     1057 2023-09-24 16:51:29.000000 yymake-0.8.5/ymake/log.py
+-rw-r--r--   0 evil       (501) staff       (20)     8083 2024-03-31 02:30:02.000000 yymake-0.8.5/ymake/node.py
+-rw-r--r--   0 evil       (501) staff       (20)     3575 2023-11-04 07:58:55.000000 yymake-0.8.5/ymake/op.py
+-rw-r--r--   0 evil       (501) staff       (20)      400 2023-09-29 15:56:48.000000 yymake-0.8.5/ymake/toolchain.py
+-rw-r--r--   0 evil       (501) staff       (20)      336 2023-09-29 15:19:38.000000 yymake-0.8.5/ymake/version.py
+-rw-r--r--   0 evil       (501) staff       (20)    10868 2024-03-13 14:18:51.000000 yymake-0.8.5/ymake/yaya.py
+drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-04-05 02:29:16.183199 yymake-0.8.5/ymake/yymake.egg-info/
+-rw-r--r--   0 evil       (501) staff       (20)      886 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/PKG-INFO
+-rw-r--r--   0 evil       (501) staff       (20)      465 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/SOURCES.txt
+-rw-r--r--   0 evil       (501) staff       (20)        1 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/dependency_links.txt
+-rw-r--r--   0 evil       (501) staff       (20)       99 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/entry_points.txt
+-rw-r--r--   0 evil       (501) staff       (20)       44 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/requires.txt
+-rw-r--r--   0 evil       (501) staff       (20)        1 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/top_level.txt
```

### Comparing `yymake-0.8.1/LICENSE` & `yymake-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yymake-0.8.1/PKG-INFO` & `yymake-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yymake
-Version: 0.8.1
+Version: 0.8.5
 Summary: A cross build dsl make tool
 Home-page: https://github.com/evilbinary/ymake
 Author: evilbinary
 Author-email: rootntsd@gmail.com
 Project-URL: Bug Tracker, https://github.com/evilbinary/ymake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yymake-0.8.1/setup.py` & `yymake-0.8.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 import os,sys,re
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="yymake",
-    version="0.8.1",
+    version="0.8.5",
     author="evilbinary",
     author_email="rootntsd@gmail.com",
     description="A cross build dsl make tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/evilbinary/ymake",
     project_urls={
```

### Comparing `yymake-0.8.1/ymake/automake.py` & `yymake-0.8.5/ymake/automake.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,19 @@
     args+=['--prefix='+build_dir_abs]
     try:
         shell(tool.get('configure'),args,cwd=sourcedir)
         
     except Exception as e:
         print('build error',e)
         pass
-
-    shell(tool.get('make'),['install','-j'+str(jobnum)],cwd=sourcedir)
+    try:
+        shell(tool.get('make'),['install','-j'+str(jobnum)],cwd=sourcedir)
+    except Exception as e:
+        shell(tool.get('make'),['-j'+str(jobnum)],cwd=sourcedir)
+        pass
 
     pass
     
 def automake(name=None, **kwargs):
     cur=node_current()
     if name==None:
         name=cur.get('name')
```

### Comparing `yymake-0.8.1/ymake/builder.py` & `yymake-0.8.5/ymake/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,16 +70,17 @@
             n=nodes_get_type_and_name('target',d)
             if n:
                 include=get_includedirs(n)
 
                 n_build_dir=node_get_formated(n,'build-dir')
                 n_build_lib_dir =node_get_formated(n,'build-lib-dir')
                 if not n_build_lib_dir:
-                    tool=node_get_parent(n,'toolchain')
-                    build_prepare(tool,n)
+                    toolchain_name=node_get_parent(n,'toolchain')
+                    toolchain=nodes_get_type_and_name('toolchain',toolchain_name)
+                    build_prepare(toolchain,n)
                     n_build_lib_dir =node_get_formated(n,'build-lib-dir')
 
                 if n_build_lib_dir:
                     include=['-I' + os.path.relpath(os.path.join(n_build_lib_dir,item)) for item in include]
                     include=include + get_include(n)
                     includes+=include
                 else:
@@ -169,16 +170,15 @@
                 if os.path.exists(lib_file):
                     flags+=['-L'+n_build_dir]
                     flags+=['-l'+d]
 
 
 
 
-    log.debug('ldflags no uniq======>{} {}'.format(len(flags),target.get('name')))
-
+    log.debug('ldflags no uniq======>{} {}'.format(len(flags),target.get('name')))    
     flags=list(OrderedDict.fromkeys(flags))
     lib_path_flags = []
     lib_name_flags = []
     flags_rest =[]
     for f in flags:
         if f.startswith('-L'):
             lib_path_flags.append(f)
@@ -301,37 +301,43 @@
         
         build_obj_dir=node_get_formated(target,'build-obj-dir')
 
         match_files=file_match(files,dir_name)
         obj_files=[]
         
         kind=None
-        normal_kind=['c','cc','cxx','cpp','s','h','hpp']
+
+        normal_kind=tool.get('ext')
+        if not normal_kind:
+            normal_kind=['c','cc','cxx','cpp','s','h','hpp','S']
         for f in match_files:
             ext=get_ext(f)
             obj_name=get_object_name(f)
             build_obj=os.path.join(build_obj_dir,obj_name)
             obj_files.append({
                 'obj': build_obj,
                 'src': f
                 })
             if ext not in normal_kind:
                 kind='rule'
+                log.warn('target %s kind set rule, file is %s',target.get('name'),f)
 
         if len(match_files)<=0:
             match_files=file_match(files)            
             for f in match_files:
                 obj_name=get_object_name(f)
                 obj_files.append({
                     'obj': f,
                     'src': f
                     })
                 ext=get_ext(f)
                 if ext not in normal_kind:
                     kind='rule'
+                    log.warn('target %s kind set rule, file is %s',target.get('name'),f)
+
         if kind:
             target.set('kind',kind)
         
         log.debug('{} {} prepare add obj files match {} => {} pwd: {}'.format(target.get('type'),target.get('name') ,files,match_files,os.getcwd() ))
         target['file-objs'].extend(obj_files)
 
 
@@ -408,36 +414,42 @@
     
     for file_obj_dir in file_obj_dirs:
         if file_obj_dir:
             os.makedirs(file_obj_dir,exist_ok=True)
 
     is_modify_target=False
 
-    log.debug('target {} is exist {} {}'.format(target.get('name'),build_target,os.path.exists(build_target)))
+    is_target_exist=os.path.exists(build_target)
 
-    if not os.path.exists(build_target):
+    log.debug('target {} is exist {} {}'.format(target.get('name'),build_target,is_target_exist))
+
+    if not is_target_exist:
         is_modify_target=True
     
     # deps change
     deps= get_dep_order(target)
     for d in deps:
         n=nodes_get_type_and_name('target',d)
         t=get_build_target(n)
         if n.get('kind')=='lib':
             continue
         is_modify=tool.get('is_modify')(t,build_target)
         if is_modify:
             is_modify_target=True
 
 
+    log.debug('target modify objs num %o , modify target %o ',len(modify_file_objs),is_modify_target )
+
     if len(modify_file_objs)<=0 and not is_modify_target:
         call_hook_event(target,'after_link')
         call_hook_event(target,'after_build')
         return
-        
+    
+    log.debug('target %s kind is %s',target.get('name'),target.get('kind'))
+
     includedirs=get_target_include(target)
     log.debug("includedirs {}".format(includedirs))
 
     cflags=get_target_cflags(target)
     log.debug('{} cflags {}'.format(target.get("name"),cflags))
     
     cxxflags=get_target_cxxflags(target)
@@ -460,15 +472,15 @@
         
         obj_name=get_object_name(obj)
 
         log.debug('build_obj=>{} {}'.format(obj,obj_name))
 
         ext=get_ext(obj)
 
-        if src[-2:] in [".c",".s"]:
+        if src[-2:] in [".c",".s",".S"]:
             build_commands.append([obj_name,tool.get("cc"),[src]+cflags+includedirs+['-c','-o',obj] ])
         elif src.endswith(".cpp") or obj_name.endswith(".cc"):
             build_commands.append([obj_name,tool.get("cxx"),[src]+cxxflags+includedirs+['-c','-o',obj] ])
         elif src.endswith(".o"):
             pass
         elif ext=='' or ext=='bin':
             pass
@@ -487,28 +499,27 @@
 
     ldflags=get_target_ldflags(target)
     log.debug('ldflags {}'.format(ldflags))
 
     if len(modify_file_objs)==0 and not is_modify_target:
         log.warn('target {} obj file is 0'.format(target.get('name')))
         return
-
     build_target_commands=[]
     if target.get('kind')=='static':
          build_target_commands.append([build_target,tool.get("ar"),['-r',build_target]+file_objs ])
          process_build(build_target_commands,progress_info,jobnum)
     elif target.get('kind')=='shared':
         flags+=['-shared']
         build_target_commands.append([build_target,tool.get("ld"),file_objs+['-o',build_target]+ ldflags ])
         process_build(build_target_commands,progress_info,jobnum)
     elif target.get('kind')=='binary':
         build_target_commands.append([build_target,tool.get("ld"),file_objs+['-o',build_target]+ ldflags ])
         process_build(build_target_commands,progress_info,jobnum)
     else:
-
+        log.error('target {} kind {} not found'.format(target.get('name'),target.get('kind')))
         pass
     
 
     call_hook_event(target,'after_link')
     call_hook_event(target,'after_build')
 
     # is_modify=tool.get('is_modify')(build_target,build_target)
```

### Comparing `yymake-0.8.1/ymake/cmake.py` & `yymake-0.8.5/ymake/cmake.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.1/ymake/detect.py` & `yymake-0.8.5/ymake/detect.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.1/ymake/function.py` & `yymake-0.8.5/ymake/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,15 @@
 def get_build_dir():
     cur=node_current()
     return node_get_parent(cur,'build-dir')
 
 def get_build_obj_dir():
     cur=node_current()
     build_obj_dir=node_get_parent(cur,'build-obj-dir')
+    build_obj_dir=node_get_formated(cur,'build-obj-dir')
     return build_obj_dir
 
 def add_deps(*deps):
     deps=get_list_args(deps)
     node_extend('deps',deps)
 
 def add_packages(*deps):
@@ -648,15 +649,18 @@
     module_spec = importlib.util.spec_from_file_location(module_name, file)
     module = importlib.util.module_from_spec(module_spec)
 
     # for node
     module.target=target
     module.rule=rule
     module.project=project
+    module.toolchain=toolchain
 
+
+    module.rule_end=target_end
     module.rule_end=rule_end
     module.project_end=project_end
     module.toolchain_end=toolchain_end
 
     module.option=option
     module.option_end=option_end
     module.set_showmenu=set_showmenu
```

### Comparing `yymake-0.8.1/ymake/graph.py` & `yymake-0.8.5/ymake/graph.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # *******************************************************************
 # * Copyright 2023-present evilbinary
 # * 作者: evilbinary on 01/01/20
 # * 邮箱: rootdebug@163.com
 # ********************************************************************
 import networkx as nx
 from node import nodes_get_type_and_name,nodes_get_all_type
+from log import log
 
 def build_graph(project,kind=None):
     graph={}    
     if project.get('type')=='target':
         target=project
         graph[target.get('name')]= target.get('deps')
     else:
@@ -27,20 +28,30 @@
                     if target:
                         graph[target_name]= target.get('deps')
                     else:
                         log.warn('target {} not belong any project'.format(target_name))
     return graph
 
 def build_dep_graph(graph,target,kind=None):
-    deps=target.get('deps')
-    for d in deps:
-        n=nodes_get_type_and_name('target',d)
-        build_dep_graph(graph,n,kind)
-        graph[d]= n.get('deps')
-
+    try:
+        deps=target.get('deps')
+        for d in deps:
+            n=nodes_get_type_and_name('target',d)
+            if not n:
+                log.warn('target %s get deps %s not found',target.get('name'),d)
+                log.warn('target info is %s',target)
+                continue
+            build_dep_graph(graph,n,kind)
+            if n:
+                graph[d]= n.get('deps')
+    except Exception as ex:
+        if target and target.get('name'):
+            log.error('target %s get deps erro ',target.get('name'),ex)
+        else:
+            log.error('target is null get deps erro',ex)
 
 def get_dep_order(target,kind=None,reverse=False):
     project=nodes_get_all_type('project')
     graph={}
     if len(project)>0:
         build_dep_graph(graph,target,kind)
     if graph.get(target.get('name')):
```

### Comparing `yymake-0.8.1/ymake/log.py` & `yymake-0.8.5/ymake/log.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.1/ymake/node.py` & `yymake-0.8.5/ymake/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
         toolchain=nodes_get_type_and_name('toolchain',toolchain_name)
         if toolchain:
             return toolchain.get(tool)
         return None
 
     def get(self,key):
-        if key in['arch_type','arch' ]:
+        if key in['arch_type','arch','plat' ]:
             return node_get_parent(self,key)
         if key in self:
             return self[key]
         return None
 
     def get_arch(self):
         return self.get('arch')
```

### Comparing `yymake-0.8.1/ymake/op.py` & `yymake-0.8.5/ymake/op.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.1/ymake/yaya.py` & `yymake-0.8.5/ymake/yaya.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,14 +363,18 @@
             build(args.b)
         else:
             build(args.b)
         if args.r:
             run(args.r)
     except (KeyboardInterrupt):
         pass
+    except Exception as e:
+        if verborse=='D':
+            raise e
+        pass
 
 if __name__ == 'yaya':
     init()
     load()
     process()
 
 else:
```

### Comparing `yymake-0.8.1/ymake/yymake.egg-info/PKG-INFO` & `yymake-0.8.5/ymake/yymake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yymake
-Version: 0.8.1
+Version: 0.8.5
 Summary: A cross build dsl make tool
 Home-page: https://github.com/evilbinary/ymake
 Author: evilbinary
 Author-email: rootntsd@gmail.com
 Project-URL: Bug Tracker, https://github.com/evilbinary/ymake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

