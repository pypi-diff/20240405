# Comparing `tmp/adelie-1.1.27.tar.gz` & `tmp/adelie-1.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adelie-1.1.27.tar", last modified: Thu Apr  4 04:57:54 2024, max compression
+gzip compressed data, was "adelie-1.1.28.tar", last modified: Fri Apr  5 16:11:29 2024, max compression
```

## Comparing `adelie-1.1.27.tar` & `adelie-1.1.28.tar`

### file list

```diff
@@ -1,722 +1,722 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.690470 adelie-1.1.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 04:57:50.000000 adelie-1.1.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-04 04:57:50.000000 adelie-1.1.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-04 04:57:54.690470 adelie-1.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-04 04:57:50.000000 adelie-1.1.27/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 04:57:50.000000 adelie-1.1.27/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.578469 adelie-1.1.27/adelie/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/bcd.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/cv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15834 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    39441 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16258 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/glm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14462 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    37071 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.582469 adelie-1.1.27/adelie/src/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/adelie_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/bcd.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/configs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/decl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/glm.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.566469 adelie-1.1.27/adelie/src/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.582469 adelie-1.1.27/adelie/src/include/adelie_core/
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/bcd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/configs.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.582469 adelie-1.1.27/adelie/src/include/adelie_core/glm/
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_binomial.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_cox.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_gaussian.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_multibase.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_multinomial.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_poisson.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.582469 adelie-1.1.27/adelie/src/include/adelie_core/io/
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/io/io_snp_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/io/io_snp_unphased.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.586470 adelie-1.1.27/adelie/src/include/adelie_core/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/matrix/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.586470 adelie-1.1.27/adelie/src/include/adelie_core/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/optimization/bisect.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/optimization/newton.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/optimization/search_pivot.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.586470 adelie-1.1.27/adelie/src/include/adelie_core/solver/
--rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23177 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/solver/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.590469 adelie-1.1.27/adelie/src/include/adelie_core/state/
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_glm_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.590469 adelie-1.1.27/adelie/src/include/adelie_core/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/algorithm.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.590469 adelie-1.1.27/adelie/src/include/adelie_core/util/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/exceptions.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/format.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/functional.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/queue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/stopwatch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/tqdm.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/include/adelie_core/util/types.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23039 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/optimization.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    69765 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/state.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.566469 adelie-1.1.27/adelie/src/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.590469 adelie-1.1.27/adelie/src/third_party/eigen3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.594469 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/KLUSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/PaStiXSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.570469 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.594469 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.594469 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.610470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (127)    41673 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (127)    63841 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    36282 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    24484 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)    38812 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    60784 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    24343 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    23856 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    49193 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (127)    53832 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (127)    17606 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (127)    38277 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    35168 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.570469 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.610470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    64608 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.610470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    87891 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.614470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (127)    16540 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   119355 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)    24820 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-r--r--   0 runner    (1001) docker     (127)   102394 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.614470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.614470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (127)    26903 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    67696 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner    (1001) docker     (127)    35534 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.614470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    57047 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.566469 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.614470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.614470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.618470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (127)    22503 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)   189525 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    51286 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.618470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    64465 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.618470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.618470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.618470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)    36894 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.622470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    40146 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.626470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (127)   108448 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (127)    20104 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    21724 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.626470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/
--rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (127)    52909 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    46661 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h
--rw-r--r--   0 runner    (1001) docker     (127)    29336 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.630470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    22970 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    22764 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.634470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (127)    61930 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.634470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.634470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.634470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.634470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (127)    16383 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.634470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (127)    32383 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (127)    15727 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (127)    61681 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (127)    25498 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    23429 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.638470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (127)    54214 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)    32988 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.642470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.646470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (127)    24360 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.650470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.650470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (127)    29167 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.650470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.650470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    34324 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.650470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (127)    24456 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.654470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h
--rw-r--r--   0 runner    (1001) docker     (127)  1058369 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.654470 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    59020 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/signature_of_eigen3_matrix_library
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.570469 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.658470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/BVH
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.658470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.574469 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.670470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
--rw-r--r--   0 runner    (1001) docker     (127)    57932 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    60851 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    42150 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
--rw-r--r--   0 runner    (1001) docker     (127)    19707 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
--rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
--rw-r--r--   0 runner    (1001) docker     (127)    45320 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)    63402 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
--rw-r--r--   0 runner    (1001) docker     (127)    89042 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    70687 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
--rw-r--r--   0 runner    (1001) docker     (127)    48686 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    27527 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    40367 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
--rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
--rw-r--r--   0 runner    (1001) docker     (127)    40005 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
--rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
--rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
--rw-r--r--   0 runner    (1001) docker     (127)    24345 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
--rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
--rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
--rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
--rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
--rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
--rw-r--r--   0 runner    (1001) docker     (127)    14191 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
--rw-r--r--   0 runner    (1001) docker     (127)    43284 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
--rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
--rw-r--r--   0 runner    (1001) docker     (127)    44395 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
--rw-r--r--   0 runner    (1001) docker     (127)    40719 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
--rw-r--r--   0 runner    (1001) docker     (127)    30074 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
--rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
--rw-r--r--   0 runner    (1001) docker     (127)    20091 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
--rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
--rw-r--r--   0 runner    (1001) docker     (127)    18256 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
--rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.674470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
--rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.674470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
--rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.674470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
--rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.674470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/
--rw-r--r--   0 runner    (1001) docker     (127)    22752 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles
--rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/FFT
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport
--rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff
--rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/Splines
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.574469 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.674470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
--rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.674470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.674470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (127)    29075 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.678470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.678470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.678470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
--rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.678470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/
--rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.678470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.682470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/
--rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
--rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)    17557 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
--rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.682470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.682470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/
--rw-r--r--   0 runner    (1001) docker     (127)    19837 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)    22135 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.682470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.682470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h
--rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.686470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
--rw-r--r--   0 runner    (1001) docker     (127)    31105 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.686470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    40316 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.686470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
--rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
--rw-r--r--   0 runner    (1001) docker     (127)    58539 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.574469 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.690470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.690470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.690470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
--rw-r--r--   0 runner    (1001) docker     (127)    10864 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.690470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.690470 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/
--rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h
--rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h
--rw-r--r--   0 runner    (1001) docker     (127)   113555 2024-04-04 04:57:50.000000 adelie-1.1.27/adelie/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:57:54.690470 adelie-1.1.27/adelie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-04 04:57:54.000000 adelie-1.1.27/adelie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    41758 2024-04-04 04:57:54.000000 adelie-1.1.27/adelie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:57:54.000000 adelie-1.1.27/adelie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:57:54.000000 adelie-1.1.27/adelie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 04:57:54.000000 adelie-1.1.27/adelie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 04:57:54.000000 adelie-1.1.27/adelie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-04 04:57:50.000000 adelie-1.1.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:57:54.690470 adelie-1.1.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-04 04:57:50.000000 adelie-1.1.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-05 16:11:24.000000 adelie-1.1.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 16:11:24.000000 adelie-1.1.28/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-05 16:11:29.415938 adelie-1.1.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-05 16:11:24.000000 adelie-1.1.28/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 16:11:24.000000 adelie-1.1.28/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.307938 adelie-1.1.28/adelie/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/bcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15834 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39441 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16258 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/glm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15484 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37164 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.311938 adelie-1.1.28/adelie/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/adelie_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/bcd.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/configs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/decl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20125 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/glm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.295938 adelie-1.1.28/adelie/src/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.311938 adelie-1.1.28/adelie/src/include/adelie_core/
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/bcd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/configs.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.311938 adelie-1.1.28/adelie/src/include/adelie_core/glm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_binomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18161 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_cox.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_gaussian.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multibase.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multinomial.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_poisson.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.311938 adelie-1.1.28/adelie/src/include/adelie_core/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_unphased.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.315938 adelie-1.1.28/adelie/src/include/adelie_core/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14994 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_concatenate.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/matrix/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.315938 adelie-1.1.28/adelie/src/include/adelie_core/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/optimization/bisect.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/optimization/newton.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/optimization/search_pivot.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.315938 adelie-1.1.28/adelie/src/include/adelie_core/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)    16562 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23177 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17609 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/solver/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.319938 adelie-1.1.28/adelie/src/include/adelie_core/state/
+-rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_glm_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.319938 adelie-1.1.28/adelie/src/include/adelie_core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/algorithm.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.319938 adelie-1.1.28/adelie/src/include/adelie_core/util/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/exceptions.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/format.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/functional.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/queue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/stopwatch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/tqdm.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/include/adelie_core/util/types.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23931 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/optimization.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    69765 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/state.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.295938 adelie-1.1.28/adelie/src/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.319938 adelie-1.1.28/adelie/src/third_party/eigen3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.323938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (127)    12799 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/KLUSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/PaStiXSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.299938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.323938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18760 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.323938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    25441 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    19214 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    41673 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18648 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63841 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36282 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31529 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24484 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38812 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60784 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24343 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23856 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20748 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49193 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53832 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9368 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17606 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38277 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35168 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.299938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)    15223 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    64608 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)    17160 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    87891 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (127)    16540 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   119355 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9490 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24820 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-r--r--   0 runner    (1001) docker     (127)   102394 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.339938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (127)    17317 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (127)    26903 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67696 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35534 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57047 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.295938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33615 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.343938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)    22503 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   189525 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    51286 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (127)    14251 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    64465 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21856 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36894 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.347938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20921 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40146 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.351938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (127)   108448 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20104 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21724 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21354 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.355938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    23156 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52909 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    46661 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29336 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.359938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22970 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35182 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22764 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.359938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20726 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34367 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61930 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.359938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (127)    16383 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32383 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15727 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22069 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61681 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    22249 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.363938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.367938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (127)    25498 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23429 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26768 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.367938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.367938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (127)    54214 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32988 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15957 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.367938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.371938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13166 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24360 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13606 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25889 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.375938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (127)    33316 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.375938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (127)    29167 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.375938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.375938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    34324 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.379938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)    24456 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.379938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30560 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h
+-rw-r--r--   0 runner    (1001) docker     (127)  1058369 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.383938 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59020 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/signature_of_eigen3_matrix_library
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.299938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.383938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/BVH
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.387938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.299938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.399938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57932 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60851 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    42150 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19707 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45320 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63402 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23586 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h
+-rw-r--r--   0 runner    (1001) docker     (127)    89042 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    70687 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48686 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27527 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40367 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40005 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26655 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24345 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14486 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15269 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10920 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28066 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9094 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14191 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43284 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h
+-rw-r--r--   0 runner    (1001) docker     (127)    44395 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionCuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40719 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30074 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20091 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25279 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18256 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30089 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.399938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.399938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    21046 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.399938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    22752 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles
+-rw-r--r--   0 runner    (1001) docker     (127)    13948 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/FFT
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff
+-rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Splines
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.303938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29107 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9166 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (127)    29075 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.403938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    16624 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22671 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17557 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/
+-rw-r--r--   0 runner    (1001) docker     (127)    19837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22135 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.407938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.411938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15683 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.411938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31105 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.411938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40316 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58539 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.303938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/
+-rw-r--r--   0 runner    (1001) docker     (127)    10864 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/
+-rw-r--r--   0 runner    (1001) docker     (127)    18307 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h
+-rw-r--r--   0 runner    (1001) docker     (127)   113575 2024-04-05 16:11:24.000000 adelie-1.1.28/adelie/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:11:29.415938 adelie-1.1.28/adelie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    41758 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:11:28.000000 adelie-1.1.28/adelie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 16:11:29.000000 adelie-1.1.28/adelie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-05 16:11:24.000000 adelie-1.1.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:11:29.415938 adelie-1.1.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-05 16:11:24.000000 adelie-1.1.28/setup.py
```

### Comparing `adelie-1.1.27/LICENSE` & `adelie-1.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/PKG-INFO` & `adelie-1.1.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adelie
-Version: 1.1.27
+Version: 1.1.28
 Summary: A fast, flexible package for group elastic net.
 Author: James Yang
 Author-email: James Yang <jamesyang916@gmail.com>
 Maintainer: James Yang
 Maintainer-email: James Yang <jamesyang916@gmail.com>
 License: MIT License
```

### Comparing `adelie-1.1.27/README.md` & `adelie-1.1.28/README.md`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/bcd.py` & `adelie-1.1.28/adelie/bcd.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/cv.py` & `adelie-1.1.28/adelie/cv.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/data.py` & `adelie-1.1.28/adelie/data.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/diagnostic.py` & `adelie-1.1.28/adelie/diagnostic.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/glm.py` & `adelie-1.1.28/adelie/glm.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/io.py` & `adelie-1.1.28/adelie/io.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/logger.py` & `adelie-1.1.28/adelie/logger.py`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/matrix.py` & `adelie-1.1.28/adelie/matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,21 +94,36 @@
 
     return _block_diag()
 
 
 def concatenate(
     mats: list,
     *,
+    axis: int=0,
     n_threads: int =1,
 ):
-    """Creates a column-wise concatenation of the matrices.
+    """Creates a concatenation of the matrices.
 
     If ``mats`` represents a list of matrices :math:`X_1,\\ldots, X_L`,
-    then the resulting matrix represents the column-wise concatenated matrix
-    given by
+    then the resulting matrix represents the concatenated matrix along 
+    the given axis ``axis``.
+    
+    If ``axis=0``, the matrix is concatenated row-wise:
+
+    .. math::
+        \\begin{align*}
+            \\begin{bmatrix}
+                \\unicode{x2014} & X_1 & \\unicode{x2014} \\\\
+                \\unicode{x2014} & X_2 & \\unicode{x2014} \\\\
+                \\vdots & \\vdots & \\vdots \\\\
+                \\unicode{x2014} & X_L & \\unicode{x2014}
+            \\end{bmatrix}
+        \\end{align*}
+
+    If ``axis=1``, the matrix is concatenated column-wise:
 
     .. math::
         \\begin{align*}
             \\begin{bmatrix}
                 \\vert & \\vert & \\cdots & \\vert \\\\
                 X_1 & X_2 & \\cdots & X_L \\\\
                 \\vert & \\vert & \\cdots & \\vert
@@ -117,15 +132,18 @@
 
     .. note::
         This matrix only works for naive method!
 
     Parameters
     ----------
     mats : list
-        List of matrices to concatenate along the columns.
+        List of matrices to concatenate.
+    axis : int, optional
+        The axis along which the matrices will be joined.
+        Default is ``0``.
     n_threads : int, optional
         Number of threads.
         Default is ``1``.
 
     Returns
     -------
     wrap
@@ -143,20 +161,28 @@
     ]
     dtype = _to_dtype(mats[0])
 
     for mat in mats:
         if dtype == _to_dtype(mat): continue
         raise ValueError("All matrices must have the same underlying data type.")
 
+    cdispatcher = {
+        np.float64: core.matrix.MatrixNaiveCConcatenate64,
+        np.float32: core.matrix.MatrixNaiveCConcatenate32,
+    }
+    rdispatcher = {
+        np.float64: core.matrix.MatrixNaiveRConcatenate64,
+        np.float32: core.matrix.MatrixNaiveRConcatenate32,
+    }
     dispatcher = {
-        np.float64: core.matrix.MatrixNaiveConcatenate64,
-        np.float32: core.matrix.MatrixNaiveConcatenate32,
+        0: rdispatcher,
+        1: cdispatcher,
     }
 
-    core_base = dispatcher[dtype]
+    core_base = dispatcher[axis][dtype]
 
     class _concatenate(core_base):
         def __init__(self):
             self.mats = mats
             core_base.__init__(self, self.mats, n_threads)
 
     return _concatenate()
@@ -220,18 +246,24 @@
     dispatcher = {
         "naive" : naive_dispatcher,
         "cov" : cov_dispatcher,
     }
 
     dtype = mat.dtype
     order = (
-        "C"
-        if mat.flags.c_contiguous else
         "F"
+        # prioritize choosing Fortran contiguity
+        if mat.flags.f_contiguous else
+        "C"
     )
+    if order == "C":
+        warnings.warn(
+            "Detected matrix to be C-contiguous. "
+            "Performance may improve with F-contiguous matrix."
+        )
     core_base = dispatcher[method][dtype][order]
 
     class _dense(core_base):
         def __init__(self):
             self.mat = mat
             core_base.__init__(self, self.mat, n_threads)
```

### Comparing `adelie-1.1.27/adelie/solver.py` & `adelie-1.1.28/adelie/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -760,20 +760,24 @@
         solver_args["screen_set"] = screen_set
         solver_args["screen_beta"] = screen_beta
         solver_args["screen_is_active"] = screen_is_active
 
         # represent the augmented X matrix as used in single-response reformatted problem.
         X_aug = matrix.kronecker_eye(X_raw, K, n_threads=n_threads)
         if intercept:
-            X_aug = matrix.concatenate([
-                matrix.kronecker_eye(
-                    np.ones((n, 1)), K, n_threads=n_threads
-                ),
-                X_aug,
-            ], n_threads=n_threads)
+            X_aug = matrix.concatenate(
+                [
+                    matrix.kronecker_eye(
+                        np.ones((n, 1)), K, n_threads=n_threads
+                    ),
+                    X_aug,
+                ], 
+                axis=1, 
+                n_threads=n_threads,
+            )
 
         # special gaussian case
         if is_gaussian_opt:
             y = glm.y
             weights = glm.weights
             weights_mscaled = weights / K
             if warm_start is None:
```

### Comparing `adelie-1.1.27/adelie/src/adelie_core.cpp` & `adelie-1.1.28/adelie/src/adelie_core.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/bcd.cpp` & `adelie-1.1.28/adelie/src/bcd.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/configs.cpp` & `adelie-1.1.28/adelie/src/configs.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/decl.hpp` & `adelie-1.1.28/adelie/src/decl.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/glm.cpp` & `adelie-1.1.28/adelie/src/glm.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/bcd.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/bcd.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_base.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_binomial.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_binomial.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_cox.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_cox.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_gaussian.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_gaussian.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_multibase.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multibase.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multigaussian.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_multinomial.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_multinomial.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/glm/glm_poisson.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/glm/glm_poisson.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/io/io_snp_base.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_phased_ancestry.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/io/io_snp_unphased.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/io/io_snp_unphased.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_block_diag.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_dense.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_lazy_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_cov_sparse.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_dense.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_kronecker_eye.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_snp_phased_ancestry.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_snp_unphased.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/matrix_naive_sparse.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/matrix/utils.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/matrix/utils.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/optimization/bisect.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/optimization/bisect.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/optimization/newton.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/optimization/newton.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/optimization/search_pivot.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/optimization/search_pivot.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/optimization/symmetric_penalty.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_base.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_gaussian_pin_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_glm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_multigaussian_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/solver_multiglm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/solver/utils.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/solver/utils.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_base.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_base.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_cov.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_gaussian_pin_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_glm_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_glm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_multigaussian_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/state/state_multiglm_naive.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/util/algorithm.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/util/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/util/eigen/map_sparsevector.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/util/exceptions.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/util/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/util/format.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/util/format.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/util/macros.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/util/macros.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/util/stopwatch.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/util/stopwatch.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/util/tqdm.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/util/tqdm.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/include/adelie_core/util/types.hpp` & `adelie-1.1.28/adelie/src/include/adelie_core/util/types.hpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/io.cpp` & `adelie-1.1.28/adelie/src/io.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/matrix.cpp` & `adelie-1.1.28/adelie/src/matrix.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -519,17 +519,38 @@
             py::arg("value"),
             py::arg("n_threads")
         )
         ;
 }
 
 template <class ValueType>
-void matrix_naive_concatenate(py::module_& m, const char* name)
+void matrix_naive_cconcatenate(py::module_& m, const char* name)
 {
-    using internal_t = ad::matrix::MatrixNaiveConcatenate<ValueType>;
+    using internal_t = ad::matrix::MatrixNaiveCConcatenate<ValueType>;
+    using base_t = typename internal_t::base_t;
+    py::class_<internal_t, base_t>(m, name)
+        .def(
+            py::init([](py::list mat_list_py, size_t n_threads) {
+                std::vector<base_t*> mat_list;
+                mat_list.reserve(mat_list_py.size());
+                for (auto obj : mat_list_py) {
+                    mat_list.push_back(py::cast<base_t*>(obj));
+                }
+                return new internal_t(mat_list, n_threads);
+            }), 
+            py::arg("mat_list").noconvert(),
+            py::arg("n_threads")
+        )
+        ;
+}
+
+template <class ValueType>
+void matrix_naive_rconcatenate(py::module_& m, const char* name)
+{
+    using internal_t = ad::matrix::MatrixNaiveRConcatenate<ValueType>;
     using base_t = typename internal_t::base_t;
     py::class_<internal_t, base_t>(m, name)
         .def(
             py::init([](py::list mat_list_py, size_t n_threads) {
                 std::vector<base_t*> mat_list;
                 mat_list.reserve(mat_list_py.size());
                 for (auto obj : mat_list_py) {
@@ -689,16 +710,18 @@
     matrix_cov_lazy_cov<dense_type<float, Eigen::RowMajor>>(m, "MatrixCovLazyCov32C");
     matrix_cov_lazy_cov<dense_type<float, Eigen::ColMajor>>(m, "MatrixCovLazyCov32F");
 
     matrix_cov_sparse<sparse_type<double, Eigen::ColMajor>>(m, "MatrixCovSparse64F");
     matrix_cov_sparse<sparse_type<float, Eigen::ColMajor>>(m, "MatrixCovSparse32F");
 
     /* naive matrices */
-    matrix_naive_concatenate<double>(m, "MatrixNaiveConcatenate64");
-    matrix_naive_concatenate<float>(m, "MatrixNaiveConcatenate32");
+    matrix_naive_cconcatenate<double>(m, "MatrixNaiveCConcatenate64");
+    matrix_naive_cconcatenate<float>(m, "MatrixNaiveCConcatenate32");
+    matrix_naive_rconcatenate<double>(m, "MatrixNaiveRConcatenate64");
+    matrix_naive_rconcatenate<float>(m, "MatrixNaiveRConcatenate32");
 
     matrix_naive_dense<dense_type<double, Eigen::RowMajor>>(m, "MatrixNaiveDense64C");
     matrix_naive_dense<dense_type<double, Eigen::ColMajor>>(m, "MatrixNaiveDense64F");
     matrix_naive_dense<dense_type<float, Eigen::RowMajor>>(m, "MatrixNaiveDense32C");
     matrix_naive_dense<dense_type<float, Eigen::ColMajor>>(m, "MatrixNaiveDense32F");
 
     matrix_naive_kronecker_eye<double>(m, "MatrixNaiveKroneckerEye64");
```

### Comparing `adelie-1.1.27/adelie/src/optimization.cpp` & `adelie-1.1.28/adelie/src/optimization.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/solver.cpp` & `adelie-1.1.28/adelie/src/solver.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/state.cpp` & `adelie-1.1.28/adelie/src/state.cpp`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Cholesky` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/CholmodSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Core` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Core`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Eigenvalues` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Geometry` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Householder` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Jacobi` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/KLUSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/LU` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/LU`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/MetisSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/OrderingMethods` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/PaStiXSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/PardisoSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/QR` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/QR`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SPQRSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SVD` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/Sparse` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SparseCholesky` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SparseCore` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SparseLU` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SparseQR` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/StdDeque` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/StdList` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/StdVector` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/SuperLUSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/UmfPackSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AdolcForward`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AlignedVector3`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/ArpackSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/AutoDiff`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/BVH` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/BVH`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/Tensor`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/TensorSymmetry`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/ThreadPool`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/Tensor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorArgMax.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorAssign.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBlock.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorBroadcasting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorChipping.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConcatenation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContraction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionBlocking.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionMapper.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorContractionThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConversion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolution.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorConvolutionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCostModel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorCustomOp.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDevice.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceDefault.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDeviceThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensionList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorDimensions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvalTo.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorEvaluator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExecutor.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorExpr.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFFT.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFixedSize.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForcedEval.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGenerator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaDefines.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorGpuHipCudaUndefines.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorImagePatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIndexList.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInflation.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorInitializer.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorIntDiv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorLayoutSwap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMacros.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMap.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMeta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorMorphing.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPadding.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorPatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRandom.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReduction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionGpu.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReductionSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorRef.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorReverse.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScan.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorScanSycl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorShuffling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorStriding.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTrace.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorTraits.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorUInt128.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/Tensor/TensorVolumePatch.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/DynamicSymmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/StaticSymmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/Symmetry.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/TensorSymmetry/util/TemplateGroupTheory.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/Barrier.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/EventCount.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/NonBlockingThreadPool.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/RunQueue.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadCancel.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadEnvironment.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadLocal.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadPoolInterface.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/ThreadPool/ThreadYield.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Meta.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/CXX11Workarounds.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/EmulateArray.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/CXX11/src/util/MaxSizeVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/EulerAngles`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/FFT` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/FFT`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/IterativeSolvers`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/KroneckerProduct`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/LevenbergMarquardt`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MPRealSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MatrixFunctions`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/MoreVectorization`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/NonLinearOptimization`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/NumericalDiff`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/OpenGLSupport`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Polynomials`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Skyline`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/SparseExtra`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/SpecialFunctions`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/Splines` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/Splines`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffJacobian.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffScalar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/AutoDiff/AutoDiffVector.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/BVAlgorithms.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/BVH/KdBVH.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Eigenvalues/ArpackSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/EulerAngles/EulerSystem.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_fftw_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/FFT/ei_kissfft_impl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/ConstrainedConjGrad.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/DGMRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/GMRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IDRS.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IncompleteLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/IterationController.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/MINRES.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/IterativeSolvers/Scaling.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/KroneckerProduct/KroneckerTensorProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMcovar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMonestep.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMpar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LMqrsolv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/LevenbergMarquardt/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixExponential.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixFunction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixLogarithm.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixPower.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/MatrixSquareRoot.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MatrixFunctions/StemFunction.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/MoreVectorization/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/HybridNonLinearSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/LevenbergMarquardt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/chkder.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/covar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/dogleg.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/fdjac1.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/lmpar.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/qrsolv.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1mpyq.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/r1updt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NonLinearOptimization/rwupdt.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/NumericalDiff/NumericalDiff.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/Companion.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialSolver.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Polynomials/PolynomialUtils.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineInplaceLU.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineMatrixBase.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineProduct.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineStorage.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Skyline/SkylineUtil.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockOfDynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/BlockSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/DynamicSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MarketIO.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/MatrixMarketIterator.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SparseExtra/RandomSetter.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/BesselFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/HipVectorCompatibility.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsArrayAPI.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsBFloat16.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsFunctors.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsHalf.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/SpecialFunctionsPacketMath.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/AVX512/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/GPU/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/BesselFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/SpecialFunctions/arch/NEON/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/Spline.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFitting.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h` & `adelie-1.1.28/adelie/src/third_party/eigen3/unsupported/Eigen/src/Splines/SplineFwd.h`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/adelie/state.py` & `adelie-1.1.28/adelie/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1124,14 +1124,15 @@
     offsets = np.array(offsets, order="C", copy=False)
     n, n_classes = offsets.shape
     X = matrix.kronecker_eye(X, n_classes, n_threads=n_threads)
     if intercept:
         ones_kron = matrix.kronecker_eye(np.ones((n, 1)), n_classes, n_threads=n_threads)
         X = matrix.concatenate(
             [ones_kron, X], 
+            axis=1,
             n_threads=n_threads,
         )
 
     # G == (p+intercept) * K if and only if ungrouped
     if groups.shape[0] == X.cols():
         group_type = "ungrouped"
     else:
```

### Comparing `adelie-1.1.27/adelie.egg-info/PKG-INFO` & `adelie-1.1.28/adelie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adelie
-Version: 1.1.27
+Version: 1.1.28
 Summary: A fast, flexible package for group elastic net.
 Author: James Yang
 Author-email: James Yang <jamesyang916@gmail.com>
 Maintainer: James Yang
 Maintainer-email: James Yang <jamesyang916@gmail.com>
 License: MIT License
```

### Comparing `adelie-1.1.27/adelie.egg-info/SOURCES.txt` & `adelie-1.1.28/adelie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/pyproject.toml` & `adelie-1.1.28/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adelie-1.1.27/setup.py` & `adelie-1.1.28/setup.py`

 * *Files identical despite different names*

