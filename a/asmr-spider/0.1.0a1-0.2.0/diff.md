# Comparing `tmp/asmr_spider-0.1.0a1.tar.gz` & `tmp/asmr_spider-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmr_spider-0.1.0a1.tar", max compression
+gzip compressed data, was "asmr_spider-0.2.0.tar", max compression
```

## Comparing `asmr_spider-0.1.0a1.tar` & `asmr_spider-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/LICENSE
--rw-r--r--   0        0        0      894 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/README.md
--rw-r--r--   0        0        0      318 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/asmr_spider/__init__.py
--rw-r--r--   0        0        0      340 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/asmr_spider/__main__.py
--rw-r--r--   0        0        0     1814 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/asmr_spider/config.py
--rw-r--r--   0        0        0     5102 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/asmr_spider/spider.py
--rw-r--r--   0        0        0      940 2023-04-12 10:41:21.675749 asmr_spider-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     1672 1970-01-01 00:00:00.000000 asmr_spider-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 00:23:52.770018 asmr_spider-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2777 2024-04-05 00:23:52.770018 asmr_spider-0.2.0/README.md
+-rw-r--r--   0        0        0      808 2024-04-05 00:23:52.770018 asmr_spider-0.2.0/asmr_spider/__init__.py
+-rw-r--r--   0        0        0      780 2024-04-05 00:23:52.770018 asmr_spider-0.2.0/asmr_spider/__main__.py
+-rw-r--r--   0        0        0     1803 2024-04-05 00:23:52.770018 asmr_spider-0.2.0/asmr_spider/config.py
+-rw-r--r--   0        0        0     7221 2024-04-05 00:23:52.770018 asmr_spider-0.2.0/asmr_spider/spider.py
+-rw-r--r--   0        0        0     1022 2024-04-05 00:23:52.774018 asmr_spider-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 asmr_spider-0.2.0/PKG-INFO
```

### Comparing `asmr_spider-0.1.0a1/LICENSE` & `asmr_spider-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.1.0a1/asmr_spider/config.py` & `asmr_spider-0.2.0/asmr_spider/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 import sys, yaml
-from pydantic import BaseModel, Extra, ConfigDict
+from pydantic import BaseModel, ConfigDict
 from loguru import logger
 from rich.progress import (
     BarColumn,
     DownloadColumn,
     Progress,
     TextColumn,
     TransferSpeedColumn,
@@ -59,15 +59,15 @@
         sys.exit(1)
 
 
 _config = yaml.safe_load(confpath.read_text('utf-8'))
 
 
 class Config(BaseModel):
-    model_config = ConfigDict(extra=Extra.ignore)
+    model_config = ConfigDict(extra="ignore")
     username: str = 'guest'
     password: str = 'guest'
     proxy: str = ''
     user_agent: str = 'Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)'
 
 
 config = Config.model_validate(_config)
```

