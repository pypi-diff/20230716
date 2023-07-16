# Comparing `tmp/CMGDB-1.0.2.tar.gz` & `tmp/CMGDB-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CMGDB-1.0.2.tar", last modified: Sat Dec 31 01:59:33 2022, max compression
+gzip compressed data, was "CMGDB-1.0.3.tar", last modified: Sun Jul 16 03:05:55 2023, max compression
```

## Comparing `CMGDB-1.0.2.tar` & `CMGDB-1.0.3.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.675611 CMGDB-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2022-12-31 01:59:26.000000 CMGDB-1.0.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-31 01:59:26.000000 CMGDB-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2022-12-31 01:59:26.000000 CMGDB-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2022-12-31 01:59:33.679611 CMGDB-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2022-12-31 01:59:26.000000 CMGDB-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.663611 CMGDB-1.0.2/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.663611 CMGDB-1.0.2/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23979 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65660 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28251 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    52861 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    26498 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42613 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    31418 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79408 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126420 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    93883 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.667611 CMGDB-1.0.2/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.671611 CMGDB-1.0.2/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2022-12-31 01:59:29.000000 CMGDB-1.0.2/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-31 01:59:26.000000 CMGDB-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-31 01:59:33.679611 CMGDB-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3726 2022-12-31 01:59:26.000000 CMGDB-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.663611 CMGDB-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.671611 CMGDB-1.0.2/src/CMGDB/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1907 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/ComputeBoxMap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      303 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/LoadMorseSetFile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2459 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/PlotMorseGraph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5797 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/PlotMorseSets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      454 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/SaveMorseData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      218 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.671611 CMGDB-1.0.2/src/CMGDB/_cmgdb/
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/CMGDB.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.663611 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.675611 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Algebra.h
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/BitmapSubcomplex.h
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Chain.h
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Closure.h
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/ConleyIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/CoreductionDecomposer.h
--rw-r--r--   0 runner    (1001) docker     (123)    39775 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/CubicalComplex.h
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Decomposer.h
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/FiberComplex.h
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Field.h
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/FrobeniusNormalForm.h
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Generators.h
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11001 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/MorseComplex.h
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/PolyRing.h
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Preboundary.h
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Prism.h
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Real.h
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Rect.h
--rw-r--r--   0 runner    (1001) docker     (123)    19260 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/RelativeMapHomology.h
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/RelativePair.h
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Ring.h
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/SmithNormalForm.h
--rw-r--r--   0 runner    (1001) docker     (123)    47561 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/SparseMatrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.675611 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Atlas.h
--rw-r--r--   0 runner    (1001) docker     (123)      720 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/AtlasGeo.h
--rw-r--r--   0 runner    (1001) docker     (123)      648 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ChompMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/CompressedTree.h
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/CompressedTreeGrid.h
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Compute_Morse_Graph.h
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Compute_Morse_Graph.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Configuration.h
--rw-r--r--   0 runner    (1001) docker     (123)    14134 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/EdgeGrid.h
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/EuclideanParameterSpace.h
--rw-r--r--   0 runner    (1001) docker     (123)      641 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Geo.h
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/GraphTheory.h
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/GraphTheory.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Grid.h
--rw-r--r--   0 runner    (1001) docker     (123)      558 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/IntersectionGeo.h
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/MapGraph.h
--rw-r--r--   0 runner    (1001) docker     (123)    23837 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Model.h
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ModelMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ModelMapF.h
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ModelPointMapF.h
--rw-r--r--   0 runner    (1001) docker     (123)    14758 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/MorseGraph.h
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ParameterSpace.h
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/PointerGrid.h
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/PointerTree.h
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/PrismGeo.h
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/RankSelect.h
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Real.h
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/RectGeo.h
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/SingleOutput.h
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/SuccinctGrid.h
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/SuccinctTree.h
--rw-r--r--   0 runner    (1001) docker     (123)    20130 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    45701 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/TreeGrid.h
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/UniformGrid.h
--rw-r--r--   0 runner    (1001) docker     (123)      523 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/UnionGeo.h
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/conleyIndexString.h
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/join.h
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2022-12-31 01:59:26.000000 CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/simple_interval.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 01:59:33.671611 CMGDB-1.0.2/src/CMGDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2022-12-31 01:59:33.000000 CMGDB-1.0.2/src/CMGDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2022-12-31 01:59:33.000000 CMGDB-1.0.2/src/CMGDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 01:59:33.000000 CMGDB-1.0.2/src/CMGDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 01:59:33.000000 CMGDB-1.0.2/src/CMGDB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-31 01:59:33.000000 CMGDB-1.0.2/src/CMGDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-31 01:59:33.000000 CMGDB-1.0.2/src/CMGDB.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.893920 CMGDB-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-16 03:05:50.000000 CMGDB-1.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-16 03:05:50.000000 CMGDB-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-16 03:05:50.000000 CMGDB-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-16 03:05:55.893920 CMGDB-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-16 03:05:50.000000 CMGDB-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.881920 CMGDB-1.0.3/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.881920 CMGDB-1.0.3/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52861 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26498 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    93883 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.885920 CMGDB-1.0.3/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-07-16 03:05:51.000000 CMGDB-1.0.3/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-16 03:05:50.000000 CMGDB-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 03:05:55.893920 CMGDB-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3726 2023-07-16 03:05:50.000000 CMGDB-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.881920 CMGDB-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.889920 CMGDB-1.0.3/src/CMGDB/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1907 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/ComputeBoxMap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      303 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/LoadMorseSetFile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2459 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/PlotMorseGraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6411 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/PlotMorseSets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/SaveMorseData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      218 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.889920 CMGDB-1.0.3/src/CMGDB/_cmgdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/CMGDB.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.881920 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.889920 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Algebra.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/BitmapSubcomplex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Chain.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Closure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/ConleyIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/CoreductionDecomposer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39775 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/CubicalComplex.h
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Decomposer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/FiberComplex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Field.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/FrobeniusNormalForm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Generators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/MorseComplex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/PolyRing.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Preboundary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Prism.h
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Real.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Rect.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19260 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/RelativeMapHomology.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/RelativePair.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Ring.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/SmithNormalForm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47561 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/SparseMatrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.893920 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Atlas.h
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/AtlasGeo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ChompMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/CompressedTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/CompressedTreeGrid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Compute_Morse_Graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Compute_Morse_Graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Configuration.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14134 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/EdgeGrid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/EuclideanParameterSpace.h
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Geo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/GraphTheory.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/GraphTheory.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Grid.h
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/IntersectionGeo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/MapGraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ModelMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ModelMapF.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ModelPointMapF.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/MorseGraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ParameterSpace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/PointerGrid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/PointerTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/PrismGeo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/RankSelect.h
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Real.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/RectGeo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/SingleOutput.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/SuccinctGrid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/SuccinctTree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20130 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45701 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/TreeGrid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/UniformGrid.h
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/UnionGeo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/conleyIndexString.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/join.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-16 03:05:50.000000 CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/simple_interval.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:05:55.889920 CMGDB-1.0.3/src/CMGDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-16 03:05:55.000000 CMGDB-1.0.3/src/CMGDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-16 03:05:55.000000 CMGDB-1.0.3/src/CMGDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:05:55.000000 CMGDB-1.0.3/src/CMGDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:05:55.000000 CMGDB-1.0.3/src/CMGDB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-16 03:05:55.000000 CMGDB-1.0.3/src/CMGDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-16 03:05:55.000000 CMGDB-1.0.3/src/CMGDB.egg-info/top_level.txt
```

### Comparing `CMGDB-1.0.2/CMakeLists.txt` & `CMGDB-1.0.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/LICENSE` & `CMGDB-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/PKG-INFO` & `CMGDB-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMGDB
-Version: 1.0.2
+Version: 1.0.3
 Summary: CMGDB (Conley Morse Graph Database) Python Extension
 Home-page: https://github.com/marciogameiro/CMGDB
 Author: Marcio Gameiro
 Author-email: marciogameiro@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `CMGDB-1.0.2/README.md` & `CMGDB-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/attr.h` & `CMGDB-1.0.3/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/buffer_info.h` & `CMGDB-1.0.3/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/cast.h` & `CMGDB-1.0.3/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/chrono.h` & `CMGDB-1.0.3/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/complex.h` & `CMGDB-1.0.3/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/detail/class.h` & `CMGDB-1.0.3/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/detail/common.h` & `CMGDB-1.0.3/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/detail/descr.h` & `CMGDB-1.0.3/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/detail/init.h` & `CMGDB-1.0.3/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/detail/internals.h` & `CMGDB-1.0.3/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/detail/type_caster_base.h` & `CMGDB-1.0.3/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/detail/typeid.h` & `CMGDB-1.0.3/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/eigen/matrix.h` & `CMGDB-1.0.3/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/eigen/tensor.h` & `CMGDB-1.0.3/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/embed.h` & `CMGDB-1.0.3/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/eval.h` & `CMGDB-1.0.3/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/functional.h` & `CMGDB-1.0.3/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/gil.h` & `CMGDB-1.0.3/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/iostream.h` & `CMGDB-1.0.3/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/numpy.h` & `CMGDB-1.0.3/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/operators.h` & `CMGDB-1.0.3/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/options.h` & `CMGDB-1.0.3/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/pybind11.h` & `CMGDB-1.0.3/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/pytypes.h` & `CMGDB-1.0.3/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/stl/filesystem.h` & `CMGDB-1.0.3/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/stl.h` & `CMGDB-1.0.3/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/include/pybind11/stl_bind.h` & `CMGDB-1.0.3/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/test_cmake_build/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tests/test_embed/CMakeLists.txt` & `CMGDB-1.0.3/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tools/FindCatch.cmake` & `CMGDB-1.0.3/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tools/FindEigen3.cmake` & `CMGDB-1.0.3/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tools/FindPythonLibsNew.cmake` & `CMGDB-1.0.3/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tools/JoinPaths.cmake` & `CMGDB-1.0.3/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tools/pybind11Common.cmake` & `CMGDB-1.0.3/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tools/pybind11NewTools.cmake` & `CMGDB-1.0.3/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/pybind11/tools/pybind11Tools.cmake` & `CMGDB-1.0.3/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/setup.py` & `CMGDB-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 # Read the contents of README.md file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='CMGDB',
-    version='1.0.2',
+    version='1.0.3',
     author='Marcio Gameiro',
     author_email='marciogameiro@gmail.com',
     description='CMGDB (Conley Morse Graph Database) Python Extension',
     long_description=long_description,
     long_description_content_type='text/markdown',
     package_dir = {'': 'src'},
     ext_package='CMGDB',
```

### Comparing `CMGDB-1.0.2/src/CMGDB/ComputeBoxMap.py` & `CMGDB-1.0.3/src/CMGDB/ComputeBoxMap.py`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/PlotMorseGraph.py` & `CMGDB-1.0.3/src/CMGDB/PlotMorseGraph.py`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/PlotMorseSets.py` & `CMGDB-1.0.3/src/CMGDB/PlotMorseSets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # PlotMorseSets.py
 # Marcio Gameiro
 # MIT LICENSE
-# 2022-05-28
+# 2023-07-15
 
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 import CMGDB
 
-def PlotMorseSets(morse_sets, morse_nodes=None, proj_dims=None, cmap=None,
-                  clist=None, fig_w=8, fig_h=8, xlim=None, ylim=None):
+def PlotMorseSets(morse_sets, morse_nodes=None, proj_dims=None, cmap=None, clist=None,
+                  fig_w=8, fig_h=8, xlim=None, ylim=None, axis_labels=True,
+                  xlabel='$x$', ylabel='$y$', fontsize=15, fig_fname=None, dpi=300):
     # Check if morse_sets is a Morse graph, file name, or list
     if type(morse_sets) == CMGDB._cmgdb.MorseGraph: # Morse graph
         morse_graph = morse_sets
         num_morse_sets = morse_graph.num_vertices()
         if morse_nodes == None:
             morse_nodes = range(num_morse_sets)
         morse_sets = [box + [node] for node in morse_nodes for box in morse_graph.morse_set_boxes(node)]
@@ -21,19 +22,21 @@
         morse_fname = morse_sets
         morse_sets = CMGDB.LoadMorseSetFile(morse_fname)
         num_morse_sets = None
     else: # List of Morse sets
         num_morse_sets = None
     # Plot Morse set boxes as a scatter plot
     PlotBoxesScatter(morse_sets, num_morse_sets=num_morse_sets, morse_nodes=morse_nodes,
-                     proj_dims=proj_dims, cmap=cmap, clist=clist, fig_w=fig_w,
-                     fig_h=fig_h, xlim=xlim, ylim=ylim)
+                     proj_dims=proj_dims, cmap=cmap, clist=clist, fig_w=fig_w, fig_h=fig_h,
+                     xlim=xlim, ylim=ylim, axis_labels=axis_labels, xlabel=xlabel,
+                     ylabel=ylabel, fontsize=fontsize, fig_fname=fig_fname, dpi=dpi)
 
-def PlotBoxesScatter(morse_sets, num_morse_sets=None, morse_nodes=None, proj_dims=None,
-                     cmap=None, clist=None, fig_w=8, fig_h=8, xlim=None, ylim=None):
+def PlotBoxesScatter(morse_sets, num_morse_sets=None, morse_nodes=None, proj_dims=None, cmap=None,
+                     clist=None, fig_w=8, fig_h=8, xlim=None, ylim=None, axis_labels=True,
+                     xlabel='$x$', ylabel='$y$', fontsize=15, fig_fname=None, dpi=300):
     # Default colormap
     default_cmap = matplotlib.cm.brg
     rect = morse_sets[0]
     assert len(rect) % 2 == 1, "Wrong dimension in Morse sets data"
     dim = int((len(rect) - 1) / 2)
     if dim == 1:
         # Add extra fake dimension to plot
@@ -117,13 +120,21 @@
             # Alternative way to set marker size in data units
             # s_x = (x_scale * s[0]) ** 2 # Scatter x-axis size
             # s_y = (y_scale * s[1]) ** 2 # Scatter y-axis size
             X.append(p[0])
             Y.append(p[1])
             # Use max of both sizes
             S.append(max(s_x, s_y))
-        plt.scatter(X, Y, s=S, marker='s', c=clr)
-        # plt.scatter(X, Y, s=S, marker='s', c=clr, edgecolors=None)
-        # plt.scatter(X, Y, s=S, marker='s', c=clr, alpha=0.5)
+        ax.scatter(X, Y, s=S, marker='s', c=clr)
+        # ax.scatter(X, Y, s=S, marker='s', c=clr, edgecolors=None)
+        # ax.scatter(X, Y, s=S, marker='s', c=clr, alpha=0.5)
+    # Add axis labels
+    if axis_labels:
+        ax.set_xlabel(xlabel, fontsize=fontsize)
+        ax.set_ylabel(ylabel, fontsize=fontsize)
+    # Set tick labels size
+    ax.tick_params(labelsize=fontsize)
     # ax.set_aspect('equal')
     # plt.grid(True)
+    if fig_fname:
+        fig.savefig(fig_fname, dpi=dpi, bbox_inches='tight')
     plt.show()
```

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/CMGDB.cpp` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/CMGDB.cpp`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Algebra.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Algebra.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/BitmapSubcomplex.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/BitmapSubcomplex.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Chain.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Chain.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Closure.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Closure.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Complex.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Complex.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/ConleyIndex.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/ConleyIndex.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/CoreductionDecomposer.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/CoreductionDecomposer.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/CubicalComplex.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/CubicalComplex.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Decomposer.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Decomposer.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/FiberComplex.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/FiberComplex.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Field.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Field.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/FrobeniusNormalForm.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/FrobeniusNormalForm.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Generators.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Generators.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/LICENSE` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/LICENSE`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Matrix.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Matrix.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/MorseComplex.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/MorseComplex.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/PolyRing.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/PolyRing.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Preboundary.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Preboundary.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Prism.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Prism.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Rect.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Rect.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/RelativeMapHomology.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/RelativeMapHomology.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/RelativePair.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/RelativePair.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/Ring.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/Ring.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/SmithNormalForm.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/SmithNormalForm.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/chomp/SparseMatrix.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/chomp/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Atlas.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Atlas.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/AtlasGeo.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/AtlasGeo.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ChompMap.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ChompMap.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/CompressedTree.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/CompressedTree.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/CompressedTreeGrid.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/CompressedTreeGrid.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Compute_Morse_Graph.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Compute_Morse_Graph.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Compute_Morse_Graph.hpp` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Compute_Morse_Graph.hpp`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Configuration.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Configuration.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/EdgeGrid.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/EdgeGrid.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/EuclideanParameterSpace.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/EuclideanParameterSpace.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Geo.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Geo.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/GraphTheory.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/GraphTheory.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/GraphTheory.hpp` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/GraphTheory.hpp`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Grid.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Grid.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/IntersectionGeo.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/IntersectionGeo.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/MapGraph.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/MapGraph.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Model.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Model.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ModelMap.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ModelMap.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ModelMapF.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ModelMapF.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ModelPointMapF.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ModelPointMapF.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/MorseGraph.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/MorseGraph.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/ParameterSpace.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/ParameterSpace.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/PointerGrid.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/PointerGrid.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/PointerTree.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/PointerTree.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/PrismGeo.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/PrismGeo.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/RankSelect.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/RankSelect.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/RectGeo.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/RectGeo.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/SingleOutput.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/SingleOutput.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/SuccinctGrid.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/SuccinctGrid.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/SuccinctTree.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/SuccinctTree.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/Tree.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/Tree.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/TreeGrid.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/TreeGrid.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/UniformGrid.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/UniformGrid.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/UnionGeo.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/UnionGeo.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/conleyIndexString.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/conleyIndexString.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/join.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/join.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB/_cmgdb/include/database/simple_interval.h` & `CMGDB-1.0.3/src/CMGDB/_cmgdb/include/database/simple_interval.h`

 * *Files identical despite different names*

### Comparing `CMGDB-1.0.2/src/CMGDB.egg-info/PKG-INFO` & `CMGDB-1.0.3/src/CMGDB.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CMGDB
-Version: 1.0.2
+Version: 1.0.3
 Summary: CMGDB (Conley Morse Graph Database) Python Extension
 Home-page: https://github.com/marciogameiro/CMGDB
 Author: Marcio Gameiro
 Author-email: marciogameiro@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `CMGDB-1.0.2/src/CMGDB.egg-info/SOURCES.txt` & `CMGDB-1.0.3/src/CMGDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

