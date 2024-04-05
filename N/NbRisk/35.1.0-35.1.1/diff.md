# Comparing `tmp/NbRisk-35.1.0.tar.gz` & `tmp/NbRisk-35.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NbRisk-35.1.0.tar", last modified: Sun Aug 20 02:31:46 2023, max compression
+gzip compressed data, was "NbRisk-35.1.1.tar", last modified: Fri Apr  5 18:54:29 2024, max compression
```

## Comparing `NbRisk-35.1.0.tar` & `NbRisk-35.1.1.tar`

### file list

```diff
@@ -1,60 +1,74 @@
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-08-20 02:31:46.686333 NbRisk-35.1.0/
--rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-35.1.0/LICENSE
--rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-35.1.0/MANIFEST.in
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-08-20 02:31:46.614331 NbRisk-35.1.0/NbRisk.egg-info/
--rw-rw-r--   0 renato    (1000) renato    (1000)     3209 2023-08-20 02:31:46.000000 NbRisk-35.1.0/NbRisk.egg-info/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     1719 2023-08-20 02:31:46.000000 NbRisk-35.1.0/NbRisk.egg-info/SOURCES.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-08-20 02:31:46.000000 NbRisk-35.1.0/NbRisk.egg-info/dependency_links.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-08-20 02:31:46.000000 NbRisk-35.1.0/NbRisk.egg-info/top_level.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)     3209 2023-08-20 02:31:46.686333 NbRisk-35.1.0/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2780 2023-08-20 02:22:34.000000 NbRisk-35.1.0/README.md
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-08-20 02:31:46.638332 NbRisk-35.1.0/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-35.1.0/nb_risk/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-35.1.0/nb_risk/admin.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-08-20 02:31:46.646332 NbRisk-35.1.0/nb_risk/api/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.0/nb_risk/api/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-35.1.0/nb_risk/api/nested_serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5107 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/api/serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-35.1.0/nb_risk/api/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-35.1.0/nb_risk/api/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-35.1.0/nb_risk/choices.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-35.1.0/nb_risk/columns.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-35.1.0/nb_risk/cve.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-35.1.0/nb_risk/filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4997 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/forms.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.0/nb_risk/middleware.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-08-20 02:31:46.662332 NbRisk-35.1.0/nb_risk/migrations/
--rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-35.1.0/nb_risk/migrations/0001_initial.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-35.1.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-35.1.0/nb_risk/migrations/0003_control.py
--rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-35.1.0/nb_risk/migrations/0004_alter_vulnerability_options.py
--rw-r--r--   0 renato    (1000) renato    (1000)      434 2023-05-13 16:13:09.000000 NbRisk-35.1.0/nb_risk/migrations/0005_alter_vulnerability_cvssbasescore.py
--rw-r--r--   0 renato    (1000) renato    (1000)      424 2023-05-13 17:11:12.000000 NbRisk-35.1.0/nb_risk/migrations/0006_vulnerability_unique_vuln_name.py
--rw-r--r--   0 renato    (1000) renato    (1000)      615 2023-08-20 02:18:04.000000 NbRisk-35.1.0/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-35.1.0/nb_risk/migrations/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     8712 2023-08-20 02:17:50.000000 NbRisk-35.1.0/nb_risk/models.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-35.1.0/nb_risk/navigation.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.0/nb_risk/signals.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4050 2023-05-12 20:01:49.000000 NbRisk-35.1.0/nb_risk/tables.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      803 2023-08-20 02:15:03.000000 NbRisk-35.1.0/nb_risk/template_content.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-08-20 02:31:46.606330 NbRisk-35.1.0/nb_risk/templates/
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-08-20 02:31:46.686333 NbRisk-35.1.0/nb_risk/templates/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/control.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/control_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/control_risks.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/generic_vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/risk.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/threatevent.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/threatsource.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/vulnerability.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-35.1.0/nb_risk/templates/nb_risk/vulnerability_search.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     4982 2023-05-12 19:59:37.000000 NbRisk-35.1.0/nb_risk/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       23 2023-08-20 02:25:18.000000 NbRisk-35.1.0/nb_risk/version.py
--rw-rw-r--   0 renato    (1000) renato    (1000)    10234 2023-08-20 02:15:59.000000 NbRisk-35.1.0/nb_risk/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-08-20 02:31:46.686333 NbRisk-35.1.0/setup.cfg
--rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-35.1.0/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.389345 NbRisk-35.1.1/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-35.1.1/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-35.1.1/MANIFEST.in
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.385345 NbRisk-35.1.1/NbRisk.egg-info/
+-rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-04-05 18:54:29.000000 NbRisk-35.1.1/NbRisk.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2091 2024-04-05 18:54:29.000000 NbRisk-35.1.1/NbRisk.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2024-04-05 18:54:29.000000 NbRisk-35.1.1/NbRisk.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        8 2024-04-05 18:54:29.000000 NbRisk-35.1.1/NbRisk.egg-info/top_level.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-04-05 18:54:29.385345 NbRisk-35.1.1/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2780 2024-04-05 18:53:39.000000 NbRisk-35.1.1/README.md
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.353345 NbRisk-35.1.1/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      715 2024-04-05 18:50:37.000000 NbRisk-35.1.1/nb_risk/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-35.1.1/nb_risk/admin.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.357345 NbRisk-35.1.1/nb_risk/api/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.1/nb_risk/api/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-35.1.1/nb_risk/api/nested_serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5107 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/api/serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-35.1.1/nb_risk/api/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-35.1.1/nb_risk/api/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-35.1.1/nb_risk/choices.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-35.1.1/nb_risk/columns.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-35.1.1/nb_risk/cve.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1975 2024-04-05 18:31:15.000000 NbRisk-35.1.1/nb_risk/filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5607 2024-03-23 01:17:05.000000 NbRisk-35.1.1/nb_risk/forms.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.1/nb_risk/middleware.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.361345 NbRisk-35.1.1/nb_risk/migrations/
+-rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-35.1.1/nb_risk/migrations/0001_initial.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-35.1.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-35.1.1/nb_risk/migrations/0003_control.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-35.1.1/nb_risk/migrations/0004_alter_vulnerability_options.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      434 2023-05-13 16:13:09.000000 NbRisk-35.1.1/nb_risk/migrations/0005_alter_vulnerability_cvssbasescore.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      424 2023-05-13 17:11:12.000000 NbRisk-35.1.1/nb_risk/migrations/0006_vulnerability_unique_vuln_name.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      615 2023-08-20 02:18:04.000000 NbRisk-35.1.1/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-35.1.1/nb_risk/migrations/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     8712 2023-08-20 02:17:50.000000 NbRisk-35.1.1/nb_risk/models.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-35.1.1/nb_risk/navigation.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.1/nb_risk/signals.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4050 2023-05-12 20:01:49.000000 NbRisk-35.1.1/nb_risk/tables.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      803 2023-08-20 02:15:03.000000 NbRisk-35.1.1/nb_risk/template_content.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.337345 NbRisk-35.1.1/nb_risk/templates/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.377345 NbRisk-35.1.1/nb_risk/templates/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/control.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/control_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/control_risks.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/generic_vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/risk.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/threatevent.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/threatsource.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_search.html
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.377345 NbRisk-35.1.1/nb_risk/tests/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 00:49:42.000000 NbRisk-35.1.1/nb_risk/tests/__init__.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.377345 NbRisk-35.1.1/nb_risk/tests/control/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:28.000000 NbRisk-35.1.1/nb_risk/tests/control/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1133 2024-03-23 00:50:09.000000 NbRisk-35.1.1/nb_risk/tests/custom.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.381345 NbRisk-35.1.1/nb_risk/tests/threatsource/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:12.000000 NbRisk-35.1.1/nb_risk/tests/threatsource/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1900 2024-04-05 18:41:28.000000 NbRisk-35.1.1/nb_risk/tests/threatsource/test_api.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2158 2024-03-31 19:52:14.000000 NbRisk-35.1.1/nb_risk/tests/threatsource/test_filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2359 2024-04-05 18:34:59.000000 NbRisk-35.1.1/nb_risk/tests/threatsource/test_views.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.385345 NbRisk-35.1.1/nb_risk/tests/vulnerability/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-05 18:16:40.000000 NbRisk-35.1.1/nb_risk/tests/vulnerability/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1809 2024-04-05 18:28:15.000000 NbRisk-35.1.1/nb_risk/tests/vulnerability/test_filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1982 2024-04-05 18:35:09.000000 NbRisk-35.1.1/nb_risk/tests/vulnerability/test_views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4410 2024-03-23 01:58:21.000000 NbRisk-35.1.1/nb_risk/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       23 2024-04-05 18:53:47.000000 NbRisk-35.1.1/nb_risk/version.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10772 2024-03-23 01:43:26.000000 NbRisk-35.1.1/nb_risk/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       38 2024-04-05 18:54:29.389345 NbRisk-35.1.1/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-35.1.1/setup.py
```

### Comparing `NbRisk-35.1.0/LICENSE` & `NbRisk-35.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/NbRisk.egg-info/PKG-INFO` & `NbRisk-35.1.1/NbRisk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.1.0
+Version: 35.1.1
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-35.1.0/NbRisk.egg-info/SOURCES.txt` & `NbRisk-35.1.1/NbRisk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -44,8 +44,18 @@
 nb_risk/templates/nb_risk/threatevent.html
 nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
 nb_risk/templates/nb_risk/threatsource.html
 nb_risk/templates/nb_risk/vulnerability.html
 nb_risk/templates/nb_risk/vulnerability_affected_assets.html
 nb_risk/templates/nb_risk/vulnerability_assignment_button.html
 nb_risk/templates/nb_risk/vulnerability_list.html
-nb_risk/templates/nb_risk/vulnerability_search.html
+nb_risk/templates/nb_risk/vulnerability_search.html
+nb_risk/tests/__init__.py
+nb_risk/tests/custom.py
+nb_risk/tests/control/__init__.py
+nb_risk/tests/threatsource/__init__.py
+nb_risk/tests/threatsource/test_api.py
+nb_risk/tests/threatsource/test_filters.py
+nb_risk/tests/threatsource/test_views.py
+nb_risk/tests/vulnerability/__init__.py
+nb_risk/tests/vulnerability/test_filters.py
+nb_risk/tests/vulnerability/test_views.py
```

### Comparing `NbRisk-35.1.0/PKG-INFO` & `NbRisk-35.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.1.0
+Version: 35.1.1
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-35.1.0/README.md` & `NbRisk-35.1.1/README.md`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/__init__.py` & `NbRisk-35.1.1/nb_risk/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     name = "nb_risk"
     base_url = "nb_risk"
     verbose_name = "Risk Management"
     description = "NIST 800-30 Risk Management for Netbox"
     version = __version__
     author = "Renato Almdida Oliveira"
     author_email = "renato.almeida.oliveira@gmail.com"
+    min_version = "3.5.0"
+    max_version = "3.7.99"
     required_settings = []
     default_settings = {
         "supported_assets": [
             "dcim.device",
             "virtualization.virtualmachine",
             "tenancy.tenant",
             "dcim.site",
```

### Comparing `NbRisk-35.1.0/nb_risk/api/nested_serializers.py` & `NbRisk-35.1.1/nb_risk/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/api/serializers.py` & `NbRisk-35.1.1/nb_risk/api/serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/api/views.py` & `NbRisk-35.1.1/nb_risk/api/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/choices.py` & `NbRisk-35.1.1/nb_risk/choices.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/columns.py` & `NbRisk-35.1.1/nb_risk/columns.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/cve.py` & `NbRisk-35.1.1/nb_risk/cve.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/filters.py` & `NbRisk-35.1.1/nb_risk/filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # ThreatSource Filters
 
 
 class ThreatSourceFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = models.ThreatSource
-        fields = ["threat_type", "capability", "intent", "targeting"]
+        fields = ["id", "name", "threat_type", "capability", "intent", "targeting"]
 
 
 # ThreatEvent Filters
 
 
 class ThreatEventFilterSet(NetBoxModelFilterSet):
     class Meta:
@@ -24,15 +24,27 @@
 # Vulnerability Filters
 
 
 class VulnerabilityFilterSet(NetBoxModelFilterSet):
 
     class Meta:
         model = models.Vulnerability
-        fields = ("name", "cve",)
+        fields = [
+            "id",
+            "name",
+            "cve",
+            "description",
+            "cvssaccessVector",
+            "cvssaccessComplexity",
+            "cvssauthentication",
+            "cvssconfidentialityImpact",
+            "cvssintegrityImpact",
+            "cvssavailabilityImpact",
+            "cvssbaseScore",
+            ]
 
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
         qs_filter = (
             Q(name__icontains=value)
             | Q(cve__icontains=value)
```

### Comparing `NbRisk-35.1.0/nb_risk/forms.py` & `NbRisk-35.1.1/nb_risk/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from django import forms
 
-from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelImportForm
+from netbox.forms import (
+    NetBoxModelForm,
+    NetBoxModelFilterSetForm,
+    NetBoxModelBulkEditForm,
+    NetBoxModelImportForm,
+)
+
 from dcim.models import Device, DeviceType
 from utilities.forms import BootstrapMixin
 from utilities.forms.fields import (
     DynamicModelMultipleChoiceField,
     SlugField,
     DynamicModelChoiceField,
 )
@@ -31,14 +37,36 @@
 class ThreatSourceFilterForm(NetBoxModelFilterSetForm):
     model = models.ThreatSource
 
     class Meta:
         fields = ["name", "threat_type", "capability", "intent", "targeting"]
 
 
+class ThreatSourceImportForm(NetBoxModelImportForm):
+    class Meta:
+        model = models.ThreatSource
+        fields = [
+            "name",
+            "threat_type",
+            "capability",
+            "intent",
+            "targeting",
+            "description",
+            "notes",
+        ]
+
+class ThreatSourceBulkEditForm(NetBoxModelBulkEditForm):
+    model = models.ThreatSource
+
+    comments = forms.Textarea(
+        attrs={'class': 'font-monospace'}
+    )
+
+    class Meta:
+        nullable_fields = ("intent", "targeting", "description", "notes")
 # ThreatEvent Forms
 
 
 class ThreatEventForm(NetBoxModelForm):
 
     vulnerability = DynamicModelMultipleChoiceField(
         queryset=models.VulnerabilityAssignment.objects.all(),
```

### Comparing `NbRisk-35.1.0/nb_risk/migrations/0001_initial.py` & `NbRisk-35.1.1/nb_risk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py` & `NbRisk-35.1.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/migrations/0003_control.py` & `NbRisk-35.1.1/nb_risk/migrations/0003_control.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py` & `NbRisk-35.1.1/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/models.py` & `NbRisk-35.1.1/nb_risk/models.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/navigation.py` & `NbRisk-35.1.1/nb_risk/navigation.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/tables.py` & `NbRisk-35.1.1/nb_risk/tables.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/template_content.py` & `NbRisk-35.1.1/nb_risk/template_content.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/templates/nb_risk/control.html` & `NbRisk-35.1.1/nb_risk/templates/nb_risk/control.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html` & `NbRisk-35.1.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/templates/nb_risk/risk.html` & `NbRisk-35.1.1/nb_risk/templates/nb_risk/risk.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/templates/nb_risk/threatevent.html` & `NbRisk-35.1.1/nb_risk/templates/nb_risk/threatevent.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/templates/nb_risk/threatsource.html` & `NbRisk-35.1.1/nb_risk/templates/nb_risk/threatsource.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/templates/nb_risk/vulnerability.html` & `NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/templates/nb_risk/vulnerability_search.html` & `NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_search.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.0/nb_risk/urls.py` & `NbRisk-35.1.1/nb_risk/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,142 +4,59 @@
 
 from . import models, views, cve
 
 app_name = 'nb_risk'
 
 urlpatterns = (
     # ThreatSource URLs
-    path(
-        "threat-source/", views.ThreatSourceListView.as_view(), name="threatsource_list"
-    ),
-    path(
-        "threat-source/add/",
-        views.ThreatSourceEditView.as_view(),
-        name="threatsource_add",
-    ),
-    path(
-        "threat-source/<int:pk>/", views.ThreatSourceView.as_view(), name="threatsource"
-    ),
-    path(
-        "threat-source/<int:pk>/edit/",
-        views.ThreatSourceEditView.as_view(),
-        name="threatsource_edit",
-    ),
-    path(
-        "threat-source/<int:pk>/delete/",
-        views.ThreatSourceDeleteView.as_view(),
-        name="threatsource_delete",
-    ),
-    path(
-        "threat-source/<int:pk>/changelog/",
-        ObjectChangeLogView.as_view(),
-        name="threatsource_changelog",
-        kwargs={"model": models.ThreatSource},
-    ),
+    path("threat-source/", views.ThreatSourceListView.as_view(), name="threatsource_list"),
+    path("threat-source/add/",views.ThreatSourceEditView.as_view(),name="threatsource_add"),
+    path("threat-source/<int:pk>/", views.ThreatSourceView.as_view(), name="threatsource"),
+    path('threat-source/<int:pk>/', include(get_model_urls(app_name, 'threatsource'))),
+    path("threat-source/<int:pk>/edit/",views.ThreatSourceEditView.as_view(),name="threatsource_edit"),
+    path("threat-source/<int:pk>/delete/",views.ThreatSourceDeleteView.as_view(), name="threatsource_delete"),
+    path('threat-source/import/', views.ThreatSourceImportView.as_view(), name='threatsource_import'),
+    path('threat-source/edit/', views.ThreatSourceBulkEditView.as_view(), name='threatsource_bulk_edit'),
+    path('threat-source/delete/', views.ThreatSourceBulkDeleteView.as_view(), name='threatsource_bulk_delete'),
+
     # ThreatEvent URLs
     path("threat-event/", views.ThreatEventListView.as_view(), name="threatevent_list"),
-    path(
-        "threat-event/add/", views.ThreatEventEditView.as_view(), name="threatevent_add"
-    ),
+    path("threat-event/add/", views.ThreatEventEditView.as_view(), name="threatevent_add"),
     path("threat-event/<int:pk>/", views.ThreatEventView.as_view(), name="threatevent"),
     path('threat-event/<int:pk>/', include(get_model_urls(app_name, 'threatevent'))),
-    path(
-        "threat-event/<int:pk>/edit/",
-        views.ThreatEventEditView.as_view(),
-        name="threatevent_edit",
-    ),
-    path(
-        "threat-event/<int:pk>/delete/",
-        views.ThreatEventDeleteView.as_view(),
-        name="threatevent_delete",
-    ),
-    path(
-        "threat-event/delete/",
-        views.ThreatEventBulkDeleteView.as_view(),
-        name="threatevent_bulk_delete",
-    ),
+    path("threat-event/<int:pk>/edit/", views.ThreatEventEditView.as_view(),name="threatevent_edit",),
+    path("threat-event/<int:pk>/delete/", views.ThreatEventDeleteView.as_view(), name="threatevent_delete",),
+    path("threat-event/delete/", views.ThreatEventBulkDeleteView.as_view(), name="threatevent_bulk_delete",),
+
     # Vulnerability URLs
-    path(
-        "vulnerability/",
-        views.VulnerabilityListView.as_view(),
-        name="vulnerability_list",
-    ),
-    path(
-        "vulnerability/add/",
-        views.VulnerabilityEditView.as_view(),
-        name="vulnerability_add",
-    ),
-    path(
-        "vulnerability/<int:pk>/",
-        views.VulnerabilityView.as_view(),
-        name="vulnerability",
-    ),
-    path(
-        "vulnerability/<int:pk>/edit/",
-        views.VulnerabilityEditView.as_view(),
-        name="vulnerability_edit",
-    ),
+    path("vulnerability/", views.VulnerabilityListView.as_view(), name="vulnerability_list",),
+    path("vulnerability/add/", views.VulnerabilityEditView.as_view(), name="vulnerability_add",),
+    path("vulnerability/<int:pk>/", views.VulnerabilityView.as_view(), name="vulnerability",),
+    path("vulnerability/<int:pk>/edit/", views.VulnerabilityEditView.as_view(), name="vulnerability_edit",),
     path('vulnerability/import/', views.VulnerabilityBulkImportView.as_view(), name='vulnerability_import'),
-    path(
-        "vulnerability/<int:pk>/delete/",
-        views.VulnerabilityDeleteView.as_view(),
-        name="vulnerability_delete",
-    ),
-    path(
-        "vulnerability/delete/",
-        views.VulnerabilityBulkDeleteView.as_view(),
-        name="vulnerability_bulk_delete",
-    ),
+    path("vulnerability/<int:pk>/delete/", views.VulnerabilityDeleteView.as_view(), name="vulnerability_delete",),
+    path("vulnerability/delete/", views.VulnerabilityBulkDeleteView.as_view(), name="vulnerability_bulk_delete",),
     path('vulnerability/<int:pk>/', include(get_model_urls(app_name, 'vulnerability'))),
-    path(
-        "vulnerability/search/",
-        cve.VulnerabilitySearchView.as_view(),
-        name="vulnerability_search",
-    ),
+    path("vulnerability/search/", cve.VulnerabilitySearchView.as_view(), name="vulnerability_search",),
+
     # VulnerabilityAssignment URLs
-    path(
-        "vulnerability-assignments/add/",
-        views.VulnerabilityAssignmentEditView.as_view(),
-        name="vulnerabilityassignment_add",
-    ),
-    path("vulnerability-assignments/",
-        views.VulnerabilityAssignmentListView.as_view(),
-        name="vulnerabilityassignment_list",
-    ),
-    path(
-        "vulnerability-assignments/<int:pk>/delete/",
-        views.VulnerabilityAssignmentDeleteView.as_view(),
-        name="vulnerabilityassignment_delete",
-    ),
+    path("vulnerability-assignments/add/", views.VulnerabilityAssignmentEditView.as_view(), name="vulnerabilityassignment_add",),
+    path("vulnerability-assignments/", views.VulnerabilityAssignmentListView.as_view(), name="vulnerabilityassignment_list",),
+    path("vulnerability-assignments/<int:pk>/delete/", views.VulnerabilityAssignmentDeleteView.as_view(), name="vulnerabilityassignment_delete",),
     # Risk URLs
     path("risk/", views.RiskListView.as_view(), name="risk_list"),
     path("risk/add/", views.RiskEditView.as_view(), name="risk_add"),
     path("risk/<int:pk>/", views.RiskView.as_view(), name="risk"),
+    path('risk/<int:pk>/', include(get_model_urls(app_name, 'risk'))),
     path("risk/<int:pk>/edit/", views.RiskEditView.as_view(), name="risk_edit"),
     path("risk/<int:pk>/delete/", views.RiskDeleteView.as_view(), name="risk_delete"),
     path("risk/delete/", views.RiskBulkDeleteView.as_view(), name="risk_bulk_delete"),
-    path(
-        "risk/<int:pk>/changelog/",
-        ObjectChangeLogView.as_view(),
-        name="risk_changelog",
-        kwargs={"model": models.Risk},
-    ),
-    path(
-        "risk/<int:pk>/journal/",
-        ObjectJournalView.as_view(),
-        name="risk_journal",
-        kwargs={"model": models.Risk},
-    ),
+
     # Control URLs
     path("control/", views.ControlListView.as_view(), name="control_list"),
     path("control/add/", views.ControlEditView.as_view(), name="control_add"),
     path("control/<int:pk>/", views.ControlView.as_view(), name="control"),
     path("control/<int:pk>/edit/", views.ControlEditView.as_view(), name="control_edit"),
-    path(
-        "control/<int:pk>/delete/", views.ControlDeleteView.as_view(), name="control_delete"
-    ),
-    path(
-        "control/delete/", views.ControlBulkDeleteView.as_view(), name="control_bulk_delete"
-    ),
-    path('control/<int:pk>/', include(get_model_urls(app_name, 'control'))),
-    
+    path("control/<int:pk>/delete/", views.ControlDeleteView.as_view(), name="control_delete"),
+    path("control/delete/", views.ControlBulkDeleteView.as_view(), name="control_bulk_delete"),
+    path('control/<int:pk>/', include(get_model_urls(app_name, 'control'))),    
 )
```

### Comparing `NbRisk-35.1.0/nb_risk/views.py` & `NbRisk-35.1.1/nb_risk/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from netbox.views import generic
 from dcim.models import Device, Site
 from tenancy.models import Tenant
 from virtualization.models import VirtualMachine
+from core.models import ContentType
 
 from extras.plugins.utils import get_plugin_config
 from utilities.views import ViewTab, register_model_view
-from django.contrib.contenttypes.models import ContentType
 from django.shortcuts import get_object_or_404
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 from . import forms, models, tables, filters
@@ -29,14 +29,29 @@
 
 
 class ThreatSourceEditView(generic.ObjectEditView):
     queryset = models.ThreatSource.objects.all()
     form = forms.ThreatSourceForm
 
 
+class ThreatSourceImportView(generic.BulkImportView):
+    queryset = models.ThreatSource.objects.all()
+    model_form = forms.ThreatSourceImportForm
+    table = tables.ThreatSourceTable
+
+class ThreatSourceBulkEditView(generic.BulkEditView):
+    queryset = models.ThreatSource.objects.all()
+    filterset = filters.ThreatSourceFilterSet
+    table = tables.ThreatSourceTable
+    form = forms.ThreatSourceBulkEditForm
+
+class ThreatSourceBulkDeleteView(generic.BulkDeleteView):
+    queryset = models.ThreatSource.objects.all()
+    table = tables.ThreatSourceTable
+
 class ThreatSourceDeleteView(generic.ObjectDeleteView):
     queryset = models.ThreatSource.objects.all()
 
 
 # ThreatEvent Views
```

### Comparing `NbRisk-35.1.0/setup.py` & `NbRisk-35.1.1/setup.py`

 * *Files identical despite different names*

