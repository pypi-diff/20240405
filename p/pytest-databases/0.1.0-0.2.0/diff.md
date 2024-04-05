# Comparing `tmp/pytest_databases-0.1.0.tar.gz` & `tmp/pytest_databases-0.2.0.tar.gz`

## Comparing `pytest_databases-0.1.0.tar` & `pytest_databases-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/__metadata__.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/py.typed
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/__init__.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/cockroachdb.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/docker-compose.yml
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/mariadb.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/mssql.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/mysql.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/oracle.py
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/postgres.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pytest_databases/docker/spanner.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/LICENSE
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/README.md
--rw-r--r--   0        0        0    16747 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/PKG-INFO
--rw-r--r--   0        0        0    10238 2020-02-02 00:00:00.000000 pytest_databases-0.1.0/setup.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/__metadata__.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/py.typed
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/__init__.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/cockroachdb.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/docker-compose.yml
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/dragonfly.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/keydb.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/mariadb.py
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/mssql.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/mysql.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/oracle.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/postgres.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/redis.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pytest_databases/docker/spanner.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/LICENSE
+-rw-r--r--   0        0        0    12148 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/README.md
+-rw-r--r--   0        0        0    17313 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13824 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13648 2020-02-02 00:00:00.000000 pytest_databases-0.2.0/setup.py
```

### Comparing `pytest_databases-0.1.0/pytest_databases/docker/docker-compose.yml` & `pytest_databases-0.2.0/pytest_databases/docker/docker-compose.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-version: "3"
-
 services:
   postgres12:
     networks:
       - default
     image: postgres:12
     ports:
       - "5423:5432" # use a non-standard port here
@@ -154,10 +152,32 @@
       - "26257:26257"
       - "8880:8080"
     healthcheck:
       test: ["CMD", "curl", "-f", "http://localhost:8080/health?ready=1"]
       interval: 3s
       timeout: 3s
       retries: 5
+  redis:
+    image: redis
+    ports:
+      - "6397:6379"
+  keydb:
+    image: eqalpha/keydb
+    ports:
+      - "6396:6379"
+  dragonfly:
+    image: "docker.dragonflydb.io/dragonflydb/dragonfly"
+    ulimits:
+      memlock: -1
+    ports:
+      - "6398:6379"
+    # For better performance, consider `host` mode instead `port` to avoid docker NAT.
+    # `host` mode is NOT currently supported in Swarm Mode.
+    # https://docs.docker.com/compose/compose-file/compose-file-v3/#network_mode
+    # network_mode: "host"
+    volumes:
+      - dragonflydata:/data
 networks:
   default:
     driver: bridge
+volumes:
+  dragonflydata:
```

### Comparing `pytest_databases-0.1.0/.gitignore` & `pytest_databases-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.1.0/LICENSE` & `pytest_databases-0.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Jolt
+Copyright (c) 2024 Litestar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytest_databases-0.1.0/pyproject.toml` & `pytest_databases-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 
 [project]
 description = 'Reusable database fixtures for any and all databases.'
 license = "MIT"
 name = "pytest-databases"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.1.0"
+version = "0.2.0"
 #
 authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
 keywords = [
   "database",
   "migration",
   "postgres",
   "mysql",
   "oracle",
   "mssql",
   "duckdb",
   "bigquery",
   "spanner",
   "cockroachdb",
+  "redis",
 ]
 # options under https://pypi.org/classifiers/
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -39,68 +40,70 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 # direct dependencies of this package
 dependencies = ["pytest"]
 
 [project.urls]
-Documentation = "https://github.com/jolt-org/pytest-databases#readme"
-Issues = "https://github.com/jolt-org/pytest-databases/issues"
-Source = "https://github.com/jolt-org/pytest-databases"
+Documentation = "https://github.com/litestar-org/pytest-databases#readme"
+Issues = "https://github.com/litestar-org/pytest-databases/issues"
+Source = "https://github.com/litestar-org/pytest-databases"
 
 [project.optional-dependencies]
 cockroachdb = ["psycopg"]
 mssql = ["aioodbc"]
 mysql = ["asyncmy>=0.2.9"]
 oracle = ["oracledb"]
 postgres = ["asyncpg>=0.29.0"]
+redis = ["redis"]
 spanner = ["google-cloud-spanner"]
 sqlite = ["aiosqlite"]
 
 ######################
 # Build & Versioning #
 ######################
 [tool.hatch.metadata]
 # direct dependency references, e.g `pip @ git+https://github.com/pypa/pip.git@master`
 allow-direct-references = true
 
 [tool.hatch.build]
 dev-mode-dirs = ["src/"]
+include = ["src/pytest_databases/**/*.yml"]
 packages = ["src/pytest_databases"]
 sources = ["src"]
 
 [tool.hatch.build.targets.sdist]
 exclude = [".github", "./docs"]
 support-legacy = true           # Create setup.py
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/pytest_databases"]
 
 [tool.git-cliff.changelog]
 body = """
 {% if version %}\
-    `Release [v{{ version | trim_start_matches(pat="v") }}] - {{ timestamp | date(format="%Y-%m-%d") }} <https://github.com/jolt-org/pytest-databases/releases/tag/v{{ version | trim_start_matches(pat="v") }}>`_
+    `Release [v{{ version | trim_start_matches(pat="v") }}] - {{ timestamp | date(format="%Y-%m-%d") }} <https://github.com/litestar-org/pytest-databases/releases/tag/v{{ version | trim_start_matches(pat="v") }}>`_
     ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-    * `See All commits in v{{ version | trim_start_matches(pat="v") }} <https://github.com/jolt-org/pytest-databases/commits/v{{ version | trim_start_matches(pat="v") }}>`_
+    * `See All commits in v{{ version | trim_start_matches(pat="v") }} <https://github.com/litestar-org/pytest-databases/commits/v{{ version | trim_start_matches(pat="v") }}>`_
 {% else %}\
     [unreleased]
     ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 {% endif %}\
 {% if previous %}\
     {% if previous.commit_id %}
-        `{{ previous.commit_id | truncate(length=7, end="") }} <https://github.com/jolt-org/pytest-databases/commit/{{ previous.commit_id }}>`_ ... \
-            `{{ commit_id | truncate(length=7, end="") }} <https://github.com/jolt-org/pytest-databases/commit/{{ commit_id }}>`_ \
-            | `See diff for {{ version | trim_start_matches(pat="v") }} <https://github.com/jolt-org/pytest-databases/compare/{{ previous.commit_id }}...{{ commit_id }}>`_
+        `{{ previous.commit_id | truncate(length=7, end="") }} <https://github.com/litestar-org/pytest-databases/commit/{{ previous.commit_id }}>`_ ... \
+            `{{ commit_id | truncate(length=7, end="") }} <https://github.com/litestar-org/pytest-databases/commit/{{ commit_id }}>`_ \
+            | `See diff for {{ version | trim_start_matches(pat="v") }} <https://github.com/litestar-org/pytest-databases/compare/{{ previous.commit_id }}...{{ commit_id }}>`_
     {% endif %}\
 {% endif %}\
 {% for group, commits in commits | group_by(attribute="group") %}
     {{ group | upper_first }}
     ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     {% for commit in commits %}
-        * (`{{ commit.id | truncate(length=7, end="") }} <https://github.com/jolt-org/pytest-databases/commit/{{ commit.id }}>`_) {% if commit.breaking %}[**breaking**] {% endif %} - {{ commit.message | upper_first }} ({{ commit.author.name  }})\
+        * (`{{ commit.id | truncate(length=7, end="") }} <https://github.com/litestar-org/pytest-databases/commit/{{ commit.id }}>`_) {% if commit.breaking %}[**breaking**] {% endif %} - {{ commit.message | upper_first }} ({{ commit.author.name  }})\
           {% for footer in commit.footers -%}
             , {{ footer.token }}{{ footer.separator }}{{ footer.value }}\
           {% endfor %}\
     {% endfor %}
 {% endfor %}\n
 """
 footer = """
@@ -167,16 +170,17 @@
   "coverage[toml]>=6.2",
   "pytest",
   "pytest-cov",
   "pytest-mock",
   "pytest-vcr",
   "pytest-sugar",
   "pytest-click",
+  "pytest-xdist",
 ]
-features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb", "spanner"]
+features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb", "spanner", "redis"]
 template = "default"
 type = "virtual"
 
 [tool.hatch.envs.test.env-vars]
 PYTHONPATH = "."
 PYTHONUNBUFFERED = "1"
 SOURCE_DATE_EPOCH = "1580601600"
@@ -207,20 +211,22 @@
   "pytest-sugar",
   "pytest-click",
   "pytest-xdist",
   # Plugins
   "sphinx>=7.1.2",
   "sphinx-autobuild>=2021.3.14",
   "sphinx-copybutton>=0.5.2",
-  "shibuya==2023.10.26",
+  "litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git",
   "sphinx-click>=5.0.1",
   "sphinx-toolbox>=3.5.0",
   "sphinx-design>=0.5.0",
+  "sphinxcontrib-mermaid>=0.9.2",
+  "auto-pytabs[sphinx]>=0.4.0",
 ]
-features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb", "spanner"]
+features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb", "spanner", "redis"]
 lock-filename = "requirements/requirements-docs.txt"
 pip-compile-constraint = "default"
 python = "3.11"
 template = "test"
 type = "pip-compile"
 
 [tool.hatch.envs.docs.env-vars]
@@ -233,30 +239,55 @@
 # --ignore-url=None since the SUMMARY.md file leaves a <toc>None</toc> in sitemap.xml
 validate = "linkchecker --config .linkcheckerrc --ignore-url=/reference --ignore-url=None site"
 # https://github.com/linkchecker/linkchecker/issues/678
 build-check = ["build", "validate"]
 
 [tool.hatch.envs.local]
 extra-dependencies = [
+  # tests
+  "nodeenv",
+  # required test dependencies
+  "cython",
+  "anyio",
+  "coverage[toml]>=6.2",
+  "pytest",
+  "pytest-cov",
+  "pytest-mock",
+  "pytest-vcr",
+  "pytest-sugar",
+  "pytest-click",
+  "pytest-xdist",
+  # Plugins
+  "sphinx>=7.1.2",
+  "sphinx-autobuild>=2021.3.14",
+  "sphinx-copybutton>=0.5.2",
+  "litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git",
+  "sphinx-click>=5.0.1",
+  "sphinx-toolbox>=3.5.0",
+  "sphinx-design>=0.5.0",
+  "sphinxcontrib-mermaid>=0.9.2",
+  "auto-pytabs[sphinx]>=0.4.0",
   # cli databasae brwoser
   "harlequin",
   # linting
   "cython",
   "anyio",
   "mypy",
   "ruff",
   "pylint",
   "pre-commit",
   "types-click",
   "types-six",
   "types-decorator",
   "types-pyyaml",
   "asyncpg-stubs",
+  "types-docutils",
+  "types-redis",
 ]
-features = ["oracle", "mysql", "mssql", "postgres", "cockroachdb", "spanner"]
+features = ["oracle", "mysql", "mssql", "postgres", "cockroachdb", "spanner", "redis"]
 lock-filename = "requirements/requirements-dev.txt"
 path = ".venv/"
 pip-compile-constraint = "docs"
 python = "3.11"
 template = "docs"
 type = "pip-compile"
 
@@ -273,16 +304,18 @@
   "pylint",
   "pre-commit",
   "types-click",
   "types-six",
   "types-decorator",
   "types-pyyaml",
   "asyncpg-stubs",
+  "types-docutils",
+  "types-redis",
 ]
-features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb"]
+features = ["oracle", "mysql", "mssql", "postgres", "spanner", "cockroachdb", "redis"]
 python = "3.11"
 template = "docs"
 
 [tool.hatch.envs.lint.scripts]
 check = ["style", "typing"]
 fix = [
   "typing",
@@ -327,30 +360,16 @@
 module = ["tests.*"]
 warn_unused_ignores = false
 
 [[tool.mypy.overrides]]
 disable_error_code = ["arg-type"]
 disallow_untyped_calls = false
 disallow_untyped_decorators = false
-module = ["aisoql.*"]
-
-[[tool.mypy.overrides]]
-disallow_untyped_calls = false
-disallow_untyped_defs = false
-module = [
-  "pytest_databases.lib.db.adapters.*",
-  "pytest_databases.lib.db.adapters",
-  "pytest_databases.lib.db.base",
-  "pytest_databases.lib.db",
-]
-warn_unused_ignores = false
+module = ["docutils.nodes.*"]
 
-[[tool.mypy.overrides]]
-ignore_missing_imports = true
-module = ["sqlalchemy.*", "nodeenv"]
 
 [tool.ruff]
 exclude = [
   ".bzr",
   ".direnv",
   ".eggs",
   ".git",
@@ -480,15 +499,15 @@
   "PLR6301",
   "FA102",
 ]
 
 # copyright
 # Enable once this is released: https://github.com/astral-sh/ruff/issues/10021
 # Ruff v0.3.4 has not included this release yet
-"**/*.py" = ["CPY001"]
+# "**/*.py" = ["CPY001"]
 
 [tool.ruff.lint.mccabe]
 max-complexity = 12
 
 [tool.ruff.lint.pep8-naming]
 classmethod-decorators = ["classmethod"]
```

### Comparing `pytest_databases-0.1.0/setup.py` & `pytest_databases-0.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='pytest-databases',
-    version='0.1.0',
+    version='0.2.0',
     description='Reusable database fixtures for any and all databases.',
-    long_description='# pytest-databases\n\nReusable test fixtures for any and all databases.\n\n<div align="center">\n\n| Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |\n| --------- | :-- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |\n| CI/CD     |     | [![Latest Release](https://github.com/jolt-org/pytest-databases/actions/workflows/publish.yaml/badge.svg)](https://github.com/jolt-org/pytest-databases/actions/workflows/publish.yaml) [![Tests And Linting](https://github.com/jolt-org/pytest-databases/actions/workflows/ci.yaml/badge.svg)](https://github.com/jolt-org/pytest-databases/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/jolt-org/pytest-databases/actions/workflows/docs.yaml/badge.svg)](https://github.com/jolt-org/pytest-databases/actions/workflows/docs.yaml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| Quality   |     | [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=jolt-org_pytest-databases&metric=coverage)](https://sonarcloud.io/summary/new_code?id=jolt-org_pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=jolt-org_pytest-databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=jolt-org_pytest-databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=jolt-org_pytest-databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=jolt-org_pytest-databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=jolt-org_pytest-databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=jolt-org_pytest-databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=jolt-org_pytest-databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=jolt-org_pytest-databases)                            |\n| Community |     | [![Discord](https://img.shields.io/discord/1149784127659319356?labelColor=F50057&color=202020&label=chat%20on%20discord&logo=discord&logoColor=202020)](https://discord.gg/XpFNTjjtTK)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |\n| Meta      |     | [![Jolt Project](https://img.shields.io/badge/Jolt%20Org-%E2%AD%90-F50057.svg?logo=python&labelColor=F50057&color=202020&logoColor=202020)](https://github.com/jolt-org/) [![types - Mypy](https://img.shields.io/badge/types-Mypy-F50057.svg?logo=python&labelColor=F50057&color=202020&logoColor=202020)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-F50057.svg?logo=python&labelColor=F50057&color=202020&logoColor=202020)](https://spdx.org/licenses/) [![Jolt Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23202020.svg?&logo=github&logoColor=202020&labelColor=F50057)](https://github.com/sponsors/jolt-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=F50057)](https://github.com/astral-sh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=python&labelColor=F50057&logoColor=202020)](https://github.com/psf/black) |\n\n</div>\n\n> [!WARNING] > **Pre-Release Alpha Stage**\n>\n> Please note that pytest-databases is currently in a pre-release alpha stage of development. This means the library is still under\n> active development, and its API is subject to change. We encourage developers to experiment with pytest-databases and provide\n> feedback, but we recommend against using it in production environments until a stable release is available.`\n\n## About\n\nThe `pytest-databases` library aims to make testing with a database as simple as possible.\nIt is designed to offer pre-configured testing setups for many different types and versions of databases.\n\n## Features\n\n`pytest-databases` currently utilizes `docker compose` (or the legacy `docker-compose`) commands to manage the startup and shutdown of each database service. The following databases are currently available:\n\n- **Postgres**: Version 12, 13, 14, 15, and 16 are available\n- **MySQL**: Version 5.6, 5.7 and 8 are available\n- **Oracle**: Version 18c XE and 23C Free are available\n- **SQL Server**: Version 2022 is available\n- **Spanner**: The latest cloud-emulator from Google is available\n- **Cockroach**: Version 23.1-latest is available\n\n## Contributing\n\nAll [Jolt][jolt-org] projects will always be a community-centered, available for contributions of any size.\n\nBefore contributing, please review the [contribution guide][contributing].\n\nIf you have any questions, reach out to us on [Discord][discord], our org-wide [GitHub discussions][jolt-discussions] page,\nor the [project-specific GitHub discussions page][project-discussions].\n\n<hr>\n\n<!-- markdownlint-disable -->\n<p align="center">\n  <!-- github-banner-start -->\n  <img src="https://raw.githubusercontent.com/jolt-org/meta/2901c9c5c5895a83fbfa56944c33bca287f88d42/branding/SVG%20-%20Transparent/logo-full-wide.svg" alt="Litestar Logo - Light" width="20%" height="auto" />\n  <br>A <a href="https://github.com/jolt-org">Jolt Organization</a> Project\n  <!-- github-banner-end -->\n</p>\n\n[jolt-org]: https://github.com/jolt-org\n[contributing]: https://docs.pytest-databases.jolt.rs/latest/contribution-guide.html\n[discord]: https://discord.gg/XpFNTjjtTK\n[jolt-discussions]: https://github.com/orgs/jolt-org/discussions\n[project-discussions]: https://github.com/jolt-org/pytest-databases/discussions\n[project-docs]: https://docs.pytest-databases.jolt.rs\n[install-guide]: https://docs.pytest-databases.jolt.rs/latest/#installation\n[newrepo]: https://github.com/organizations/jolt-org/repositories/new?template=pytest-databases\n',
+    long_description='# pytest-databases\n\nReusable test fixtures for any and all databases.\n\n<!-- markdownlint-disable -->\n<p align="center">\n  <!-- github-banner-start -->\n  <img src="https://raw.githubusercontent.com/litestar-org/branding/main/assets/Branding%20-%20SVG%20-%20Transparent/Logo%20-%20Banner%20-%20Inline%20-%20Light.svg#gh-light-mode-only" alt="Litestar Logo - Light" width="100%" height="auto" />\n  <img src="https://raw.githubusercontent.com/litestar-org/branding/main/assets/Branding%20-%20SVG%20-%20Transparent/Logo%20-%20Banner%20-%20Inline%20-%20Dark.svg#gh-dark-mode-only" alt="Litestar Logo - Dark" width="100%" height="auto" />\n  <!-- github-banner-end -->\n</p>\n<!-- markdownlint-restore -->\n<div align="center">\n\n<!-- prettier-ignore-start -->\n\n| Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |\n|-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/publish.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/publish.yml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |\n| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)                                                                                                                                                                                                                                                                                                                               |\n| Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/litestar) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/litestar?labelColor=202235&color=edb641&logo=python&logoColor=edb641) ![Starlite PyPI - Downloads](https://img.shields.io/pypi/dm/starlite?logo=python&label=starlite%20downloads&labelColor=202235&color=edb641&logoColor=edb641) ![Litestar PyPI - Downloads](https://img.shields.io/pypi/dm/litestar?logo=python&label=litestar%20downloads&labelColor=202235&color=edb641&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |\n| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |\n| Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/pytest-databases) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black)|\n\n<!-- prettier-ignore-end -->\n</div>\n\n> [!WARNING] > **Pre-Release Alpha Stage**\n>\n> Please note that pytest-databases is currently in a pre-release alpha stage of development. This means the library is still under\n> active development, and its API is subject to change. We encourage developers to experiment with pytest-databases and provide\n> feedback, but we recommend against using it in production environments until a stable release is available.`\n\n## About\n\nThe `pytest-databases` library aims to make testing with a database as simple as possible.\nIt is designed to offer pre-configured testing setups for many different types and versions of databases.\n\n## Features\n\n`pytest-databases` currently utilizes `docker compose` (or the legacy `docker-compose`) commands to manage the startup and shutdown of each database service. The following databases are currently available:\n\n- **Postgres**: Version 12, 13, 14, 15, and 16 are available\n- **MySQL**: Version 5.6, 5.7 and 8 are available\n- **Oracle**: Version 18c XE and 23C Free are available\n- **SQL Server**: Version 2022 is available\n- **Spanner**: The latest cloud-emulator from Google is available\n- **Cockroach**: Version 23.1-latest is available\n- **Redis**: Latest server\n- **Dragonfly**: Latest server\n- **KeyDB**: Latest server\n\n## Contributing\n\nAll [Litestar][litestar-org] projects will always be a community-centered, available for contributions of any size.\n\nBefore contributing, please review the [contribution guide][contributing].\n\nIf you have any questions, reach out to us on [Discord][discord], our org-wide [GitHub discussions][litestar-discussions] page,\nor the [project-specific GitHub discussions page][project-discussions].\n\n<hr>\n\n<!-- markdownlint-disable -->\n<p align="center">\n  <!-- github-banner-start -->\n  <img src="https://raw.githubusercontent.com/litestar-org/meta/2901c9c5c5895a83fbfa56944c33bca287f88d42/branding/SVG%20-%20Transparent/logo-full-wide.svg" alt="Litestar Logo - Light" width="20%" height="auto" />\n  <br>A <a href="https://github.com/litestar-org">Litestar Organization</a> Project\n  <!-- github-banner-end -->\n</p>\n\n[litestar-org]: https://github.com/litestar-org\n[contributing]: https://docs.pytest-databases.litestar.dev/latest/contribution-guide.html\n[discord]: https://discord.gg/litestar-919193495116337154\n[litestar-discussions]: https://github.com/orgs/litestar-org/discussions\n[project-discussions]: https://github.com/litestar-org/pytest-databases/discussions\n[project-docs]: https://docs.pytest-databases.litestar.dev\n[install-guide]: https://docs.pytest-databases.litestar.dev/latest/#installation\n[newrepo]: https://github.com/organizations/litestar-org/repositories/new?template=pytest-databases\n',
     author_email='Cody Fincher <cody.fincher@gmail.com>',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
@@ -33,14 +33,17 @@
         ],
         'oracle': [
             'oracledb',
         ],
         'postgres': [
             'asyncpg>=0.29.0',
         ],
+        'redis': [
+            'redis',
+        ],
         'spanner': [
             'google-cloud-spanner',
         ],
         'sqlite': [
             'aiosqlite',
         ],
     },
```

