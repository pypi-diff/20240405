# Comparing `tmp/super-ide-1.4.7.tar.gz` & `tmp/super-ide-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super-ide-1.4.7.tar", last modified: Wed Apr  3 15:56:45 2024, max compression
+gzip compressed data, was "super-ide-1.4.8.tar", last modified: Fri Apr  5 05:04:10 2024, max compression
```

## Comparing `super-ide-1.4.7.tar` & `super-ide-1.4.8.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.699095 super-ide-1.4.7/
--rwxrwxrwx   0 denk      (1000) denk      (1000)    34520 2024-04-03 15:40:53.000000 super-ide-1.4.7/LICENSE
--rwxrwxrwx   0 denk      (1000) denk      (1000)      111 2024-04-03 15:40:53.000000 super-ide-1.4.7/MANIFEST.in
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2206 2024-04-03 15:56:45.695076 super-ide-1.4.7/PKG-INFO
--rwxrwxrwx   0 denk      (1000) denk      (1000)      790 2024-04-03 15:40:53.000000 super-ide-1.4.7/README.rst
--rwxrwxrwx   0 denk      (1000) denk      (1000)       38 2024-04-03 15:56:45.701098 super-ide-1.4.7/setup.cfg
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3436 2024-04-03 15:40:53.000000 super-ide-1.4.7/setup.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:35.453491 super-ide-1.4.7/super_ide.egg-info/
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2206 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/PKG-INFO
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2565 2024-04-03 15:56:34.000000 super-ide-1.4.7/super_ide.egg-info/SOURCES.txt
--rwxrwxrwx   0 denk      (1000) denk      (1000)        1 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/dependency_links.txt
--rwxrwxrwx   0 denk      (1000) denk      (1000)      162 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/entry_points.txt
--rwxrwxrwx   0 denk      (1000) denk      (1000)      284 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/requires.txt
--rwxrwxrwx   0 denk      (1000) denk      (1000)        9 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/top_level.txt
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:35.900990 super-ide-1.4.7/superide/
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2026 2024-04-03 15:46:41.000000 super-ide-1.4.7/superide/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     4449 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/__main__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     8340 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/app.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:36.009641 super-ide-1.4.7/superide/boards/
--rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/boards/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      207 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/boards/boards.json
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2937 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/boards/cli.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5203 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/cache.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3277 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/cli.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3553 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/compat.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:36.184642 super-ide-1.4.7/superide/debug/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6135 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/cli.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:41.617090 super-ide-1.4.7/superide/debug/config/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     8965 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/base.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2068 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/blackmagic.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1742 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/factory.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      969 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/generic.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1161 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/jlink.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      921 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/mspdebug.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      962 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/native.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      962 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/qemu.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1156 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/renode.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1195 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/exception.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5085 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/helpers.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:42.211835 super-ide-1.4.7/superide/debug/process/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/debug/process/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     4891 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/debug/process/base.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3449 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/debug/process/client.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     7087 2024-04-03 15:46:34.000000 super-ide-1.4.7/superide/debug/process/gdb.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5727 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/debug/process/server.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3197 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/exception.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6701 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/fs.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:42.577465 super-ide-1.4.7/superide/home/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/home/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3986 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/home/app.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3208 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/home/cli.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:42.666453 super-ide-1.4.7/superide/home/rpc/
--rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/__init__.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:43.538758 super-ide-1.4.7/superide/home/rpc/handlers/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2839 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/app.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      603 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/base.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2928 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/ide.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6430 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/os.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    16695 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/project.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1202 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/registry.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      627 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/runServer.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:43.639614 super-ide-1.4.7/superide/home/static/
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:44.106059 super-ide-1.4.7/superide/home/static/assets/
--rwxrwxrwx   0 denk      (1000) denk      (1000)    15406 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/static/assets/favicon.ico
--rwxrwxrwx   0 denk      (1000) denk      (1000)   107097 2024-04-03 15:41:01.000000 super-ide-1.4.7/superide/home/static/assets/index-6fed80ed.css
--rwxrwxrwx   0 denk      (1000) denk      (1000)   439260 2024-04-03 15:41:02.000000 super-ide-1.4.7/superide/home/static/assets/index-d2bbbc6e.js
--rwxrwxrwx   0 denk      (1000) denk      (1000)      529 2024-04-03 15:41:04.000000 super-ide-1.4.7/superide/home/static/index.html
--rwxrwxrwx   0 denk      (1000) denk      (1000)     7468 2024-04-03 15:41:05.000000 super-ide-1.4.7/superide/http.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3522 2024-04-03 15:41:05.000000 super-ide-1.4.7/superide/lockfile.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    10459 2024-04-03 15:41:05.000000 super-ide-1.4.7/superide/maintenance.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6432 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/proc.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:44.635321 super-ide-1.4.7/superide/project/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      960 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/cli.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:44.935488 super-ide-1.4.7/superide/project/commands/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/commands/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3253 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/commands/config.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5446 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/commands/init.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2833 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/commands/metadata.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    18874 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/config.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1846 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/exception.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6607 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/helpers.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    31369 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/options.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3084 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/savedeps.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     8513 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/vcsclient.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1392 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/public.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.096112 super-ide-1.4.7/superide/registry/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/registry/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2900 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/registry/cli.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     8683 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/registry/client.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3690 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/registry/mirror.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.240996 super-ide-1.4.7/superide/run/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/run/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     9493 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/run/cli.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     1600 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/run/helpers.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     6718 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/run/processor.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.408798 super-ide-1.4.7/superide/system/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/system/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)      971 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/system/cli.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.605661 super-ide-1.4.7/superide/system/commands/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/system/commands/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2448 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/system/commands/completion.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     2933 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/system/commands/info.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3242 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/system/completion.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)    10925 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/telemetry.py
-drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.666665 super-ide-1.4.7/superide/toolchain/
--rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/toolchain/__init__.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     3569 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/toolchain/toolchain.py
--rwxrwxrwx   0 denk      (1000) denk      (1000)     5895 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/util.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:10.845612 super-ide-1.4.8/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    34520 2024-04-03 15:40:53.000000 super-ide-1.4.8/LICENSE
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      111 2024-04-03 15:40:53.000000 super-ide-1.4.8/MANIFEST.in
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2187 2024-04-05 05:04:10.822430 super-ide-1.4.8/PKG-INFO
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      790 2024-04-03 15:40:53.000000 super-ide-1.4.8/README.rst
+-rwxrwxrwx   0 denk      (1000) denk      (1000)       38 2024-04-05 05:04:10.848112 super-ide-1.4.8/setup.cfg
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3436 2024-04-03 15:40:53.000000 super-ide-1.4.8/setup.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:51.684482 super-ide-1.4.8/super_ide.egg-info/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2187 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/PKG-INFO
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2588 2024-04-05 05:03:50.000000 super-ide-1.4.8/super_ide.egg-info/SOURCES.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        1 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/dependency_links.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      161 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/entry_points.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      284 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/requires.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        9 2024-04-05 05:03:48.000000 super-ide-1.4.8/super_ide.egg-info/top_level.txt
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:54.064067 super-ide-1.4.8/superide/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2026 2024-04-05 04:45:54.000000 super-ide-1.4.8/superide/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     4449 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/__main__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8340 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/app.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:54.657714 super-ide-1.4.8/superide/boards/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/boards/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      207 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/boards/boards.json
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2937 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/boards/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5203 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/cache.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3277 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3553 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/compat.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:56.971315 super-ide-1.4.8/superide/debug/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6135 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:58.331334 super-ide-1.4.8/superide/debug/config/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8965 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2068 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/blackmagic.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1742 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/factory.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      969 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/generic.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1161 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/jlink.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      921 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/mspdebug.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      962 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/native.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      962 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/qemu.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1156 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/config/renode.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1195 2024-04-03 15:40:53.000000 super-ide-1.4.8/superide/debug/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5218 2024-04-05 04:51:38.000000 super-ide-1.4.8/superide/debug/helpers.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:58.890354 super-ide-1.4.8/superide/debug/process/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/debug/process/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     4891 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/debug/process/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3449 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/debug/process/client.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     7141 2024-04-05 04:49:29.000000 super-ide-1.4.8/superide/debug/process/gdb.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5727 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/debug/process/server.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3197 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6701 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/fs.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:59.253784 super-ide-1.4.8/superide/home/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/home/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3986 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/home/app.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3208 2024-04-03 15:40:54.000000 super-ide-1.4.8/superide/home/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:03:59.334033 super-ide-1.4.8/superide/home/rpc/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/__init__.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:00.747522 super-ide-1.4.8/superide/home/rpc/handlers/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2839 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/app.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      603 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2928 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/ide.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6430 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/os.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    16695 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/project.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1202 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/rpc/handlers/registry.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      627 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/runServer.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:00.792499 super-ide-1.4.8/superide/home/static/
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:00.981417 super-ide-1.4.8/superide/home/static/assets/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    15406 2024-04-03 15:41:00.000000 super-ide-1.4.8/superide/home/static/assets/favicon.ico
+-rwxrwxrwx   0 denk      (1000) denk      (1000)   107097 2024-04-03 15:41:01.000000 super-ide-1.4.8/superide/home/static/assets/index-6fed80ed.css
+-rwxrwxrwx   0 denk      (1000) denk      (1000)   439260 2024-04-03 15:41:02.000000 super-ide-1.4.8/superide/home/static/assets/index-d2bbbc6e.js
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      529 2024-04-03 15:41:04.000000 super-ide-1.4.8/superide/home/static/index.html
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     7468 2024-04-03 15:41:05.000000 super-ide-1.4.8/superide/http.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3522 2024-04-03 15:41:05.000000 super-ide-1.4.8/superide/lockfile.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    10459 2024-04-03 15:41:05.000000 super-ide-1.4.8/superide/maintenance.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6432 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/proc.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:01.421762 super-ide-1.4.8/superide/project/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      960 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:04.150597 super-ide-1.4.8/superide/project/commands/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/commands/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3253 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/commands/config.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5446 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/commands/init.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2833 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/commands/metadata.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    18874 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/config.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1846 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6607 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/helpers.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    31369 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/options.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3084 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/savedeps.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8513 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/project/vcsclient.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1392 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/public.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:04.539155 super-ide-1.4.8/superide/registry/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/registry/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2900 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/registry/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8683 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/registry/client.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3690 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/registry/mirror.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:05.034778 super-ide-1.4.8/superide/run/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/run/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     9493 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/run/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1600 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/run/helpers.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6718 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/run/processor.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:05.345009 super-ide-1.4.8/superide/system/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/system/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      971 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/system/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:09.805641 super-ide-1.4.8/superide/system/commands/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.8/superide/system/commands/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2448 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/system/commands/completion.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2933 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/system/commands/info.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3242 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/system/completion.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    10925 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/telemetry.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:10.654629 super-ide-1.4.8/superide/toolchain/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/toolchain/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3569 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/toolchain/toolchain.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5895 2024-04-03 15:41:07.000000 super-ide-1.4.8/superide/util.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-05 05:04:10.746552 super-ide-1.4.8/tests/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3437 2024-04-03 15:41:07.000000 super-ide-1.4.8/tests/test_examples.py
```

### Comparing `super-ide-1.4.7/LICENSE` & `super-ide-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/PKG-INFO` & `super-ide-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: super-ide
-Version: 1.4.7
+Version: 1.4.8
 Summary: A professional Cross-platform IDE. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://mengning.com.cn
 Author: Mengning Software
 Author-email: contact@mengning.com.cn
 License: AGPL-3.0 License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
@@ -43,8 +42,7 @@
 
 License
 -------
 
 Copyright (c) 2022-present Mengning <contact@mengning.com.cn>
 
 The Super IDE is licensed under the AGPL 3.0 license or commercial license.
-
```

### Comparing `super-ide-1.4.7/README.rst` & `super-ide-1.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/setup.py` & `super-ide-1.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/super_ide.egg-info/PKG-INFO` & `super-ide-1.4.8/super_ide.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: super-ide
-Version: 1.4.7
+Version: 1.4.8
 Summary: A professional Cross-platform IDE. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://mengning.com.cn
 Author: Mengning Software
 Author-email: contact@mengning.com.cn
 License: AGPL-3.0 License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
@@ -43,8 +42,7 @@
 
 License
 -------
 
 Copyright (c) 2022-present Mengning <contact@mengning.com.cn>
 
 The Super IDE is licensed under the AGPL 3.0 license or commercial license.
-
```

### Comparing `super-ide-1.4.7/super_ide.egg-info/SOURCES.txt` & `super-ide-1.4.8/super_ide.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -84,8 +84,9 @@
 superide/system/__init__.py
 superide/system/cli.py
 superide/system/completion.py
 superide/system/commands/__init__.py
 superide/system/commands/completion.py
 superide/system/commands/info.py
 superide/toolchain/__init__.py
-superide/toolchain/toolchain.py
+superide/toolchain/toolchain.py
+tests/test_examples.py
```

### Comparing `super-ide-1.4.7/superide/__init__.py` & `super-ide-1.4.8/superide/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #    https://www.gnu.org/licenses/agpl-3.0.txt
 #
 # THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
 # PURPOSE.
 # See the AGPL-3.0 for more details.
 
-VERSION = (1, 4, 7)
+VERSION = (1, 4, 8)
 __version__ = ".".join([str(s) for s in VERSION])
 
 __title__ = "super-ide"
 __description__ = (
     "A professional Cross-platform IDE. "
     "Cross-platform IDE and Unified Debugger. "
     "Static Code Analyzer and Remote Unit Testing. "
```

### Comparing `super-ide-1.4.7/superide/__main__.py` & `super-ide-1.4.8/superide/__main__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/app.py` & `super-ide-1.4.8/superide/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/boards/cli.py` & `super-ide-1.4.8/superide/boards/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/cache.py` & `super-ide-1.4.8/superide/cache.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/cli.py` & `super-ide-1.4.8/superide/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/compat.py` & `super-ide-1.4.8/superide/compat.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/__init__.py` & `super-ide-1.4.8/superide/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/cli.py` & `super-ide-1.4.8/superide/debug/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/__init__.py` & `super-ide-1.4.8/superide/debug/config/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/base.py` & `super-ide-1.4.8/superide/debug/config/base.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/blackmagic.py` & `super-ide-1.4.8/superide/debug/config/blackmagic.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/factory.py` & `super-ide-1.4.8/superide/debug/config/factory.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/generic.py` & `super-ide-1.4.8/superide/debug/config/generic.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/jlink.py` & `super-ide-1.4.8/superide/debug/config/jlink.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/mspdebug.py` & `super-ide-1.4.8/superide/debug/config/mspdebug.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/native.py` & `super-ide-1.4.8/superide/debug/config/native.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/qemu.py` & `super-ide-1.4.8/superide/debug/config/qemu.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/config/renode.py` & `super-ide-1.4.8/superide/debug/config/renode.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/exception.py` & `super-ide-1.4.8/superide/debug/exception.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/helpers.py` & `super-ide-1.4.8/superide/debug/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,47 +73,49 @@
             return env
     return default_envs[0] if default_envs else all_envs[0]
 
 
 def predebug_project(
     ctx, project_dir, project_config, env_name, preload, verbose
 ):  # pylint: disable=too-many-arguments
-    debug_testname = project_config.get("env:" + env_name, "debug_test")
-    if debug_testname:
-        # test_names = list_test_names(project_config)
-        # if debug_testname not in test_names:
-        #     raise DebugInvalidOptionsError(
-        #         "Unknown test name `%s`. Valid names are `%s`"
-        #         % (debug_testname, ", ".join(test_names))
-        #     )
-        print_processing_header(env_name, project_config, verbose)
-        # test_runner = TestRunnerFactory.new(
-        #     TestSuite(env_name, debug_testname),
-        #     project_config,
-        #     TestRunnerOptions(
-        #         verbose=3 if verbose else 0,
-        #         without_building=False,
-        #         without_debugging=False,
-        #         without_uploading=not preload,
-        #         without_testing=True,
-        #     ),
-        # )
-        # test_runner.start(ctx)
-    else:
-        ctx.invoke(
-            cmd_run,
-            project_dir=project_dir,
-            project_conf=project_config.path,
-            environment=[env_name],
-            target=["__debug"] + (["upload"] if preload else []),
-            verbose=verbose,
-        )
+    # predebug与run功能类似，此处旧版代码停用
+    pass
+    # debug_testname = project_config.get("env:" + env_name, "debug_test")
+    # if debug_testname:
+    #     # test_names = list_test_names(project_config)
+    #     # if debug_testname not in test_names:
+    #     #     raise DebugInvalidOptionsError(
+    #     #         "Unknown test name `%s`. Valid names are `%s`"
+    #     #         % (debug_testname, ", ".join(test_names))
+    #     #     )
+    #     print_processing_header(env_name, project_config, verbose)
+    #     # test_runner = TestRunnerFactory.new(
+    #     #     TestSuite(env_name, debug_testname),
+    #     #     project_config,
+    #     #     TestRunnerOptions(
+    #     #         verbose=3 if verbose else 0,
+    #     #         without_building=False,
+    #     #         without_debugging=False,
+    #     #         without_uploading=not preload,
+    #     #         without_testing=True,
+    #     #     ),
+    #     # )
+    #     # test_runner.start(ctx)
+    # else:
+    #     ctx.invoke(
+    #         cmd_run,
+    #         project_dir=project_dir,
+    #         project_conf=project_config.path,
+    #         environment=[env_name],
+    #         target=["__debug"] + (["upload"] if preload else []),
+    #         verbose=verbose,
+    #     )
 
-    if preload:
-        time.sleep(5)
+    # if preload:
+    #     time.sleep(5)
 
 
 def has_debug_symbols(prog_path):
     if not os.path.isfile(prog_path):
         return False
     matched = {
         b".debug_info": False,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `super-ide-1.4.7/superide/debug/process/__init__.py` & `super-ide-1.4.8/superide/debug/process/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/process/base.py` & `super-ide-1.4.8/superide/debug/process/base.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/process/client.py` & `super-ide-1.4.8/superide/debug/process/client.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/debug/process/gdb.py` & `super-ide-1.4.8/superide/debug/process/gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,17 @@
     def stdin_data_received(self, data):
         super().stdin_data_received(data)
         if b"-exec-run" in data:
             if self._target_is_running:
                 token, _ = data.split(b"-", 1)
                 self.stdout_data_received(token + b"^running\n")
                 return
-            if self.debug_config.platform.is_embedded():
-                data = data.replace(b"-exec-run", b"-exec-continue")
+            # config和platform部分代码停用
+            # if self.debug_config.platform.is_embedded():
+            #     data = data.replace(b"-exec-run", b"-exec-continue")
 
         if b"-exec-continue" in data:
             self._target_is_running = True
         if b"-gdb-exit" in data or data.strip() in (b"q", b"quit"):
             # Allow terminating via SIGINT/CTRL+C
             signal.signal(signal.SIGINT, signal.default_int_handler)
             self.transport.get_pipe_transport(0).write(b"pio_reset_run_target\n")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `super-ide-1.4.7/superide/debug/process/server.py` & `super-ide-1.4.8/superide/debug/process/server.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/exception.py` & `super-ide-1.4.8/superide/exception.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/fs.py` & `super-ide-1.4.8/superide/fs.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/__init__.py` & `super-ide-1.4.8/superide/home/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/app.py` & `super-ide-1.4.8/superide/home/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/cli.py` & `super-ide-1.4.8/superide/home/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/rpc/handlers/__init__.py` & `super-ide-1.4.8/superide/home/rpc/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/rpc/handlers/app.py` & `super-ide-1.4.8/superide/home/rpc/handlers/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/rpc/handlers/base.py` & `super-ide-1.4.8/superide/home/rpc/handlers/base.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/rpc/handlers/ide.py` & `super-ide-1.4.8/superide/home/rpc/handlers/ide.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/rpc/handlers/os.py` & `super-ide-1.4.8/superide/home/rpc/handlers/os.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/rpc/handlers/project.py` & `super-ide-1.4.8/superide/home/rpc/handlers/project.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/rpc/handlers/registry.py` & `super-ide-1.4.8/superide/home/rpc/handlers/registry.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/runServer.py` & `super-ide-1.4.8/superide/home/runServer.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/static/assets/favicon.ico` & `super-ide-1.4.8/superide/home/static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/static/assets/index-6fed80ed.css` & `super-ide-1.4.8/superide/home/static/assets/index-6fed80ed.css`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/static/assets/index-d2bbbc6e.js` & `super-ide-1.4.8/superide/home/static/assets/index-d2bbbc6e.js`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/home/static/index.html` & `super-ide-1.4.8/superide/home/static/index.html`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/http.py` & `super-ide-1.4.8/superide/http.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/lockfile.py` & `super-ide-1.4.8/superide/lockfile.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/maintenance.py` & `super-ide-1.4.8/superide/maintenance.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/proc.py` & `super-ide-1.4.8/superide/proc.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/__init__.py` & `super-ide-1.4.8/superide/project/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/cli.py` & `super-ide-1.4.8/superide/project/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/commands/__init__.py` & `super-ide-1.4.8/superide/project/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/commands/config.py` & `super-ide-1.4.8/superide/project/commands/config.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/commands/init.py` & `super-ide-1.4.8/superide/project/commands/init.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/commands/metadata.py` & `super-ide-1.4.8/superide/project/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/config.py` & `super-ide-1.4.8/superide/project/config.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/exception.py` & `super-ide-1.4.8/superide/project/exception.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/helpers.py` & `super-ide-1.4.8/superide/project/helpers.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/options.py` & `super-ide-1.4.8/superide/project/options.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/savedeps.py` & `super-ide-1.4.8/superide/project/savedeps.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/project/vcsclient.py` & `super-ide-1.4.8/superide/project/vcsclient.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/public.py` & `super-ide-1.4.8/superide/public.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/registry/__init__.py` & `super-ide-1.4.8/superide/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/registry/cli.py` & `super-ide-1.4.8/superide/registry/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/registry/client.py` & `super-ide-1.4.8/superide/registry/client.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/registry/mirror.py` & `super-ide-1.4.8/superide/registry/mirror.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/run/__init__.py` & `super-ide-1.4.8/superide/run/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/run/cli.py` & `super-ide-1.4.8/superide/run/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/run/helpers.py` & `super-ide-1.4.8/superide/run/helpers.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/run/processor.py` & `super-ide-1.4.8/superide/run/processor.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/system/__init__.py` & `super-ide-1.4.8/superide/system/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/system/cli.py` & `super-ide-1.4.8/superide/system/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/system/commands/__init__.py` & `super-ide-1.4.8/superide/system/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/system/commands/completion.py` & `super-ide-1.4.8/superide/system/commands/completion.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/system/commands/info.py` & `super-ide-1.4.8/superide/system/commands/info.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/system/completion.py` & `super-ide-1.4.8/superide/system/completion.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/telemetry.py` & `super-ide-1.4.8/superide/telemetry.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/toolchain/__init__.py` & `super-ide-1.4.8/superide/toolchain/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/toolchain/toolchain.py` & `super-ide-1.4.8/superide/toolchain/toolchain.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.7/superide/util.py` & `super-ide-1.4.8/superide/util.py`

 * *Files identical despite different names*

