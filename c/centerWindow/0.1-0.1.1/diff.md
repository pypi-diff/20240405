# Comparing `tmp/centerWindow-0.1.tar.gz` & `tmp/centerWindow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centerWindow-0.1.tar", last modified: Thu Apr  4 17:32:18 2024, max compression
+gzip compressed data, was "centerWindow-0.1.1.tar", last modified: Thu Apr  4 18:28:17 2024, max compression
```

## Comparing `centerWindow-0.1.tar` & `centerWindow-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 leonardobartolelli   (501) staff       (20)        0 2024-04-04 17:32:18.594361 centerWindow-0.1/
--rw-r--r--   0 leonardobartolelli   (501) staff       (20)       54 2024-04-04 17:32:18.594186 centerWindow-0.1/PKG-INFO
-drwxr-xr-x   0 leonardobartolelli   (501) staff       (20)        0 2024-04-04 17:32:18.593210 centerWindow-0.1/centerWindow/
--rw-r--r--   0 leonardobartolelli   (501) staff       (20)      360 2024-04-04 17:24:34.000000 centerWindow-0.1/centerWindow/main.py
-drwxr-xr-x   0 leonardobartolelli   (501) staff       (20)        0 2024-04-04 17:32:18.594008 centerWindow-0.1/centerWindow.egg-info/
--rw-r--r--   0 leonardobartolelli   (501) staff       (20)       54 2024-04-04 17:32:18.000000 centerWindow-0.1/centerWindow.egg-info/PKG-INFO
--rw-r--r--   0 leonardobartolelli   (501) staff       (20)      173 2024-04-04 17:32:18.000000 centerWindow-0.1/centerWindow.egg-info/SOURCES.txt
--rw-r--r--   0 leonardobartolelli   (501) staff       (20)        1 2024-04-04 17:32:18.000000 centerWindow-0.1/centerWindow.egg-info/dependency_links.txt
--rw-r--r--   0 leonardobartolelli   (501) staff       (20)       13 2024-04-04 17:32:18.000000 centerWindow-0.1/centerWindow.egg-info/top_level.txt
--rw-r--r--   0 leonardobartolelli   (501) staff       (20)       38 2024-04-04 17:32:18.594404 centerWindow-0.1/setup.cfg
--rw-r--r--   0 leonardobartolelli   (501) staff       (20)      115 2024-04-04 17:32:14.000000 centerWindow-0.1/setup.py
+drwxr-xr-x   0 leonardobartolelli   (501) staff       (20)        0 2024-04-04 18:28:17.081889 centerWindow-0.1.1/
+-rw-r--r--   0 leonardobartolelli   (501) staff       (20)       56 2024-04-04 18:28:17.081709 centerWindow-0.1.1/PKG-INFO
+drwxr-xr-x   0 leonardobartolelli   (501) staff       (20)        0 2024-04-04 18:28:17.080263 centerWindow-0.1.1/centerWindow/
+-rw-r--r--   0 leonardobartolelli   (501) staff       (20)      360 2024-04-04 17:24:34.000000 centerWindow-0.1.1/centerWindow/main.py
+drwxr-xr-x   0 leonardobartolelli   (501) staff       (20)        0 2024-04-04 18:28:17.081505 centerWindow-0.1.1/centerWindow.egg-info/
+-rw-r--r--   0 leonardobartolelli   (501) staff       (20)       56 2024-04-04 18:28:17.000000 centerWindow-0.1.1/centerWindow.egg-info/PKG-INFO
+-rw-r--r--   0 leonardobartolelli   (501) staff       (20)      173 2024-04-04 18:28:17.000000 centerWindow-0.1.1/centerWindow.egg-info/SOURCES.txt
+-rw-r--r--   0 leonardobartolelli   (501) staff       (20)        1 2024-04-04 18:28:17.000000 centerWindow-0.1.1/centerWindow.egg-info/dependency_links.txt
+-rw-r--r--   0 leonardobartolelli   (501) staff       (20)       13 2024-04-04 18:28:17.000000 centerWindow-0.1.1/centerWindow.egg-info/top_level.txt
+-rw-r--r--   0 leonardobartolelli   (501) staff       (20)       38 2024-04-04 18:28:17.081941 centerWindow-0.1.1/setup.cfg
+-rw-r--r--   0 leonardobartolelli   (501) staff       (20)      117 2024-04-04 18:26:38.000000 centerWindow-0.1.1/setup.py
```

