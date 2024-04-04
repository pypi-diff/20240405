# Comparing `tmp/gwpopulation-1.0.0rc0.tar.gz` & `tmp/gwpopulation-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwpopulation-1.0.0rc0.tar", last modified: Wed Jan 10 21:54:50 2024, max compression
+gzip compressed data, was "gwpopulation-1.0.0rc1.tar", last modified: Thu Feb  1 22:40:05 2024, max compression
```

## Comparing `gwpopulation-1.0.0rc0.tar` & `gwpopulation-1.0.0rc1.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.321552 gwpopulation-1.0.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.305551 gwpopulation-1.0.0rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.309551 gwpopulation-1.0.0rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-01-10 21:54:50.321552 gwpopulation-1.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.309551 gwpopulation-1.0.0rc0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/docs/Makefile.gh_pages
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/docs/Makefile.std
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.313552 gwpopulation-1.0.0rc0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.313552 gwpopulation-1.0.0rc0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)  5402044 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/examples/GWTC1.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.317551 gwpopulation-1.0.0rc0/gwpopulation/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-10 21:54:50.000000 gwpopulation-1.0.0rc0/gwpopulation/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/hyperpe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.317551 gwpopulation-1.0.0rc0/gwpopulation/models/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/models/interped.py
--rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/models/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/models/redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/models/spin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/gwpopulation/vt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.321552 gwpopulation-1.0.0rc0/gwpopulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-01-10 21:54:50.000000 gwpopulation-1.0.0rc0/gwpopulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-01-10 21:54:50.000000 gwpopulation-1.0.0rc0/gwpopulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 21:54:50.000000 gwpopulation-1.0.0rc0/gwpopulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-10 21:54:50.000000 gwpopulation-1.0.0rc0/gwpopulation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-10 21:54:50.000000 gwpopulation-1.0.0rc0/gwpopulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/pages_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.317551 gwpopulation-1.0.0rc0/priors/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/priors/bbh_population.prior
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/priors/mass_rates.prior
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/priors/spin.prior
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/priors/spin_talbot_thrane.prior
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-10 21:54:50.321552 gwpopulation-1.0.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 21:54:50.321552 gwpopulation-1.0.0rc0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/example_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/likelihood_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12213 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/mass_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/spin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/test.prior
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-10 21:54:43.000000 gwpopulation-1.0.0rc0/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.923865 gwpopulation-1.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.923865 gwpopulation-1.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.927865 gwpopulation-1.0.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/Makefile.gh_pages
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/Makefile.std
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.927865 gwpopulation-1.0.0rc1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.927865 gwpopulation-1.0.0rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  5402044 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/examples/GWTC1.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.931865 gwpopulation-1.0.0rc1/gwpopulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.931865 gwpopulation-1.0.0rc1/gwpopulation/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/experimental/jax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/experimental/numpyro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15537 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/hyperpe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.931865 gwpopulation-1.0.0rc1/gwpopulation/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/interped.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30430 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/models/spin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/gwpopulation/vt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/gwpopulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-01 22:40:05.000000 gwpopulation-1.0.0rc1/gwpopulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/pages_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.931865 gwpopulation-1.0.0rc1/priors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/priors/bbh_population.prior
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/priors/mass_rates.prior
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/priors/spin.prior
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/priors/spin_talbot_thrane.prior
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:40:05.935865 gwpopulation-1.0.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/likelihood_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12213 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/mass_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/spin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/test.prior
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-01 22:39:58.000000 gwpopulation-1.0.0rc1/test_requirements.txt
```

### Comparing `gwpopulation-1.0.0rc0/.codeclimate.yml` & `gwpopulation-1.0.0rc1/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/.github/workflows/pages.yml` & `gwpopulation-1.0.0rc1/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/.github/workflows/publish-to-pypi.yml` & `gwpopulation-1.0.0rc1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/.github/workflows/python-package.yml` & `gwpopulation-1.0.0rc1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/.pre-commit-config.yaml` & `gwpopulation-1.0.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/LICENSE.md` & `gwpopulation-1.0.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/PKG-INFO` & `gwpopulation-1.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpopulation
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: Unified population inference
 Home-page: https://github.com/ColmTalbot/gwpopulation
 Author: Colm Talbot
 Author-email: talbotcolm@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gwpopulation-1.0.0rc0/README.md` & `gwpopulation-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/docs/Makefile.gh_pages` & `gwpopulation-1.0.0rc1/docs/Makefile.gh_pages`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/docs/Makefile.std` & `gwpopulation-1.0.0rc1/docs/Makefile.std`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/docs/_templates/custom-class-template.rst` & `gwpopulation-1.0.0rc1/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/docs/_templates/custom-module-template.rst` & `gwpopulation-1.0.0rc1/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/docs/conf.py` & `gwpopulation-1.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/examples/GWTC1.ipynb` & `gwpopulation-1.0.0rc1/examples/GWTC1.ipynb`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/__init__.py` & `gwpopulation-1.0.0rc1/gwpopulation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """
 GWPopulation
 ============
 
-A collection of code for doing population inference with the
-gravitational-wave transient catalogue.
+:code:`GWPopulation` is a Python package for doing population inference
+with the gravitational-wave transient catalogue supporting a range of 
+numpy-like backends.
 
 This includes:
   - commonly used likelihood functions in the Bilby framework.
   - population models for gravitational-wave sources.
   - selection functions for gravitational-wave sources.
 
-:code:`GWPopulation` supports multiple numpy-like backends, including
-:code:`numpy`, :code:`jax`, and :code:`cupy`. The :code:`jax` and
-:code:`cupy` backends allow for GPU acceleration.
-
 The code is hosted at `<www.github.com/ColmTalbot/gwpopulation>`_ and
 available via :code:`conda-forge` and :code:`pypi`.
 """
 from . import conversions, hyperpe, models, utils, vt
 from ._version import __version__
 from .backend import SUPPORTED_BACKENDS, set_backend
```

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/backend.py` & `gwpopulation-1.0.0rc1/gwpopulation/backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,31 @@
 
 __backend__ = ""
 SUPPORTED_BACKENDS = ["numpy", "cupy", "jax"]
 _np_module = dict(numpy="numpy", cupy="cupy", jax="jax.numpy")
 _scipy_module = dict(numpy="scipy", cupy="cupyx.scipy", jax="jax.scipy")
 
 
+__doc__ = f"""
+:code:`GWPopulation` provides a unified interface to a number of :code:`numpy/scipy` like APIs.
+
+The backend can be set using :code:`gwpopulation.set_backend(backend)`, where
+:code:`backend` is one of :code:`{', '.join(SUPPORTED_BACKENDS)}`.
+
+Downstream packages can automatically track the active backend using :code:`entry_points`.
+With this set up, packages can use :code:`xp` and :code:`scs` in specified modules.
+
+..note::
+    Each module that wants to use the :code:`GWPopulation` backend must be specified independently
+    for the automatic propagation to work.
+
+If there is a backend that you would like to use that is not currently supported, please open an issue.
+"""
+
+
 def modules_to_update():
     import sys
 
     if sys.version_info < (3, 10):
         from importlib_metadata import entry_points
     else:
         from importlib.metadata import entry_points
```

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/conversions.py` & `gwpopulation-1.0.0rc1/gwpopulation/conversions.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/hyperpe.py` & `gwpopulation-1.0.0rc1/gwpopulation/hyperpe.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,25 +207,25 @@
         """
         self.parameters.update(sample.copy())
         self.parameters, added_keys = self.conversion_function(self.parameters)
         self.hyper_prior.parameters.update(self.parameters)
         ln_ls, variances = self._compute_per_event_ln_bayes_factors(
             return_uncertainty=True
         )
-        total_variance = float(sum(variances))
+        total_variance = sum(variances)
         for ii in range(self.n_posteriors):
-            sample[f"ln_bf_{ii}"] = float(ln_ls[ii])
-            sample[f"var_{ii}"] = float(variances[ii])
+            sample[f"ln_bf_{ii}"] = to_number(ln_ls[ii], float)
+            sample[f"var_{ii}"] = to_number(variances[ii], float)
         selection, variance = self._selection_function_with_uncertainty()
         variance /= selection**2
         selection_variance = variance * self.n_posteriors**2
         sample["selection"] = selection
         sample["selection_variance"] = variance
         total_variance += selection_variance
-        sample["variance"] = float(total_variance)
+        sample["variance"] = to_number(total_variance, float)
         if added_keys is not None:
             for key in added_keys:
                 self.parameters.pop(key)
         return sample
 
     def generate_rate_posterior_sample(self):
         r"""
```

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/models/interped.py` & `gwpopulation-1.0.0rc1/gwpopulation/models/interped.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/models/mass.py` & `gwpopulation-1.0.0rc1/gwpopulation/models/mass.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,15 +576,15 @@
         """Calculate the normalisation factor for the primary mass"""
         mmin = kwargs.get("mmin", self.mmin)
         if "jax" not in xp.__name__ and delta_m == 0:
             return 1
         p_m = self.__class__.primary_model(self.m1s, **kwargs)
         p_m *= self.smoothing(self.m1s, mmin=mmin, mmax=self.mmax, delta_m=delta_m)
 
-        norm = xp.where(delta_m > 0, xp.trapz(p_m, self.m1s), 1)
+        norm = xp.where(xp.array(delta_m) > 0, xp.trapz(p_m, self.m1s), 1)
         return norm
 
     def p_q(self, dataset, beta, mmin, delta_m):
         p_q = powerlaw(dataset["mass_ratio"], beta, 1, mmin / dataset["mass_1"])
         p_q *= self.smoothing(
             dataset["mass_1"] * dataset["mass_ratio"],
             mmin=mmin,
@@ -602,15 +602,15 @@
     def norm_p_q(self, beta, mmin, delta_m):
         """Calculate the mass ratio normalisation by linear interpolation"""
         p_q = powerlaw(self.qs_grid, beta, 1, mmin / self.m1s_grid)
         p_q *= self.smoothing(
             self.m1s_grid * self.qs_grid, mmin=mmin, mmax=self.m1s_grid, delta_m=delta_m
         )
         norms = xp.where(
-            delta_m > 0,
+            xp.array(delta_m) > 0,
             xp.nan_to_num(xp.trapz(p_q, self.qs, axis=0)),
             xp.ones(self.m1s.shape),
         )
 
         return self._q_interpolant(norms)
 
     def _cache_q_norms(self, masses):
```

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/models/redshift.py` & `gwpopulation-1.0.0rc1/gwpopulation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/models/spin.py` & `gwpopulation-1.0.0rc1/gwpopulation/models/spin.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/utils.py` & `gwpopulation-1.0.0rc1/gwpopulation/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Helper functions for probability distributions.
+Helper functions for probability distributions and backend switching.
 """
 from numbers import Number
 from operator import eq, ge, gt, le, lt, ne
 
 import numpy as np
 from scipy import special as scs
```

### Comparing `gwpopulation-1.0.0rc0/gwpopulation/vt.py` & `gwpopulation-1.0.0rc1/gwpopulation/vt.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/gwpopulation.egg-info/PKG-INFO` & `gwpopulation-1.0.0rc1/gwpopulation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpopulation
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: Unified population inference
 Home-page: https://github.com/ColmTalbot/gwpopulation
 Author: Colm Talbot
 Author-email: talbotcolm@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gwpopulation-1.0.0rc0/gwpopulation.egg-info/SOURCES.txt` & `gwpopulation-1.0.0rc1/gwpopulation.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 gwpopulation/utils.py
 gwpopulation/vt.py
 gwpopulation.egg-info/PKG-INFO
 gwpopulation.egg-info/SOURCES.txt
 gwpopulation.egg-info/dependency_links.txt
 gwpopulation.egg-info/requires.txt
 gwpopulation.egg-info/top_level.txt
+gwpopulation/experimental/__init__.py
+gwpopulation/experimental/jax.py
+gwpopulation/experimental/numpyro.py
 gwpopulation/models/__init__.py
 gwpopulation/models/interped.py
 gwpopulation/models/mass.py
 gwpopulation/models/redshift.py
 gwpopulation/models/spin.py
 priors/bbh_population.prior
 priors/mass_rates.prior
```

### Comparing `gwpopulation-1.0.0rc0/priors/bbh_population.prior` & `gwpopulation-1.0.0rc1/priors/bbh_population.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/priors/mass_rates.prior` & `gwpopulation-1.0.0rc1/priors/mass_rates.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/priors/spin.prior` & `gwpopulation-1.0.0rc1/priors/spin.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/setup.cfg` & `gwpopulation-1.0.0rc1/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -36,11 +36,16 @@
 [flake8]
 exclude = .git,build,dist,docs,test,*__init__.py
 max-line-length = 120
 ignore = E129 W503
 
 [tool:pytest]
 
+[coverage:run]
+omit = 
+	gwpopulation/experimental/**
+	gwpopulation/_version.py
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gwpopulation-1.0.0rc0/test/backend_test.py` & `gwpopulation-1.0.0rc1/test/backend_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/conversion_test.py` & `gwpopulation-1.0.0rc1/test/conversion_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/example_test.py` & `gwpopulation-1.0.0rc1/test/example_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/jax_utils.py` & `gwpopulation-1.0.0rc1/gwpopulation/experimental/jax.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/likelihood_test.py` & `gwpopulation-1.0.0rc1/test/likelihood_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/mass_test.py` & `gwpopulation-1.0.0rc1/test/mass_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/redshift_test.py` & `gwpopulation-1.0.0rc1/test/redshift_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/spin_test.py` & `gwpopulation-1.0.0rc1/test/spin_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/test.prior` & `gwpopulation-1.0.0rc1/test/test.prior`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/utils_test.py` & `gwpopulation-1.0.0rc1/test/utils_test.py`

 * *Files identical despite different names*

### Comparing `gwpopulation-1.0.0rc0/test/vt_test.py` & `gwpopulation-1.0.0rc1/test/vt_test.py`

 * *Files identical despite different names*

