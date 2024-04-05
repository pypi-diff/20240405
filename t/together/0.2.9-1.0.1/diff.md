# Comparing `tmp/together-0.2.9.tar.gz` & `tmp/together-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "together-0.2.9.tar", max compression
+gzip compressed data, was "together-1.0.1.tar", max compression
```

## Comparing `together-0.2.9.tar` & `together-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,55 @@
--rw-r--r--   0        0        0    11357 2023-12-06 21:03:48.975631 together-0.2.9/LICENSE
--rw-r--r--   0        0        0    25472 2023-12-06 21:03:48.975631 together-0.2.9/README.md
--rw-r--r--   0        0        0     1686 2023-12-06 21:03:48.979631 together-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     2251 2023-12-06 21:03:48.979631 together-0.2.9/src/together/__init__.py
--rw-r--r--   0        0        0        0 2023-12-06 21:03:48.979631 together-0.2.9/src/together/cli/__init__.py
--rw-r--r--   0        0        0     1655 2023-12-06 21:03:48.979631 together-0.2.9/src/together/cli/cli.py
--rw-r--r--   0        0        0        0 2023-12-06 21:03:48.979631 together-0.2.9/src/together/commands/__init__.py
--rw-r--r--   0        0        0     4343 2023-12-06 21:03:48.979631 together-0.2.9/src/together/commands/chat.py
--rw-r--r--   0        0        0     5833 2023-12-06 21:03:48.979631 together-0.2.9/src/together/commands/complete.py
--rw-r--r--   0        0        0     1175 2023-12-06 21:03:48.979631 together-0.2.9/src/together/commands/embeddings.py
--rw-r--r--   0        0        0     5890 2023-12-06 21:03:48.979631 together-0.2.9/src/together/commands/files.py
--rw-r--r--   0        0        0    11240 2023-12-06 21:03:48.979631 together-0.2.9/src/together/commands/finetune.py
--rw-r--r--   0        0        0     4007 2023-12-06 21:03:48.983631 together-0.2.9/src/together/commands/image.py
--rw-r--r--   0        0        0     6201 2023-12-06 21:03:48.983631 together-0.2.9/src/together/commands/models.py
--rw-r--r--   0        0        0     5505 2023-12-06 21:03:48.983631 together-0.2.9/src/together/complete.py
--rw-r--r--   0        0        0     1884 2023-12-06 21:03:48.983631 together-0.2.9/src/together/embeddings.py
--rw-r--r--   0        0        0     2631 2023-12-06 21:03:48.983631 together-0.2.9/src/together/error.py
--rw-r--r--   0        0        0    12256 2023-12-06 21:03:48.983631 together-0.2.9/src/together/files.py
--rw-r--r--   0        0        0    12187 2023-12-06 21:03:48.983631 together-0.2.9/src/together/finetune.py
--rw-r--r--   0        0        0     1106 2023-12-06 21:03:48.983631 together-0.2.9/src/together/image.py
--rw-r--r--   0        0        0     3072 2023-12-06 21:03:48.983631 together-0.2.9/src/together/models.py
--rw-r--r--   0        0        0        0 2023-12-06 21:03:48.983631 together-0.2.9/src/together/tools/__init__.py
--rw-r--r--   0        0        0     1859 2023-12-06 21:03:48.983631 together-0.2.9/src/together/tools/conversation.py
--rw-r--r--   0        0        0     3063 2023-12-06 21:03:48.983631 together-0.2.9/src/together/types.py
--rw-r--r--   0        0        0     5334 2023-12-06 21:03:48.983631 together-0.2.9/src/together/utils.py
--rw-r--r--   0        0        0      126 2023-12-06 21:03:48.983631 together-0.2.9/src/together/version.py
--rw-r--r--   0        0        0    26634 1970-01-01 00:00:00.000000 together-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-05 19:08:02.492677 together-1.0.1/LICENSE
+-rw-r--r--   0        0        0     9667 2024-04-05 19:08:02.492677 together-1.0.1/README.md
+-rw-r--r--   0        0        0     1897 2024-04-05 19:08:02.496677 together-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1401 2024-04-05 19:08:02.496677 together-1.0.1/src/together/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-05 19:08:02.496677 together-1.0.1/src/together/abstract/__init__.py
+-rw-r--r--   0        0        0    25103 2024-04-05 19:08:02.496677 together-1.0.1/src/together/abstract/api_requestor.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/__init__.py
+-rw-r--r--   0        0        0     7838 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/chat.py
+-rw-r--r--   0        0        0     3691 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/completions.py
+-rw-r--r--   0        0        0     3186 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/files.py
+-rw-r--r--   0        0        0     4954 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/finetune.py
+-rw-r--r--   0        0        0     2363 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/images.py
+-rw-r--r--   0        0        0     1126 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/api/models.py
+-rw-r--r--   0        0        0     1977 2024-04-05 19:08:02.496677 together-1.0.1/src/together/cli/cli.py
+-rw-r--r--   0        0        0     4774 2024-04-05 19:08:02.496677 together-1.0.1/src/together/client.py
+-rw-r--r--   0        0        0      801 2024-04-05 19:08:02.496677 together-1.0.1/src/together/constants.py
+-rw-r--r--   0        0        0     5329 2024-04-05 19:08:02.496677 together-1.0.1/src/together/error.py
+-rw-r--r--   0        0        0    10916 2024-04-05 19:08:02.496677 together-1.0.1/src/together/filemanager.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/base.py
+-rw-r--r--   0        0        0     2343 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/complete.py
+-rw-r--r--   0        0        0      591 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/embeddings.py
+-rw-r--r--   0        0        0     3863 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/files.py
+-rw-r--r--   0        0        0     4917 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/finetune.py
+-rw-r--r--   0        0        0      582 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/images.py
+-rw-r--r--   0        0        0     1053 2024-04-05 19:08:02.496677 together-1.0.1/src/together/legacy/models.py
+-rw-r--r--   0        0        0      701 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/__init__.py
+-rw-r--r--   0        0        0      617 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/chat/__init__.py
+-rw-r--r--   0        0        0    11140 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/chat/completions.py
+-rw-r--r--   0        0        0     8403 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/completions.py
+-rw-r--r--   0        0        0     2546 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/embeddings.py
+-rw-r--r--   0        0        0     4593 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/files.py
+-rw-r--r--   0        0        0    12424 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/finetune.py
+-rw-r--r--   0        0        0     4775 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/images.py
+-rw-r--r--   0        0        0     1786 2024-04-05 19:08:02.496677 together-1.0.1/src/together/resources/models.py
+-rw-r--r--   0        0        0     1319 2024-04-05 19:08:02.496677 together-1.0.1/src/together/together_response.py
+-rw-r--r--   0        0        0     1402 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/abstract.py
+-rw-r--r--   0        0        0     3630 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/chat_completions.py
+-rw-r--r--   0        0        0     1491 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/common.py
+-rw-r--r--   0        0        0     2173 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/completions.py
+-rw-r--r--   0        0        0      751 2024-04-05 19:08:02.496677 together-1.0.1/src/together/types/embeddings.py
+-rw-r--r--   0        0        0      370 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/error.py
+-rw-r--r--   0        0        0     1934 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/files.py
+-rw-r--r--   0        0        0     5779 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/finetune.py
+-rw-r--r--   0        0        0      915 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/images.py
+-rw-r--r--   0        0        0     1013 2024-04-05 19:08:02.500677 together-1.0.1/src/together/types/models.py
+-rw-r--r--   0        0        0      662 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1665 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/_log.py
+-rw-r--r--   0        0        0     2407 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/api_helpers.py
+-rw-r--r--   0        0        0     4835 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/files.py
+-rw-r--r--   0        0        0     1788 2024-04-05 19:08:02.500677 together-1.0.1/src/together/utils/tools.py
+-rw-r--r--   0        0        0      126 2024-04-05 19:08:02.500677 together-1.0.1/src/together/version.py
+-rw-r--r--   0        0        0    10963 1970-01-01 00:00:00.000000 together-1.0.1/PKG-INFO
```

### Comparing `together-0.2.9/LICENSE` & `together-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `together-0.2.9/pyproject.toml` & `together-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,81 @@
 [build-system]
 requires = ["poetry"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "together"
-version = "0.2.9"
+version = "1.0.1"
 authors = [
   "Together AI <support@together.ai>"
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
 ]
-repository = "https://github.com/togethercomputer/together"
-homepage = "https://github.com/togethercomputer/together"
+repository = "https://github.com/togethercomputer/together-python"
+homepage = "https://github.com/togethercomputer/together-python"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-typer = "^0.9.0"
+python = "^3.8"
+typer = ">=0.9,<0.13"
 requests = "^2.31.0"
-tqdm = "^4.66.1"
-sseclient-py = "^1.7.2"
+tqdm = "^4.66.2"
 tabulate = "^0.9.0"
-pydantic = "^2.5.0"
+pydantic = "^2.6.3"
+aiohttp = "^3.9.3"
+filelock = "^3.13.1"
+eval-type-backport = "^0.1.3"
+click = "^8.1.7"
+pillow = "^10.3.0"
 
 [tool.poetry.group.quality]
 optional = true
 
 [tool.poetry.group.quality.dependencies]
-black = "^23.1"
-ruff = "^0.0.241" 
-mypy = "^1.3.0"
-types-requests = "^2.31.0.1"
+black = ">=23.1,<25.0"
+ruff = "^0.3.2"
 types-tqdm = "^4.65.0.0"
 types-tabulate = "^0.9.0.3"
+pre-commit = "3.5.0"
+types-requests = "^2.31.0.20240218"
+mypy = "^1.9.0"
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
-pytest = "^7.4.2"
+pytest = ">=7.4.2,<9.0.0"
+pytest-watch = "^4.2.0"
+tox = "^4.14.1"
+
 
 [tool.poetry.urls]
-"Homepage" = "https://github.com/togethercomputer/together"
-"Bug Tracker" = "https://github.com/togethercomputer/together/issues"
+"Homepage" = "https://github.com/togethercomputer/together-python"
+"Bug Tracker" = "https://github.com/togethercomputer/together-python/issues"
 
 [tool.poetry.scripts]
 together = "together.cli.cli:main"
 
 [tool.black]
 target-version = ['py310']
 
-[tool.ruff]
+[tool.ruff.lint]
 # Never enforce `E501` (line length violations).
 ignore = ["C901", "E501", "E741", "W605"]
 select = ["C", "E", "F", "I", "W"]
 
 # Ignore import violations in all `__init__.py` files.
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["E402", "F401", "F403", "F811"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 lines-after-imports = 2
 known-first-party = ["together"]
 
 [tool.mypy]
 strict = true
 mypy_path = "."
```

