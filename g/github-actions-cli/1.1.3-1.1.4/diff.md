# Comparing `tmp/github_actions_cli-1.1.3.tar.gz` & `tmp/github_actions_cli-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_actions_cli-1.1.3.tar", max compression
+gzip compressed data, was "github_actions_cli-1.1.4.tar", max compression
```

## Comparing `github_actions_cli-1.1.3.tar` & `github_actions_cli-1.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1500 2024-01-28 14:41:41.547705 github_actions_cli-1.1.3/LICENSE
--rw-r--r--   0        0        0     3609 2024-01-28 15:37:51.574705 github_actions_cli-1.1.3/README.md
--rw-r--r--   0        0        0        0 2024-01-28 14:41:41.547916 github_actions_cli-1.1.3/gha_cli/__init__.py
--rwxr-xr-x   0        0        0    13032 2024-02-16 16:53:03.713630 github_actions_cli-1.1.3/gha_cli/cli.py
--rw-r--r--   0        0        0     2915 2024-02-05 17:04:53.703619 github_actions_cli-1.1.3/gha_cli/scanner.py
--rw-r--r--   0        0        0     1663 2024-02-16 16:53:35.355471 github_actions_cli-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 github_actions_cli-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1500 2024-04-05 10:09:44.316464 github_actions_cli-1.1.4/LICENSE
+-rw-r--r--   0        0        0     3609 2024-04-05 10:09:44.316464 github_actions_cli-1.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 10:09:44.316464 github_actions_cli-1.1.4/gha_cli/__init__.py
+-rwxr-xr-x   0        0        0    13032 2024-04-05 10:09:44.316464 github_actions_cli-1.1.4/gha_cli/cli.py
+-rw-r--r--   0        0        0     2915 2024-04-05 10:09:44.316464 github_actions_cli-1.1.4/gha_cli/scanner.py
+-rw-r--r--   0        0        0     1663 2024-04-05 10:10:51.671034 github_actions_cli-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 github_actions_cli-1.1.4/PKG-INFO
```

### Comparing `github_actions_cli-1.1.3/LICENSE` & `github_actions_cli-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `github_actions_cli-1.1.3/README.md` & `github_actions_cli-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `github_actions_cli-1.1.3/gha_cli/cli.py` & `github_actions_cli-1.1.4/gha_cli/cli.py`

 * *Files identical despite different names*

### Comparing `github_actions_cli-1.1.3/gha_cli/scanner.py` & `github_actions_cli-1.1.4/gha_cli/scanner.py`

 * *Files identical despite different names*

### Comparing `github_actions_cli-1.1.3/pyproject.toml` & `github_actions_cli-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry.scripts]
 github-actions-cli = "gha_cli.cli:cli"
 #github-scanner = "gha_cli.scanner:cli"
 
 [tool.poetry]
 name = "github-actions-cli"
-version = "1.1.3"
+version = "1.1.4"
 description = "GitHub Actions CLI - allows updating workflows, etc."
 readme = "README.md"
 keywords = ["GitHub Actions", "CLI"]
 packages = [
     { include = "gha_cli" },
 ]
```

### Comparing `github_actions_cli-1.1.3/PKG-INFO` & `github_actions_cli-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-actions-cli
-Version: 1.1.3
+Version: 1.1.4
 Summary: GitHub Actions CLI - allows updating workflows, etc.
 Home-page: https://github.com/dsoftwareinc/github-actions-cli
 License: BSD-3-Clause
 Keywords: GitHub Actions,CLI
 Author: Daniel Moran
 Author-email: daniel@moransoftware.ca
 Maintainer: Daniel Moran
```

