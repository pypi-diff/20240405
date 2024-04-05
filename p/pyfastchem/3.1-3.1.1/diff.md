# Comparing `tmp/pyfastchem-3.1.tar.gz` & `tmp/pyfastchem-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfastchem-3.1.tar", last modified: Thu Mar 14 13:18:56 2024, max compression
+gzip compressed data, was "pyfastchem-3.1.1.tar", last modified: Fri Apr  5 12:41:48 2024, max compression
```

## Comparing `pyfastchem-3.1.tar` & `pyfastchem-3.1.1.tar`

### file list

```diff
@@ -1,443 +1,443 @@
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.776880 pyfastchem-3.1/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      203 2023-09-11 14:26:36.000000 pyfastchem-3.1/MANIFEST.in
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      253 2024-03-14 13:18:56.776880 pyfastchem-3.1/PKG-INFO
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3841 2024-03-14 13:12:50.000000 pyfastchem-3.1/README.md
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.736881 pyfastchem-3.1/_ext/
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.740881 pyfastchem-3.1/_ext/Eigen/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1161 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/Cholesky
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1900 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/CholmodSupport
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12799 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/Core
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      122 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/Dense
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)       35 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/Eigen
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1777 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/Eigenvalues
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1940 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/Geometry
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      829 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/Householder
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2083 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/IterativeLinearSolvers
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      894 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/Jacobi
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1389 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/KLUSupport
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1268 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/LU
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      991 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/MetisSupport
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2451 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/OrderingMethods
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1751 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/PaStiXSupport
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1116 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/PardisoSupport
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1272 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/QR
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      900 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/QtAlignedMalloc
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1162 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/SPQRSupport
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1584 2023-09-04 16:33:05.000000 pyfastchem-3.1/_ext/Eigen/SVD
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      888 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/Sparse
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1235 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/SparseCholesky
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2240 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/SparseCore
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1814 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/SparseLU
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1195 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/SparseQR
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      797 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/StdDeque
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      726 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/StdList
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      803 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/StdVector
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2243 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/SuperLUSupport
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1382 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/UmfPackSupport
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.736881 pyfastchem-3.1/_ext/Eigen/src/
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.740881 pyfastchem-3.1/_ext/Eigen/src/Cholesky/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24934 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Cholesky/LDLT.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    18760 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Cholesky/LLT.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3974 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.740881 pyfastchem-3.1/_ext/Eigen/src/CholmodSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25441 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.748881 pyfastchem-3.1/_ext/Eigen/src/Core/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    19214 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/ArithmeticSequence.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16782 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Array.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8217 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/ArrayBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7018 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/ArrayWrapper.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2738 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Assign.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    41673 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/AssignEvaluator.h
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    12488 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Assign_MKL.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14075 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/BandMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    18648 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Block.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4429 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/BooleanRedux.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5981 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/CommaInitializer.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6990 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/ConditionEstimator.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    63841 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/CoreEvaluators.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4745 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/CoreIterators.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7909 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    36282 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8256 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3937 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5551 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    31529 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/DenseBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24484 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25360 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/DenseStorage.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9870 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Diagonal.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14670 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      988 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/DiagonalProduct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11654 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Dot.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5841 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/EigenBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4909 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5759 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Fuzzy.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21679 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/GeneralProduct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    38812 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/GenericPacketMath.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11543 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/GlobalFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8238 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/IO.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9620 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/IndexedView.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3503 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Inverse.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7256 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Map.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11281 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/MapBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    60784 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7156 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24343 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Matrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    23856 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/MatrixBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2520 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/NestByValue.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3620 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/NoAlias.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12884 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/NumTraits.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9207 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/PartialReduxEvaluator.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20748 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/PermutationMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    49193 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/PlainObjectBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7336 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Product.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    53832 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/ProductEvaluators.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7756 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Random.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    19195 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Redux.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17821 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Ref.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5656 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Replicate.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17033 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Reshaped.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4284 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/ReturnByValue.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7522 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Reverse.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6143 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Select.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14999 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/SelfAdjointView.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1697 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6837 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Solve.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9368 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/SolveTriangular.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6170 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/SolverBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8700 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/StableNorm.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21641 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/StlIterators.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4212 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Stride.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2765 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Swap.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17606 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Transpose.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13567 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Transpositions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    38277 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/TriangularMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3488 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/VectorBlock.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    35168 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/VectorwiseOp.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11997 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/Visitor.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.736881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.748881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15223 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/Complex.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8102 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    64608 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2564 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17160 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/Complex.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13344 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    87891 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2134 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16540 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2323 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)   119355 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9490 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24820 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)   102394 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/CUDA/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17317 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/CUDA/Complex.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    26903 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/BFloat16.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5251 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    67696 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3770 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    35534 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/Half.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1746 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/Settings.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3746 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/GPU/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2695 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    57047 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2256 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.736881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/HIP/
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/HIP/hcc/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      691 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/MSA/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17541 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/MSA/Complex.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16159 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    33615 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22503 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6815 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3083 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)   189525 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    51286 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14251 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6765 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    64465 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3650 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.752881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SVE/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1194 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21200 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1351 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.756881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7428 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12539 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    27786 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21856 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2626 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.756881 pyfastchem-3.1/_ext/Eigen/src/Core/arch/ZVector/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16728 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/ZVector/Complex.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8024 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    36894 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.756881 pyfastchem-3.1/_ext/Eigen/src/Core/functors/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6686 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20921 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8334 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4998 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      607 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    40146 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.756881 pyfastchem-3.1/_ext/Eigen/src/Core/products/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)   108448 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20104 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15948 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6936 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5106 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21724 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6368 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5582 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/Parallelizer.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21354 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11570 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9958 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5209 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6164 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4126 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20987 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13867 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14722 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10571 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14678 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6707 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5882 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.760881 pyfastchem-3.1/_ext/Eigen/src/Core/util/
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    23156 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/BlasUtil.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    19876 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/ConfigureVectorization.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21931 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/Constants.h
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)     4892 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15555 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6696 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/IndexedViewHelper.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10949 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/IntegralConstant.h
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)     4268 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/MKL_support.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    52909 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/Macros.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    46661 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/Memory.h
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    29336 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/Meta.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)       85 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/NonMPL2.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1024 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1432 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/ReshapedHelper.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10676 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/StaticAssert.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12003 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/SymbolicIndex.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    35762 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Core/util/XprHelper.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.760881 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12559 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17274 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4178 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22970 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17176 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9716 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14349 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5575 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    23640 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21078 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3650 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    35182 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4104 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22764 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.760881 pyfastchem-3.1/_ext/Eigen/src/Geometry/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    18939 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/AlignedBox.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8403 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/AngleAxis.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3624 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/EulerAngles.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20726 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/Homogeneous.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11962 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/Hyperplane.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8955 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9812 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    34367 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/Quaternion.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6862 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/Rotation2D.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8063 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/RotationBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6724 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/Scaling.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    61930 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/Transform.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7664 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/Translation.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6190 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/Umeyama.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.760881 pyfastchem-3.1/_ext/Eigen/src/Geometry/arch/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5945 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.760881 pyfastchem-3.1/_ext/Eigen/src/Householder/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4784 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5365 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Householder/Householder.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    23611 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6771 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6850 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8887 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15036 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14940 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13379 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7349 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4212 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/Jacobi/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16383 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/Jacobi/Jacobi.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/KLUSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11555 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/KLUSupport/KLUSupport.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/LU/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3439 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/LU/Determinant.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    32383 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/LU/FullPivLU.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15727 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/LU/InverseImpl.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22069 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/LU/PartialPivLU.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3555 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/LU/arch/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13693 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/LU/arch/InverseSize4.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/MetisSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4588 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/OrderingMethods/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16105 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/OrderingMethods/Amd.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    61681 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5248 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/PaStiXSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22249 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/PardisoSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20092 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/QR/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25498 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4662 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    23429 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    26768 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14641 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/QR/HouseholderQR.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2993 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/SPQRSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11826 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/SVD/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    54214 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SVD/BDCSVD.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    32988 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SVD/JacobiSVD.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5099 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14743 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SVD/SVDBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15957 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.764881 pyfastchem-3.1/_ext/Eigen/src/SparseCholesky/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24216 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5830 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.768880 pyfastchem-3.1/_ext/Eigen/src/SparseCore/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10670 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8743 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13166 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2191 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11368 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24360 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6485 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13606 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25524 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4757 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13256 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5808 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3080 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseDot.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1107 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12589 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseMap.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    57475 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17451 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7329 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7593 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1699 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15600 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseRef.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25889 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4424 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8704 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3175 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6437 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6827 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14832 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseVector.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8127 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseView.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9657 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.768880 pyfastchem-3.1/_ext/Eigen/src/SparseLU/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    33316 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4303 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7602 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4974 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12837 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2049 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6712 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6584 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3681 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10217 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4181 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5723 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8485 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9028 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4979 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4545 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2889 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.768880 pyfastchem-3.1/_ext/Eigen/src/SparseQR/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    29167 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SparseQR/SparseQR.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.768880 pyfastchem-3.1/_ext/Eigen/src/StlSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4730 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/StlSupport/StdDeque.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4155 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/StlSupport/StdList.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5338 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/StlSupport/StdVector.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2809 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/StlSupport/details.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.768880 pyfastchem-3.1/_ext/Eigen/src/SuperLUSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    34324 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.768880 pyfastchem-3.1/_ext/Eigen/src/UmfPackSupport/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24456 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.772880 pyfastchem-3.1/_ext/Eigen/src/misc/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2913 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/misc/Image.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2742 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/misc/Kernel.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1748 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/misc/RealSvd2x2.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    30560 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/misc/blas.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7834 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/misc/lapack.h
--rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)  1058369 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/misc/lapacke.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      474 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/misc/lapacke_mangling.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.772880 pyfastchem-3.1/_ext/Eigen/src/plugins/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14060 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21431 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    59020 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/BlockMethods.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4828 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6089 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12283 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/IndexedViewMethods.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6387 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3350 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6915 2023-09-04 16:33:06.000000 pyfastchem-3.1/_ext/Eigen/src/plugins/ReshapedMethods.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.772880 pyfastchem-3.1/fastchem_src/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    18039 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/calc_densities.cpp
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.772880 pyfastchem-3.1/fastchem_src/condensed_phase/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17322 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/condensed_phase/calculate.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4780 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/condensed_phase/condensate_struct.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5508 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/condensed_phase/condensed_phase.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5459 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/condensed_phase/condensed_phase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5299 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/condensed_phase/read_condensate_data.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16226 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/condensed_phase/solver.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5919 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/condensed_phase/solver.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.772880 pyfastchem-3.1/fastchem_src/elements/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4038 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/elements/chemical_element_data.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6543 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/elements/element_struct.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5499 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/elements/elements.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2011 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/elements/elements.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3035 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/elements/read_files.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5472 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/fastchem.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4919 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/fastchem.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1648 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/fastchem_constants.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10211 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/fastchem_get_set.cpp
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.776880 pyfastchem-3.1/fastchem_src/gas_phase/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5271 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/calc_electron_densities.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1334 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/calc_mean_mol_weight.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4358 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/gas_phase/calc_species_densities.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6119 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/gas_phase/calculate.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9299 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/gas_phase.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3417 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/gas_phase.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4646 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/init_read_files.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3329 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/init_solver.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2582 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/molecule_struct.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1536 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/solver.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5488 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/gas_phase/solver.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2700 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/solver_bisection.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6824 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/solver_coeff.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3600 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/solver_linsol_quadsol.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5858 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/solver_nelder_mead_electron.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9056 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/gas_phase/solver_newtsol.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5610 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/gas_phase/solver_newtsol_mult.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1631 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/input_output_struct.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4283 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/options.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3877 2024-03-14 12:42:04.000000 pyfastchem-3.1/fastchem_src/options.h
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5012 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/options_read_files.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6185 2023-09-04 16:33:06.000000 pyfastchem-3.1/fastchem_src/species_struct.h
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.776880 pyfastchem-3.1/pyfastchem.egg-info/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      253 2024-03-14 13:18:56.000000 pyfastchem-3.1/pyfastchem.egg-info/PKG-INFO
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15313 2024-03-14 13:18:56.000000 pyfastchem-3.1/pyfastchem.egg-info/SOURCES.txt
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)        1 2024-03-14 13:18:56.000000 pyfastchem-3.1/pyfastchem.egg-info/dependency_links.txt
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)       11 2024-03-14 13:18:56.000000 pyfastchem-3.1/pyfastchem.egg-info/top_level.txt
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      120 2022-02-17 09:56:50.000000 pyfastchem-3.1/pyproject.toml
-drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-03-14 13:18:56.776880 pyfastchem-3.1/python/
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5284 2023-09-04 16:33:06.000000 pyfastchem-3.1/python/fastchem_python_wrapper.cpp
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)       38 2024-03-14 13:18:56.776880 pyfastchem-3.1/setup.cfg
--rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3003 2024-03-14 13:16:31.000000 pyfastchem-3.1/setup.py
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.719473 pyfastchem-3.1.1/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      203 2023-09-11 14:26:36.000000 pyfastchem-3.1.1/MANIFEST.in
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      255 2024-04-05 12:41:48.719473 pyfastchem-3.1.1/PKG-INFO
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3841 2024-04-05 12:39:56.000000 pyfastchem-3.1.1/README.md
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.639475 pyfastchem-3.1.1/_ext/
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.655475 pyfastchem-3.1.1/_ext/Eigen/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1161 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/Cholesky
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1900 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/CholmodSupport
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12799 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/Core
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      122 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/Dense
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)       35 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/Eigen
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1777 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/Eigenvalues
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1940 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/Geometry
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      829 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/Householder
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2083 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/IterativeLinearSolvers
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      894 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/Jacobi
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1389 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/KLUSupport
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1268 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/LU
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      991 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/MetisSupport
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2451 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/OrderingMethods
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1751 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/PaStiXSupport
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1116 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/PardisoSupport
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1272 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/QR
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      900 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/QtAlignedMalloc
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1162 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/SPQRSupport
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1584 2023-09-04 16:33:05.000000 pyfastchem-3.1.1/_ext/Eigen/SVD
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      888 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/Sparse
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1235 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/SparseCholesky
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2240 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/SparseCore
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1814 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/SparseLU
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1195 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/SparseQR
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      797 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/StdDeque
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      726 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/StdList
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      803 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/StdVector
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2243 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/SuperLUSupport
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1382 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/UmfPackSupport
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.647475 pyfastchem-3.1.1/_ext/Eigen/src/
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.655475 pyfastchem-3.1.1/_ext/Eigen/src/Cholesky/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24934 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Cholesky/LDLT.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    18760 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Cholesky/LLT.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3974 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.655475 pyfastchem-3.1.1/_ext/Eigen/src/CholmodSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25441 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.663474 pyfastchem-3.1.1/_ext/Eigen/src/Core/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    19214 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/ArithmeticSequence.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16782 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Array.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8217 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/ArrayBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7018 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2738 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Assign.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    41673 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/AssignEvaluator.h
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    12488 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Assign_MKL.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14075 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/BandMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    18648 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Block.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4429 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/BooleanRedux.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5981 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/CommaInitializer.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6990 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/ConditionEstimator.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    63841 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/CoreEvaluators.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4745 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/CoreIterators.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7909 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    36282 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8256 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseTernaryOp.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3937 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5551 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    31529 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/DenseBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24484 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25360 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/DenseStorage.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9870 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Diagonal.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14670 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      988 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11654 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Dot.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5841 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/EigenBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4909 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5759 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Fuzzy.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21679 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/GeneralProduct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    38812 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11543 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8238 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/IO.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9620 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/IndexedView.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3503 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Inverse.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7256 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Map.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11281 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/MapBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    60784 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7156 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/MathFunctionsImpl.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24343 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Matrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    23856 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/MatrixBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2520 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/NestByValue.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3620 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/NoAlias.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12884 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/NumTraits.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9207 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20748 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    49193 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7336 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Product.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    53832 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/ProductEvaluators.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7756 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Random.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    19195 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Redux.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17821 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Ref.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5656 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Replicate.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17033 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Reshaped.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4284 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/ReturnByValue.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7522 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Reverse.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6143 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Select.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14999 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1697 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6837 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Solve.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9368 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/SolveTriangular.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6170 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/SolverBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8700 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/StableNorm.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21641 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/StlIterators.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4212 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Stride.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2765 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Swap.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17606 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Transpose.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13567 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Transpositions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    38277 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3488 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/VectorBlock.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    35168 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11997 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/Visitor.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.643475 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.667474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15223 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/Complex.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8102 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    64608 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2564 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.667474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17160 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13344 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    87891 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2134 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.671474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16540 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2323 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)   119355 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9490 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24820 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)   102394 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.671474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/CUDA/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17317 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/CUDA/Complex.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.671474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    26903 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5251 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    67696 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3770 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    35534 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/Half.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1746 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/Settings.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3746 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.671474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/GPU/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2695 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    57047 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2256 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.643475 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/HIP/
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.671474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/HIP/hcc/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      691 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.671474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/MSA/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17541 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/MSA/Complex.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16159 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    33615 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.671474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22503 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6815 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3083 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)   189525 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    51286 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.675474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14251 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6765 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    64465 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3650 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.675474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SVE/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1194 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21200 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1351 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.675474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7428 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12539 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    27786 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21856 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2626 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.675474 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/ZVector/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16728 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8024 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    36894 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.675474 pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6686 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20921 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8334 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4998 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/StlFunctors.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      607 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    40146 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.679474 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)   108448 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20104 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15948 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6936 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5106 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21724 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6368 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5582 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21354 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11570 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9958 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5209 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6164 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4126 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20987 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13867 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14722 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10571 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14678 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6707 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5882 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.683474 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    23156 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    19876 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21931 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/Constants.h
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)     4892 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15555 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6696 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10949 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/IntegralConstant.h
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)     4268 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/MKL_support.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    52909 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/Macros.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    46661 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/Memory.h
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)    29336 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/Meta.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)       85 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1024 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1432 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/ReshapedHelper.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10676 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12003 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/SymbolicIndex.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    35762 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Core/util/XprHelper.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.683474 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12559 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17274 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4178 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22970 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17176 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9716 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14349 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5575 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    23640 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21078 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3650 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    35182 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4104 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22764 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.683474 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    18939 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8403 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3624 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20726 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11962 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8955 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9812 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    34367 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Quaternion.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6862 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8063 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/RotationBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6724 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Scaling.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    61930 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Transform.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7664 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Translation.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6190 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Umeyama.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.683474 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/arch/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5945 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.683474 pyfastchem-3.1.1/_ext/Eigen/src/Householder/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4784 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5365 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Householder/Householder.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    23611 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6771 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6850 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8887 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15036 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14940 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13379 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7349 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4212 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/Jacobi/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16383 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/Jacobi/Jacobi.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/KLUSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11555 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/KLUSupport/KLUSupport.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/LU/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3439 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/LU/Determinant.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    32383 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/LU/FullPivLU.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15727 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/LU/InverseImpl.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22069 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/LU/PartialPivLU.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3555 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/LU/arch/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13693 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/LU/arch/InverseSize4.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/MetisSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4588 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/OrderingMethods/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16105 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    61681 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5248 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/PaStiXSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    22249 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.687474 pyfastchem-3.1.1/_ext/Eigen/src/PardisoSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    20092 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.691474 pyfastchem-3.1.1/_ext/Eigen/src/QR/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25498 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4662 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    23429 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    26768 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14641 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/QR/HouseholderQR.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2993 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.691474 pyfastchem-3.1.1/_ext/Eigen/src/SPQRSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11826 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.691474 pyfastchem-3.1.1/_ext/Eigen/src/SVD/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    54214 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SVD/BDCSVD.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    32988 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5099 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14743 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SVD/SVDBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15957 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.691474 pyfastchem-3.1.1/_ext/Eigen/src/SparseCholesky/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24216 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5830 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.695474 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10670 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8743 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13166 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2191 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    11368 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseAssign.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24360 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6485 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13606 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25524 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4757 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    13256 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5808 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3080 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1107 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12589 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseMap.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    57475 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17451 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7329 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7593 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1699 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15600 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseRef.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    25889 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4424 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8704 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3175 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6437 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6827 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14832 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8127 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseView.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9657 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.695474 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    33316 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4303 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7602 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4974 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12837 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2049 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6712 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6584 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3681 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10217 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4181 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5723 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     8485 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9028 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4979 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4545 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2889 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.695474 pyfastchem-3.1.1/_ext/Eigen/src/SparseQR/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    29167 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SparseQR/SparseQR.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.699474 pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4730 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/StdDeque.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4155 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/StdList.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5338 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/StdVector.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2809 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/details.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.699474 pyfastchem-3.1.1/_ext/Eigen/src/SuperLUSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    34324 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.699474 pyfastchem-3.1.1/_ext/Eigen/src/UmfPackSupport/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    24456 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.703474 pyfastchem-3.1.1/_ext/Eigen/src/misc/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2913 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/misc/Image.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2742 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/misc/Kernel.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1748 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/misc/RealSvd2x2.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    30560 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/misc/blas.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     7834 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/misc/lapack.h
+-rwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)  1058369 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/misc/lapacke.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      474 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/misc/lapacke_mangling.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.707474 pyfastchem-3.1.1/_ext/Eigen/src/plugins/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    14060 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    21431 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    59020 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/BlockMethods.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4828 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6089 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    12283 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/IndexedViewMethods.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6387 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3350 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6915 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/_ext/Eigen/src/plugins/ReshapedMethods.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.707474 pyfastchem-3.1.1/fastchem_src/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    18481 2024-04-05 12:40:06.000000 pyfastchem-3.1.1/fastchem_src/calc_densities.cpp
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.711474 pyfastchem-3.1.1/fastchem_src/condensed_phase/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    17322 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/condensed_phase/calculate.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4780 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/condensed_phase/condensate_struct.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5398 2024-04-05 12:40:06.000000 pyfastchem-3.1.1/fastchem_src/condensed_phase/condensed_phase.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5459 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/condensed_phase/condensed_phase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5299 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/condensed_phase/read_condensate_data.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    16226 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/condensed_phase/solver.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5919 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/condensed_phase/solver.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.711474 pyfastchem-3.1.1/fastchem_src/elements/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4038 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/elements/chemical_element_data.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6543 2024-03-14 12:42:04.000000 pyfastchem-3.1.1/fastchem_src/elements/element_struct.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5499 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/elements/elements.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2011 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/elements/elements.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3035 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/elements/read_files.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5472 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/fastchem.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4919 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/fastchem.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1648 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/fastchem_constants.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    10211 2024-03-14 12:42:04.000000 pyfastchem-3.1.1/fastchem_src/fastchem_get_set.cpp
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.719473 pyfastchem-3.1.1/fastchem_src/gas_phase/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5271 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/calc_electron_densities.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1334 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/calc_mean_mol_weight.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4358 2024-03-14 12:42:04.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/calc_species_densities.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6119 2024-03-14 12:42:04.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/calculate.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9299 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/gas_phase.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3417 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/gas_phase.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4646 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/init_read_files.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3329 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/init_solver.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2582 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/molecule_struct.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1536 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/solver.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5488 2024-03-14 12:42:04.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/solver.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     2700 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/solver_bisection.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6824 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/solver_coeff.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3600 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/solver_linsol_quadsol.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5858 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/solver_nelder_mead_electron.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     9056 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/solver_newtsol.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5610 2024-03-14 12:42:04.000000 pyfastchem-3.1.1/fastchem_src/gas_phase/solver_newtsol_mult.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     1631 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/input_output_struct.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     4283 2024-03-14 12:42:04.000000 pyfastchem-3.1.1/fastchem_src/options.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3877 2024-03-14 12:42:04.000000 pyfastchem-3.1.1/fastchem_src/options.h
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5012 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/options_read_files.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     6185 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/fastchem_src/species_struct.h
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.719473 pyfastchem-3.1.1/pyfastchem.egg-info/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      255 2024-04-05 12:41:48.000000 pyfastchem-3.1.1/pyfastchem.egg-info/PKG-INFO
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)    15313 2024-04-05 12:41:48.000000 pyfastchem-3.1.1/pyfastchem.egg-info/SOURCES.txt
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)        1 2024-04-05 12:41:48.000000 pyfastchem-3.1.1/pyfastchem.egg-info/dependency_links.txt
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)       11 2024-04-05 12:41:48.000000 pyfastchem-3.1.1/pyfastchem.egg-info/top_level.txt
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)      120 2022-02-17 09:56:50.000000 pyfastchem-3.1.1/pyproject.toml
+drwxrwxr-x   0 kitzmann  (1000) kitzmann  (1000)        0 2024-04-05 12:41:48.719473 pyfastchem-3.1.1/python/
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     5284 2023-09-04 16:33:06.000000 pyfastchem-3.1.1/python/fastchem_python_wrapper.cpp
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)       38 2024-04-05 12:41:48.719473 pyfastchem-3.1.1/setup.cfg
+-rw-rw-r--   0 kitzmann  (1000) kitzmann  (1000)     3005 2024-04-05 12:41:19.000000 pyfastchem-3.1.1/setup.py
```

### Comparing `pyfastchem-3.1/README.md` & `pyfastchem-3.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 FastChem is an equilibrium chemistry code that calculates the chemical composition of the gas and condensed phase for given temperatures and pressures. The calculation of the gas phase is based on a semi-analytic approach, described in detail in Stock et al. (2018) and Stock et al. (2022). The new version 3 version of FastChem, called FastChem Cond, adds condensation to the code. It can now compute the chemical composition using equilibrium condensation or the rainout approximation that is commonly used in the field of exoplanets or brown dwarfs. FastChem Cond is described in detail in Kitzmann, Stock & Patzer (2023).
 
 The code is written in object-oriented C++, including template programming that allows the model to run with either double or long double precision. The exact computational precision of long double depends on your compiler and operating system. Long double precision usually allows the model to properly converge for very low temperatures. FastChem has been tested for temperatures as low as 100 K. For many cases, we were also able to obtain converged results for temperatures well below 100 K. Overall, the model has been successfully tested for temperatures from 100 K to 6000 K and pressures from 1e-13 bar to 1000 bar for solar element abundances.
 
 Besides the actual FastChem model, we provide a C++ stand-alone version in the *model_src* folder that allows to calculate the equilibrium chemistry for a given temperature-pressure structure. This stand-alone version can be adapted further to perform also more sophisticated calculations. In addition to the C++ stand-alone version, we also provide the Python interface PyFastChem.
 
-Version 3.1 includes updates to the calculation of the gas-phase chemistry. The new version will now switch to a multi-dimensional Newton's method for more complicated scenarios what were previously challenging to solve with the standard hierarchical approach of FastChem.
+Version 3.1 includes updates to the calculation of the gas-phase chemistry. The new version will now switch to a multi-dimensional Newton's method for more complicated scenarios that were previously challenging to solve with the standard hierarchical approach of FastChem.
 
 
 # PyFastChem #
 
 FastChem includes the Python interface, PyFastChem, that allows to run the C++ code as a normal Python module. PyFastChem is also available as a PyPy package and can easily be installed via pip. We provide several examples that show how to call FastChem from within a Python script, including the possibility to, for example, iterate over different metallicity values or C/O ratios or how to compute chemical compositions with condensation. The Python examples can be found in the *python* directory.
```

### Comparing `pyfastchem-3.1/_ext/Eigen/Cholesky` & `pyfastchem-3.1.1/_ext/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/CholmodSupport` & `pyfastchem-3.1.1/_ext/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/Core` & `pyfastchem-3.1.1/_ext/Eigen/Core`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/Eigenvalues` & `pyfastchem-3.1.1/_ext/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/Geometry` & `pyfastchem-3.1.1/_ext/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/Householder` & `pyfastchem-3.1.1/_ext/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/IterativeLinearSolvers` & `pyfastchem-3.1.1/_ext/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/Jacobi` & `pyfastchem-3.1.1/_ext/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/KLUSupport` & `pyfastchem-3.1.1/_ext/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/LU` & `pyfastchem-3.1.1/_ext/Eigen/LU`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/MetisSupport` & `pyfastchem-3.1.1/_ext/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/OrderingMethods` & `pyfastchem-3.1.1/_ext/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/PaStiXSupport` & `pyfastchem-3.1.1/_ext/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/PardisoSupport` & `pyfastchem-3.1.1/_ext/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/QR` & `pyfastchem-3.1.1/_ext/Eigen/QR`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/QtAlignedMalloc` & `pyfastchem-3.1.1/_ext/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/SPQRSupport` & `pyfastchem-3.1.1/_ext/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/SVD` & `pyfastchem-3.1.1/_ext/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/Sparse` & `pyfastchem-3.1.1/_ext/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/SparseCholesky` & `pyfastchem-3.1.1/_ext/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/SparseCore` & `pyfastchem-3.1.1/_ext/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/SparseLU` & `pyfastchem-3.1.1/_ext/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/SparseQR` & `pyfastchem-3.1.1/_ext/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/StdDeque` & `pyfastchem-3.1.1/_ext/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/StdList` & `pyfastchem-3.1.1/_ext/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/StdVector` & `pyfastchem-3.1.1/_ext/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/SuperLUSupport` & `pyfastchem-3.1.1/_ext/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/UmfPackSupport` & `pyfastchem-3.1.1/_ext/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Cholesky/LDLT.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Cholesky/LLT.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Cholesky/LLT_LAPACKE.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/CholmodSupport/CholmodSupport.h` & `pyfastchem-3.1.1/_ext/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/ArithmeticSequence.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Array.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/ArrayBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/ArrayWrapper.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Assign.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/AssignEvaluator.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Assign_MKL.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/BandMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Block.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/BooleanRedux.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/CommaInitializer.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/ConditionEstimator.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/CoreEvaluators.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/CoreIterators.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/CwiseBinaryOp.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/CwiseNullaryOp.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/CwiseTernaryOp.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/CwiseUnaryOp.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/CwiseUnaryView.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/DenseBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/DenseCoeffsBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/DenseStorage.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Diagonal.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/DiagonalMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/DiagonalProduct.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Dot.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/EigenBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/ForceAlignedAccess.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Fuzzy.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/GeneralProduct.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/GenericPacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/GlobalFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/IO.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/IndexedView.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Inverse.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Map.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/MapBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/MathFunctionsImpl.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Matrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/MatrixBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/NestByValue.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/NoAlias.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/NumTraits.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/PartialReduxEvaluator.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/PermutationMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/PlainObjectBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Product.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/ProductEvaluators.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Random.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Redux.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Ref.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Replicate.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Reshaped.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/ReturnByValue.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Reverse.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Select.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/SelfAdjointView.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/SelfCwiseBinaryOp.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Solve.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/SolveTriangular.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/SolverBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/StableNorm.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/StlIterators.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Stride.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Swap.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Transpose.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Transpositions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/TriangularMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/VectorBlock.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/VectorwiseOp.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/Visitor.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/Complex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX/TypeCasting.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/Complex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/Complex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/CUDA/Complex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/BFloat16.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/ConjHelper.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/Half.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/Settings.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/Default/TypeCasting.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/GPU/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/GPU/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/GPU/TypeCasting.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/MSA/Complex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/MSA/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/MSA/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/Complex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/NEON/TypeCasting.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/Complex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SSE/TypeCasting.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SVE/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SVE/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SVE/TypeCasting.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/ZVector/Complex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/arch/ZVector/PacketMath.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/functors/AssignmentFunctors.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/functors/BinaryFunctors.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/functors/NullaryFunctors.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/functors/StlFunctors.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/functors/TernaryFunctors.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/functors/UnaryFunctors.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixVector.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/Parallelizer.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointProduct.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/SelfadjointRank2Update.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularMatrixVector.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularSolverMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/products/TriangularSolverVector.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/BlasUtil.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/ConfigureVectorization.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/Constants.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/DisableStupidWarnings.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/ForwardDeclarations.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/IndexedViewHelper.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/IntegralConstant.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/MKL_support.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/Macros.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/Memory.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/Meta.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/ReenableStupidWarnings.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/ReshapedHelper.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/StaticAssert.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/SymbolicIndex.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Core/util/XprHelper.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/ComplexSchur.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/EigenSolver.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/RealQZ.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/RealSchur.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Eigenvalues/Tridiagonalization.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/AlignedBox.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/AngleAxis.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/EulerAngles.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/Homogeneous.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/Hyperplane.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/OrthoMethods.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/ParametrizedLine.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/Quaternion.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/Rotation2D.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/RotationBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/Scaling.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/Transform.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/Translation.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/Umeyama.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Householder/BlockHouseholder.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Householder/Householder.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Householder/HouseholderSequence.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `pyfastchem-3.1.1/_ext/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/Jacobi/Jacobi.h` & `pyfastchem-3.1.1/_ext/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/KLUSupport/KLUSupport.h` & `pyfastchem-3.1.1/_ext/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/LU/Determinant.h` & `pyfastchem-3.1.1/_ext/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/LU/FullPivLU.h` & `pyfastchem-3.1.1/_ext/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/LU/InverseImpl.h` & `pyfastchem-3.1.1/_ext/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/LU/PartialPivLU.h` & `pyfastchem-3.1.1/_ext/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `pyfastchem-3.1.1/_ext/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/LU/arch/InverseSize4.h` & `pyfastchem-3.1.1/_ext/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/MetisSupport/MetisSupport.h` & `pyfastchem-3.1.1/_ext/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/OrderingMethods/Amd.h` & `pyfastchem-3.1.1/_ext/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `pyfastchem-3.1.1/_ext/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/OrderingMethods/Ordering.h` & `pyfastchem-3.1.1/_ext/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `pyfastchem-3.1.1/_ext/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/PardisoSupport/PardisoSupport.h` & `pyfastchem-3.1.1/_ext/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/QR/ColPivHouseholderQR.h` & `pyfastchem-3.1.1/_ext/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `pyfastchem-3.1.1/_ext/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `pyfastchem-3.1.1/_ext/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/QR/FullPivHouseholderQR.h` & `pyfastchem-3.1.1/_ext/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/QR/HouseholderQR.h` & `pyfastchem-3.1.1/_ext/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `pyfastchem-3.1.1/_ext/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SVD/BDCSVD.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SVD/JacobiSVD.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SVD/SVDBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SVD/UpperBidiagonalization.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/AmbiVector.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/CompressedStorage.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/MappedSparseMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseAssign.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseBlock.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseColEtree.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseCompressedBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseDenseProduct.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseDot.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseFuzzy.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseMap.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseMatrixBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparsePermutation.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseProduct.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseRedux.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseRef.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseSolverBase.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseTranspose.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseTriangularView.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseUtil.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseVector.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/SparseView.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseCore/TriangularSolver.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLUImpl.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_Memory.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_Structs.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_Utils.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_pivotL.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_pruneL.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SparseQR/SparseQR.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/StlSupport/StdDeque.h` & `pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/StlSupport/StdList.h` & `pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/StlSupport/StdVector.h` & `pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/StlSupport/details.h` & `pyfastchem-3.1.1/_ext/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `pyfastchem-3.1.1/_ext/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `pyfastchem-3.1.1/_ext/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/misc/Image.h` & `pyfastchem-3.1.1/_ext/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/misc/Kernel.h` & `pyfastchem-3.1.1/_ext/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/misc/RealSvd2x2.h` & `pyfastchem-3.1.1/_ext/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/misc/blas.h` & `pyfastchem-3.1.1/_ext/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/misc/lapack.h` & `pyfastchem-3.1.1/_ext/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/misc/lapacke.h` & `pyfastchem-3.1.1/_ext/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/BlockMethods.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/IndexedViewMethods.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/_ext/Eigen/src/plugins/ReshapedMethods.h` & `pyfastchem-3.1.1/_ext/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/calc_densities.cpp` & `pyfastchem-3.1.1/fastchem_src/calc_densities.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 /*
 * This file is part of the FastChem code (https://github.com/exoclime/fastchem).
-* Copyright (C) 2024 Daniel Kitzmann, Joachim Stock
+* Copyright (C) 2022 Daniel Kitzmann, Joachim Stock
 *
 * FastChem is free software: you can redistribute it and/or modify
 * it under the terms of the GNU General Public License as published by
 * the Free Software Foundation, either version 3 of the License, or
 * (at your option) any later version.
 *
 * FastChem is distributed in the hope that it will be useful,
@@ -391,25 +391,21 @@
     i.maxDensity(element_data.elements, total_element_density);
   }
 
   std::vector<Condensate<double_type>*> condensates_act;
   std::vector<Element<double_type>*> elements_cond;
 
   condensed_phase.selectActiveCondensates(condensates_act, elements_cond);
-
-
-  //check for the phase rule
-  if (elements_cond.size() == element_data.elements_wo_e.size())
-    return FASTCHEM_PHASE_RULE_VIOLATION;
-
+  
 
   bool cond_converged = false;
   bool combined_converged = false;
 
   bool chem_backup_solver_default = options.chem_use_backup_solver;
+  size_t nb_condensed_elements = 0;
 
 
   if (condensates_act.size() > 0)
   {
     options.chem_use_backup_solver = true;
 
     std::vector<double_type> number_density_old(element_data.nb_elements, 0.0);
@@ -418,20 +414,14 @@
       number_density_old[i] = element_data.elements[i].number_density;
 
     //run the equilibrium condensation and gas phase iteration
     for (nb_combined_iter=0; nb_combined_iter<options.nb_chem_cond_iter; ++nb_combined_iter)
     {
       condensed_phase.selectActiveCondensates(condensates_act, elements_cond);
 
-
-      //check for the phase rule
-      if (elements_cond.size() == element_data.elements_wo_e.size())
-        return FASTCHEM_PHASE_RULE_VIOLATION;
-
-
       for (auto & i : condensates_act)
       {
         i->calcActivity(temperature, element_data.elements, options.cond_use_data_validity_limits);
         i->maxDensity(element_data.elements, total_element_density);
       }
 
       cond_converged = condensed_phase.calculate(
@@ -443,14 +433,31 @@
         gas_phase.molecules,
         nb_iter);
 
       nb_cond_iter += nb_iter;
 
       //gas_phase.reInitialise();
 
+      for (auto & e : element_data.elements)
+      {
+        bool is_condensed = false;
+
+        for (auto & c : e.condensate_list)
+        {
+          if (condensed_phase.condensates[c].log_activity > -0.01)
+          {
+            is_condensed = true;
+            break;
+          }
+        }
+        
+        if (!is_condensed)
+          e.fixed_by_condensation = false;
+      }
+
       fastchem_converged = gas_phase.calculate(
         temperature,
         gas_density,
         nb_iter);
    
       nb_chem_iter += nb_iter;
 
@@ -476,26 +483,32 @@
     //sanity check for the condensate activities
     for (auto & i : condensed_phase.condensates)
       if (i.log_activity > 0.001)
       { 
         cond_converged = false;
       }
 
-
     //remove condensates that are not present 
     //i.e. those with an activity smaller than 1
     for (auto & i : condensed_phase.condensates)
       if (i.log_activity < -0.01) i.number_density = 0.0;
     
     //and run the gas phase calculation one last time
     double_type phi_sum = 0;
+    nb_condensed_elements = 0;
 
     for (auto & i : element_data.elements)
     {
       i.calcDegreeOfCondensation(condensed_phase.condensates, total_element_density);
+      
+      if (i.degree_of_condensation == 0) 
+        i.fixed_by_condensation = false;
+      else
+        nb_condensed_elements++;
+
       phi_sum += i.phi;
     }
 
     for (auto & i : element_data.elements)
       i.normalisePhi(phi_sum);
 
     fastchem_converged = gas_phase.calculate(
@@ -555,14 +568,17 @@
 
 
   unsigned int return_state = FASTCHEM_SUCCESS;
 
   if (!fastchem_converged || !cond_converged || !combined_converged) 
     return_state = FASTCHEM_NO_CONVERGENCE;
 
+  //check for the phase rule
+  if (nb_condensed_elements == element_data.elements_wo_e.size())
+    return_state = FASTCHEM_PHASE_RULE_VIOLATION;
 
   return return_state;
 }
 
 
 
 template class FastChem<double>;
```

### Comparing `pyfastchem-3.1/fastchem_src/condensed_phase/calculate.cpp` & `pyfastchem-3.1.1/fastchem_src/condensed_phase/calculate.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/condensed_phase/condensate_struct.cpp` & `pyfastchem-3.1.1/fastchem_src/condensed_phase/condensate_struct.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/condensed_phase/condensed_phase.cpp` & `pyfastchem-3.1.1/fastchem_src/condensed_phase/condensed_phase.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,16 @@
       {
         elements_cond.push_back(&i);
         elements_cond.back()->fixed_by_condensation = true;
         break;
       }
   }
 
-
-  if (elements_cond.size() == element_data.elements_wo_e.size())
-    std::cout << "Phase rule violated! The number of condensing elements equals the total number of elements.\n";
+  for (auto & e : elements_cond)
+    e->fixed_by_condensation = true;
 }
 
 
 
 template <class double_type>
 void CondensedPhase<double_type>::selectJacobianCondensates(
   const std::vector<Condensate<double_type>*>& condensates_act,
```

### Comparing `pyfastchem-3.1/fastchem_src/condensed_phase/condensed_phase.h` & `pyfastchem-3.1.1/fastchem_src/condensed_phase/condensed_phase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/condensed_phase/read_condensate_data.cpp` & `pyfastchem-3.1.1/fastchem_src/condensed_phase/read_condensate_data.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/condensed_phase/solver.cpp` & `pyfastchem-3.1.1/fastchem_src/condensed_phase/solver.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/condensed_phase/solver.h` & `pyfastchem-3.1.1/fastchem_src/condensed_phase/solver.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/elements/chemical_element_data.h` & `pyfastchem-3.1.1/fastchem_src/elements/chemical_element_data.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/elements/element_struct.cpp` & `pyfastchem-3.1.1/fastchem_src/elements/element_struct.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/elements/elements.cpp` & `pyfastchem-3.1.1/fastchem_src/elements/elements.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/elements/elements.h` & `pyfastchem-3.1.1/fastchem_src/elements/elements.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/elements/read_files.cpp` & `pyfastchem-3.1.1/fastchem_src/elements/read_files.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/fastchem.cpp` & `pyfastchem-3.1.1/fastchem_src/fastchem.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/fastchem.h` & `pyfastchem-3.1.1/fastchem_src/fastchem.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/fastchem_constants.h` & `pyfastchem-3.1.1/fastchem_src/fastchem_constants.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/fastchem_get_set.cpp` & `pyfastchem-3.1.1/fastchem_src/fastchem_get_set.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/calc_electron_densities.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/calc_electron_densities.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/calc_mean_mol_weight.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/calc_mean_mol_weight.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/calc_species_densities.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/calc_species_densities.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/calculate.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/calculate.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/gas_phase.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/gas_phase.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/gas_phase.h` & `pyfastchem-3.1.1/fastchem_src/gas_phase/gas_phase.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/init_read_files.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/init_read_files.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/init_solver.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/init_solver.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/molecule_struct.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/molecule_struct.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/solver.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/solver.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/solver.h` & `pyfastchem-3.1.1/fastchem_src/gas_phase/solver.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/solver_bisection.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/solver_bisection.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/solver_coeff.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/solver_coeff.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/solver_linsol_quadsol.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/solver_linsol_quadsol.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/solver_nelder_mead_electron.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/solver_nelder_mead_electron.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/solver_newtsol.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/solver_newtsol.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/gas_phase/solver_newtsol_mult.cpp` & `pyfastchem-3.1.1/fastchem_src/gas_phase/solver_newtsol_mult.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/input_output_struct.h` & `pyfastchem-3.1.1/fastchem_src/input_output_struct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/options.cpp` & `pyfastchem-3.1.1/fastchem_src/options.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/options.h` & `pyfastchem-3.1.1/fastchem_src/options.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/options_read_files.cpp` & `pyfastchem-3.1.1/fastchem_src/options_read_files.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/fastchem_src/species_struct.h` & `pyfastchem-3.1.1/fastchem_src/species_struct.h`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/pyfastchem.egg-info/SOURCES.txt` & `pyfastchem-3.1.1/pyfastchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/python/fastchem_python_wrapper.cpp` & `pyfastchem-3.1.1/python/fastchem_python_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `pyfastchem-3.1/setup.py` & `pyfastchem-3.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tempfile
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from distutils.dir_util import mkpath
 from distutils.errors import CCompilerError
 from distutils import sysconfig
 
 
-__version__ = "3.1"
+__version__ = "3.1.1"
 
 
 #Custom build class that provides additional checks for OpenMP
 class custom_build_ext(build_ext):
   
   #Compile a test program to determine if C++ compiler supports OpenMP
   def check_openmp_support(self):
```

