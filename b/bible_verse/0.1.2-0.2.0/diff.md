# Comparing `tmp/bible_verse-0.1.2.tar.gz` & `tmp/bible_verse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bible_verse-0.1.2.tar", max compression
+gzip compressed data, was "bible_verse-0.2.0.tar", max compression
```

## Comparing `bible_verse-0.1.2.tar` & `bible_verse-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-15 19:42:48.852217 bible_verse-0.1.2/bible_verse/__init__.py
--rw-r--r--   0        0        0     2441 2024-03-18 16:18:15.500940 bible_verse-0.1.2/bible_verse/main.py
--rw-r--r--   0        0        0      409 2024-03-18 16:21:15.380995 bible_verse-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      816 2024-03-15 22:40:20.483264 bible_verse-0.1.2/README.md
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 bible_verse-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-04 23:30:42.390736 bible_verse-0.2.0/bible_verse/__init__.py
+-rw-r--r--   0        0        0     4882 2024-04-04 23:41:29.293313 bible_verse-0.2.0/bible_verse/main.py
+-rw-r--r--   0        0        0      473 2024-04-04 23:52:45.642058 bible_verse-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1187 2024-04-04 23:46:02.061540 bible_verse-0.2.0/README.md
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 bible_verse-0.2.0/PKG-INFO
```

