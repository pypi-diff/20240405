# Comparing `tmp/CUQIpy-1.0.0.post0.dev84.tar.gz` & `tmp/CUQIpy-1.0.0.post0.dev91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-1.0.0.post0.dev84.tar", last modified: Fri Mar 15 09:59:33 2024, max compression
+gzip compressed data, was "CUQIpy-1.0.0.post0.dev91.tar", last modified: Thu Apr  4 14:41:36 2024, max compression
```

## Comparing `CUQIpy-1.0.0.post0.dev84.tar` & `CUQIpy-1.0.0.post0.dev91.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.913754 CUQIpy-1.0.0.post0.dev84/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.913754 CUQIpy-1.0.0.post0.dev84/CUQIpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18418 2024-03-15 09:59:33.000000 CUQIpy-1.0.0.post0.dev84/CUQIpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-03-15 09:59:33.000000 CUQIpy-1.0.0.post0.dev84/CUQIpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 09:59:33.000000 CUQIpy-1.0.0.post0.dev84/CUQIpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-15 09:59:33.000000 CUQIpy-1.0.0.post0.dev84/CUQIpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-15 09:59:33.000000 CUQIpy-1.0.0.post0.dev84/CUQIpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18418 2024-03-15 09:59:33.913754 CUQIpy-1.0.0.post0.dev84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.913754 CUQIpy-1.0.0.post0.dev84/cuqi/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-15 09:59:33.913754 CUQIpy-1.0.0.post0.dev84/cuqi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.893754 CUQIpy-1.0.0.post0.dev84/cuqi/array/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/array/_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.897754 CUQIpy-1.0.0.post0.dev84/cuqi/data/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   786696 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/data/astronaut.npz
--rw-r--r--   0 runner    (1001) docker     (127)   262408 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/data/camera.npz
--rw-r--r--   0 runner    (1001) docker     (127)   406164 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/data/cat.npz
--rw-r--r--   0 runner    (1001) docker     (127)   984680 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/data/cookie.png
--rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/data/satellite.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.897754 CUQIpy-1.0.0.post0.dev84/cuqi/density/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/density/_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.901754 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_cauchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_cmrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    18351 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)    33026 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_gmrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_inverse_gamma.py
--rw-r--r--   0 runner    (1001) docker     (127)    15043 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_laplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_lmrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_posterior.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.901754 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.901754 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_cwmh.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_langevin_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_mh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_pcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.901754 CUQIpy-1.0.0.post0.dev84/cuqi/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46804 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/geometry/_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.905754 CUQIpy-1.0.0.post0.dev84/cuqi/implicitprior/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/implicitprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/implicitprior/_regularizedGMRF.py
--rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/implicitprior/_regularizedGaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.905754 CUQIpy-1.0.0.post0.dev84/cuqi/likelihood/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/likelihood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/likelihood/_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.905754 CUQIpy-1.0.0.post0.dev84/cuqi/model/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26627 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.905754 CUQIpy-1.0.0.post0.dev84/cuqi/operator/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/operator/_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.905754 CUQIpy-1.0.0.post0.dev84/cuqi/pde/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/pde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/pde/_pde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.905754 CUQIpy-1.0.0.post0.dev84/cuqi/problem/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32018 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/problem/_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.905754 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_conjugate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_conjugate_approx.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_cwmh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_langevin_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_laplace_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_mh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_pcn.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_rto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.909754 CUQIpy-1.0.0.post0.dev84/cuqi/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34640 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/samples/_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.909754 CUQIpy-1.0.0.post0.dev84/cuqi/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.909754 CUQIpy-1.0.0.post0.dev84/cuqi/testproblem/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/testproblem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52540 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/testproblem/_testproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.909754 CUQIpy-1.0.0.post0.dev84/cuqi/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/utilities/_get_python_variable_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/cuqi/utilities/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 09:59:33.913754 CUQIpy-1.0.0.post0.dev84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:59:33.913754 CUQIpy-1.0.0.post0.dev84/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_MRFs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_abstract_distribution_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_bayesian_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    31681 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_distributions_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_implicit_priors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (127)    21330 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_pde.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_posterior.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    17657 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_testproblem.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-15 09:59:23.000000 CUQIpy-1.0.0.post0.dev84/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.279333 CUQIpy-1.0.0.post0.dev91/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.279333 CUQIpy-1.0.0.post0.dev91/CUQIpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18423 2024-04-04 14:41:36.000000 CUQIpy-1.0.0.post0.dev91/CUQIpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-04 14:41:36.000000 CUQIpy-1.0.0.post0.dev91/CUQIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:41:36.000000 CUQIpy-1.0.0.post0.dev91/CUQIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 14:41:36.000000 CUQIpy-1.0.0.post0.dev91/CUQIpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 14:41:36.000000 CUQIpy-1.0.0.post0.dev91/CUQIpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18423 2024-04-04 14:41:36.279333 CUQIpy-1.0.0.post0.dev91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.279333 CUQIpy-1.0.0.post0.dev91/cuqi/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-04 14:41:36.279333 CUQIpy-1.0.0.post0.dev91/cuqi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.259333 CUQIpy-1.0.0.post0.dev91/cuqi/array/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/array/_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.263333 CUQIpy-1.0.0.post0.dev91/cuqi/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   786696 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/data/astronaut.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   262408 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/data/camera.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   406164 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/data/cat.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   984680 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/data/cookie.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/data/satellite.mat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.263333 CUQIpy-1.0.0.post0.dev91/cuqi/density/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/density/_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.267333 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_cmrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10661 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18351 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33026 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_gmrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_inverse_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15043 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_lmrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.267333 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.267333 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_cwmh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_langevin_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_mh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_pcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.267333 CUQIpy-1.0.0.post0.dev91/cuqi/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46804 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/geometry/_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.267333 CUQIpy-1.0.0.post0.dev91/cuqi/implicitprior/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/implicitprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/implicitprior/_regularizedGMRF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/implicitprior/_regularizedGaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.267333 CUQIpy-1.0.0.post0.dev91/cuqi/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/likelihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/likelihood/_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.267333 CUQIpy-1.0.0.post0.dev91/cuqi/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26627 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.271333 CUQIpy-1.0.0.post0.dev91/cuqi/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/operator/_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.271333 CUQIpy-1.0.0.post0.dev91/cuqi/pde/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/pde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/pde/_pde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.271333 CUQIpy-1.0.0.post0.dev91/cuqi/problem/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32018 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/problem/_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.271333 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_conjugate_approx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_cwmh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_langevin_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_laplace_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_mh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_pcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_rto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.271333 CUQIpy-1.0.0.post0.dev91/cuqi/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34804 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/samples/_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.271333 CUQIpy-1.0.0.post0.dev91/cuqi/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22776 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.271333 CUQIpy-1.0.0.post0.dev91/cuqi/testproblem/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/testproblem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52540 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/testproblem/_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.275333 CUQIpy-1.0.0.post0.dev91/cuqi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/utilities/_get_python_variable_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/cuqi/utilities/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:41:36.279333 CUQIpy-1.0.0.post0.dev91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:41:36.275333 CUQIpy-1.0.0.post0.dev91/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_MRFs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_abstract_distribution_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_bayesian_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31681 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_distributions_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_implicit_priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21330 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_pde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17657 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-04 14:41:28.000000 CUQIpy-1.0.0.post0.dev91/tests/test_utilities.py
```

### Comparing `CUQIpy-1.0.0.post0.dev84/CUQIpy.egg-info/PKG-INFO` & `CUQIpy-1.0.0.post0.dev91/CUQIpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 1.0.0.post0.dev84
+Version: 1.0.0.post0.dev91
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>, Chao Zhang <chaz@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -198,15 +198,15 @@
 Project-URL: Download, https://github.com/CUQI-DTU/CUQIpy/releases
 Project-URL: Tracker, https://github.com/CUQI-DTU/CUQIpy/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy>=1.17.0
-Requires-Dist: scipy
+Requires-Dist: scipy<1.13
 Requires-Dist: arviz
 
 <div align="center">
 <img src="https://cuqi-dtu.github.io/CUQIpy/_static/logo.png" alt="CUQIpy logo" width="250"/>
 </div>
 
 # Computational Uncertainty Quantification for Inverse Problems in python
```

### Comparing `CUQIpy-1.0.0.post0.dev84/CUQIpy.egg-info/SOURCES.txt` & `CUQIpy-1.0.0.post0.dev91/CUQIpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/LICENSE` & `CUQIpy-1.0.0.post0.dev91/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/PKG-INFO` & `CUQIpy-1.0.0.post0.dev91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 1.0.0.post0.dev84
+Version: 1.0.0.post0.dev91
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>, Chao Zhang <chaz@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -198,15 +198,15 @@
 Project-URL: Download, https://github.com/CUQI-DTU/CUQIpy/releases
 Project-URL: Tracker, https://github.com/CUQI-DTU/CUQIpy/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy>=1.17.0
-Requires-Dist: scipy
+Requires-Dist: scipy<1.13
 Requires-Dist: arviz
 
 <div align="center">
 <img src="https://cuqi-dtu.github.io/CUQIpy/_static/logo.png" alt="CUQIpy logo" width="250"/>
 </div>
 
 # Computational Uncertainty Quantification for Inverse Problems in python
```

### Comparing `CUQIpy-1.0.0.post0.dev84/README.md` & `CUQIpy-1.0.0.post0.dev91/README.md`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/array/_array.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/array/_array.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/config.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/config.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/data/_data.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/data/_data.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/data/astronaut.npz` & `CUQIpy-1.0.0.post0.dev91/cuqi/data/astronaut.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/data/camera.npz` & `CUQIpy-1.0.0.post0.dev91/cuqi/data/camera.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/data/cat.npz` & `CUQIpy-1.0.0.post0.dev91/cuqi/data/cat.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/data/cookie.png` & `CUQIpy-1.0.0.post0.dev91/cuqi/data/cookie.png`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/data/satellite.mat` & `CUQIpy-1.0.0.post0.dev91/cuqi/data/satellite.mat`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/density/_density.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/density/_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/diagnostics.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/diagnostics.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/__init__.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_beta.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_beta.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_cauchy.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_cauchy.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_cmrf.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_cmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_custom.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_custom.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_distribution.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_gamma.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_gaussian.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_gaussian.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_gmrf.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_gmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_inverse_gamma.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_joint_distribution.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_laplace.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_laplace.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_lmrf.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_lmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_lognormal.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_lognormal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_normal.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_normal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_posterior.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_posterior.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/distribution/_uniform.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/distribution/_uniform.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_cwmh.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_cwmh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_langevin_algorithm.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_langevin_algorithm.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_mh.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_mh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_pcn.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_pcn.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/experimental/mcmc/_sampler.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/experimental/mcmc/_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/geometry/__init__.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/geometry/_geometry.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/geometry/_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/implicitprior/_regularizedGMRF.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/implicitprior/_regularizedGMRF.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/implicitprior/_regularizedGaussian.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/implicitprior/_regularizedGaussian.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/likelihood/__init__.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/likelihood/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/likelihood/_likelihood.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/likelihood/_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/model/_model.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/model/_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/operator/_operator.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/operator/_operator.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/pde/_pde.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/pde/_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/problem/_problem.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/problem/_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_conjugate.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_conjugate.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_conjugate_approx.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_conjugate_approx.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_cwmh.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_cwmh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_gibbs.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_gibbs.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_hmc.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_hmc.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_langevin_algorithm.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_langevin_algorithm.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_laplace_approximation.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_laplace_approximation.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_mh.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_mh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_pcn.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_pcn.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_rto.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_rto.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/sampler/_sampler.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/sampler/_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/samples/_samples.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/samples/_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,28 @@
 from cuqi.geometry import _DefaultGeometry1D, Continuous2D, Image2D
 from cuqi.array import CUQIarray
 from cuqi.utilities import force_ndarray
 from copy import copy
 from numbers import Number
 
 try:
-    import arviz # Plotting tool
-except ImportError:
+    import arviz  # Plotting tool
+except ImportError as e:
     arviz = None
+    arviz_import_error = e
+
 
 def _check_for_arviz():
     if arviz is None:
-        raise ImportError("The arviz package is required for this functionality. Please install arviz using `pip install arviz`.")
+        msg = "The arviz package is required for this functionality. "\
+            + "Please make sure arviz is installed. "\
+            + "See below for the original error message:\n"\
+            + arviz_import_error.args[0]
+
+        raise ImportError(msg)
 
 
 class Samples(object):
     """
     An object used to store samples from distributions. 
 
     Parameters
```

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/solver/_solver.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/testproblem/_testproblem.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/testproblem/_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/utilities/_get_python_variable_name.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/utilities/_get_python_variable_name.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/cuqi/utilities/_utilities.py` & `CUQIpy-1.0.0.post0.dev91/cuqi/utilities/_utilities.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/pyproject.toml` & `CUQIpy-1.0.0.post0.dev91/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_MRFs.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_MRFs.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_abstract_distribution_density.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_abstract_distribution_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_bayesian_inversion.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_bayesian_inversion.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_density.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_distribution.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_distributions_shape.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_distributions_shape.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_geometry.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_implicit_priors.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_implicit_priors.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_joint_distribution.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_likelihood.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_model.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_pde.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_posterior.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_posterior.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_problem.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_sampler.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_samples.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_solver.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_testproblem.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-1.0.0.post0.dev84/tests/test_utilities.py` & `CUQIpy-1.0.0.post0.dev91/tests/test_utilities.py`

 * *Files identical despite different names*

