# Comparing `tmp/svgcheck-0.7.1.tar.gz` & `tmp/svgcheck-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgcheck-0.7.1.tar", last modified: Wed Feb  1 20:40:14 2023, max compression
+gzip compressed data, was "svgcheck-0.8.0.tar", last modified: Thu Apr  4 23:26:39 2024, max compression
```

## Comparing `svgcheck-0.7.1.tar` & `svgcheck-0.8.0.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:40:14.961400 svgcheck-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-02-01 20:39:13.000000 svgcheck-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-01 20:39:13.000000 svgcheck-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-01 20:39:13.000000 svgcheck-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-02-01 20:40:14.961400 svgcheck-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-02-01 20:39:13.000000 svgcheck-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-01 20:39:13.000000 svgcheck-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-01 20:39:13.000000 svgcheck-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-02-01 20:40:14.961400 svgcheck-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:40:14.941400 svgcheck-0.7.1/svgcheck/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:40:14.953400 svgcheck-0.7.1/svgcheck/Results/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/DrawBerry-sample-2.out
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/DrawBerry-sample-2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/IETF-test.out
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/IETF-test.svg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/circle.out
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/clear-cache.err
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/clear-cache.out
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/colors.err
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/colors.out
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/dia-sample-svg.out
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/dia-sample-svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/empty
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/example-dot.out
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/example-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/full-tiny-02.err
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/full-tiny-02.out
--rw-r--r--   0 runner    (1001) docker     (123)   614705 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/full-tiny.err
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/full-tiny.out
--rw-r--r--   0 runner    (1001) docker     (123)   388155 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/full-tiny.xml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/good.err
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/httpbis-proxy20-fig6.out
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/httpbis-proxy20-fig6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/malformed.out
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/malformed.svg
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-01.err
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-01.out
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-01.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-02.err
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-02.out
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-03.err
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-03.out
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-svg.err
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rfc-svg.out
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rgb.out
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/rgb.svg
--rw-r--r--   0 runner    (1001) docker     (123)    40451 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/svg-wordle.out
--rw-r--r--   0 runner    (1001) docker     (123)   352314 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/svg-wordle.svg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/utf8-2.err
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/utf8-2.out
--rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/utf8-2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/utf8.err
--rw-r--r--   0 runner    (1001) docker     (123)    31711 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/utf8.out
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/viewBox-both.out
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/viewBox-both.svg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/viewBox-height.out
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/viewBox-height.svg
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/viewBox-none.out
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/viewBox-none.svg
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/viewBox-width.out
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Results/viewBox-width.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:40:14.961400 svgcheck-0.7.1/svgcheck/Tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/DrawBerry-sample-2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/IETF-test.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:40:14.961400 svgcheck-0.7.1/svgcheck/Tests/cache_saved/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/cache_saved/reference.RFC.1847.xml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/colors.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/dia-sample-svg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/example-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)  4264869 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/full-tiny.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/good.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/httpbis-proxy20-fig6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/malformed.svg
--rw-r--r--   0 runner    (1001) docker     (123)   301354 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/rfc-svg.xml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/rfc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/rgb.svg
--rw-r--r--   0 runner    (1001) docker     (123)   355486 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/svg-wordle.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/threshold.svg
--rw-r--r--   0 runner    (1001) docker     (123)    51830 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/utf8.svg
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/viewBox-both.svg
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/viewBox-height.svg
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/viewBox-none.svg
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/Tests/viewBox-width.svg
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-01 20:39:53.000000 svgcheck-0.7.1/svgcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/checksvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/pycode.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/run.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-02-01 20:39:13.000000 svgcheck-0.7.1/svgcheck/word_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:40:14.945400 svgcheck-0.7.1/svgcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-02-01 20:40:14.000000 svgcheck-0.7.1/svgcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-02-01 20:40:14.000000 svgcheck-0.7.1/svgcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:40:14.000000 svgcheck-0.7.1/svgcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-01 20:40:14.000000 svgcheck-0.7.1/svgcheck.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:40:00.000000 svgcheck-0.7.1/svgcheck.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-01 20:40:14.000000 svgcheck-0.7.1/svgcheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-01 20:40:14.000000 svgcheck-0.7.1/svgcheck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:39.467104 svgcheck-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-04 23:26:10.000000 svgcheck-0.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-04 23:26:10.000000 svgcheck-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 23:26:10.000000 svgcheck-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-04 23:26:39.467104 svgcheck-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-04 23:26:10.000000 svgcheck-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 23:26:10.000000 svgcheck-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 23:26:10.000000 svgcheck-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-04 23:26:39.467104 svgcheck-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:39.447104 svgcheck-0.8.0/svgcheck/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:39.459104 svgcheck-0.8.0/svgcheck/Results/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/DrawBerry-sample-2.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/DrawBerry-sample-2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/IETF-test.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/IETF-test.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/circle.out
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/clear-cache.err
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/clear-cache.out
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/colors.err
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/colors.out
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/dia-sample-svg.out
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/dia-sample-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/empty
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/example-dot.out
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/example-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/full-tiny-02.err
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/full-tiny-02.out
+-rw-r--r--   0 runner    (1001) docker     (127)   614705 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/full-tiny.err
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/full-tiny.out
+-rw-r--r--   0 runner    (1001) docker     (127)   388155 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/full-tiny.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/good.err
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/httpbis-proxy20-fig6.out
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/httpbis-proxy20-fig6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/malformed.out
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/malformed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-01.err
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-01.out
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-01.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-02.err
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-02.out
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-03.err
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-03.out
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-svg.err
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rfc-svg.out
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rgb.out
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/rgb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    40451 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/svg-wordle.out
+-rw-r--r--   0 runner    (1001) docker     (127)   352314 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/svg-wordle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/utf8-2.err
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/utf8-2.out
+-rw-r--r--   0 runner    (1001) docker     (127)    31809 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/utf8-2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17243 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/utf8.err
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/utf8.out
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/viewBox-both.out
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/viewBox-both.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/viewBox-height.out
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/viewBox-height.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/viewBox-none.out
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/viewBox-none.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/viewBox-width.out
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Results/viewBox-width.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:39.467104 svgcheck-0.8.0/svgcheck/Tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/DrawBerry-sample-2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/IETF-test.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:39.467104 svgcheck-0.8.0/svgcheck/Tests/cache_saved/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/cache_saved/reference.RFC.1847.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/colors.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/dia-sample-svg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/example-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (127)  4264869 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/full-tiny.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/good.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/httpbis-proxy20-fig6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/malformed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   301354 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/rfc-svg.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/rfc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/rgb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   355486 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/svg-wordle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/threshold.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    51830 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/utf8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/viewBox-both.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/viewBox-height.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/viewBox-none.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/Tests/viewBox-width.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 23:26:37.000000 svgcheck-0.8.0/svgcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/checksvg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/pycode.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12400 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-04-04 23:26:10.000000 svgcheck-0.8.0/svgcheck/word_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:26:39.467104 svgcheck-0.8.0/svgcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-04 23:26:39.000000 svgcheck-0.8.0/svgcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-04 23:26:39.000000 svgcheck-0.8.0/svgcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:26:39.000000 svgcheck-0.8.0/svgcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 23:26:39.000000 svgcheck-0.8.0/svgcheck.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:26:39.000000 svgcheck-0.8.0/svgcheck.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 23:26:39.000000 svgcheck-0.8.0/svgcheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 23:26:39.000000 svgcheck-0.8.0/svgcheck.egg-info/top_level.txt
```

### Comparing `svgcheck-0.7.1/CHANGELOG.md` & `svgcheck-0.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v0.7.1] - 2023-02-01
+### :bug: Bug Fixes
+- [`182b486`](https://github.com/ietf-tools/svgcheck/commit/182b486d86cb98561d34bda2050e53a5dba34400) - No op --no-xinclude option *(PR [#35](https://github.com/ietf-tools/svgcheck/pull/35) by [@kesara](https://github.com/kesara))*
+
+
 ## [v0.7.0] - 2023-01-31
 ### :sparkles: New Features
 - [`ac1cc51`](https://github.com/ietf-tools/svgcheck/commit/ac1cc516f29da1495dfa10e4cfed0b7f720363be) - Use xml2rfc *(PR [#28](https://github.com/ietf-tools/svgcheck/pull/28) by [@kesara](https://github.com/kesara))*
 - [`8935e20`](https://github.com/ietf-tools/svgcheck/commit/8935e206769cfe158247c935120271190c27d17a) - Add support for Python 3.11 *(PR [#30](https://github.com/ietf-tools/svgcheck/pull/30) by [@kesara](https://github.com/kesara))*
 - [`d1076d2`](https://github.com/ietf-tools/svgcheck/commit/d1076d2ec1a4f73e9992f23d942b38730c7f56a2) - Remove command line option --no-xinclude *(PR [#32](https://github.com/ietf-tools/svgcheck/pull/32) by [@kesara](https://github.com/kesara))*
 
 ### :recycle: Refactors
@@ -146,8 +151,9 @@
 [0.5.0]: https://github.com/ietf-tools/rfc2html/compare/0.0.3...0.5.0
 [0.0.3]: https://github.com/ietf-tools/rfc2html/compare/0.0.2...0.0.3
 [0.0.2]: https://github.com/ietf-tools/rfc2html/compare/0.0.1...0.0.2
 [0.0.1]: https://github.com/ietf-tools/rfc2html/releases/tag/0.0.1
 
 [v0.6.1]: https://github.com/ietf-tools/svgcheck/compare/0.6.0...v0.6.1
 [v0.6.2]: https://github.com/ietf-tools/svgcheck/compare/v0.6.1...v0.6.2
-[v0.7.0]: https://github.com/ietf-tools/svgcheck/compare/v0.6.2...v0.7.0
+[v0.7.0]: https://github.com/ietf-tools/svgcheck/compare/v0.6.2...v0.7.0
+[v0.7.1]: https://github.com/ietf-tools/svgcheck/compare/v0.7.0...v0.7.1
```

### Comparing `svgcheck-0.7.1/LICENSE` & `svgcheck-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/PKG-INFO` & `svgcheck-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: svgcheck
-Version: 0.7.1
+Version: 0.8.0
 Summary: Verify that an svg file is compliant with the RFC standards.
 Home-page: https://github.com/ietf-tools/svgcheck
 Author: IETF Tools Team
 License: BSD-3-Clause
 Keywords: svg,validation,rfc
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml>=4.1.1
+Requires-Dist: xml2rfc>=3.16.0
 
 <div align="center">
     
 <img src="https://raw.githubusercontent.com/ietf-tools/common/main/assets/logos/svgcheck.svg" alt="SVGCHECK" height="125" />
     
 [![Release](https://img.shields.io/github/release/ietf-tools/svgcheck.svg?style=flat&maxAge=360)](https://github.com/ietf-tools/svgcheck/releases)
 [![License](https://img.shields.io/github/license/ietf-tools/svgcheck)](https://github.com/ietf-tools/svgcheck/blob/main/LICENSE)
```

### Comparing `svgcheck-0.7.1/README.md` & `svgcheck-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/setup.cfg` & `svgcheck-0.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.7.1
+version = 0.8.0
 name = svgcheck
 description = Verify that an svg file is compliant with the RFC standards.
 long_description = file:  README.md, LICENSE
 long_description_content_type = text/markdown
 keywords = svg, validation, rfc
 author = IETF Tools Team
 license = BSD-3-Clause
@@ -11,23 +11,23 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Other Audience
 	Topic :: Text Processing
 	Topic :: Text Processing :: Markup :: XML
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 
 [options]
 packages = svgcheck, svgcheck.Results, svgcheck.Tests, svgcheck.Tests.cache_saved
-python_requires = >=3.7, <3.12
+python_requires = >=3.8
 install_requires = 
 	lxml>=4.1.1
 	xml2rfc>=3.16.0
 include_package_data = True
 tests_require = 
 	pycodestyle
 	pyflakes>=0.8.1
```

### Comparing `svgcheck-0.7.1/svgcheck/Results/DrawBerry-sample-2.out` & `svgcheck-0.8.0/svgcheck/Results/DrawBerry-sample-2.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/DrawBerry-sample-2.svg` & `svgcheck-0.8.0/svgcheck/Results/DrawBerry-sample-2.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/IETF-test.out` & `svgcheck-0.8.0/svgcheck/Results/IETF-test.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/IETF-test.svg` & `svgcheck-0.8.0/svgcheck/Results/IETF-test.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/colors.err` & `svgcheck-0.8.0/svgcheck/Results/colors.err`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/colors.out` & `svgcheck-0.8.0/svgcheck/Results/colors.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/dia-sample-svg.out` & `svgcheck-0.8.0/svgcheck/Results/dia-sample-svg.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/dia-sample-svg.svg` & `svgcheck-0.8.0/svgcheck/Results/dia-sample-svg.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/example-dot.out` & `svgcheck-0.8.0/svgcheck/Results/example-dot.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/example-dot.svg` & `svgcheck-0.8.0/svgcheck/Results/example-dot.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/full-tiny.err` & `svgcheck-0.8.0/svgcheck/Results/full-tiny.err`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/full-tiny.xml` & `svgcheck-0.8.0/svgcheck/Results/full-tiny.xml`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/httpbis-proxy20-fig6.svg` & `svgcheck-0.8.0/svgcheck/Results/httpbis-proxy20-fig6.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/malformed.out` & `svgcheck-0.8.0/svgcheck/Results/malformed.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/rfc-01.xml` & `svgcheck-0.8.0/svgcheck/Results/rfc-01.xml`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/rfc-02.out` & `svgcheck-0.8.0/svgcheck/Results/rfc-02.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/rgb.out` & `svgcheck-0.8.0/svgcheck/Results/rgb.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/rgb.svg` & `svgcheck-0.8.0/svgcheck/Results/rgb.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/svg-wordle.out` & `svgcheck-0.8.0/svgcheck/Results/svg-wordle.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/svg-wordle.svg` & `svgcheck-0.8.0/svgcheck/Results/svg-wordle.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/utf8-2.svg` & `svgcheck-0.8.0/svgcheck/Results/utf8-2.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/utf8.err` & `svgcheck-0.8.0/svgcheck/Results/utf8.err`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Results/utf8.out` & `svgcheck-0.8.0/svgcheck/Results/utf8.out`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/DrawBerry-sample-2.svg` & `svgcheck-0.8.0/svgcheck/Tests/DrawBerry-sample-2.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/IETF-test.svg` & `svgcheck-0.8.0/svgcheck/Tests/IETF-test.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/cache_saved/reference.RFC.1847.xml` & `svgcheck-0.8.0/svgcheck/Tests/cache_saved/reference.RFC.1847.xml`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/colors.svg` & `svgcheck-0.8.0/svgcheck/Tests/colors.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/dia-sample-svg.svg` & `svgcheck-0.8.0/svgcheck/Tests/dia-sample-svg.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/example-dot.svg` & `svgcheck-0.8.0/svgcheck/Tests/example-dot.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/full-tiny.xml` & `svgcheck-0.8.0/svgcheck/Tests/full-tiny.xml`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/good.svg` & `svgcheck-0.8.0/svgcheck/Tests/good.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/httpbis-proxy20-fig6.svg` & `svgcheck-0.8.0/svgcheck/Tests/httpbis-proxy20-fig6.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/malformed.svg` & `svgcheck-0.8.0/svgcheck/Tests/malformed.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/rfc-svg.xml` & `svgcheck-0.8.0/svgcheck/Tests/rfc-svg.xml`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/rfc.xml` & `svgcheck-0.8.0/svgcheck/Tests/rfc.xml`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/rgb.svg` & `svgcheck-0.8.0/svgcheck/Tests/rgb.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/svg-wordle.svg` & `svgcheck-0.8.0/svgcheck/Tests/svg-wordle.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/threshold.svg` & `svgcheck-0.8.0/svgcheck/Tests/threshold.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/Tests/utf8.svg` & `svgcheck-0.8.0/svgcheck/Tests/utf8.svg`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/checksvg.py` & `svgcheck-0.8.0/svgcheck/checksvg.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             if '%' in triple[0]:
                 shade = sum([int(t.replace('%', ''))*255/100 for t in triple])
             else:
                 shade = sum([int(t) for t in triple])
         else:
             shade = 0
 
-        log.note(u"Color or grayscale heuristic applied to: '{0}' yields shade: '{1}'".
+        log.note("Color or grayscale heuristic applied to: '{0}' yields shade: '{1}'".
                  format(v, shade))
         if shade > wp.color_threshold:
             return (False, 'white')
         return (False, wp.color_default)
 
     return (False, replaceWith)
 
@@ -232,20 +232,20 @@
                 pass
             else:
                 ok, new_val = value_ok(attr, val)
                 if vals and not ok:
                     errorCount += 1
                     if new_val is not None:
                         el.attrib[attr] = new_val
-                        log.warn(u"The attribute '{1}' does not allow the value '{0}',"
-                                 u" replaced with '{2}'".format(val, attr, new_val), where=el)
+                        log.warn("The attribute '{1}' does not allow the value '{0}',"
+                                 " replaced with '{2}'".format(val, attr, new_val), where=el)
                     else:
                         attribs_to_remove.append(nsAttrib)
-                        log.warn(u"The attribute '{1}' does not allow the value '{0}',"
-                                 u" attribute to be removed".format(val, attr), where=el)
+                        log.warn("The attribute '{1}' does not allow the value '{0}',"
+                                 " attribute to be removed".format(val, attr), where=el)
 
     for attrib in attribs_to_remove:
         del el.attrib[attrib]
 
     # Need to have a viewBox on the root
     if (depth == 0):
         if el.get("viewBox"):
```

### Comparing `svgcheck-0.7.1/svgcheck/log.py` & `svgcheck-0.8.0/svgcheck/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         prefix = "{0}:{1}: ".format(fileName, where.sourceline)
     if 'file' in kwargs:
         fileName = make_relative(kwargs['file'])
         prefix = "{0}:{1}: ".format(fileName, kwargs['line'])
     if 'additional' in kwargs:
         prefix = ' ' * kwargs['additional']
 
-    write_err.write(prefix + u' '.join(args))
+    write_err.write(prefix + ' '.join(args))
     write_err.write('\n')
     write_err.flush()
 
 
 def exception(message, list):
     error(message)
     if isinstance(list, Exception):
```

### Comparing `svgcheck-0.7.1/svgcheck/run.py` & `svgcheck-0.8.0/svgcheck/run.py`

 * *Files identical despite different names*

### Comparing `svgcheck-0.7.1/svgcheck/test.py` & `svgcheck-0.8.0/svgcheck/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pycodestyle
 import unittest
 import os
 import shutil
 import lxml.etree
 import subprocess
-import six
 import sys
 from xml2rfc.parser import XmlRfcParser
 import difflib
 from svgcheck.checksvg import checkTree
 from svgcheck import log
 import io
 
@@ -42,17 +41,16 @@
     def test_pyflakes_confrmance(self):
         p = subprocess.Popen(['pyflakes', 'run.py', 'checksvg.py', 'test.py',
                               'word_properties.py'],
                              stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         (stdoutX, stderrX) = p.communicate()
         ret = p.wait()
         if ret > 0:
-            if six.PY3:
-                stdoutX = stdoutX.decode('utf-8')
-                stderrX = stderrX.decode('utf-8')
+            stdoutX = stdoutX.decode('utf-8')
+            stderrX = stderrX.decode('utf-8')
             print(stdoutX)
             print(stderrX)
             self.assertEqual(ret, 0)
 
 
 class TestCommandLineOptions(unittest.TestCase):
     """ Run a set of command line checks to make sure they work """
@@ -217,15 +215,15 @@
 
 
 def check_results(file1, file2Name):
     """  Compare two files and say what the differences are or even if there are
          any differences
     """
 
-    with io.open(file2Name, 'r', encoding='utf-8') as f:
+    with open(file2Name, encoding='utf-8') as f:
         lines2 = f.readlines()
 
     if os.name == 'nt' and (file2Name.endswith(".out") or file2Name.endswith(".err")):
         lines2 = [line.replace('Tests/', 'Tests\\').replace('Temp/', 'Temp\\') for line in lines2]
 
     if not file2Name.endswith(".out"):
         cwd = os.getcwd()
@@ -262,21 +260,18 @@
         args = args[1:]
     p = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     (stdoutX, stderr) = p.communicate()
     p.wait()
 
     returnValue = True
     if stdoutFile is not None:
-        with io.open(stdoutFile, 'r', encoding='utf-8') as f:
+        with open(stdoutFile, encoding='utf-8') as f:
             lines2 = f.readlines()
 
-        if six.PY2:
-            lines1 = stdoutX.decode('utf-8').splitlines(True)
-        else:
-            lines1 = stdoutX.decode('utf-8').splitlines(True)
+        lines1 = stdoutX.decode('utf-8').splitlines(True)
 
         if os.name == 'nt':
             lines2 = [line.replace('Tests/', 'Tests\\').replace('Temp/', 'Temp\\')
                       for line in lines2]
             lines1 = [line.replace('\r', '') for line in lines1]
 
         d = difflib.Differ()
@@ -285,25 +280,22 @@
         hasError = False
         for line in result:
             if line[0:2] == '+ ' or line[0:2] == '- ':
                 hasError = True
                 break
         if hasError:
             print("stdout:")
-            print(u"".join(result))
+            print("".join(result))
             returnValue = False
 
     if errFile is not None:
-        with io.open(errFile, 'r', encoding='utf-8') as f:
+        with open(errFile, encoding='utf-8') as f:
             lines2 = f.readlines()
 
-        if six.PY2:
-            lines1 = stderr.decode('utf-8').splitlines(True)
-        else:
-            lines1 = stderr.decode('utf-8').splitlines(True)
+        lines1 = stderr.decode('utf-8').splitlines(True)
 
         if os.name == 'nt':
             lines2 = [line.replace('Tests/', 'Tests\\').replace('Temp/', 'Temp\\')
                       for line in lines2]
             lines1 = [line.replace('\r', '') for line in lines1]
 
         d = difflib.Differ()
@@ -316,32 +308,32 @@
                 break
         if hasError:
             print("stderr")
             print("".join(result))
             returnValue = False
 
     if generatedFile is not None:
-        with io.open(generatedFile, 'r', encoding='utf-8') as f:
+        with open(generatedFile, encoding='utf-8') as f:
             lines2 = f.readlines()
 
-        with io.open(compareFile, 'r', encoding='utf-8') as f:
+        with open(compareFile, encoding='utf-8') as f:
             lines1 = f.readlines()
 
         d = difflib.Differ()
         result = list(d.compare(lines1, lines2))
 
         hasError = False
         for line in result:
             if line[0:2] == '+ ' or line[0:2] == '- ':
                 hasError = True
                 break
 
         if hasError:
             print(generatedFile)
-            print(u"".join(result))
+            print("".join(result))
             returnValue = False
 
     tester.assertTrue(returnValue, "Comparisons failed")
 
 
 def clear_cache(parser):
     parser.delete_cache()
```

### Comparing `svgcheck-0.7.1/svgcheck/word_properties.py` & `svgcheck-0.8.0/svgcheck/word_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,16 +172,14 @@
     'direction':           ('ltr', 'rtl', 'inherit'),
     'unicode-bidi':        ('normal', 'embed', 'bidi-override', 'inherit'),
     'text-anchor':         ('start', 'middle', 'end', 'inherit'),
     'fill':                ('none', 'inherit', '<color>'),  # # = RGB val
     'fill-rule':           ('nonzero', 'evenodd', 'inherit'),
     'fill-opacity':        (),  # 'inherit'
 
-    'height':              ('<number>',),
-
     'requiredFeatures': (),
     'requiredFormats': (),
     'requiredExtensions': (),
     'requiredFonts': (),
     'systemLanguage': ()
 }
```

### Comparing `svgcheck-0.7.1/svgcheck.egg-info/PKG-INFO` & `svgcheck-0.8.0/svgcheck.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: svgcheck
-Version: 0.7.1
+Version: 0.8.0
 Summary: Verify that an svg file is compliant with the RFC standards.
 Home-page: https://github.com/ietf-tools/svgcheck
 Author: IETF Tools Team
 License: BSD-3-Clause
 Keywords: svg,validation,rfc
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml>=4.1.1
+Requires-Dist: xml2rfc>=3.16.0
 
 <div align="center">
     
 <img src="https://raw.githubusercontent.com/ietf-tools/common/main/assets/logos/svgcheck.svg" alt="SVGCHECK" height="125" />
     
 [![Release](https://img.shields.io/github/release/ietf-tools/svgcheck.svg?style=flat&maxAge=360)](https://github.com/ietf-tools/svgcheck/releases)
 [![License](https://img.shields.io/github/license/ietf-tools/svgcheck)](https://github.com/ietf-tools/svgcheck/blob/main/LICENSE)
```

### Comparing `svgcheck-0.7.1/svgcheck.egg-info/SOURCES.txt` & `svgcheck-0.8.0/svgcheck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

