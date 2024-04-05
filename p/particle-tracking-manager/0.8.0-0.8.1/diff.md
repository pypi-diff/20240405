# Comparing `tmp/particle_tracking_manager-0.8.0.tar.gz` & `tmp/particle_tracking_manager-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "particle_tracking_manager-0.8.0.tar", last modified: Tue Apr  2 18:01:25 2024, max compression
+gzip compressed data, was "particle_tracking_manager-0.8.1.tar", last modified: Fri Apr  5 18:00:33 2024, max compression
```

## Comparing `particle_tracking_manager-0.8.0.tar` & `particle_tracking_manager-0.8.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.337570 particle_tracking_manager-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.337570 particle_tracking_manager-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.337570 particle_tracking_manager-0.8.0/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/ci/environment-py3.10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/ci/environment-py3.11.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/ci/environment-py3.9.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.337570 particle_tracking_manager-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/more_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/quick_start.md
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/docs/whats_new.md
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/particle_tracking_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/particle_tracking_manager/models/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    46883 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/opendrift.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    24426 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/the_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/particle_tracking_manager/the_manager_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 18:01:25.000000 particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:01:25.341570 particle_tracking_manager-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_opendrift.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_realistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-02 18:01:17.000000 particle_tracking_manager-0.8.0/tests/test_seeding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.355611 particle_tracking_manager-0.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.355611 particle_tracking_manager-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.355611 particle_tracking_manager-0.8.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/ci/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/ci/environment-py3.11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/ci/environment-py3.9.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.355611 particle_tracking_manager-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/more_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/quick_start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/docs/whats_new.md
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/particle_tracking_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/particle_tracking_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49101 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/opendrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24422 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/the_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/particle_tracking_manager/the_manager_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 18:00:33.000000 particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-05 18:00:33.363611 particle_tracking_manager-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:00:33.359611 particle_tracking_manager-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15617 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_opendrift.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_realistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 18:00:28.000000 particle_tracking_manager-0.8.1/tests/test_seeding.py
```

### Comparing `particle_tracking_manager-0.8.0/.github/workflows/release.yaml` & `particle_tracking_manager-0.8.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/.github/workflows/test.yaml` & `particle_tracking_manager-0.8.1/.github/workflows/test.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -24,29 +24,46 @@
         uses: actions/cache@v4
         env:
           # Increase this value to reset cache if ci/environment.yml has not changed
           CACHE_NUMBER: 0
         with:
           path: ~/conda_pkgs_dir
           key: ${{ runner.os }}-conda-${{ env.CACHE_NUMBER }}-${{ hashFiles('ci/environment-py${{ matrix.python-version }}.yml') }}
-      - uses: conda-incubator/setup-miniconda@v3
+      # - uses: conda-incubator/setup-miniconda@v3
+      #   with:
+      #     # mamba-version: "*" # activate this to build with mamba.
+      #     python-version: ${{ matrix.python-version }}
+      #     miniforge-variant: Mambaforge
+      #     channels: conda-forge, defaults # These need to be specified to use mamba
+      #     channel-priority: true
+      #     environment-file: ci/environment-py${{ matrix.python-version }}.yml
+
+      #     activate-environment: test_env_particle-tracking-manager
+      #     use-only-tar-bz2: true # IMPORTANT: This needs to be set for caching to work properly!
+      # - name: Set up conda environment
+      #   shell: bash -l {0}
+      #   run: |
+      #     python -m pip install -e . --no-deps --force-reinstall
+
+      - name: Setup Micromamba Python ${{ matrix.python-version }}
+        uses: mamba-org/setup-micromamba@v1
         with:
-          # mamba-version: "*" # activate this to build with mamba.
-          python-version: ${{ matrix.python-version }}
-          miniforge-variant: Mambaforge
-          channels: conda-forge, defaults # These need to be specified to use mamba
-          channel-priority: true
+          init-shell: bash
+          create-args: >-
+            python=${{ matrix.python-version }} --channel conda-forge
           environment-file: ci/environment-py${{ matrix.python-version }}.yml
+          cache-environment: true
+          post-cleanup: 'all'
 
-          activate-environment: test_env_particle-tracking-manager
-          use-only-tar-bz2: true # IMPORTANT: This needs to be set for caching to work properly!
-      - name: Set up conda environment
+      - name: Install package
         shell: bash -l {0}
         run: |
           python -m pip install -e . --no-deps --force-reinstall
+
+
       - name: Run Tests
         shell: bash -l {0}
         run: |
           pytest --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
         uses: codecov/codecov-action@v4
         with:
```

### Comparing `particle_tracking_manager-0.8.0/.gitignore` & `particle_tracking_manager-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/.pre-commit-config.yaml` & `particle_tracking_manager-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/LICENSE.txt` & `particle_tracking_manager-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/PKG-INFO` & `particle_tracking_manager-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: particle_tracking_manager
-Version: 0.8.0
+Version: 0.8.1
 Summary: Manager for particle tracking simulations.
 Home-page: https://github.com/axiom-data-science/particle-tracking-manager
 Author: axiom-data-science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `particle_tracking_manager-0.8.0/README.md` & `particle_tracking_manager-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/ci/environment-py3.10.yml` & `particle_tracking_manager-0.8.1/ci/environment-py3.10.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 name: test_env_particle-tracking-manager
 channels:
   - conda-forge
 dependencies:
   - python=3.10
   ############## These will have to be adjusted to your specific project
-  # - adios_db
+  # - adios-db
   - appdirs
   - aiohttp
+  - kerchunk
   - numpy
-  # opendrift reqs
-  - matplotlib>=3.5
-  - numpy>=1.17
-  - scipy>=1.6
-  - netcdf4<=1.6.1
-  - ffmpeg
-  - pyproj>=2.3
-  - libgdal>=3.1
-  - gdal>=3.1
-  - xarray
-  - dask
-  - cfgrib
-  - pygrib
-  - xhistogram
-  - requests
-  - pytest<8
-  - pytest-cov
-  - pytest-benchmark
-  - pytest-mpl
-  - cartopy>=0.20
-  - nc-time-axis
-  - geojson
-  - pynucos>=2.12
-  - isodate
-  - coloredlogs
-  - cmocean
-  - utm
-  - roaring-landmask>=0.7
-  # - trajan>=0.1.3
-  # - adios_db
+  # # opendrift reqs
+  # - matplotlib>=3.5
+  # - numpy>=1.17
+  # - scipy>=1.6
+  # - netcdf4<=1.6.1
+  # - ffmpeg
+  # - pyproj>=2.3
+  # - libgdal>=3.1
+  # - gdal>=3.1
+  # - xarray
+  # - dask
+  # - cfgrib
+  # - pygrib
+  # - xhistogram
+  # - requests
+  # - pytest<8
+  # - pytest-cov
+  # - pytest-benchmark
+  # - pytest-mpl
+  # - cartopy>=0.20
+  # - nc-time-axis
+  # - geojson
+  # - pynucos>=2.12
+  # - isodate
+  # - coloredlogs
+  # - cmocean
+  # - utm
+  # - roaring-landmask>=0.7
+  # # - trajan>=0.1.3
+  # # - adios_db
   ##
-    #- opendrift
+  - opendrift>=1.11.2
   - scipy
   - xarray
   # - xroms
   ##############
   - codecov
   - pytest-cov
   - coverage
   - pip
   - pytest
-  - pip:
-    - git+https://github.com/OpenDrift/opendrift
-    - git+https://github.com/fsspec/kerchunk
+  # - pip:
+    # - adios_db
+    # - git+https://github.com/OpenDrift/opendrift
+    # - git+https://github.com/fsspec/kerchunk
     # - xroms  # can't be found on conda-forge for CI, but don't need since in runslow tests?
```

### Comparing `particle_tracking_manager-0.8.0/ci/environment-py3.11.yml` & `particle_tracking_manager-0.8.1/ci/environment-py3.9.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 name: test_env_particle-tracking-manager
 channels:
   - conda-forge
 dependencies:
-  - python=3.11
+  - python=3.9
   ############## These will have to be adjusted to your specific project
-  # - adios_db
+  # - adios-db
   - appdirs
   - aiohttp
+  - kerchunk
   - numpy
-  # opendrift reqs
-  - matplotlib>=3.5
-  - numpy>=1.17
-  - scipy>=1.6
-  - netcdf4<=1.6.1
-  - ffmpeg
-  - pyproj>=2.3
-  - libgdal>=3.1
-  - gdal>=3.1
-  - xarray
-  - dask
-  - cfgrib
-  - pygrib
-  - xhistogram
-  - requests
-  - pytest<8
-  - pytest-cov
-  - pytest-benchmark
-  - pytest-mpl
-  - cartopy>=0.20
-  - nc-time-axis
-  - geojson
-  - pynucos>=2.12
-  - isodate
-  - coloredlogs
-  - cmocean
-  - utm
-  - roaring-landmask>=0.7
+  # # opendrift reqs
+  # - matplotlib>=3.5
+  # - numpy>=1.17
+  # - scipy>=1.6
+  # - netcdf4<=1.6.1
+  # - ffmpeg
+  # - pyproj>=2.3
+  # - libgdal>=3.1
+  # - gdal>=3.1
+  # - xarray
+  # - dask
+  # - cfgrib
+  # - pygrib
+  # - xhistogram
+  # - requests
+  # - pytest<8
+  # - pytest-cov
+  # - pytest-benchmark
+  # - pytest-mpl
+  # - cartopy>=0.20
+  # - nc-time-axis
+  # - geojson
+  # - pynucos>=2.12
+  # - isodate
+  # - coloredlogs
+  # - cmocean
+  # - utm
+  # - roaring-landmask>=0.7
   # - trajan>=0.1.3
   # - adios_db
   ##
-    #- opendrift
+  - opendrift>=1.11.2
   - scipy
   - xarray
   # - xroms
   ##############
   - codecov
   - pytest-cov
   - coverage
   - pip
   - pytest
-  - pip:
-    - git+https://github.com/OpenDrift/opendrift
-    - git+https://github.com/fsspec/kerchunk
+  # - pip:
+    # - adios_db
+    # - git+https://github.com/OpenDrift/opendrift
+    # - git+https://github.com/fsspec/kerchunk
     # - xroms  # can't be found on conda-forge for CI, but don't need since in runslow tests?
```

### Comparing `particle_tracking_manager-0.8.0/ci/environment-py3.9.yml` & `particle_tracking_manager-0.8.1/ci/environment-py3.11.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 name: test_env_particle-tracking-manager
 channels:
   - conda-forge
 dependencies:
-  - python=3.9
+  - python=3.11
   ############## These will have to be adjusted to your specific project
-  # - adios_db
+  # - adios-db
   - appdirs
   - aiohttp
+  - kerchunk
   - numpy
-  # opendrift reqs
-  - matplotlib>=3.5
-  - numpy>=1.17
-  - scipy>=1.6
-  - netcdf4<=1.6.1
-  - ffmpeg
-  - pyproj>=2.3
-  - libgdal>=3.1
-  - gdal>=3.1
-  - xarray
-  - dask
-  - cfgrib
-  - pygrib
-  - xhistogram
-  - requests
-  - pytest<8
-  - pytest-cov
-  - pytest-benchmark
-  - pytest-mpl
-  - cartopy>=0.20
-  - nc-time-axis
-  - geojson
-  - pynucos>=2.12
-  - isodate
-  - coloredlogs
-  - cmocean
-  - utm
-  - roaring-landmask>=0.7
+  # # opendrift reqs
+  # - matplotlib>=3.5
+  # - numpy>=1.17
+  # - scipy>=1.6
+  # - netcdf4<=1.6.1
+  # - ffmpeg
+  # - pyproj>=2.3
+  # - libgdal>=3.1
+  # - gdal>=3.1
+  # - xarray
+  # - dask
+  # - cfgrib
+  # - pygrib
+  # - xhistogram
+  # - requests
+  # - pytest<8
+  # - pytest-cov
+  # - pytest-benchmark
+  # - pytest-mpl
+  # - cartopy>=0.20
+  # - nc-time-axis
+  # - geojson
+  # - pynucos>=2.12
+  # - isodate
+  # - coloredlogs
+  # - cmocean
+  # - utm
+  # - roaring-landmask>=0.7
   # - trajan>=0.1.3
   # - adios_db
   ##
-    #- opendrift
+  - opendrift>=1.11.2
   - scipy
   - xarray
   # - xroms
   ##############
   - codecov
   - pytest-cov
   - coverage
   - pip
   - pytest
-  - pip:
-    - git+https://github.com/OpenDrift/opendrift
-    - git+https://github.com/fsspec/kerchunk
+  # - pip:
+    # - adios_db
+    # - git+https://github.com/OpenDrift/opendrift
+    # - git+https://github.com/fsspec/kerchunk
     # - xroms  # can't be found on conda-forge for CI, but don't need since in runslow tests?
```

### Comparing `particle_tracking_manager-0.8.0/docs/Makefile` & `particle_tracking_manager-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/docs/conf.py` & `particle_tracking_manager-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/docs/configuration.md` & `particle_tracking_manager-0.8.1/docs/configuration.md`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,20 @@
 
 All config:
 
 ```
 m.show_config()
 ```
 
+Config for the specified OpenDrift drift_model; that is, the selections going into the OpenDrift simulation that were specified by PTM as opposed to using the defaults (though they might be the same as the OpenDrift defaults):
+
+```
+m.drift_model_config()
+```
+
 
 ### Showing Configuration Parameter Details
 
 Show seed parameters that are in OpenDrift for `drift_model`:
 
 ```
 m.show_config(prefix="seed", level=[1,2,3]).keys()
@@ -150,17 +156,19 @@
 ```
 m.show_config(key="ocean_model")
 ```
 
 The built-in ocean models are:
 * NWGOA (1999–2008) over the Northwest Gulf of Alaska (Danielson, S. L., K. S. Hedstrom, E. Curchitser,	2016. Cook Inlet Model Calculations, Final Report to Bureau of Ocean Energy Management,	M14AC00014,	OCS	Study BOEM 2015-050, University	of Alaska Fairbanks, Fairbanks,	AK,	149 pp.)
 * CIOFS (1999–2022) across Cook Inlet, Alaska, a hindcast version of NOAA's CIOFS model. (Thyng, K. M., C. Liu, M. Feen, E. L. Dobbins, 2023. Cook Inlet Circulation Modeling, Final Report to Oil Spill Recovery Institute, Axiom Data Science, Anchorage, AK.)
-* CIOFS_NOW (mid-2021 through 48 hours from present time) which is the nowcast/forecast version of the CIOFS model. (Shi, L., L. Lanerolle, Y. Chen, D. Cao, R. Patchen, A. Zhang,
+* CIOFSOP (mid-2021 through 48 hours from present time) which is the nowcast/forecast version of the CIOFS model. (Shi, L., L. Lanerolle, Y. Chen, D. Cao, R. Patchen, A. Zhang,
 and E. P. Myers, 2020. NOS Cook Inlet Operational Forecast System: Model development and hindcast skill assessment, NOAA Technical Report NOS CS 40, Silver Spring, Maryland, September 2020.)
 
+If you are running locally on an Axiom server you can use `ocean_model_local=True` to access the model output locally instead of remotely.
+
 An alternative ocean model can be used instead by initializing the `Manager` then setting up the reader manually, as shown in a {ref}`Quick Start<new_reader>` example:
 
 ```
 import particle_tracking_manager as ptm
 import xroms
 
 m = ptm.OpenDriftModel(lon=-90, lat=28.7, number=1, steps=2)
@@ -229,14 +237,16 @@
 ```
 
 To limit the variables saved in the export file, input a list of just the variables that you want to save, keeping in mind that `['lon', 'lat', 'ID', 'status']` will also be included regardless. For example:
 ```
 m = ptm.OpenDriftModel(export_variables=[])
 ```
 
+The default list of `export_variables` is set in `config_model` but is modified depending on the `drift_model` set.
+
 
 #### How to modify details for Stokes Drift
 
 Turn on (on by default):
 
 ```
 m = ptm.OpenDriftModel(stokes_drift=True)
```

### Comparing `particle_tracking_manager-0.8.0/docs/environment.yml` & `particle_tracking_manager-0.8.1/docs/environment.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,16 @@
   - conda-forge
   - nodefaults
 dependencies:
    - python=3.10
    # If your docs code examples depend on other packages add them here
    - adios_db
    - aiohttp
+   - appdirs
+   - cmocean
    - numpy
    - xarray
    # These are needed for the docs themselves
    - furo
    - jupytext
    - numpydoc
    - opendrift
```

### Comparing `particle_tracking_manager-0.8.0/docs/index.rst` & `particle_tracking_manager-0.8.1/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 .. toctree::
    :maxdepth: 3
    :hidden:
    :caption: Examples and demos
 
    quick_start
+   tutorial
    configuration
 
 
 .. toctree::
    :maxdepth: 3
    :hidden:
    :caption: Developer docs
```

### Comparing `particle_tracking_manager-0.8.0/docs/more_examples.md` & `particle_tracking_manager-0.8.1/docs/more_examples.md`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/docs/quick_start.md` & `particle_tracking_manager-0.8.1/docs/quick_start.md`

 * *Files 14% similar despite different names*

```diff
@@ -55,47 +55,60 @@
 
 This demo will run using easily-available ROMS model output from `xroms`.
 
 ```{code-cell} ipython3
 
 import particle_tracking_manager as ptm
 import xroms
+import xarray as xr
 
 
-m = ptm.OpenDriftModel(lon = -90, lat = 28.7, number=1, steps=2)
+m = ptm.OpenDriftModel(lon = -90, lat = 28.7, number=10, steps=20,
+                       use_static_masks=True)
+
 
 url = xroms.datasets.CLOVER.fetch("ROMS_example_full_grid.nc")
-reader_kwargs = dict(loc=url, kwargs_xarray={})
-m.add_reader(**reader_kwargs)
+ds = xr.open_dataset(url, decode_times=False)
+m.add_reader(ds=ds)
 
 # m.run_all() or the following
 m.seed()
 m.run()
 ```
 
+Plot using `OpenDrift`'s built in plotting. Many options are available, including animations (see [OpenDrift docs for more information](https://opendrift.github.io/)).
+
+```{code-cell} ipython3
+m.o.plot(fast=True)
+```
+
 ## Idealized simulation
 
 To run an idealized scenario, no reader should be added but configuration parameters can be manually changed, for example:
 
 ```{code-cell} ipython3
 import particle_tracking_manager as ptm
 from datetime import datetime
 m = ptm.OpenDriftModel(lon=4.0, lat=60.0, start_time=datetime(2015, 9, 22, 6),
-                       use_auto_landmask=True,)
+                       use_auto_landmask=True, steps=20)
 
 # idealized simulation, provide a fake current
 m.o.set_config('environment:fallback:y_sea_water_velocity', 1)
 
 # seed
 m.seed()
 
 # run simulation
 m.run()
 ```
 
+```{code-cell} ipython3
+m.o.plot(fast=True)
+```
+
 ## Ways to Get Information
 
 Check drifter initialization properties:
 
 ```
 m.initial_drifters
 ```
```

### Comparing `particle_tracking_manager-0.8.0/docs/whats_new.md` & `particle_tracking_manager-0.8.1/docs/whats_new.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # What's New
 
+## v0.8.1 (April 5, 2024)
+
+* updated docs
+
 ## v0.8.0 (April 2, 2024)
 
 * `time_step_output` behavior has changed — 1 hour by default
 * `time_step` is now 5 min by default
 * added `Dcrit` parameter for accurately finding where drifters are stranded in tidal flats
 * `vertical_mixing` is True by default now
 * added seafloor_action option
```

### Comparing `particle_tracking_manager-0.8.0/particle_tracking_manager/cli.py` & `particle_tracking_manager-0.8.1/particle_tracking_manager/cli.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/config.json` & `particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/config.json`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/particle_tracking_manager/models/opendrift/opendrift.py` & `particle_tracking_manager-0.8.1/particle_tracking_manager/models/opendrift/opendrift.py`

 * *Files 3% similar despite different names*

```diff
@@ -401,18 +401,36 @@
             )
 
         if name == "do3D" and value and self.drift_model != "Leeway":
             self.logger.info("do3D is True so turning on vertical advection.")
             self.o.set_config("drift:vertical_advection", True)
         elif name == "do3D" and value and self.drift_model == "Leeway":
             self.logger.info(
-                "do3D is True but drift_model is Leeway so " "changing do3D to False."
+                "do3D is True but drift_model is Leeway so changing do3D to False."
             )
             self.do3D = False
 
+        # if drift_model is LarvalFish, vertical_mixing has to be True
+        if name == "vertical_mixing" and not value and self.drift_model == "LarvalFish":
+            raise ValueError(
+                "drift_model is LarvalFish which always has vertical mixing on in OpenDrift so vertical_mixing must be True."
+            )
+
+        # if drift_model is LarvalFish, surface_only can't be True
+        if name == "surface_only" and value and self.drift_model == "LarvalFish":
+            raise ValueError(
+                "drift_model is LarvalFish which is always 3D in OpenDrift so surface_only must be False."
+            )
+
+        # if drift_model is LarvalFish, do3D has to be True
+        if name == "do3D" and not value and self.drift_model == "LarvalFish":
+            raise ValueError(
+                "drift_model is LarvalFish which is always 3D in OpenDrift so do3D must be True."
+            )
+
         # Make sure vertical_mixing_timestep equals default value if vertical_mixing False
         if name in ["vertical_mixing", "vertical_mixing_timestep"]:
             vmtdef = self.config_model["vertical_mixing_timestep"]["default"]
             if (
                 not self.vertical_mixing
                 and self.vertical_mixing_timestep != vmtdef
                 and self.vertical_mixing_timestep is not None
@@ -502,14 +520,25 @@
             ]
             self.__dict__["export_variables"] += oil_vars
             self.config_model["export_variables"]["value"] += oil_vars
         elif name == "export_variables" and self.drift_model == "Leeway":
             vars = ["object_type"]
             self.__dict__["export_variables"] += vars
             self.config_model["export_variables"]["value"] += vars
+        elif name == "export_variables" and self.drift_model == "LarvalFish":
+            vars = [
+                "diameter",
+                "neutral_buoyancy_salinity",
+                "stage_fraction",
+                "hatched",
+                "length",
+                "weight",
+            ]
+            self.__dict__["export_variables"] += vars
+            self.config_model["export_variables"]["value"] += vars
 
         self._update_config()
 
     def run_add_reader(
         self,
         ds=None,
         name=None,
@@ -721,34 +750,36 @@
             # so they aren't rotated in the ROMS reader (the standard names have to be x/y not east/north)
             elif self.ocean_model == "CIOFSOP":
                 ds = ds.rename_vars({"urot": "u_eastward", "vrot": "v_northward"})
                 # grid = xr.open_dataset("/mnt/vault/ciofs/HINDCAST/nos.ciofs.romsgrid.nc")
                 # ds["angle"] = grid["angle"]
 
             try:
-                units_date = pd.Timestamp(
-                    ds.ocean_time.attrs["units"].split("since ")[1]
-                )
-            except KeyError:  # for remote
-                units_date = pd.Timestamp(
-                    ds.ocean_time.encoding["units"].split("since ")[0]
-                )
+                units = ds.ocean_time.attrs["units"]
+            except KeyError:
+                units = ds.ocean_time.encoding["units"]
+            datestr = units.split("since ")[1]
+            units_date = pd.Timestamp(datestr)
+
             # use reader start time if not otherwise input
             if self.start_time is None:
                 self.logger.info("setting reader start_time as simulation start_time")
                 # self.start_time = reader.start_time
                 # convert using pandas instead of netCDF4
                 self.start_time = units_date + pd.to_timedelta(
                     ds.ocean_time[0].values, unit="s"
                 )
-
             # narrow model output to simulation time if possible before sending to Reader
             if self.start_time is not None and self.end_time is not None:
+                dt_model = float(
+                    ds.ocean_time[1] - ds.ocean_time[0]
+                )  # time step of the model output in seconds
                 start_time_num = (self.start_time - units_date).total_seconds()
-                end_time_num = (self.end_time - units_date).total_seconds()
+                # want to include the next ocean model output after the last drifter simulation time
+                end_time_num = (self.end_time - units_date).total_seconds() + dt_model
                 ds = ds.sel(ocean_time=slice(start_time_num, end_time_num))
                 self.logger.info("Narrowed model output to simulation time")
             else:
                 raise ValueError(
                     "start_time and end_time must be set to narrow model output to simulation time"
                 )
 
@@ -779,19 +810,37 @@
 
         else:
             raise ValueError("reader did not set an ocean_model")
 
     def run_seed(self):
         """Seed drifters for model."""
 
+        already_there = [
+            "seed:number",
+            "seed:z",
+            "seed:seafloor",
+            "seed:droplet_diameter_mu",
+            "seed:droplet_diameter_min_subsea",
+            "seed:droplet_size_distribution",
+            "seed:droplet_diameter_sigma",
+            "seed:droplet_diameter_max_subsea",
+            "seed:object_type",
+        ]
+
         seed_kws = {
             "time": self.start_time.to_pydatetime(),
             "z": self.z,
         }
 
+        # update seed_kws with drift_model-specific seed parameters
+        seedlist = self.drift_model_config(prefix="seed")
+        seedlist = [(one, two) for one, two in seedlist if one not in already_there]
+        seedlist = [(one.replace("seed:", ""), two) for one, two in seedlist]
+        seed_kws.update(seedlist)
+
         if self.seed_flag == "elements":
             # add additional seed parameters
             seed_kws.update(
                 {
                     "lon": self.lon,
                     "lat": self.lat,
                     "radius": self.radius,
```

### Comparing `particle_tracking_manager-0.8.0/particle_tracking_manager/plotting.py` & `particle_tracking_manager-0.8.1/particle_tracking_manager/plotting.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/particle_tracking_manager/the_manager.py` & `particle_tracking_manager-0.8.1/particle_tracking_manager/the_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
                             ciofs_operational_start_time
                             <= self.start_time
                             <= ciofs_operational_end_time
                         )
 
             # deal with if input longitudes need to be shifted due to model
             if name == "oceanmodel_lon0_360" and value:
-                if self.ocean_model is not "test" and self.lon is not None:
+                if self.ocean_model != "test" and self.lon is not None:
                     # move longitude to be 0 to 360 for this model
                     # this is not a user-defined option
                     if -180 < self.lon < 0:
                         self.__dict__["lon"] += 360
                         self.config_ptm["lon"]["value"] += 360  # this isn't really used
 
             if name == "surface_only" and value:
```

### Comparing `particle_tracking_manager-0.8.0/particle_tracking_manager/the_manager_config.json` & `particle_tracking_manager-0.8.1/particle_tracking_manager/the_manager_config.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971590909090909%*

 * *Differences: {"'use_static_masks'": "{'default': True}"}*

```diff
@@ -150,15 +150,15 @@
         "type": [
             "float",
             "datetime.timedelta"
         ],
         "units": "seconds"
     },
     "use_static_masks": {
-        "default": false,
+        "default": true,
         "description": "Set to True to use static masks for known models instead of wetdry masks. If False, the masks are change in time.",
         "ptm_level": 2,
         "type": "bool"
     },
     "vertical_mixing": {
         "default": true,
         "od_mapping": "drift:vertical_mixing",
```

### Comparing `particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/PKG-INFO` & `particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: particle_tracking_manager
-Version: 0.8.0
+Version: 0.8.1
 Summary: Manager for particle tracking simulations.
 Home-page: https://github.com/axiom-data-science/particle-tracking-manager
 Author: axiom-data-science
 Author-email: kristen@axds.co
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `particle_tracking_manager-0.8.0/particle_tracking_manager.egg-info/SOURCES.txt` & `particle_tracking_manager-0.8.1/particle_tracking_manager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 docs/api.rst
 docs/conf.py
 docs/configuration.md
 docs/environment.yml
 docs/index.rst
 docs/more_examples.md
 docs/quick_start.md
+docs/tutorial.md
 docs/whats_new.md
 particle_tracking_manager/__init__.py
-particle_tracking_manager/_version.py
 particle_tracking_manager/cli.py
 particle_tracking_manager/plotting.py
 particle_tracking_manager/the_manager.py
 particle_tracking_manager/the_manager_config.json
 particle_tracking_manager.egg-info/PKG-INFO
 particle_tracking_manager.egg-info/SOURCES.txt
 particle_tracking_manager.egg-info/dependency_links.txt
```

### Comparing `particle_tracking_manager-0.8.0/pyproject.toml` & `particle_tracking_manager-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/setup.cfg` & `particle_tracking_manager-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/tests/conftest.py` & `particle_tracking_manager-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/tests/test_cli.py` & `particle_tracking_manager-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/tests/test_config.py` & `particle_tracking_manager-0.8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/tests/test_manager.py` & `particle_tracking_manager-0.8.1/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/tests/test_opendrift.py` & `particle_tracking_manager-0.8.1/tests/test_opendrift.py`

 * *Files 12% similar despite different names*

```diff
@@ -115,49 +115,25 @@
         "s_rho": (("Z"), np.linspace(-1, 0, 3)),
         "lon_rho": (("Y", "X"), np.array([[1, 2, 3], [1, 2, 3]])),
         "lat_rho": (("Y", "X"), np.array([[1, 1, 1], [2, 2, 2]])),
     },
 )
 
 
-class TestOpenDriftModel_OceanDrift(unittest.TestCase):
+class TestOpenDriftModel_OceanDrift_static_mask(unittest.TestCase):
     def setUp(self):
-        self.model = OpenDriftModel(drift_model="OceanDrift")
-
-    def test_error_no_end_of_simulation(self):
-        self.model.do3D = False
-        self.use_static_masks = False
-        # need to input steps, duration, or end_time but don't here
-        with pytest.raises(ValueError):
-            self.model.add_reader(ds=ds)
+        self.model = OpenDriftModel(drift_model="OceanDrift", use_static_masks=True)
 
     def test_ocean_model_not_known_ds_None(self):
         self.model.ocean_model = "wrong_name"
         self.model.ds = None  # this is the default
         # need to input steps, duration, or end_time but don't here
         with pytest.raises(ValueError):
             self.model.add_reader(ds=ds)
 
-    def test_drop_vars_do3D_false(self):
-        self.model.do3D = False
-        self.use_static_masks = False
-        self.model.steps = 4
-        self.model.add_reader(ds=ds)
-        assert self.model.reader.variables == [
-            "x_sea_water_velocity",
-            "y_sea_water_velocity",
-            "land_binary_mask",
-            "x_wind",
-            "y_wind",
-            "wind_speed",
-            "sea_water_speed",
-        ]
-        assert "wetdry_mask_rho" in self.model.reader.Dataset.data_vars
-        assert "mask_rho" not in self.model.reader.Dataset.data_vars
-
     def test_drop_vars_do3D_true(self):
         self.model.do3D = True
         self.model.steps = 4
         self.model.add_reader(ds=ds)
         assert self.model.reader.variables == [
             "x_sea_water_velocity",
             "y_sea_water_velocity",
@@ -167,15 +143,14 @@
             "y_wind",
             "wind_speed",
             "sea_water_speed",
         ]
 
     def test_drop_vars_use_static_masks(self):
         self.model.do3D = False
-        self.model.use_static_masks = True
         self.model.duration = pd.Timedelta("24h")
         self.model.add_reader(ds=ds)
         assert self.model.reader.variables == [
             "x_sea_water_velocity",
             "y_sea_water_velocity",
             "land_binary_mask",
             "x_wind",
@@ -197,36 +172,46 @@
             "x_sea_water_velocity",
             "y_sea_water_velocity",
             "land_binary_mask",
             "sea_water_speed",
         ]
 
 
-class TestOpenDriftModel_LarvalFish(unittest.TestCase):
+class TestOpenDriftModel_OceanDrift_wetdry_mask(unittest.TestCase):
     def setUp(self):
-        self.model = OpenDriftModel(drift_model="LarvalFish")
+        self.model = OpenDriftModel(drift_model="OceanDrift", use_static_masks=False)
+
+    def test_error_no_end_of_simulation(self):
+        self.model.do3D = False
+        # need to input steps, duration, or end_time but don't here
+        with pytest.raises(ValueError):
+            self.model.add_reader(ds=ds)
 
     def test_drop_vars_do3D_false(self):
         self.model.do3D = False
-        self.model.end_time = pd.Timestamp("1970-01-01T02:00")
+        self.model.steps = 4
         self.model.add_reader(ds=ds)
         assert self.model.reader.variables == [
             "x_sea_water_velocity",
             "y_sea_water_velocity",
-            "sea_water_salinity",
-            "sea_water_temperature",
             "land_binary_mask",
             "x_wind",
             "y_wind",
             "wind_speed",
             "sea_water_speed",
         ]
+        assert "wetdry_mask_rho" in self.model.reader.Dataset.data_vars
+        assert "mask_rho" not in self.model.reader.Dataset.data_vars
 
-    def test_drop_vars_do3D_true(self):
-        self.model.do3D = True
+
+class TestOpenDriftModel_LarvalFish(unittest.TestCase):
+    def setUp(self):
+        self.model = OpenDriftModel(drift_model="LarvalFish", do3D=True)
+
+    def test_drop_vars_wind(self):
         self.model.duration = pd.Timedelta("1h")
         self.model.add_reader(ds=ds)
         assert self.model.reader.variables == [
             "x_sea_water_velocity",
             "y_sea_water_velocity",
             "upward_sea_water_velocity",
             "sea_water_salinity",
@@ -234,44 +219,27 @@
             "land_binary_mask",
             "x_wind",
             "y_wind",
             "wind_speed",
             "sea_water_speed",
         ]
 
-    def test_drop_vars_no_wind(self):
-        self.model.stokes_drift = False
-        self.model.wind_drift_factor = 0
-        self.model.wind_uncertainty = 0
-        self.model.vertical_mixing = False
-        self.model.steps = 3
-        self.model.add_reader(ds=ds)
-        # import pdb; pdb.set_trace()
-        assert self.model.reader.variables == [
-            "x_sea_water_velocity",
-            "y_sea_water_velocity",
-            "sea_water_salinity",
-            "sea_water_temperature",
-            "land_binary_mask",
-            "sea_water_speed",
-        ]
-
 
 def test_drift_model():
-    """can't change the drift_model after class initialization"""
     with pytest.raises(ValueError):
         m = OpenDriftModel(drift_model="not_a_real_model")
 
 
 class TestTheManager(unittest.TestCase):
     def setUp(self):
         self.m = OpenDriftModel()
         # self.m.config_model = {"test_key": {"value": "old_value"}}
 
     def test_set_drift_model(self):
+        """can't change the drift_model after class initialization"""
         with self.assertRaises(KeyError):
             self.m.drift_model = "new_model"
 
     def test_set_o(self):
         with self.assertRaises(KeyError):
             self.m.o = "new_o"
 
@@ -322,20 +290,24 @@
         self.m.mixed_layer_depth = 10
         d = self.m.show_config(key="mixed_layer_depth")
         assert d["value"] == d["default"]
 
 
 class TestOpenDriftModel_Leeway(unittest.TestCase):
     def setUp(self):
-        self.m = OpenDriftModel(drift_model="Leeway")
+        self.m = OpenDriftModel(
+            drift_model="Leeway", object_type=">PIW, scuba suit (face up)"
+        )
 
     def test_leeway_model_wind_drift_factor_not_default(self):
         self.m.wind_drift_factor = 10
         d = self.m.show_config(key="wind_drift_factor")
         assert d["value"] == d["default"]
+        assert self.m.object_type == ">PIW, scuba suit (face up)"
+        assert self.m.o._config["object_type"]["value"] == ">PIW, scuba suit (face up)"
 
     def test_leeway_model_wind_drift_depth_not_default(self):
         self.m.wind_drift_depth = 10
         d = self.m.show_config(key="wind_drift_depth")
         assert d["value"] == d["default"]
 
     def test_leeway_model_stokes_drift_true(self):
@@ -360,9 +332,100 @@
     m.ocean_model = "CIOFSOP"
     assert m.horizontal_diffusivity == 10.0  # known grid values
 
     m = OpenDriftModel(ocean_model="NWGOA")
     assert m.horizontal_diffusivity == 150.0  # known grid values
 
 
+def test_LarvalFish_disallowed_settings():
+    """LarvalFish is incompatible with some settings.
+
+    LarvalFish has to always be 3D.
+    """
+
+    with pytest.raises(ValueError):
+        m = OpenDriftModel(drift_model="LarvalFish", vertical_mixing=False)
+
+    with pytest.raises(ValueError):
+        m = OpenDriftModel(drift_model="LarvalFish", surface_only=True)
+
+    m = OpenDriftModel(drift_model="LarvalFish", do3D=True)
+    with pytest.raises(ValueError):
+        m.surface_only = True
+
+    with pytest.raises(ValueError):
+        m = OpenDriftModel(drift_model="LarvalFish", do3D=False)
+
+
+def test_LarvalFish_seeding():
+    """Make sure special seed parameter comes through"""
+
+    m = OpenDriftModel(
+        drift_model="LarvalFish",
+        lon=-151,
+        lat=60,
+        do3D=True,
+        hatched=1,
+        start_time="2021-01-01T00:00:00",
+        use_auto_landmask=True,
+    )
+    m.seed()
+    assert m.o.elements_scheduled.hatched == 1
+
+
+def test_OpenOil_seeding():
+    """Make sure special seed parameters comes through"""
+
+    m = OpenDriftModel(
+        drift_model="OpenOil",
+        lon=-151,
+        lat=60,
+        do3D=True,
+        start_time="2021-01-01T00:00:00",
+        use_auto_landmask=True,
+        m3_per_hour=5,
+        droplet_diameter_max_subsea=0.1,
+        droplet_diameter_min_subsea=0.01,
+        droplet_diameter_mu=0.01,
+        droplet_size_distribution="normal",
+        droplet_diameter_sigma=10,
+        oil_film_thickness=5,
+        oil_type="GENERIC DIESEL",
+    )
+    m.o.set_config("environment:constant:x_wind", -1)
+    m.o.set_config("environment:constant:y_wind", -1)
+    m.o.set_config("environment:constant:x_sea_water_velocity", -1)
+    m.o.set_config("environment:constant:y_sea_water_velocity", -1)
+    m.seed()
+
+    # to check impact of m3_per_hour: mass_oil for m3_per_hour of 1 * 5
+    assert np.allclose(m.o.elements_scheduled.mass_oil, 8.412 * 5)
+    assert m.o._config["m3_per_hour"]["value"] == 5
+    assert m.o._config["droplet_diameter_max_subsea"]["value"] == 0.1
+    assert m.o._config["droplet_diameter_min_subsea"]["value"] == 0.01
+    assert m.o._config["droplet_diameter_mu"]["value"] == 0.01
+    assert m.o._config["droplet_size_distribution"]["value"] == "normal"
+    assert m.o._config["droplet_diameter_sigma"]["value"] == 10
+    assert m.o.elements_scheduled.oil_film_thickness == 5
+    assert m.o._config["oil_type"]["value"] == "GENERIC DIESEL"
+
+
+def test_wind_drift():
+    """Make sure changed wind drift numbers comes through"""
+
+    m = OpenDriftModel(
+        drift_model="OceanDrift",
+        lon=-151,
+        lat=60,
+        do3D=True,
+        wind_drift_factor=1,
+        wind_drift_depth=10,
+        start_time="2021-01-01T00:00:00",
+        use_auto_landmask=True,
+    )
+    m.seed()
+    assert m.o.elements_scheduled.wind_drift_factor == 1
+    assert m.o._config["wind_drift_depth"]["value"] == 10
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `particle_tracking_manager-0.8.0/tests/test_realistic.py` & `particle_tracking_manager-0.8.1/tests/test_realistic.py`

 * *Files identical despite different names*

### Comparing `particle_tracking_manager-0.8.0/tests/test_seeding.py` & `particle_tracking_manager-0.8.1/tests/test_seeding.py`

 * *Files identical despite different names*

