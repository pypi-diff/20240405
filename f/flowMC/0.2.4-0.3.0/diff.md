# Comparing `tmp/flowMC-0.2.4.tar.gz` & `tmp/flowMC-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowMC-0.2.4.tar", last modified: Wed Jan  3 21:14:48 2024, max compression
+gzip compressed data, was "flowMC-0.3.0.tar", last modified: Fri Apr  5 21:30:46 2024, max compression
```

## Comparing `flowMC-0.2.4.tar` & `flowMC-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:48.464051 flowMC-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-03 21:14:39.000000 flowMC-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-01-03 21:14:48.464051 flowMC-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-01-03 21:14:39.000000 flowMC-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-03 21:14:39.000000 flowMC-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-03 21:14:48.464051 flowMC-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:48.460051 flowMC-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:48.460051 flowMC-0.2.4/src/flowMC/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:48.464051 flowMC-0.2.4/src/flowMC/nfmodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/nfmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/nfmodel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/nfmodel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/nfmodel/realNVP.py
--rw-r--r--   0 runner    (1001) docker     (127)    18406 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/nfmodel/rqSpline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/nfmodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:48.464051 flowMC-0.2.4/src/flowMC/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/sampler/Gaussian_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/sampler/HMC.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/sampler/MALA.py
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/sampler/NF_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/sampler/Proposal_Base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20867 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/sampler/Sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/sampler/flowHMC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:48.464051 flowMC-0.2.4/src/flowMC/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/utils/EvolutionaryOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/utils/PRNG_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/utils/PythonFunctionWrap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:39.000000 flowMC-0.2.4/src/flowMC/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 21:14:48.464051 flowMC-0.2.4/src/flowMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-01-03 21:14:48.000000 flowMC-0.2.4/src/flowMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-01-03 21:14:48.000000 flowMC-0.2.4/src/flowMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 21:14:48.000000 flowMC-0.2.4/src/flowMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-03 21:14:48.000000 flowMC-0.2.4/src/flowMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-03 21:14:48.000000 flowMC-0.2.4/src/flowMC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-05 21:30:39.000000 flowMC-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-05 21:30:46.194362 flowMC-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-05 21:30:39.000000 flowMC-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 21:30:39.000000 flowMC-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-05 21:30:46.194362 flowMC-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.190362 flowMC-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.190362 flowMC-0.3.0/src/flowMC/
+-rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.190362 flowMC-0.3.0/src/flowMC/nfmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/realNVP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/rqSpline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/src/flowMC/proposal/
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/Gaussian_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/HMC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/MALA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/NF_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/flowHMC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/src/flowMC/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/strategy/global_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/strategy/importance_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/src/flowMC/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/utils/EvolutionaryOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/utils/PythonFunctionWrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/utils/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/src/flowMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/top_level.txt
```

### Comparing `flowMC-0.2.4/LICENSE` & `flowMC-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.4/PKG-INFO` & `flowMC-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.2.4
+Version: 0.3.0
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax>=0.4.12
 Requires-Dist: jaxlib>=0.4.12
 Requires-Dist: equinox>=0.10.6
 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4
 Requires-Dist: tqdm
+Requires-Dist: corner
 
 # flowMC
 
 **Normalizing-flow enhanced sampling package for probabilistic inference**
 
 <a href="https://flowmc.readthedocs.io/en/main/">
 <img src="https://badgen.net/badge/Read/the doc/blue" alt="doc"/>
@@ -80,14 +81,49 @@
     * corner
     * arviz
 
 The test suite is based on pytest. To run the tests, one needs to install `pytest` and run `pytest` at the root directory of this repo.
 
 # Attribution
 
-A Jax implementation of methods described in: 
+If you used `flowMC` in your research, we would really appericiate it if you could at least cite the following papers:
+
+```
+@article{Wong:2022xvh,
+    author = "Wong, Kaze W. k. and Gabri\'e, Marylou and Foreman-Mackey, Daniel",
+    title = "{flowMC: Normalizing flow enhanced sampling package for probabilistic inference in JAX}",
+    eprint = "2211.06397",
+    archivePrefix = "arXiv",
+    primaryClass = "astro-ph.IM",
+    doi = "10.21105/joss.05021",
+    journal = "J. Open Source Softw.",
+    volume = "8",
+    number = "83",
+    pages = "5021",
+    year = "2023"
+}
+
+@article{Gabrie:2021tlu,
+    author = "Gabri\'e, Marylou and Rotskoff, Grant M. and Vanden-Eijnden, Eric",
+    title = "{Adaptive Monte Carlo augmented with normalizing flows}",
+    eprint = "2105.12603",
+    archivePrefix = "arXiv",
+    primaryClass = "physics.data-an",
+    doi = "10.1073/pnas.2109420119",
+    journal = "Proc. Nat. Acad. Sci.",
+    volume = "119",
+    number = "10",
+    pages = "e2109420119",
+    year = "2022"
+}
+```
+
+This will help `flowMC` getting more recognition, and the main benefit *for you* is this means the `flowMC` community will grow and it will be continuously improved. If you believe in the magic of open-source software, please support us by attributing our software in your work.
+
+
+`flowMC` is a Jax implementation of methods described in: 
 > *Efficient Bayesian Sampling Using Normalizing Flows to Assist Markov Chain Monte Carlo Methods* Gabrié M., Rotskoff G. M., Vanden-Eijnden E. - ICML INNF+ workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx)
 
 > *Adaptive Monte Carlo augmented with normalizing flows.*
 Gabrié M., Rotskoff G. M., Vanden-Eijnden E. - PNAS 2022 - [doi](https://www.pnas.org/doi/10.1073/pnas.2109420119), [arxiv](https://arxiv.org/abs/2105.12603)
```

#### html2text {}

```diff
@@ -1,38 +1,54 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.2.4 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.0 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
-learning,normalizing,autodiff,jax Requires-Python: >=3.9 Description-Content-
+learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
-Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm # flowMC **Normalizing-flow
-enhanced sampling package for probabilistic inference** _[_d_o_c_]_[_d_o_c_]!
-[flowMC_logo](./docs/logo_0810.png) flowMC is a Jax-based python package for
-normalizing-flow enhanced Markov chain Monte Carlo (MCMC) sampling. The code is
-open source under MIT license, and it is under active development. - Just-in-
-time compilation is supported. - Native support for GPU acceleration. - Suit
-for problems with multi-modality. - Minimal tuning. # Installation The simplest
-way to install the package is to do it through pip ``` pip install flowMC ```
-This will install the latest stable release and its dependencies. flowMC is
-based on [Jax](https://github.com/google/jax) and [Equinox](https://github.com/
-patrick-kidger/equinox). By default, installing flowMC will automatically
-install Jax and Equinox available on [PyPI](https://pypi.org). Jax does not
-install GPU support by default. If you want to use GPU with Jax, you need to
-install Jax with GPU support according to their document. At the time of
-writing this documentation page, this is the command to install Jax with GPU
-support: ``` pip install --upgrade "jax[cuda12_pip]" -f https://
+Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
+**Normalizing-flow enhanced sampling package for probabilistic inference**
+_[_d_o_c_]_[_d_o_c_]![flowMC_logo](./docs/logo_0810.png) flowMC is a Jax-based python
+package for normalizing-flow enhanced Markov chain Monte Carlo (MCMC) sampling.
+The code is open source under MIT license, and it is under active development.
+- Just-in-time compilation is supported. - Native support for GPU acceleration.
+- Suit for problems with multi-modality. - Minimal tuning. # Installation The
+simplest way to install the package is to do it through pip ``` pip install
+flowMC ``` This will install the latest stable release and its dependencies.
+flowMC is based on [Jax](https://github.com/google/jax) and [Equinox](https://
+github.com/patrick-kidger/equinox). By default, installing flowMC will
+automatically install Jax and Equinox available on [PyPI](https://pypi.org).
+Jax does not install GPU support by default. If you want to use GPU with Jax,
+you need to install Jax with GPU support according to their document. At the
+time of writing this documentation page, this is the command to install Jax
+with GPU support: ``` pip install --upgrade "jax[cuda12_pip]" -f https://
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` If you want to
 install the latest version of flowMC, you can clone this repo and install it
 locally: ``` git clone https://github.com/kazewong/flowMC.git cd flowMC pip
 install -e . ``` ## Requirements Here is a list of packages we use in the main
 library * Python 3.9+ * Jax * Jaxlib * equinox To visualize the inference
 results in the examples, we requrie the following packages in addtion to the
 above: * matplotlib * corner * arviz The test suite is based on pytest. To run
 the tests, one needs to install `pytest` and run `pytest` at the root directory
-of this repo. # Attribution A Jax implementation of methods described in: >
-*Efficient Bayesian Sampling Using Normalizing Flows to Assist Markov Chain
-Monte Carlo Methods* GabriÃ© M., Rotskoff G. M., Vanden-Eijnden E. - ICML INNF+
-workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx) > *Adaptive
-Monte Carlo augmented with normalizing flows.* GabriÃ© M., Rotskoff G. M.,
-Vanden-Eijnden E. - PNAS 2022 - [doi](https://www.pnas.org/doi/10.1073/
+of this repo. # Attribution If you used `flowMC` in your research, we would
+really appericiate it if you could at least cite the following papers: ```
+@article{Wong:2022xvh, author = "Wong, Kaze W. k. and Gabri\'e, Marylou and
+Foreman-Mackey, Daniel", title = "{flowMC: Normalizing flow enhanced sampling
+package for probabilistic inference in JAX}", eprint = "2211.06397",
+archivePrefix = "arXiv", primaryClass = "astro-ph.IM", doi = "10.21105/
+joss.05021", journal = "J. Open Source Softw.", volume = "8", number = "83",
+pages = "5021", year = "2023" } @article{Gabrie:2021tlu, author = "Gabri\'e,
+Marylou and Rotskoff, Grant M. and Vanden-Eijnden, Eric", title = "{Adaptive
+Monte Carlo augmented with normalizing flows}", eprint = "2105.12603",
+archivePrefix = "arXiv", primaryClass = "physics.data-an", doi = "10.1073/
+pnas.2109420119", journal = "Proc. Nat. Acad. Sci.", volume = "119", number =
+"10", pages = "e2109420119", year = "2022" } ``` This will help `flowMC`
+getting more recognition, and the main benefit *for you* is this means the
+`flowMC` community will grow and it will be continuously improved. If you
+believe in the magic of open-source software, please support us by attributing
+our software in your work. `flowMC` is a Jax implementation of methods
+described in: > *Efficient Bayesian Sampling Using Normalizing Flows to Assist
+Markov Chain Monte Carlo Methods* GabriÃ© M., Rotskoff G. M., Vanden-Eijnden E.
+- ICML INNF+ workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx) >
+*Adaptive Monte Carlo augmented with normalizing flows.* GabriÃ© M., Rotskoff
+G. M., Vanden-Eijnden E. - PNAS 2022 - [doi](https://www.pnas.org/doi/10.1073/
 pnas.2109420119), [arxiv](https://arxiv.org/abs/2105.12603)
```

### Comparing `flowMC-0.2.4/setup.cfg` & `flowMC-0.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flowMC
-version = 0.2.4
+version = 0.3.0
 author = Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 author_email = kazewong.physics@gmail.com
 url = https://github.com/kazewong/flowMC
 description = Normalizing flow exhanced sampler in jax
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = sampling, inference, machine learning, normalizing, autodiff, jax
@@ -17,15 +17,16 @@
 install_requires = 
 	jax>=0.4.12
 	jaxlib>=0.4.12
 	equinox>=0.10.6
 	optax>=0.1.5
 	evosax>=0.1.4
 	tqdm
-python_requires = >=3.9
+	corner
+python_requires = >=3.10
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `flowMC-0.2.4/src/flowMC/nfmodel/common.py` & `flowMC-0.3.0/src/flowMC/nfmodel/realNVP.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,207 +1,216 @@
-from typing import Callable, List, Iterable, Tuple
-
-import jax
-import jax.numpy as jnp
-from jaxtyping import Array
-import equinox as eqx
-
-from flowMC.nfmodel.base import Bijection, Distribution
-
+from typing import List, Tuple
 import jax
 import jax.numpy as jnp
+import numpy as np
 import equinox as eqx
-from jaxtyping import Array
-    
-class MLP(eqx.Module):
-    r"""Multilayer perceptron.
+from flowMC.nfmodel.base import NFModel, Distribution
+from flowMC.nfmodel.common import MLP, MaskedCouplingLayer, MLPAffine, Gaussian
+from jaxtyping import Array, Float, PRNGKeyArray
+from functools import partial
+import optax
 
-    Args:
-        shape (Iterable[int]): Shape of the MLP. The first element is the input dimension, the last element is the output dimension.
-        key (jax.random.PRNGKey): Random key.
 
-    Attributes:
-        layers (List): List of layers.
-        activation (Callable): Activation function.
-        use_bias (bool): Whether to use bias.        
+class AffineCoupling(eqx.Module):
     """
-    layers: List
-
-    def __init__(self, shape: Iterable[int], key: jax.random.PRNGKey, scale: float = 1e-4, activation: Callable = jax.nn.relu, use_bias: bool = True):
-        self.layers = []
-        for i in range(len(shape) - 2):
-            key, subkey1, subkey2 = jax.random.split(key, 3)
-            layer = eqx.nn.Linear(shape[i], shape[i + 1], key=subkey1, use_bias=use_bias)
-            weight = jax.random.normal(subkey2, (shape[i + 1], shape[i]))*jnp.sqrt(scale/shape[i])
-            layer = eqx.tree_at(lambda l: l.weight, layer, weight)
-            self.layers.append(layer)
-            self.layers.append(activation)
-        key, subkey = jax.random.split(key)
-        self.layers.append(eqx.nn.Linear(shape[-2], shape[-1], key=subkey, use_bias=use_bias))
-
-    def __call__(self, x: Array):
-        for layer in self.layers:
-            x = layer(x)
-        return x
-    
-    @property
-    def n_input(self) -> int:
-        return self.layers[0].in_features
-    
-    @property
-    def n_output(self) -> int:
-        return self.layers[-1].out_features
-
-    @property
-    def dtype(self) -> jnp.dtype:
-        return self.layers[0].weight.dtype
-
-
-class MaskedCouplingLayer(Bijection):
-
-    r"""Masked coupling layer.
-
-    f(x) = (1-m)*b(x;c(m*x;z)) + m*x
-    where b is the inner bijector, m is the mask, and c is the conditioner.
+    Affine coupling layer.
+    (Defined in the RealNVP paper https://arxiv.org/abs/1605.08803)
+    We use tanh as the default activation function.
 
     Args:
-        bijector (Bijection): inner bijector in the masked coupling layer.
-        mask (Array): Mask. 0 for the input variables that are transformed, 1 for the input variables that are not transformed.
-
+        n_features: (int) The number of features in the input.
+        n_hidden: (int) The number of hidden units in the MLP.
+        mask: (ndarray) Alternating mask for the affine coupling layer.
+        dt: (Float) Scaling factor for the affine coupling layer.
     """
 
     _mask: Array
-    bijector: Bijection
+    scale_MLP: MLP
+    translate_MLP: MLP
+    dt: Float = 1
+
+    def __init__(
+        self,
+        n_features: int,
+        n_hidden: int,
+        mask: Array,
+        key: PRNGKeyArray,
+        dt: Float = 1,
+        scale: Float = 1e-4,
+    ):
+        self._mask = mask
+        self.dt = dt
+        key, scale_subkey, translate_subkey = jax.random.split(key, 3)
+        features = [n_features, n_hidden, n_features]
+        self.scale_MLP = MLP(features, key=scale_subkey, scale=scale)
+        self.translate_MLP = MLP(features, key=translate_subkey, scale=scale)
 
     @property
     def mask(self):
         return jax.lax.stop_gradient(self._mask)
 
-    def __init__(self, bijector: Bijection, mask: Array):
-        self.bijector = bijector
-        self._mask = mask
+    @property
+    def n_features(self):
+        return self.scale_MLP.n_input
+
+    def __call__(self, x: Array):
+        return self.forward(x)
 
     def forward(self, x: Array) -> Tuple[Array, Array]:
-        y, log_det = self.bijector(x, x*self.mask)
-        y = (1-self.mask)*y + self.mask*x
-        log_det = ((1-self.mask)*log_det).sum()
-        return y, log_det
+        """From latent space to data space
 
-    def inverse(self, x: Array) -> Tuple[Array, Array]:
-        y, log_det = self.bijector.inverse(x, x*self.mask)
-        y = (1-self.mask)*y + self.mask*x
-        log_det = ((1-self.mask)*log_det).sum()
-        return y, log_det
+        Args:
+            x: (Array) Latent space.
 
-class MLPAffine(Bijection):
-    scale_MLP: MLP
-    shift_MLP: MLP
-    dt: float = 1
+        Returns:
+            outputs: (Array) Data space.
+            log_det: (Array) Log determinant of the Jacobian.
+        """
+        s = self.mask * self.scale_MLP(x * (1 - self.mask))
+        s = jnp.tanh(s) * self.dt
+        t = self.mask * self.translate_MLP(x * (1 - self.mask)) * self.dt
+
+        # Compute log determinant of the Jacobian
+        log_det = s.sum()
+
+        # Apply the transformation
+        outputs = (x + t) * jnp.exp(s)
+        return outputs, log_det
 
-    def __init__(self, scale_MLP: MLP, shift_MLP: MLP, dt: float = 1):
-        self.scale_MLP = scale_MLP
-        self.shift_MLP = shift_MLP
-        self.dt = dt
+    def inverse(self, x: Array) -> Tuple[Array, Array]:
+        """From data space to latent space
 
-    def __call__(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
-        return self.forward(x, condition_x)
+        Args:
+            x: (Array) Data space.
 
-    def forward(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
-        # Note that this note output log_det as an array instead of a number.
-        # This is because we need to sum over the log_det in the masked coupling layer.
-        scale = jnp.tanh(self.scale_MLP(condition_x)) * self.dt
-        shift = self.shift_MLP(condition_x) * self.dt
-        log_det = scale
-        y = (x + shift) * jnp.exp(scale)
-        return y, log_det
-
-    def inverse(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
-        scale = jnp.tanh(self.scale_MLP(condition_x)) * self.dt
-        shift = self.shift_MLP(condition_x) * self.dt
-        log_det = -scale
-        y = x  * jnp.exp(-scale) - shift
-        return y, log_det
-
-class ScalarAffine(Bijection):
-    scale: Array
-    shift: Array
-
-    def __init__(self, scale: float, shift: float):
-        self.scale = jnp.array(scale)
-        self.shift = jnp.array(shift)
-
-    def __call__(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
-        return self.forward(x, condition_x)
-
-    def forward(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
-        y = (x + self.shift) * jnp.exp(self.scale)
-        log_det = self.scale
-        return y, log_det
-
-    def inverse(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
-        y = x * jnp.exp(-self.scale) - self.shift
-        log_det = -self.scale
-        return y, log_det
+        Returns:
+            outputs: (Array) Latent space.
+            log_det: (Array) Log determinant of the Jacobian.
+        """
+        s = self.mask * self.scale_MLP(x * (1 - self.mask))
+        s = jnp.tanh(s) * self.dt
+        t = self.mask * self.translate_MLP(x * (1 - self.mask)) * self.dt
+        log_det = -s.sum()
+        outputs = x * jnp.exp(-s) - t
+        return outputs, log_det
 
-class Gaussian(Distribution):
 
-    r"""Multivariate Gaussian distribution.
-    
-    Args:
-        mean (Array): Mean.
-        cov (Array): Covariance matrix.
-        learnable (bool): Whether the mean and covariance matrix are learnable parameters.
-
-    Attributes:
-        mean (Array): Mean.
-        cov (Array): Covariance matrix.
+class RealNVP(NFModel):
     """
+    RealNVP mode defined in the paper https://arxiv.org/abs/1605.08803.
+    MLP is needed to make sure the scaling between layers are more or less the same.
 
-    _mean: Array
-    _cov: Array
-    learnable: bool = False
+    Args:
+        n_layers: (int) The number of affine coupling layers.
+        n_features: (int) The number of features in the input.
+        n_hidden: (int) The number of hidden units in the MLP.
+        dt: (Float) Scaling factor for the affine coupling layer.
+
+    Properties:
+        data_mean: (ndarray) Mean of Gaussian base distribution
+        data_cov: (ndarray) Covariance of Gaussian base distribution
+    """
 
-    @property
-    def mean(self) -> Array:
-        if self.learnable:
-            return self._mean
+    base_dist: Distribution
+    affine_coupling: List[MaskedCouplingLayer]
+    _n_features: int
+    _data_mean: Float[Array, " n_dim"] | None
+    _data_cov: Float[Array, " n_dim n_dim"] | None
+
+    @property
+    def n_features(self):
+        return self._n_features
+
+    @property
+    def data_mean(self):
+        return jax.lax.stop_gradient(self._data_mean)
+
+    @property
+    def data_cov(self):
+        return jax.lax.stop_gradient(jnp.atleast_2d(self._data_cov))
+
+    def __init__(
+        self,
+        n_features: int,
+        n_layers: int,
+        n_hidden: int,
+        key: PRNGKeyArray,
+        **kwargs
+    ):
+        if kwargs.get("base_dist") is not None:
+            self.base_dist = kwargs.get("base_dist")  # type: ignore
         else:
-            return jax.lax.stop_gradient(self._mean)
+            self.base_dist = Gaussian(
+                jnp.zeros(n_features), jnp.eye(n_features), learnable=False
+            )
 
-    @property
-    def cov(self) -> Array:
-        if self.learnable:
-            return self._cov
+        if kwargs.get("data_mean") is not None:
+            self._data_mean = kwargs.get("data_mean")
         else:
-            return jax.lax.stop_gradient(self._cov)
+            self._data_mean = jnp.zeros(n_features)
 
-    def __init__(self, mean: Array, cov: Array, learnable: bool = False):
-        self._mean = mean
-        self._cov = cov
-        self.learnable = learnable
+        if kwargs.get("data_cov") is not None:
+            self._data_cov = kwargs.get("data_cov")
+        else:
+            self._data_cov = jnp.eye(n_features)
 
-    def log_prob(self, x: Array) -> Array:
-        return jax.scipy.stats.multivariate_normal.logpdf(x, self.mean, self.cov)
+        self._n_features = n_features
 
-    def sample(self, key: jax.random.PRNGKey, n_samples: int = 1) -> Array:
-        return jax.random.multivariate_normal(key, self.mean, self.cov, (n_samples,))
-    
-class Composable(Distribution):
-
-    distributions: list[Distribution]
-    partitions: dict[str, tuple[int, int]]
-
-    def __init__(self, distributions: list[Distribution], partitions: dict):
-        self.distributions = distributions
-        self.partitions = partitions
+        def make_layer(i: int, key: PRNGKeyArray):
+            key, scale_subkey, shift_subkey = jax.random.split(key, 3)
+            mask = jnp.ones(n_features)
+            mask = mask.at[: int(n_features / 2)].set(0)
+            mask = jax.lax.cond(i % 2 == 0, lambda x: 1 - x, lambda x: x, mask)
+            scale_MLP = MLP([n_features, n_hidden, n_features], key=scale_subkey)
+            shift_MLP = MLP([n_features, n_hidden, n_features], key=shift_subkey)
+            return MaskedCouplingLayer(MLPAffine(scale_MLP, shift_MLP), mask)
+
+        keys = jax.random.split(key, n_layers)
+        self.affine_coupling = eqx.filter_vmap(make_layer)(jnp.arange(n_layers), keys)
+
+    def __call__(self, x: Array) -> Tuple[Array, Float]:
+        return self.forward(x)
+
+    def forward(self, x: Array) -> Tuple[Array, Float]:
+        log_det = 0.0
+        dynamics, statics = eqx.partition(self.affine_coupling, eqx.is_array)
+
+        def f(carry, data):
+            x, log_det = carry
+            layers = eqx.combine(data, statics)
+            x, log_det_i = layers(x)
+            return (x, log_det + log_det_i), None
+
+        (x, log_det), _ = jax.lax.scan(f, (x, log_det), dynamics)
+        return x, log_det
+
+    @partial(jax.vmap, in_axes=(None, 0))
+    def inverse(self, x: Array) -> Tuple[Array, Float]:
+        """From latent space to data space"""
+        log_det = 0.0
+        dynamics, statics = eqx.partition(self.affine_coupling, eqx.is_array)
+
+        def f(carry, data):
+            x, log_det = carry
+            layers = eqx.combine(data, statics)
+            x, log_det_i = layers.inverse(x)
+            return (x, log_det + log_det_i), None
+
+        (x, log_det), _ = jax.lax.scan(f, (x, log_det), dynamics, reverse=True)
+        return x, log_det
+
+    @eqx.filter_jit
+    def sample(self, rng_key: PRNGKeyArray, n_samples: int) -> Array:
+        samples = self.base_dist.sample(rng_key, n_samples)
+        samples = self.inverse(samples)[0]
+        samples = samples * jnp.sqrt(jnp.diag(self.data_cov)) + self.data_mean
+        return samples
 
+    @eqx.filter_jit
+    @partial(jax.vmap, in_axes=(None, 0))
     def log_prob(self, x: Array) -> Array:
-        log_prob = 0
-        for dist, (_, ranges) in zip(self.distributions, self.partitions.items()):
-            log_prob += dist.log_prob(x[ranges[0]:ranges[1]])
-        return log_prob
-    
-    def sample(self, rng_key: jax.random.PRNGKey, n_samples: int) -> Array:
-        samples = {}
-        for dist, (key,_) in zip(self.distributions, self.partitions.items()):
-            rng_key, sub_key = jax.random.split(rng_key)
-            samples[key] = dist.sample(sub_key, n_samples=n_samples)
+        x = (x - self.data_mean) / jnp.sqrt(jnp.diag(self.data_cov))
+        y, log_det = self.__call__(x)
+        log_det = log_det + jax.scipy.stats.multivariate_normal.logpdf(
+            y, jnp.zeros(self.n_features), jnp.eye(self.n_features)
+        )
+        return log_det
```

### Comparing `flowMC-0.2.4/src/flowMC/nfmodel/rqSpline.py` & `flowMC-0.3.0/src/flowMC/nfmodel/rqSpline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import Sequence, Tuple
 import jax
 import jax.numpy as jnp
-from jaxtyping import Array
+from jaxtyping import Array, PRNGKeyArray, Float
 import equinox as eqx
 
 from flowMC.nfmodel.base import NFModel, Bijection, Distribution
 from flowMC.nfmodel.common import MaskedCouplingLayer, ScalarAffine, MLP, Gaussian
 from functools import partial
 
 
 @partial(jax.vmap, in_axes=(0, None, None))
-def _normalize_bin_sizes(unnormalized_bin_sizes: Array,
-                         total_size: float,
-                         min_bin_size: float) -> Array:
-  """Make bin sizes sum to `total_size` and be no less than `min_bin_size`."""
-  num_bins = unnormalized_bin_sizes.shape[-1]
-  bin_sizes = jax.nn.softmax(unnormalized_bin_sizes, axis=-1)
-  return bin_sizes * (total_size - num_bins * min_bin_size) + min_bin_size
+def _normalize_bin_sizes(
+    unnormalized_bin_sizes: Array, total_size: float, min_bin_size: float
+) -> Array:
+    """Make bin sizes sum to `total_size` and be no less than `min_bin_size`."""
+    num_bins = unnormalized_bin_sizes.shape[-1]
+    bin_sizes = jax.nn.softmax(unnormalized_bin_sizes, axis=-1)
+    return bin_sizes * (total_size - num_bins * min_bin_size) + min_bin_size
+
 
 @partial(jax.vmap, in_axes=(0, None))
-def _normalize_knot_slopes(unnormalized_knot_slopes: Array,
-                           min_knot_slope: float) -> Array:
-  """Make knot slopes be no less than `min_knot_slope`."""
-  # The offset is such that the normalized knot slope will be equal to 1
-  # whenever the unnormalized knot slope is equal to 0.
-  min_knot_slope = jnp.array(
-      min_knot_slope, dtype=unnormalized_knot_slopes.dtype)
-  offset = jnp.log(jnp.exp(1. - min_knot_slope) - 1.)
-  return jax.nn.softplus(unnormalized_knot_slopes + offset) + min_knot_slope
+def _normalize_knot_slopes(
+    unnormalized_knot_slopes: Array, min_knot_slope: Float
+) -> Array:
+    """Make knot slopes be no less than `min_knot_slope`."""
+    # The offset is such that the normalized knot slope will be equal to 1
+    # whenever the unnormalized knot slope is equal to 0.
+    min_knot_slope = jnp.array(min_knot_slope, dtype=unnormalized_knot_slopes.dtype)
+    offset = jnp.log(jnp.exp(1.0 - min_knot_slope) - 1.0)
+    return jax.nn.softplus(unnormalized_knot_slopes + offset) + min_knot_slope
+
 
 @partial(jax.vmap, in_axes=(0, 0, 0, 0))
-def _rational_quadratic_spline_fwd(x: Array,
-                                   x_pos: Array,
-                                   y_pos: Array,
-                                   knot_slopes: Array) -> Tuple[Array, Array]:
+def _rational_quadratic_spline_fwd(
+    x: Array, x_pos: Array, y_pos: Array, knot_slopes: Array
+) -> tuple[Array, Array]:
     """Applies a rational-quadratic spline to a scalar.
 
     Args:
     x: a scalar (0-dimensional array). The scalar `x` can be any real number; it
         will be transformed by the spline if it's in the closed interval
         `[x_pos[0], x_pos[-1]]`, and it will be transformed linearly if it's
         outside that interval.
@@ -51,16 +51,17 @@
     # Search to find the right bin. NOTE: The bins are sorted, so we could use
     # binary search, but this is more GPU/TPU friendly.
     # The following implementation avoids indexing for faster TPU computation.
     below_range = x <= x_pos[0]
     above_range = x >= x_pos[-1]
     correct_bin = jnp.logical_and(x >= x_pos[:-1], x < x_pos[1:])
     any_bin_in_range = jnp.any(correct_bin)
-    first_bin = jnp.concatenate([jnp.array([1]),
-                                jnp.zeros(len(correct_bin)-1)]).astype(bool)
+    first_bin = jnp.concatenate(
+        [jnp.array([1]), jnp.zeros(len(correct_bin) - 1)]
+    ).astype(bool)
     # If y does not fall into any bin, we use the first spline in the following
     # computations to avoid numerical issues.
     correct_bin = jnp.where(any_bin_in_range, correct_bin, first_bin)
     # Dot product of each parameter with the correct bin mask.
     params = jnp.stack([x_pos, y_pos, knot_slopes], axis=1)
     params_bin_left = jnp.sum(correct_bin[:, None] * params[:-1], axis=0)
     params_bin_right = jnp.sum(correct_bin[:, None] * params[1:], axis=0)
@@ -73,77 +74,84 @@
     bin_height = y_pos_bin[1] - y_pos_bin[0]
     bin_slope = bin_height / bin_width
 
     z = (x - x_pos_bin[0]) / bin_width
     # `z` should be in range [0, 1] to avoid NaNs later. This can happen because
     # of small floating point issues or when x is outside of the range of bins.
     # To avoid all problems, we restrict z in [0, 1].
-    z = jnp.clip(z, 0., 1.)
+    z = jnp.clip(z, 0.0, 1.0)
     sq_z = z * z
     z1mz = z - sq_z  # z(1-z)
-    sq_1mz = (1. - z) ** 2
-    slopes_term = knot_slopes_bin[1] + knot_slopes_bin[0] - 2. * bin_slope
+    sq_1mz = (1.0 - z) ** 2
+    slopes_term = knot_slopes_bin[1] + knot_slopes_bin[0] - 2.0 * bin_slope
     numerator = bin_height * (bin_slope * sq_z + knot_slopes_bin[0] * z1mz)
     denominator = bin_slope + slopes_term * z1mz
     y = y_pos_bin[0] + numerator / denominator
 
     # Compute log det Jacobian.
     # The logdet is a sum of 3 logs. It is easy to see that the inputs of the
     # first two logs are guaranteed to be positive because we ensured that z is in
     # [0, 1]. This is also true of the log(denominator) because:
     # denominator
     # == bin_slope + (knot_slopes_bin[1] + knot_slopes_bin[0] - 2 * bin_slope) *
     # z*(1-z)
     # >= bin_slope - 2 * bin_slope * z * (1-z)
     # >= bin_slope - 2 * bin_slope * (1/4)
     # == bin_slope / 2
-    logdet = 2. * jnp.log(bin_slope) + jnp.log(
-        knot_slopes_bin[1] * sq_z + 2. * bin_slope * z1mz +
-        knot_slopes_bin[0] * sq_1mz) - 2. * jnp.log(denominator)
+    logdet = (
+        2.0 * jnp.log(bin_slope)
+        + jnp.log(
+            knot_slopes_bin[1] * sq_z
+            + 2.0 * bin_slope * z1mz
+            + knot_slopes_bin[0] * sq_1mz
+        )
+        - 2.0 * jnp.log(denominator)
+    )
 
     # If x is outside the spline range, we default to a linear transformation.
     y = jnp.where(below_range, (x - x_pos[0]) * knot_slopes[0] + y_pos[0], y)
-    y = jnp.where(above_range, (x - x_pos[-1]) * knot_slopes[-1] + y_pos[-1], y)
+    y = jnp.where(
+        above_range, (x - x_pos[-1]) * knot_slopes[-1] + y_pos[-1], y  # type: ignore
+    )
     logdet = jnp.where(below_range, jnp.log(knot_slopes[0]), logdet)
     logdet = jnp.where(above_range, jnp.log(knot_slopes[-1]), logdet)
     return y, logdet
 
 
 def _safe_quadratic_root(a: Array, b: Array, c: Array) -> Array:
     """Implement a numerically stable version of the quadratic formula."""
     # This is not a general solution to the quadratic equation, as it assumes
     # b ** 2 - 4. * a * c is known a priori to be positive (and which of the two
     # roots is to be used, see https://arxiv.org/abs/1906.04032).
     # There are two sources of instability:
     # (a) When b ** 2 - 4. * a * c -> 0, sqrt gives NaNs in gradient.
     # We clip sqrt_diff to have the smallest float number.
-    sqrt_diff = b ** 2 - 4. * a * c
+    sqrt_diff = b**2 - 4.0 * a * c
     safe_sqrt = jnp.sqrt(jnp.clip(sqrt_diff, jnp.finfo(sqrt_diff.dtype).tiny))
     # If sqrt_diff is non-positive, we set sqrt to 0. as it should be positive.
-    safe_sqrt = jnp.where(sqrt_diff > 0., safe_sqrt, 0.)
+    safe_sqrt = jnp.where(sqrt_diff > 0.0, safe_sqrt, 0.0)
     # (b) When 4. * a * c -> 0. We use the more stable quadratic solution
     # depending on the sign of b.
     # See https://people.csail.mit.edu/bkph/articles/Quadratics.pdf (eq 7 and 8).
     # Solution when b >= 0
-    numerator_1 = 2. * c
+    numerator_1 = 2.0 * c
     denominator_1 = -b - safe_sqrt
     # Solution when b < 0
-    numerator_2 = - b + safe_sqrt
+    numerator_2 = -b + safe_sqrt
     denominator_2 = 2 * a
     # Choose the numerically stable solution.
     numerator = jnp.where(b >= 0, numerator_1, numerator_2)
     denominator = jnp.where(b >= 0, denominator_1, denominator_2)
     return numerator / denominator
 
 
 @partial(jax.vmap, in_axes=(0, 0, 0, 0))
-def _rational_quadratic_spline_inv(y: Array,
-                                   x_pos: Array,
-                                   y_pos: Array,
-                                   knot_slopes: Array) -> Tuple[Array, Array]:
+def _rational_quadratic_spline_inv(
+    y: Array, x_pos: Array, y_pos: Array, knot_slopes: Array
+) -> tuple[Array, Array]:
     """Applies the inverse of a rational-quadratic spline to a scalar.
 
     Args:
     y: a scalar (0-dimensional array). The scalar `y` can be any real number; it
         will be transformed by the spline if it's in the closed interval
         `[y_pos[0], y_pos[-1]]`, and it will be transformed linearly if it's
         outside that interval.
@@ -157,16 +165,17 @@
     # Search to find the right bin. NOTE: The bins are sorted, so we could use
     # binary search, but this is more GPU/TPU friendly.
     # The following implementation avoids indexing for faster TPU computation.
     below_range = y <= y_pos[0]
     above_range = y >= y_pos[-1]
     correct_bin = jnp.logical_and(y >= y_pos[:-1], y < y_pos[1:])
     any_bin_in_range = jnp.any(correct_bin)
-    first_bin = jnp.concatenate([jnp.array([1]),
-                                jnp.zeros(len(correct_bin)-1)]).astype(bool)
+    first_bin = jnp.concatenate(
+        [jnp.array([1]), jnp.zeros(len(correct_bin) - 1)]
+    ).astype(bool)
     # If y does not fall into any bin, we use the first spline in the following
     # computations to avoid numerical issues.
     correct_bin = jnp.where(any_bin_in_range, correct_bin, first_bin)
     # Dot product of each parameter with the correct bin mask.
     params = jnp.stack([x_pos, y_pos, knot_slopes], axis=1)
     params_bin_left = jnp.sum(correct_bin[:, None] * params[:-1], axis=0)
     params_bin_right = jnp.sum(correct_bin[:, None] * params[1:], axis=0)
@@ -176,51 +185,58 @@
     y_pos_bin = (params_bin_left[1], params_bin_right[1])
     knot_slopes_bin = (params_bin_left[2], params_bin_right[2])
 
     bin_width = x_pos_bin[1] - x_pos_bin[0]
     bin_height = y_pos_bin[1] - y_pos_bin[0]
     bin_slope = bin_height / bin_width
     w = (y - y_pos_bin[0]) / bin_height
-    w = jnp.clip(w, 0., 1.)  # Ensure w is in [0, 1].
+    w = jnp.clip(w, 0.0, 1.0)  # Ensure w is in [0, 1].
     # Compute quadratic coefficients: az^2 + bz + c = 0
-    slopes_term = knot_slopes_bin[1] + knot_slopes_bin[0] - 2. * bin_slope
-    c = - bin_slope * w
+    slopes_term = knot_slopes_bin[1] + knot_slopes_bin[0] - 2.0 * bin_slope
+    c = -bin_slope * w
     b = knot_slopes_bin[0] - slopes_term * w
     a = bin_slope - b
 
     # Solve quadratic to obtain z and then x.
     z = _safe_quadratic_root(a, b, c)
-    z = jnp.clip(z, 0., 1.)  # Ensure z is in [0, 1].
+    z = jnp.clip(z, 0.0, 1.0)  # Ensure z is in [0, 1].
     x = bin_width * z + x_pos_bin[0]
 
     # Compute log det Jacobian.
     sq_z = z * z
     z1mz = z - sq_z  # z(1-z)
-    sq_1mz = (1. - z) ** 2
+    sq_1mz = (1.0 - z) ** 2
     denominator = bin_slope + slopes_term * z1mz
-    logdet = - 2. * jnp.log(bin_slope) - jnp.log(
-        knot_slopes_bin[1] * sq_z + 2. * bin_slope * z1mz +
-        knot_slopes_bin[0] * sq_1mz) + 2. * jnp.log(denominator)
+    logdet = (
+        -2.0 * jnp.log(bin_slope)
+        - jnp.log(
+            knot_slopes_bin[1] * sq_z
+            + 2.0 * bin_slope * z1mz
+            + knot_slopes_bin[0] * sq_1mz
+        )
+        + 2.0 * jnp.log(denominator)
+    )
 
     # If y is outside the spline range, we default to a linear transformation.
     x = jnp.where(below_range, (y - y_pos[0]) / knot_slopes[0] + x_pos[0], x)
-    x = jnp.where(above_range, (y - y_pos[-1]) / knot_slopes[-1] + x_pos[-1], x)
-    logdet = jnp.where(below_range, - jnp.log(knot_slopes[0]), logdet)
-    logdet = jnp.where(above_range, - jnp.log(knot_slopes[-1]), logdet)
+    x = jnp.where(
+        above_range, (y - y_pos[-1]) / knot_slopes[-1] + x_pos[-1], x  # type: ignore
+    )
+    logdet = jnp.where(below_range, -jnp.log(knot_slopes[0]), logdet)
+    logdet = jnp.where(above_range, -jnp.log(knot_slopes[-1]), logdet)
     return x, logdet
 
-class RQSpline(Bijection):
-
 
+class RQSpline(Bijection):
     _range_min: float
     _range_max: float
     _num_bins: int
     _min_bin_size: float
     _min_knot_slope: float
-    conditioner: eqx.Module
+    conditioner: MLP
 
     """A rational-quadratic spline bijection.
     
     This bijection is a piecewise rational-quadratic spline with `num_bins` bins.
     The spline is defined by the bin boundaries on the x and y axes, the slopes
     at the knot points, and the slopes at the boundaries of the spline range.
     The spline is linear outside the spline range.
@@ -250,181 +266,220 @@
     @property
     def num_bins(self):
         return jax.lax.stop_gradient(self._num_bins)
 
     @property
     def min_bin_size(self):
         return jax.lax.stop_gradient(self._min_bin_size)
-    
+
     @property
     def min_knot_slope(self):
         return jax.lax.stop_gradient(self._min_knot_slope)
 
     @property
     def dtype(self):
-        return self.conditioner.dtype 
-
-    def __init__(self,
-               conditioner: eqx.Module,
-               range_min: float,
-               range_max: float,
-               min_bin_size: float = 1e-4,
-               min_knot_slope: float = 1e-4):
+        return self.conditioner.dtype
 
+    def __init__(
+        self,
+        conditioner: MLP,
+        range_min: float,
+        range_max: float,
+        min_bin_size: float = 1e-4,
+        min_knot_slope: float = 1e-4,
+    ):
         self._range_min = range_min
         self._range_max = range_max
         self._min_bin_size = min_bin_size
         self._min_knot_slope = min_knot_slope
-        self._num_bins = int(conditioner.n_output/conditioner.n_input-1)//3
+        self._num_bins = int(conditioner.n_output / conditioner.n_input - 1) // 3
 
         self.conditioner = conditioner
 
-    def get_params(self, x: Array) -> Array:
-        params = self.conditioner(x).reshape(-1, self._num_bins*3+1)
-        unnormalized_bin_widths = params[:, :self._num_bins]
+    def get_params(
+        self, x: Float[Array, " n_condition"]
+    ) -> tuple[
+        Float[Array, " n_param"], Float[Array, " n_param"], Float[Array, " n_param"]
+    ]:
+        params = self.conditioner(x).reshape(-1, self._num_bins * 3 + 1)
+        unnormalized_bin_widths = params[:, : self._num_bins]
         unnormalized_bin_heights = params[:, self._num_bins : 2 * self._num_bins]
-        unnormalized_knot_slopes = params[:, 2 * self._num_bins:]
+        unnormalized_knot_slopes = params[:, 2 * self._num_bins :]
         # Normalize bin sizes and compute bin positions on the x and y axis.
         range_size = self.range_max - self.range_min
-        bin_widths = _normalize_bin_sizes(unnormalized_bin_widths, range_size,
-                                        self.min_bin_size)
-        bin_heights = _normalize_bin_sizes(unnormalized_bin_heights, range_size,
-                                        self.min_bin_size)
+        bin_widths = _normalize_bin_sizes(
+            unnormalized_bin_widths, range_size, self.min_bin_size
+        )
+        bin_heights = _normalize_bin_sizes(
+            unnormalized_bin_heights, range_size, self.min_bin_size
+        )
         x_pos = self.range_min + jnp.cumsum(bin_widths[..., :-1], axis=-1)
         y_pos = self.range_min + jnp.cumsum(bin_heights[..., :-1], axis=-1)
         pad_shape = params.shape[:-1] + (1,)
         pad_below = jnp.full(pad_shape, self.range_min, dtype=self.dtype)
         pad_above = jnp.full(pad_shape, self.range_max, dtype=self.dtype)
         x_pos = jnp.concatenate([pad_below, x_pos, pad_above], axis=-1)
         y_pos = jnp.concatenate([pad_below, y_pos, pad_above], axis=-1)
         # Normalize knot slopes and enforce requested boundary conditions.
-        knot_slopes = _normalize_knot_slopes(unnormalized_knot_slopes,
-                                            self.min_knot_slope)
+        knot_slopes = _normalize_knot_slopes(
+            unnormalized_knot_slopes, self.min_knot_slope
+        )
         return x_pos, y_pos, knot_slopes
 
-    def __call__(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
+    def __call__(self, x: Array, condition_x: Array) -> tuple[Array, Array]:
         return self.forward(x, condition_x)
 
-    def forward(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
+    def forward(self, x: Array, condition_x: Array) -> tuple[Array, Array]:
         x_pos, y_pos, knot_slopes = self.get_params(condition_x)
         return _rational_quadratic_spline_fwd(x, x_pos, y_pos, knot_slopes)
 
-    def inverse(self, x: Array, condition_x: Array) -> Tuple[Array, Array]:
+    def inverse(self, x: Array, condition_x: Array) -> tuple[Array, Array]:
         x_pos, y_pos, knot_slopes = self.get_params(condition_x)
         return _rational_quadratic_spline_inv(x, x_pos, y_pos, knot_slopes)
 
 
 class MaskedCouplingRQSpline(NFModel):
-    r""" Rational quadratic spline normalizing flow model using distrax.
+    r"""Rational quadratic spline normalizing flow model using distrax.
 
     Args:
         n_features (int):  Number of features in the data.
         num_layers (int): Number of layers in the conditioner.
         hidden_size (Sequence[int]): Hidden size of the conditioner.
         num_bins (int): Number of bins in the spline.
-        key (jax.random.PRNGKey): Random key for initialization.
+        key (PRNGKeyArray): Random key for initialization.
         spline_range (Sequence[float]): Range of the spline. Defaults to (-10.0, 10.0).
-    
+
     Properties:
         n_features (int) :  Number of features in the data.
         data_mean (Array) : Mean of the data.
         data_cov (Array) : Covariance of the data.
     """
 
     base_dist: Distribution
-    layers: list[eqx.Module]
+    layers: list[Bijection]
     _n_features: int
-    _data_mean: Array
-    _data_cov: Array
+    _data_mean: Float[Array, " n_dim"]
+    _data_cov: Float[Array, " n_dim n_dim"]
 
     @property
     def n_features(self):
         return self._n_features
 
     @property
     def data_mean(self):
         return jax.lax.stop_gradient(self._data_mean)
 
     @property
     def data_cov(self):
-        return jax.lax.stop_gradient(self._data_cov)
-
-    def __init__(self,
-                n_features: int,
-                n_layers: int,
-                hidden_size: Sequence[int],
-                num_bins: int,
-                key: jax.random.PRNGKey,
-                spline_range: Sequence[float] = (-10.0, 10.0), **kwargs):
+        return jax.lax.stop_gradient(jnp.atleast_2d(self._data_cov))
 
+    def __init__(
+        self,
+        n_features: int,
+        n_layers: int,
+        hidden_size: list[int],
+        num_bins: int,
+        key: PRNGKeyArray,
+        spline_range: tuple[float, float] = (-10.0, 10.0),
+        **kwargs
+    ):
         if kwargs.get("base_dist") is not None:
-            self.base_dist = kwargs.get("base_dist")
+            dist = kwargs.get("base_dist")
+            assert isinstance(dist, Distribution)
+            self.base_dist = dist
         else:
-            self.base_dist = Gaussian(jnp.zeros(n_features), jnp.eye(n_features), learnable=False)
+            self.base_dist = Gaussian(
+                jnp.zeros(n_features), jnp.eye(n_features), learnable=False
+            )
 
         if kwargs.get("data_mean") is not None:
-            self._data_mean = kwargs.get("data_mean")
+            data_mean = kwargs.get("data_mean")
+            assert isinstance(data_mean, Array)
+            self._data_mean = data_mean
         else:
             self._data_mean = jnp.zeros(n_features)
 
         if kwargs.get("data_cov") is not None:
-            self._data_cov = kwargs.get("data_cov")
+            data_cov = kwargs.get("data_cov")
+            assert isinstance(data_cov, Array)
+            self._data_cov = data_cov
         else:
             self._data_cov = jnp.eye(n_features)
 
         self._n_features = n_features
-        conditioner = []
-        for i in range(n_layers):
-            key, conditioner_key= jax.random.split(key)
-            conditioner.append(
-                MLP([n_features]+hidden_size+ [n_features*(num_bins*3+1)], conditioner_key, scale=1e-2, activation=jax.nn.tanh)
-            )
 
-        mask = (jnp.arange(0, n_features) % 2).astype(bool)
-        mask_all = (jnp.zeros(n_features)).astype(bool)
-        layers = []
-        for i in range(n_layers):
-            layers.append(
-                MaskedCouplingLayer(ScalarAffine(0.,0.), mask_all)
+        def make_layer(i: int, key: PRNGKeyArray):
+            mlp = MLP(
+                [n_features] + hidden_size + [n_features * (num_bins * 3 + 1)],
+                key,
+                scale=1e-2,
+                activation=jax.nn.tanh,
             )
-            layers.append(
-                MaskedCouplingLayer(RQSpline(conditioner[i], spline_range[0], spline_range[1]), mask)
+            mask = ((jnp.arange(0, n_features) + i) % 2).astype(bool)
+            mask_all = (jnp.zeros(n_features)).astype(bool)
+            layer1 = MaskedCouplingLayer(ScalarAffine(0.0, 0.0), mask_all)
+            layer2 = MaskedCouplingLayer(
+                RQSpline(mlp, spline_range[0], spline_range[1]), mask
             )
-            mask = jnp.logical_not(mask)
-        self.layers = layers
+            return eqx.nn.Sequential([layer1, layer2])  # type: ignore
 
-    def __call__(self, x: Array) -> Tuple[Array, Array]:
+        keys = jax.random.split(key, n_layers)
+        self.layers = eqx.filter_vmap(make_layer)(jnp.arange(n_layers), keys)
+
+    def __call__(
+        self, x: Float[Array, " n_dim"]
+    ) -> tuple[Float[Array, " n_dim"], Float]:
         return self.forward(x)
 
-    def forward(self, x: Array) -> Tuple[Array, Array]:
-        log_det = 0.
-        for layer in self.layers:
-            x, log_det_i = layer(x)
+    def forward(
+        self, x: Float[Array, " n_dim"]
+    ) -> tuple[Float[Array, " n_dim"], Float]:
+        log_det = 0.0
+        dynamics, statics = eqx.partition(self.layers, eqx.is_array)
+
+        def f(carry, data):
+            x, log_det = carry
+            layers = eqx.combine(data, statics)
+            x, log_det_i = layers[0](x)
             log_det += log_det_i
+            x, log_det_i = layers[1](x)
+            return (x, log_det + log_det_i), None
+
+        (x, log_det), _ = jax.lax.scan(f, (x, log_det), dynamics)
         return x, log_det
 
     @partial(jax.vmap, in_axes=(None, 0))
-    def inverse(self, x: Array) -> Tuple[Array, Array]:
-        """ From latent space to data space"""
-        log_det = 0.
-        for layer in reversed(self.layers):
-            x, log_det_i = layer.inverse(x)
+    def inverse(
+        self, x: Float[Array, " n_dim"]
+    ) -> tuple[Float[Array, " n_dim"], Float]:
+        """From latent space to data space"""
+        log_det = 0.0
+        dynamics, statics = eqx.partition(self.layers, eqx.is_array)
+
+        def f(carry, data):
+            x, log_det = carry
+            layers = eqx.combine(data, statics)
+            x, log_det_i = layers[0].inverse(x)
             log_det += log_det_i
+            x, log_det_i = layers[1].inverse(x)
+            return (x, log_det + log_det_i), None
+
+        (x, log_det), _ = jax.lax.scan(f, (x, log_det), dynamics, reverse=True)
         return x, log_det
 
     @eqx.filter_jit
-    def sample(self, rng_key: jax.random.PRNGKey, n_samples: int) -> Array:
+    def sample(
+        self, rng_key: PRNGKeyArray, n_samples: int
+    ) -> Float[Array, "n_samples n_dim"]:
         samples = self.base_dist.sample(rng_key, n_samples)
         samples = self.inverse(samples)[0]
         samples = samples * jnp.sqrt(jnp.diag(self.data_cov)) + self.data_mean
-        return samples 
+        return samples
 
     @eqx.filter_jit
     @partial(jax.vmap, in_axes=(None, 0))
-    def log_prob(self, x: Array) -> Array:
-        """ From data space to latent space"""
-        x = (x-self.data_mean)/jnp.sqrt(jnp.diag(self.data_cov))
+    def log_prob(self, x: Float[Array, "n_sample n_dim"]) -> Float[Array, " n_sample"]:
+        """From data space to latent space"""
+        x = (x - self.data_mean) / jnp.sqrt(jnp.diag(self.data_cov))
         y, log_det = self.__call__(x)
         log_det = log_det + self.base_dist.log_prob(y)
         return log_det
-
-
```

### Comparing `flowMC-0.2.4/src/flowMC/sampler/Gaussian_random_walk.py` & `flowMC-0.3.0/src/flowMC/proposal/Gaussian_random_walk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 from typing import Callable
 import jax
 import jax.numpy as jnp
 from tqdm import tqdm
-from flowMC.sampler.Proposal_Base import ProposalBase
+from flowMC.proposal.base import ProposalBase
 from jaxtyping import PyTree, Array, Float, Int, PRNGKeyArray
 
 
 class GaussianRandomWalk(ProposalBase):
     """
     Gaussian random walk sampler class builiding the rw_sampler method
 
     Args:
         logpdf: target logpdf function
         jit: whether to jit the sampler
         params: dictionary of parameters for the sampler
     """
 
+    step_size: Float
+
     def __init__(
         self,
-        logpdf: Callable,
+        logpdf: Callable[[Float[Array, "n_dim"], PyTree], Float],
         jit: bool,
-        params: dict,
-    ) -> Callable:
-        super().__init__(logpdf, jit, params)
-        self.params = params
+        step_size: Float,
+    ):
+        super().__init__(logpdf, jit, step_size=step_size)
+        self.step_size = step_size
         self.logpdf = logpdf
 
     def kernel(
         self,
         rng_key: PRNGKeyArray,
-        position: Float[Array, "ndim"],
+        position: Float[Array, "n_dim"],
         log_prob: Float[Array, "1"],
         data: PyTree,
-    ) -> tuple[Float[Array, "ndim"], Float[Array, "1"], Int[Array, "1"]]:
+    ) -> tuple[Float[Array, "n_dim"], Float[Array, "1"], Int[Array, "1"]]:
         """
         Random walk gaussian kernel.
         This is a kernel that only evolve a single chain.
 
         Args:
             rng_key (PRNGKeyArray): Jax PRNGKey
-            position (Float[Array, "ndim"]): current position of the chain
+            position (Float[Array, "n_dim"]): current position of the chain
             log_prob (Float[Array, "1"]): current log-probability of the chain
             data (PyTree): data to be passed to the logpdf function
 
         Returns:
-            position (Float[Array, "ndim"]): new position of the chain
+            position (Float[Array, "n_dim"]): new position of the chain
             log_prob (Float[Array, "1"]): new log-probability of the chain
             do_accept (Int[Array, "1"]): whether the new position is accepted
         """
 
         key1, key2 = jax.random.split(rng_key)
-        move_proposal = (
-            jax.random.normal(key1, shape=position.shape) * self.params["step_size"]
+        move_proposal: Float[Array, "n_dim"] = (
+            jax.random.normal(key1, shape=position.shape) * self.step_size
         )
+
         proposal = position + move_proposal
-        proposal_log_prob = self.logpdf(proposal, data)
+        proposal_log_prob: Float[Array, "n_dim"] = self.logpdf(proposal, data)
 
         log_uniform = jnp.log(jax.random.uniform(key2))
         do_accept = log_uniform < proposal_log_prob - log_prob
 
         position = jnp.where(do_accept, proposal, position)
         log_prob = jnp.where(do_accept, proposal_log_prob, log_prob)
         return position, log_prob, do_accept
 
-    def update(
-        self, i, state
-    ) -> tuple[
+    def update(self, i, state) -> tuple[
         PRNGKeyArray,
-        Float[Array, "nstep ndim"],
+        Float[Array, "nstep n_dim"],
         Float[Array, "nstep 1"],
         Int[Array, "n_step 1"],
         PyTree,
     ]:
         key, positions, log_p, acceptance, data = state
         _, key = jax.random.split(key)
         new_position, new_log_p, do_accept = self.kernel(
@@ -82,19 +83,20 @@
         acceptance = acceptance.at[i].set(do_accept)
         return (key, positions, log_p, acceptance, data)
 
     def sample(
         self,
         rng_key: PRNGKeyArray,
         n_steps: int,
-        initial_position: Float[Array, "n_chains ndim"],
+        initial_position: Float[Array, "n_chains n_dim"],
         data: PyTree,
         verbose: bool = False,
     ) -> tuple[
-        Float[Array, "n_chains n_steps ndim"],
+        PRNGKeyArray,
+        Float[Array, "n_chains n_steps n_dim"],
         Float[Array, "n_chains n_steps 1"],
         Int[Array, "n_chains n_steps 1"],
     ]:
         logp = self.logpdf_vmap(initial_position, data)
         n_chains = rng_key.shape[0]
         acceptance = jnp.zeros((n_chains, n_steps))
         all_positions = (
```

### Comparing `flowMC-0.2.4/src/flowMC/sampler/MALA.py` & `flowMC-0.3.0/src/flowMC/proposal/MALA.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,84 @@
 from typing import Callable
 import jax
 import jax.numpy as jnp
 from jax.scipy.stats import multivariate_normal
 from tqdm import tqdm
-from flowMC.sampler.Proposal_Base import ProposalBase
+from flowMC.proposal.base import ProposalBase
 from functools import partialmethod
-from jaxtyping import PyTree, Array, Float, Int, PRNGKeyArray
+from jaxtyping import PyTree, Array, Float, Int, PRNGKeyArray, Bool
 
 
 class MALA(ProposalBase):
     """
-    Metropolis-adjusted Langevin algorithm sampler class builiding the mala_sampler method
+    Metropolis-adjusted Langevin algorithm sampler clas
+    builiding the mala_sampler method
 
     Args:
         logpdf: target logpdf function
         jit: whether to jit the sampler
         params: dictionary of parameters for the sampler
     """
 
+    step_size: Float
+
     def __init__(
-        self, logpdf: Callable, jit: bool, params: dict, use_autotune=False
+        self,
+        logpdf: Callable[[Float[Array, " n_dim"], PyTree], Float],
+        jit: Bool,
+        step_size: Float,
+        use_autotune=False,
     ):
-        super().__init__(logpdf, jit, params)
-        self.params = params
-        self.logpdf = logpdf
-        self.use_autotune = use_autotune
+        super().__init__(logpdf, jit, step_size=step_size, use_autotune=use_autotune)
+        self.step_size = step_size
+        self.logpdf: Callable = logpdf
+        self.use_autotune: Bool = use_autotune
 
-    def body(self, carry, this_key):
+    def body(
+        self,
+        carry: tuple[Float[Array, " n_dim"], float, dict],
+        this_key: PRNGKeyArray,
+    ) -> tuple[
+        tuple[Float[Array, " n_dim"], float, dict],
+        tuple[Float[Array, " n_dim"], Float[Array, "1"], Float[Array, " n_dim"]],
+    ]:
         print("Compiling MALA body")
         this_position, dt, data = carry
         dt2 = dt * dt
         this_log_prob, this_d_log = jax.value_and_grad(self.logpdf)(this_position, data)
         proposal = this_position + jnp.dot(dt2, this_d_log) / 2
         proposal += jnp.dot(dt, jax.random.normal(this_key, shape=this_position.shape))
         return (proposal, dt, data), (proposal, this_log_prob, this_d_log)
 
     def kernel(
         self,
         rng_key: PRNGKeyArray,
-        position: Float[Array, "ndim"],
+        position: Float[Array, " n_dim"],
         log_prob: Float[Array, "1"],
         data: PyTree,
-    ) -> tuple[
-        Float[Array, "ndim"], Float[Array, "1"], Int[Array, "1"]
-    ]:
+    ) -> tuple[Float[Array, " n_dim"], Float[Array, "1"], Int[Array, "1"]]:
         """
         Metropolis-adjusted Langevin algorithm kernel.
         This is a kernel that only evolve a single chain.
 
         Args:
             rng_key (PRNGKeyArray): Jax PRNGKey
-            position (Float[Array, "ndim"]): current position of the chain
+            position (Float[Array, " n_dim"]): current position of the chain
             log_prob (Float[Array, "1"]): current log-probability of the chain
             data (PyTree): data to be passed to the logpdf function
 
         Returns:
-            position (Float[Array, "ndim"]): new position of the chain
+            position (Float[Array, " n_dim"]): new position of the chain
             log_prob (Float[Array, "1"]): new log-probability of the chain
             do_accept (Int[Array, "1"]): whether the new position is accepted
         """
 
         key1, key2 = jax.random.split(rng_key)
 
-        dt = self.params["step_size"]
+        dt: Float = self.step_size
         dt2 = dt * dt
 
         _, (proposal, logprob, d_logprob) = jax.lax.scan(
             self.body, (position, dt, data), jnp.array([key1, key1])
         )
 
         ratio = logprob[1] - logprob[0]
@@ -74,26 +86,26 @@
             proposal[0], position + jnp.dot(dt2, d_logprob[0]) / 2, dt2
         )
         ratio += multivariate_normal.logpdf(
             position, proposal[0] + jnp.dot(dt2, d_logprob[1]) / 2, dt2
         )
 
         log_uniform = jnp.log(jax.random.uniform(key2))
-        do_accept = log_uniform < ratio
+        do_accept: Bool[Array, " n_dim"] = log_uniform < ratio
 
         position = jnp.where(do_accept, proposal[0], position)
         log_prob = jnp.where(do_accept, logprob[1], logprob[0])
 
         return position, log_prob, do_accept
 
     def update(
         self, i, state
     ) -> tuple[
         PRNGKeyArray,
-        Float[Array, "nstep ndim"],
+        Float[Array, "nstep  n_dim"],
         Float[Array, "nstep 1"],
         Int[Array, "n_step 1"],
         PyTree,
     ]:
         """
         Update function for the MALA sampler
 
@@ -110,22 +122,24 @@
             key, positions[i - 1], log_p[i - 1], data
         )
         positions = positions.at[i].set(new_position)
         log_p = log_p.at[i].set(new_log_p)
         acceptance = acceptance.at[i].set(do_accept)
         return (key, positions, log_p, acceptance, data)
 
-    def sample(self,
+    def sample(
+        self,
         rng_key: PRNGKeyArray,
         n_steps: int,
-        initial_position: Float[Array, "n_chains ndim"],
+        initial_position: Float[Array, "n_chains  n_dim"],
         data: PyTree,
         verbose: bool = False,
     ) -> tuple[
-        Float[Array, "n_chains n_steps ndim"],
+        PRNGKeyArray,
+        Float[Array, "n_chains n_steps  n_dim"],
         Float[Array, "n_chains n_steps 1"],
         Int[Array, "n_chains n_steps 1"],
     ]:
         logp = self.logpdf_vmap(initial_position, data)
         n_chains = rng_key.shape[0]
         acceptance = jnp.zeros((n_chains, n_steps))
         all_positions = (
@@ -141,47 +155,47 @@
             )
         else:
             iterator_loop = range(1, n_steps)
         for i in iterator_loop:
             state = self.update_vmap(i, state)
         return state[:-1]
 
-
     def mala_sampler_autotune(
         self, rng_key, initial_position, log_prob, data, params, max_iter=30
     ):
         """
         Tune the step size of the MALA kernel using the acceptance rate.
 
         Args:
             mala_kernel_vmap (Callable): A MALA kernel
             rng_key: Jax PRNGKey
-            initial_position (n_chains, n_dim): initial position of the chains
+            initial_position (n_chains,  n_dim): initial position of the chains
             log_prob (n_chains, ): log-probability of the initial position
             params (dict): parameters of the MALA kernel
             max_iter (int): maximal number of iterations to tune the step size
         """
 
-        tqdm.__init__ = partialmethod(tqdm.__init__, disable=True)
+        tqdm.__init__ = partialmethod(tqdm.__init__, disable=True)  # type: ignore
 
         counter = 0
         position, log_prob, do_accept = self.kernel_vmap(
             rng_key, initial_position, log_prob, data
         )
         acceptance_rate = jnp.mean(do_accept)
         while (acceptance_rate <= 0.3) or (acceptance_rate >= 0.5):
             if counter > max_iter:
                 print(
-                    "Maximal number of iterations reached. Existing tuning with current parameters."
+                    "Maximal number of iterations reached.\
+                    Existing tuning with current parameters."
                 )
                 break
             if acceptance_rate <= 0.3:
-                params["step_size"] *= 0.8
+                self.step_size *= 0.8
             elif acceptance_rate >= 0.5:
-                params["step_size"] *= 1.25
+                self.step_size *= 1.25
             counter += 1
             position, log_prob, do_accept = self.kernel_vmap(
                 rng_key, initial_position, log_prob, data
             )
             acceptance_rate = jnp.mean(do_accept)
-        tqdm.__init__ = partialmethod(tqdm.__init__, disable=False)
+        tqdm.__init__ = partialmethod(tqdm.__init__, disable=False)  # type: ignore
         return params
```

### Comparing `flowMC-0.2.4/src/flowMC/sampler/NF_proposal.py` & `flowMC-0.3.0/src/flowMC/proposal/NF_proposal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,78 @@
-from typing import Tuple
 import jax
 import jax.numpy as jnp
 from jax import random
 from tqdm import tqdm
 from flowMC.nfmodel.base import NFModel
-from jaxtyping import Array, PRNGKeyArray, PyTree
 from typing import Callable
-from flowMC.sampler.Proposal_Base import ProposalBase
-from jaxtyping import Array, Float, Int, PRNGKeyArray
-import equinox as eqx
+from flowMC.proposal.base import ProposalBase
+from jaxtyping import Array, Float, Int, PRNGKeyArray, PyTree
 from math import ceil
 
 
 @jax.tree_util.register_pytree_node_class
 class NFProposal(ProposalBase):
-
     model: NFModel
 
     def __init__(
-        self, logpdf: Callable, jit: bool, model: NFModel, n_sample_max: int = 10000
+        self, logpdf: Callable, jit: bool, model: NFModel, n_flow_sample: int = 10000
     ):
-        super().__init__(logpdf, jit, {})
+        super().__init__(logpdf, jit)
         self.model = model
-        self.n_sample_max = n_sample_max
+        self.n_flow_sample = n_flow_sample
         self.update_vmap = jax.vmap(self.update, in_axes=(None, (0)))
-        if self.jit == True:
+        if self.jit is True:
             self.update_vmap = jax.jit(self.update_vmap)
 
     def kernel(
         self,
         rng_key: PRNGKeyArray,
-        initial_position: Float[Array, "ndim"],
-        proposal_position: Float[Array, "ndim"],
+        initial_position: Float[Array, " n_dim"],
+        proposal_position: Float[Array, " n_dim"],
         log_prob_initial: Float[Array, "1"],
         log_prob_proposal: Float[Array, "1"],
         log_prob_nf_initial: Float[Array, "1"],
         log_prob_nf_proposal: Float[Array, "1"],
-    ) -> tuple[Float[Array, "ndim"], Float[Array, "1"], Int[Array, "1"]]:
+    ) -> tuple[
+        Float[Array, " n_dim"], Float[Array, "1"], Float[Array, "1"], Int[Array, "1"]
+    ]:
         rng_key, subkey = random.split(rng_key)
 
         ratio = (log_prob_proposal - log_prob_initial) - (
             log_prob_nf_proposal - log_prob_nf_initial
         )
         uniform_random = jnp.log(jax.random.uniform(subkey))
         do_accept = uniform_random < ratio
         position = jnp.where(do_accept, proposal_position, initial_position)
         log_prob = jnp.where(do_accept, log_prob_proposal, log_prob_initial)
         log_prob_nf = jnp.where(do_accept, log_prob_nf_proposal, log_prob_nf_initial)
         return position, log_prob, log_prob_nf, do_accept
 
     def update(
-        self, i, state
+        self,
+        i: int,
+        state: tuple[
+            PRNGKeyArray,
+            Float[Array, "nstep  n_dim"],
+            Float[Array, "nstep  n_dim"],
+            Float[Array, "nstep 1"],
+            Float[Array, "nstep 1"],
+            Float[Array, "nstep 1"],
+            Float[Array, "nstep 1"],
+            Int[Array, "nstep 1"],
+        ],
     ) -> tuple[
         PRNGKeyArray,
-        Float[Array, "nstep ndim"],
+        Float[Array, "nstep  n_dim"],
+        Float[Array, "nstep  n_dim"],
+        Float[Array, "nstep 1"],
+        Float[Array, "nstep 1"],
+        Float[Array, "nstep 1"],
         Float[Array, "nstep 1"],
         Int[Array, "n_step 1"],
-        PyTree,
     ]:
         (
             key,
             positions,
             proposal,
             log_prob,
             log_prob_proposal,
@@ -93,20 +105,20 @@
             acceptance,
         )
 
     def sample(
         self,
         rng_key: PRNGKeyArray,
         n_steps: int,
-        initial_position: Float[Array, "n_chains ndim"],
+        initial_position: Float[Array, "n_chains  n_dim"],
         data: PyTree,
         verbose: bool = False,
-        mode: str = "training",
     ) -> tuple[
-        Float[Array, "n_chains n_steps ndim"],
+        PRNGKeyArray,
+        Float[Array, "n_chains n_steps  n_dim"],
         Float[Array, "n_chains n_steps 1"],
         Int[Array, "n_chains n_steps 1"],
     ]:
         rng_key, *subkeys = random.split(rng_key, 3)
 
         n_chains = initial_position.shape[0]
         n_dim = initial_position.shape[-1]
@@ -155,24 +167,24 @@
         for i in iterator_loop:
             state = self.update_vmap(i, state)
         return (rng_key, state[1], state[3], state[7])
 
     def sample_flow(
         self,
         rng_key: PRNGKeyArray,
-        initial_position: Float[Array, "n_chains ndim"],
+        initial_position: Float[Array, "n_chains  n_dim"],
         data,
         n_steps: int,
     ):
         n_chains = initial_position.shape[0]
         n_dim = initial_position.shape[-1]
         total_size = initial_position.shape[0] * n_steps
-        if total_size > self.n_sample_max:
+        if total_size > self.n_flow_sample:
             rng_key = rng_key
-            n_batch = ceil(total_size / self.n_sample_max)
+            n_batch = ceil(total_size / self.n_flow_sample)
             n_sample = total_size // n_batch
             proposal_position = jnp.zeros(
                 (n_batch, n_sample, initial_position.shape[-1])
             )
             log_prob_proposal = jnp.zeros((n_batch, n_sample))
             log_prob_nf_proposal = jnp.zeros((n_batch, n_sample))
             for i in range(n_batch):
@@ -201,9 +213,9 @@
         log_prob_nf_proposal = log_prob_nf_proposal.reshape(n_chains, n_steps)
 
         return proposal_position, log_prob_proposal, log_prob_nf_proposal
 
     def tree_flatten(self):
         children, aux_data = super().tree_flatten()
         aux_data["model"] = self.model
-        aux_data["n_sample_max"] = self.n_sample_max
+        aux_data["n_sample_max"] = self.n_flow_sample
         return (children, aux_data)
```

### Comparing `flowMC-0.2.4/src/flowMC/sampler/flowHMC.py` & `flowMC-0.3.0/src/flowMC/proposal/flowHMC.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 import jax
 import jax.numpy as jnp
 from flowMC.nfmodel.base import NFModel
 from jaxtyping import Array, PRNGKeyArray, PyTree
 from typing import Callable
-from flowMC.sampler.HMC import HMC
-from flowMC.sampler.NF_proposal import NFProposal
+from flowMC.proposal.HMC import HMC
+from flowMC.proposal.NF_proposal import NFProposal
 from jaxtyping import Array, Float, Int, PRNGKeyArray
 from math import ceil
 from jax import random
 from tqdm import tqdm
 
+###################################
+# This is not in production yet
+###################################
+
 
 # Note that the inverse metric needs float64 precision
 jax.config.update("jax_enable_x64", True)
 
 
 @jax.tree_util.register_pytree_node_class
 class flowHMC(HMC, NFProposal):
     model: NFModel
 
+    condition_matrix: Float[Array, "n_dim n_dim"]
+
     def __init__(
         self,
         logpdf: Callable,
         jit: bool,
         model: NFModel,
         n_sample_max: int = 10000,
-        params: dict = {},
+        condition_matrix: Float[Array, "n_dim n_dim"] | Float = 1,
     ):
-        super().__init__(logpdf, jit, params)
+        super().__init__(logpdf, jit, condition_matrix=condition_matrix, model=model, n_sample_max=n_sample_max)
         self.kinetic = lambda p, M: 0.5 * (p @ M @ p)
         self.grad_kinetic = jax.grad(self.kinetic)
         self.model = model
         self.n_sample_max = n_sample_max
-        self.production_covariance = params['condition_matrix'] #None if params['condition_matrix'] is None else params['condition_matrix']
+        self.production_covariance = condition_matrix
         self.update_vmap = jax.vmap(self.update, in_axes=(None, (0, 0, 0, 0, 0, 0, None)), out_axes=(0, 0, 0, 0, 0, 0, None))
         if self.jit is True:
             self.update_vmap = jax.jit(self.update_vmap)
 
     def covariance_estimate(
         self, points: Float[Array, "n_point n_dim"], k: int = 100
     ) -> Float[Array, "n_point n_dim n_dim"]:
```

### Comparing `flowMC-0.2.4/src/flowMC/utils/EvolutionaryOptimizer.py` & `flowMC-0.3.0/src/flowMC/utils/EvolutionaryOptimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from evosax import CMA_ES
 import jax
 import jax.numpy as jnp
+from jaxtyping import PRNGKeyArray
 import tqdm
 
-class EvolutionaryOptimizer:
 
+class EvolutionaryOptimizer:
     """
     A wrapper class for the evosax package.
     Note that we do not aim to solve any generic optimization problem,
     especially in a high dimension space.
 
 
     Parameters
@@ -40,15 +41,15 @@
     def __init__(self, ndims, popsize=100, verbose=False):
         self.strategy = CMA_ES(num_dims=ndims, popsize=popsize, elite_ratio=0.5)
         self.es_params = self.strategy.default_params.replace(clip_min=0, clip_max=1)
         self.verbose = verbose
         self.history = []
         self.state = None
 
-    def optimize(self, objective, bound, n_loops = 100, seed = 9527, keep_history_step = 0):
+    def optimize(self, objective, bound, n_loops=100, seed=9527, keep_history_step=0):
         """
         Optimize the objective function.
 
         Parameters
         ----------
         objective : Callable
             The objective function, which should be implemented in JAX.
@@ -61,45 +62,65 @@
 
         Returns
         -------
         None
         """
         rng = jax.random.PRNGKey(seed)
         key, subkey = jax.random.split(rng)
-        progress_bar = tqdm.tqdm(range(n_loops), "Generation: ") if self.verbose else range(n_loops)
+        progress_bar = (
+            tqdm.tqdm(range(n_loops), "Generation: ")
+            if self.verbose
+            else range(n_loops)
+        )
         self.bound = bound
         self.state = self.strategy.initialize(key, self.es_params)
         if keep_history_step > 0:
             self.history = []
             for i in progress_bar:
-                key, self.state, theta = self.optimize_step(subkey, self.state, objective, bound)
-                if i%keep_history_step == 0: self.history.append(theta)
-                if self.verbose: progress_bar.set_description(f"Generation: {i}, Fitness: {self.state.best_fitness:.4f}")
+                subkey, self.state, theta = self.optimize_step(
+                    subkey, self.state, objective, bound
+                )
+                if i % keep_history_step == 0:
+                    self.history.append(theta)
+                if self.verbose:
+                    progress_bar.set_description(
+                        f"Generation: {i}, Fitness: {self.state.best_fitness:.4f}"
+                    )
             self.history = jnp.array(self.history)
         else:
             for i in progress_bar:
-                key, self.state, _ = self.optimize_step(subkey, self.state, objective, bound)
-                if self.verbose: progress_bar.set_description(f"Generation: {i}, Fitness: {self.state.best_fitness:.4f}")
+                subkey, self.state, _ = self.optimize_step(
+                    subkey, self.state, objective, bound
+                )
+                if self.verbose:
+                    progress_bar.set_description(
+                        f"Generation: {i}, Fitness: {self.state.best_fitness:.4f}"
+                    )
 
-    def optimize_step(self, key: jax.random.PRNGKey, state, objective: callable, bound):
+    def optimize_step(self, key: PRNGKeyArray, state, objective: callable, bound):
         key, subkey = jax.random.split(key)
         x, state = self.strategy.ask(subkey, state, self.es_params)
         theta = x * (bound[:, 1] - bound[:, 0]) + bound[:, 0]
         fitness = objective(theta)
-        state = self.strategy.tell(x, fitness.astype(jnp.float32), state, self.es_params)
+        state = self.strategy.tell(
+            x, fitness.astype(jnp.float32), state, self.es_params
+        )
         return key, state, theta
 
     def get_result(self):
         """
         Get the best member and the best fitness.
 
         Returns
         -------
         best_member : (ndims,) ndarray
             The best member.
         best_fitness : float
             The best fitness.
         """
 
-        best_member = self.state.best_member* (self.bound[:, 1] - self.bound[:, 0]) + self.bound[:, 0]
+        best_member = (
+            self.state.best_member * (self.bound[:, 1] - self.bound[:, 0])
+            + self.bound[:, 0]
+        )
         best_fitness = self.state.best_fitness
-        return best_member, best_fitness
+        return best_member, best_fitness
```

### Comparing `flowMC-0.2.4/src/flowMC/utils/PythonFunctionWrap.py` & `flowMC-0.3.0/src/flowMC/utils/PythonFunctionWrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,41 +14,46 @@
 from jax._src import dtypes
 from jax._src.util import safe_zip
 from jax.custom_batching import custom_vmap
 from jax.experimental import host_callback
 from jax.tree_util import tree_flatten, tree_unflatten
 from jaxtyping import PyTree
 
+
 def wrap_python_log_prob_fn(python_log_prob_fn: Callable[..., Array]):
     @custom_vmap
     @wraps(python_log_prob_fn)
     def log_prob_fn(params: Array, data: PyTree) -> Array:
         dtype = _tree_dtype(params)
         inputs = {"params": params, "data": data}
         return host_callback.call(
             python_log_prob_fn,
             inputs,
             result_shape=jax.ShapeDtypeStruct((), dtype),
         )
 
     @log_prob_fn.def_vmap
-    def _(axis_size: int, in_batched: List[bool], params: Array, data: PyTree) -> Tuple[Array, bool]:
+    def _(
+        axis_size: int, in_batched: List[bool], params: Array, data: PyTree
+    ) -> Tuple[Array, bool]:
         del axis_size, in_batched
 
         if _arraylike(params):
             flat_params = params
             eval_one = python_log_prob_fn
         else:
             flat_params, unravel = ravel_ensemble(params)
-            eval_one = lambda x: python_log_prob_fn(unravel(x))
+
+            def eval_one(x):
+                return python_log_prob_fn(unravel(x))
 
         result_shape = jax.ShapeDtypeStruct((flat_params.shape[0],), flat_params.dtype)
 
         result = host_callback.call(
-            lambda y: np.stack([eval_one({"params":x,"data":data}) for x in y]),
+            lambda y: np.stack([eval_one({"params": x, "data": data}) for x in y]),
             flat_params,
             result_shape=result_shape,
         )
         return (
             result,
             True,
         )
@@ -75,15 +80,18 @@
 
 zip = safe_zip
 
 
 def ravel_ensemble(coords: PyTree) -> Tuple[Array, UnravelFn]:
     leaves, treedef = tree_flatten(coords)
     flat, unravel_inner = _ravel_inner(leaves)
-    unravel_one = lambda flat: tree_unflatten(treedef, unravel_inner(flat))
+
+    def unravel_one(flat):
+        return tree_unflatten(treedef, unravel_inner(flat))
+
     return flat, unravel_one
 
 
 def _ravel_inner(lst: List[Array]) -> Tuple[Array, UnravelFn]:
     if not lst:
         return jnp.array([], jnp.float32), lambda _: []
     from_dtypes = [dtypes.dtype(l) for l in lst]
@@ -94,15 +102,17 @@
     if all(dt == to_dtype for dt in from_dtypes):
         del from_dtypes, to_dtype
 
         def unravel(arr: Array) -> PyTree:
             chunks = jnp.split(arr, indices[:-1])
             return [chunk.reshape(shape) for chunk, shape in zip(chunks, shapes)]
 
-        ravel = lambda arg: jnp.concatenate([jnp.ravel(e) for e in arg])
+        def ravel(arg):
+            return jnp.concatenate([jnp.ravel(e) for e in arg])
+
         raveled = jax.vmap(ravel)(lst)
         return raveled, unravel
 
     else:
 
         def unravel(arr: Array) -> PyTree:
             arr_dtype = dtypes.dtype(arr)
@@ -115,12 +125,14 @@
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 return [
                     lax.convert_element_type(chunk.reshape(shape), dtype)
                     for chunk, shape, dtype in zip(chunks, shapes, from_dtypes)
                 ]
 
-        ravel = lambda arg: jnp.concatenate(
-            [jnp.ravel(lax.convert_element_type(e, to_dtype)) for e in arg]
-        )
+        def ravel(arg):
+            return jnp.concatenate(
+                [jnp.ravel(lax.convert_element_type(e, to_dtype)) for e in arg]
+            )
+
         raveled = jax.vmap(ravel)(lst)
         return raveled, unravel
```

### Comparing `flowMC-0.2.4/src/flowMC.egg-info/PKG-INFO` & `flowMC-0.3.0/src/flowMC.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.2.4
+Version: 0.3.0
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax>=0.4.12
 Requires-Dist: jaxlib>=0.4.12
 Requires-Dist: equinox>=0.10.6
 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4
 Requires-Dist: tqdm
+Requires-Dist: corner
 
 # flowMC
 
 **Normalizing-flow enhanced sampling package for probabilistic inference**
 
 <a href="https://flowmc.readthedocs.io/en/main/">
 <img src="https://badgen.net/badge/Read/the doc/blue" alt="doc"/>
@@ -80,14 +81,49 @@
     * corner
     * arviz
 
 The test suite is based on pytest. To run the tests, one needs to install `pytest` and run `pytest` at the root directory of this repo.
 
 # Attribution
 
-A Jax implementation of methods described in: 
+If you used `flowMC` in your research, we would really appericiate it if you could at least cite the following papers:
+
+```
+@article{Wong:2022xvh,
+    author = "Wong, Kaze W. k. and Gabri\'e, Marylou and Foreman-Mackey, Daniel",
+    title = "{flowMC: Normalizing flow enhanced sampling package for probabilistic inference in JAX}",
+    eprint = "2211.06397",
+    archivePrefix = "arXiv",
+    primaryClass = "astro-ph.IM",
+    doi = "10.21105/joss.05021",
+    journal = "J. Open Source Softw.",
+    volume = "8",
+    number = "83",
+    pages = "5021",
+    year = "2023"
+}
+
+@article{Gabrie:2021tlu,
+    author = "Gabri\'e, Marylou and Rotskoff, Grant M. and Vanden-Eijnden, Eric",
+    title = "{Adaptive Monte Carlo augmented with normalizing flows}",
+    eprint = "2105.12603",
+    archivePrefix = "arXiv",
+    primaryClass = "physics.data-an",
+    doi = "10.1073/pnas.2109420119",
+    journal = "Proc. Nat. Acad. Sci.",
+    volume = "119",
+    number = "10",
+    pages = "e2109420119",
+    year = "2022"
+}
+```
+
+This will help `flowMC` getting more recognition, and the main benefit *for you* is this means the `flowMC` community will grow and it will be continuously improved. If you believe in the magic of open-source software, please support us by attributing our software in your work.
+
+
+`flowMC` is a Jax implementation of methods described in: 
 > *Efficient Bayesian Sampling Using Normalizing Flows to Assist Markov Chain Monte Carlo Methods* Gabrié M., Rotskoff G. M., Vanden-Eijnden E. - ICML INNF+ workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx)
 
 > *Adaptive Monte Carlo augmented with normalizing flows.*
 Gabrié M., Rotskoff G. M., Vanden-Eijnden E. - PNAS 2022 - [doi](https://www.pnas.org/doi/10.1073/pnas.2109420119), [arxiv](https://arxiv.org/abs/2105.12603)
```

#### html2text {}

```diff
@@ -1,38 +1,54 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.2.4 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.0 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
-learning,normalizing,autodiff,jax Requires-Python: >=3.9 Description-Content-
+learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
-Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm # flowMC **Normalizing-flow
-enhanced sampling package for probabilistic inference** _[_d_o_c_]_[_d_o_c_]!
-[flowMC_logo](./docs/logo_0810.png) flowMC is a Jax-based python package for
-normalizing-flow enhanced Markov chain Monte Carlo (MCMC) sampling. The code is
-open source under MIT license, and it is under active development. - Just-in-
-time compilation is supported. - Native support for GPU acceleration. - Suit
-for problems with multi-modality. - Minimal tuning. # Installation The simplest
-way to install the package is to do it through pip ``` pip install flowMC ```
-This will install the latest stable release and its dependencies. flowMC is
-based on [Jax](https://github.com/google/jax) and [Equinox](https://github.com/
-patrick-kidger/equinox). By default, installing flowMC will automatically
-install Jax and Equinox available on [PyPI](https://pypi.org). Jax does not
-install GPU support by default. If you want to use GPU with Jax, you need to
-install Jax with GPU support according to their document. At the time of
-writing this documentation page, this is the command to install Jax with GPU
-support: ``` pip install --upgrade "jax[cuda12_pip]" -f https://
+Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
+**Normalizing-flow enhanced sampling package for probabilistic inference**
+_[_d_o_c_]_[_d_o_c_]![flowMC_logo](./docs/logo_0810.png) flowMC is a Jax-based python
+package for normalizing-flow enhanced Markov chain Monte Carlo (MCMC) sampling.
+The code is open source under MIT license, and it is under active development.
+- Just-in-time compilation is supported. - Native support for GPU acceleration.
+- Suit for problems with multi-modality. - Minimal tuning. # Installation The
+simplest way to install the package is to do it through pip ``` pip install
+flowMC ``` This will install the latest stable release and its dependencies.
+flowMC is based on [Jax](https://github.com/google/jax) and [Equinox](https://
+github.com/patrick-kidger/equinox). By default, installing flowMC will
+automatically install Jax and Equinox available on [PyPI](https://pypi.org).
+Jax does not install GPU support by default. If you want to use GPU with Jax,
+you need to install Jax with GPU support according to their document. At the
+time of writing this documentation page, this is the command to install Jax
+with GPU support: ``` pip install --upgrade "jax[cuda12_pip]" -f https://
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` If you want to
 install the latest version of flowMC, you can clone this repo and install it
 locally: ``` git clone https://github.com/kazewong/flowMC.git cd flowMC pip
 install -e . ``` ## Requirements Here is a list of packages we use in the main
 library * Python 3.9+ * Jax * Jaxlib * equinox To visualize the inference
 results in the examples, we requrie the following packages in addtion to the
 above: * matplotlib * corner * arviz The test suite is based on pytest. To run
 the tests, one needs to install `pytest` and run `pytest` at the root directory
-of this repo. # Attribution A Jax implementation of methods described in: >
-*Efficient Bayesian Sampling Using Normalizing Flows to Assist Markov Chain
-Monte Carlo Methods* GabriÃ© M., Rotskoff G. M., Vanden-Eijnden E. - ICML INNF+
-workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx) > *Adaptive
-Monte Carlo augmented with normalizing flows.* GabriÃ© M., Rotskoff G. M.,
-Vanden-Eijnden E. - PNAS 2022 - [doi](https://www.pnas.org/doi/10.1073/
+of this repo. # Attribution If you used `flowMC` in your research, we would
+really appericiate it if you could at least cite the following papers: ```
+@article{Wong:2022xvh, author = "Wong, Kaze W. k. and Gabri\'e, Marylou and
+Foreman-Mackey, Daniel", title = "{flowMC: Normalizing flow enhanced sampling
+package for probabilistic inference in JAX}", eprint = "2211.06397",
+archivePrefix = "arXiv", primaryClass = "astro-ph.IM", doi = "10.21105/
+joss.05021", journal = "J. Open Source Softw.", volume = "8", number = "83",
+pages = "5021", year = "2023" } @article{Gabrie:2021tlu, author = "Gabri\'e,
+Marylou and Rotskoff, Grant M. and Vanden-Eijnden, Eric", title = "{Adaptive
+Monte Carlo augmented with normalizing flows}", eprint = "2105.12603",
+archivePrefix = "arXiv", primaryClass = "physics.data-an", doi = "10.1073/
+pnas.2109420119", journal = "Proc. Nat. Acad. Sci.", volume = "119", number =
+"10", pages = "e2109420119", year = "2022" } ``` This will help `flowMC`
+getting more recognition, and the main benefit *for you* is this means the
+`flowMC` community will grow and it will be continuously improved. If you
+believe in the magic of open-source software, please support us by attributing
+our software in your work. `flowMC` is a Jax implementation of methods
+described in: > *Efficient Bayesian Sampling Using Normalizing Flows to Assist
+Markov Chain Monte Carlo Methods* GabriÃ© M., Rotskoff G. M., Vanden-Eijnden E.
+- ICML INNF+ workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx) >
+*Adaptive Monte Carlo augmented with normalizing flows.* GabriÃ© M., Rotskoff
+G. M., Vanden-Eijnden E. - PNAS 2022 - [doi](https://www.pnas.org/doi/10.1073/
 pnas.2109420119), [arxiv](https://arxiv.org/abs/2105.12603)
```

### Comparing `flowMC-0.2.4/src/flowMC.egg-info/SOURCES.txt` & `flowMC-0.3.0/src/flowMC.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
+src/flowMC/Sampler.py
 src/flowMC/__init__.py
 src/flowMC.egg-info/PKG-INFO
 src/flowMC.egg-info/SOURCES.txt
 src/flowMC.egg-info/dependency_links.txt
 src/flowMC.egg-info/requires.txt
 src/flowMC.egg-info/top_level.txt
 src/flowMC/nfmodel/__init__.py
 src/flowMC/nfmodel/base.py
 src/flowMC/nfmodel/common.py
 src/flowMC/nfmodel/realNVP.py
 src/flowMC/nfmodel/rqSpline.py
-src/flowMC/nfmodel/utils.py
-src/flowMC/sampler/Gaussian_random_walk.py
-src/flowMC/sampler/HMC.py
-src/flowMC/sampler/MALA.py
-src/flowMC/sampler/NF_proposal.py
-src/flowMC/sampler/Proposal_Base.py
-src/flowMC/sampler/Sampler.py
-src/flowMC/sampler/__init__.py
-src/flowMC/sampler/flowHMC.py
+src/flowMC/proposal/Gaussian_random_walk.py
+src/flowMC/proposal/HMC.py
+src/flowMC/proposal/MALA.py
+src/flowMC/proposal/NF_proposal.py
+src/flowMC/proposal/__init__.py
+src/flowMC/proposal/base.py
+src/flowMC/proposal/flowHMC.py
+src/flowMC/strategy/__init__.py
+src/flowMC/strategy/base.py
+src/flowMC/strategy/global_tuning.py
+src/flowMC/strategy/importance_sampling.py
 src/flowMC/utils/EvolutionaryOptimizer.py
-src/flowMC/utils/PRNG_keys.py
 src/flowMC/utils/PythonFunctionWrap.py
-src/flowMC/utils/__init__.py
+src/flowMC/utils/__init__.py
+src/flowMC/utils/postprocessing.py
```

