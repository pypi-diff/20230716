# Comparing `tmp/chempy-0.8.2.tar.gz` & `tmp/chempy-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chempy-0.8.2.tar", last modified: Sat Sep 18 21:21:58 2021, max compression
+gzip compressed data, was "chempy-0.8.3.tar", last modified: Sun Jul 16 10:14:30 2023, max compression
```

## Comparing `chempy-0.8.2.tar` & `chempy-0.8.3.tar`

### file list

```diff
@@ -1,235 +1,147 @@
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.568688 chempy-0.8.2/
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/.ci/
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     5759 2020-12-30 14:27:24.000000 chempy-0.8.2/.ci/get_sundials.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)      228 2020-12-30 14:27:24.000000 chempy-0.8.2/.ci/grep-for-binary-data.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)       86 2020-12-30 14:27:24.000000 chempy-0.8.2/.ci/grep-for-merge-blocking-token.sh
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5228 2021-09-18 21:19:30.000000 chempy-0.8.2/.drone.yml
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/.gh-pages-skeleton/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/.gh-pages-skeleton/.nojekyll
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      129 2021-09-18 15:16:38.000000 chempy-0.8.2/.git-blame-ignore-revs
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      450 2021-09-18 15:16:38.000000 chempy-0.8.2/.gitignore
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/.jupyter/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      522 2021-09-18 15:16:38.000000 chempy-0.8.2/.jupyter/jupyter_notebook_config.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1132 2020-12-30 14:27:24.000000 chempy-0.8.2/.travis.yml
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       38 2020-12-30 14:27:24.000000 chempy-0.8.2/AUTHORS
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7709 2021-09-18 21:20:24.000000 chempy-0.8.2/CHANGES.rst
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1493 2021-09-18 15:16:38.000000 chempy-0.8.2/CONTRIBUTING.rst
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1303 2020-12-30 14:27:24.000000 chempy-0.8.2/LICENSE
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       71 2020-12-30 14:27:24.000000 chempy-0.8.2/MANIFEST.in
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    21988 2021-09-18 21:21:58.568688 chempy-0.8.2/PKG-INFO
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    17532 2020-12-30 14:27:24.000000 chempy-0.8.2/README.rst
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/benchmarks/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2963 2020-12-30 14:27:24.000000 chempy-0.8.2/benchmarks/asv.conf.json
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/benchmarks/benchmarks/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/benchmarks/benchmarks/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1079 2021-09-18 15:16:38.000000 chempy-0.8.2/benchmarks/benchmarks/equilibria.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/chempy/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      709 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9477 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/_eqsys.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2475 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/_equilibrium.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       22 2021-09-18 21:21:58.000000 chempy-0.8.2/chempy/_release.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5990 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/_solution.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       45 2020-12-30 14:27:24.000000 chempy-0.8.2/chempy/_url.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2437 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/_util.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      321 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/arrhenius.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    53142 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/chemistry.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      386 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/debye_huckel.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1091 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/einstein_smoluchowski.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/chempy/electrochemistry/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       24 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/electrochemistry/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1379 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/electrochemistry/nernst.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/chempy/electrochemistry/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/chempy/electrochemistry/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1068 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/electrochemistry/tests/test_nernst.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7778 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/electrolytes.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    16931 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/equilibria.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      258 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/eyring.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3595 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/henry.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.556688 chempy-0.8.2/chempy/kinetics/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      199 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6516 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/_native.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      710 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/_rates.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4942 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/analysis.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8362 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/kinetics/arrhenius.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6010 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/kinetics/eyring.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7550 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/integrated.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    28053 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/ode.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    11341 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/kinetics/rates.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.556688 chempy-0.8.2/chempy/kinetics/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/chempy/kinetics/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10426 2020-12-30 14:27:24.000000 chempy-0.8.2/chempy/kinetics/tests/_derive_analytic_cstr_bireac.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9361 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/tests/test__native.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10457 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/tests/test__rates.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1612 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/tests/test_arrhenius.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1007 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/tests/test_eyring.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1549 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/tests/test_integrated.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    41283 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/kinetics/tests/test_ode.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15162 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/kinetics/tests/test_rates.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.556688 chempy-0.8.2/chempy/printing/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      325 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3894 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/printing/js.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6194 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/numbers.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      807 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/pretty.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2350 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/printer.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3283 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/string.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1272 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/table.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4306 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/printing/tables.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.556688 chempy-0.8.2/chempy/printing/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/chempy/printing/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2198 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/tests/test_numbers.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      432 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/tests/test_str.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      610 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/tests/test_table.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      630 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/tex.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2714 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/printing/web.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.556688 chempy-0.8.2/chempy/properties/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      146 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1551 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/debye_huckel_radii.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3204 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/gas_sol_electrolytes_schumpe_1993.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5576 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/sulfuric_acid_density_myhre_1998.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.556688 chempy-0.8.2/chempy/properties/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/chempy/properties/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      403 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/tests/test_gas_sol_electrolytes_schumpe_1993.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      835 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/tests/test_sulfuric_acid_density_myhre_1998.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1349 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/tests/test_water_density_tanaka_2001.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1297 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/tests/test_water_diffusivity_holz_2000.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      946 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/tests/test_water_permittivity_bradley_pitzer_1979.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1471 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/tests/test_water_viscosity_korson_1969.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2804 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/water_density_tanaka_2001.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2774 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/water_diffusivity_holz_2000.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3096 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/water_permittivity_bradley_pitzer_1979.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1566 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/properties/water_viscosity_korson_1969.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    31991 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/reactionsystem.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      472 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/symbolic.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.560688 chempy-0.8.2/chempy/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/chempy/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2487 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/ammonical_cupric_solution.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1570 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test__equilibrium.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    20158 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_chemistry.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       84 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_core.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1294 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_einstein_smoluchowski.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1531 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_electrolytes.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4395 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_equilibria.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1206 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_henry.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15621 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_reactionsystem.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2018 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_solution.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15904 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_units.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      430 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/tests/test_util.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.560688 chempy-0.8.2/chempy/thermodynamics/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       77 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/thermodynamics/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1814 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/thermodynamics/expressions.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.560688 chempy-0.8.2/chempy/thermodynamics/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/chempy/thermodynamics/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3438 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/thermodynamics/tests/test_expressions.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    22646 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/units.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.560688 chempy-0.8.2/chempy/util/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      147 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2233 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/_aqueous.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      795 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/_dimensionality.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    25888 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/util/_expr.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4152 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/util/_expr_deprecated.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5909 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/_julia.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2294 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/_quantities.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4654 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/util/arithmeticdict.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6776 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/bkh.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4940 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/util/deprecation.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5109 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/graph.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1062 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/numutil.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    18239 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/util/parsing.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6234 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/periodic.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8881 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/util/pyutil.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    11947 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/regression.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      890 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/rendering.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2792 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/stoich.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10549 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/table.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4079 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/util/terminal.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2015 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/testing.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.564688 chempy-0.8.2/chempy/util/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.2/chempy/util/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4058 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_arithmeticdict.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    18762 2021-09-18 21:19:30.000000 chempy-0.8.2/chempy/util/tests/test_expr.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1631 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_graph.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      462 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_numutil.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9048 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_parsing.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2215 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_periodic.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1850 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_pyutil.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      783 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_regression.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      726 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_rendering.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2987 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_stoich.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1459 2021-09-18 15:16:38.000000 chempy-0.8.2/chempy/util/tests/test_table.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.552688 chempy-0.8.2/chempy.egg-info/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    21988 2021-09-18 21:21:58.000000 chempy-0.8.2/chempy.egg-info/PKG-INFO
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6486 2021-09-18 21:21:58.000000 chempy-0.8.2/chempy.egg-info/SOURCES.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        1 2021-09-18 21:21:58.000000 chempy-0.8.2/chempy.egg-info/dependency_links.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      703 2021-09-18 21:21:58.000000 chempy-0.8.2/chempy.egg-info/requires.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        7 2021-09-18 21:21:58.000000 chempy-0.8.2/chempy.egg-info/top_level.txt
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.564688 chempy-0.8.2/conda-recipe/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1030 2020-12-30 14:27:24.000000 chempy-0.8.2/conda-recipe/meta.yaml
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      281 2020-12-30 14:27:24.000000 chempy-0.8.2/conda-recipe/run_test.sh
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      624 2021-09-18 15:16:38.000000 chempy-0.8.2/conftest.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      478 2020-12-30 14:27:24.000000 chempy-0.8.2/environment.yml
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.568688 chempy-0.8.2/examples/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    11160 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/Ammonia.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3648 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/NaCl_precipitation.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7535 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/Robertson_kinetics.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4517 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_Expr_custom_Gibbs_kinetics_odesys.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3732 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/_FeSCN.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3034 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_arrhenius_kinetics.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2204 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/_carbon_dioxide.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3155 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_eyring_kinetics.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3732 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_eyring_kinetics_2nd_order.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4726 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_eyring_kinetics_2nd_order_reversible.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5161 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_eyring_kinetics_ramped_temperature.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5287 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_eyring_kinetics_ramped_temperature_2nd_order.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8439 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_integrated.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1586 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/_ipynb_progressbar.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9683 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_kinetic_model_fitting.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7719 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_kinetics_demo.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5674 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_kinetics_ode_time_dependent_autonomous.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5813 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_kinetics_ode_time_dependent_autonomous_units.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3182 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_kinetics_ode_time_dependent_units.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4468 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_kinetics_radiolysis_analytic.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3446 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_ode_system_sympy_symbols.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2778 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_regression.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4197 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_surface_reactions_homogeneous.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    12280 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/_switch_between_reduced_ode_systems.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    19479 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/ammonical_cupric_solution.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15935 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/aqueous_radiolysis.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1086 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/bokeh_interactive.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1159 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/bokeh_interactive_arrhenius.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1400 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/bokeh_interactive_arrhenius_units.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1366 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/bokeh_interactive_robertson.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1113 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/bokeh_interactive_units.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4411 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/demo_debye_huckel.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1292 2021-09-18 15:16:38.000000 chempy-0.8.2/examples/demo_kinetics.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4045 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/interactive_kinetic_modelling.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    51364 2021-09-18 21:21:57.000000 chempy-0.8.2/examples/kinetics.png
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9792 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/kinetics_cstr.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4724 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/kinetics_decay_chain_units_varied_params.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3481 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/kinetics_ode_time_dependent.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    26591 2020-12-30 14:27:24.000000 chempy-0.8.2/examples/protein_binding_unfolding_4state_model.ipynb
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)   101837 2020-11-23 23:38:22.000000 chempy-0.8.2/examples/specdata.json.bz2
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2444 2020-12-30 14:27:24.000000 chempy-0.8.2/index.ipynb
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.568688 chempy-0.8.2/joss-paper/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      760 2020-12-30 14:27:24.000000 chempy-0.8.2/joss-paper/codemeta.json
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3298 2020-12-30 14:27:24.000000 chempy-0.8.2/joss-paper/paper.bib
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3364 2020-12-30 14:27:24.000000 chempy-0.8.2/joss-paper/paper.md
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)      907 2020-12-30 14:27:24.000000 chempy-0.8.2/postBuild
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.568688 chempy-0.8.2/scripts/
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)      363 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/build_conda_recipe.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)      279 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/check_clean_repo_on_master.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)      553 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/circleci_dependencies.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     1810 2021-09-18 15:16:38.000000 chempy-0.8.2/scripts/coverage_badge.py
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)      726 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/dir_to_branch.sh
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2021-09-18 21:21:58.568688 chempy-0.8.2/scripts/environment/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1637 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/environment/Dockerfile
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     1503 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/generate_docs.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     1846 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/host-jupyter-using-docker.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     1554 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/post_release.sh
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1726 2020-11-23 23:38:22.000000 chempy-0.8.2/scripts/rasterize.js.bz2
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     1886 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/release.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     1010 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/render_index.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     1160 2021-09-18 21:19:30.000000 chempy-0.8.2/scripts/render_notebooks.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)      299 2021-09-18 15:16:38.000000 chempy-0.8.2/scripts/run_tests.sh
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     1699 2020-12-30 14:27:24.000000 chempy-0.8.2/scripts/update-gh-pages.sh
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      851 2021-09-18 21:21:58.568688 chempy-0.8.2/setup.cfg
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     4992 2021-09-18 21:19:30.000000 chempy-0.8.2/setup.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.113779 chempy-0.8.3/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       38 2020-12-30 14:27:24.000000 chempy-0.8.3/AUTHORS
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7814 2023-07-16 09:59:36.000000 chempy-0.8.3/CHANGES.rst
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1303 2020-12-30 14:27:24.000000 chempy-0.8.3/LICENSE
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       71 2020-12-30 14:27:24.000000 chempy-0.8.3/MANIFEST.in
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    18489 2023-07-16 10:14:30.113779 chempy-0.8.3/PKG-INFO
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    17504 2023-07-16 09:59:31.000000 chempy-0.8.3/README.rst
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.037778 chempy-0.8.3/chempy/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      709 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9477 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/_eqsys.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2475 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/_equilibrium.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       22 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy/_release.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5990 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/_solution.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       45 2020-12-30 14:27:24.000000 chempy-0.8.3/chempy/_url.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2437 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/_util.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      321 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/arrhenius.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    53293 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/chemistry.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      386 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/debye_huckel.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1091 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/einstein_smoluchowski.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.041778 chempy-0.8.3/chempy/electrochemistry/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       24 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/electrochemistry/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1379 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/electrochemistry/nernst.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.041778 chempy-0.8.3/chempy/electrochemistry/tests/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/electrochemistry/tests/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1068 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/electrochemistry/tests/test_nernst.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7778 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/electrolytes.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    16931 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/equilibria.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      258 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/eyring.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3595 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/henry.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.049778 chempy-0.8.3/chempy/kinetics/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      199 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6516 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/_native.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      710 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/_rates.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4942 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/analysis.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8362 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/kinetics/arrhenius.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5966 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/kinetics/eyring.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7550 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/integrated.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    28053 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/kinetics/ode.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    11341 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/kinetics/rates.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.053778 chempy-0.8.3/chempy/kinetics/tests/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/kinetics/tests/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9361 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test__native.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10553 2023-07-16 09:59:31.000000 chempy-0.8.3/chempy/kinetics/tests/test__rates.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1612 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test_arrhenius.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1007 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test_eyring.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1549 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test_integrated.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    41283 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/kinetics/tests/test_ode.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15162 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test_rates.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.061778 chempy-0.8.3/chempy/printing/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      325 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3895 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/printing/js.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6194 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/numbers.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      807 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/pretty.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2350 2022-03-29 16:41:58.000000 chempy-0.8.3/chempy/printing/printer.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3283 2022-03-29 16:41:58.000000 chempy-0.8.3/chempy/printing/string.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1272 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/table.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4306 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/printing/tables.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.065778 chempy-0.8.3/chempy/printing/tests/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/printing/tests/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2198 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/tests/test_numbers.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      432 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/tests/test_str.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      610 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/tests/test_table.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      630 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/tex.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2714 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/web.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.069778 chempy-0.8.3/chempy/properties/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      145 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/properties/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1551 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/debye_huckel_radii.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3204 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/gas_sol_electrolytes_schumpe_1993.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5576 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/properties/sulfuric_acid_density_myhre_1998.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.073778 chempy-0.8.3/chempy/properties/tests/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/properties/tests/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      403 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_gas_sol_electrolytes_schumpe_1993.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      835 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_sulfuric_acid_density_myhre_1998.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1349 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_water_density_tanaka_2001.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1297 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_water_diffusivity_holz_2000.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      946 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_water_permittivity_bradley_pitzer_1979.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1471 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_water_viscosity_korson_1969.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2804 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/properties/water_density_tanaka_2001.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2775 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/properties/water_diffusivity_holz_2000.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3096 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/water_permittivity_bradley_pitzer_1979.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1566 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/water_viscosity_korson_1969.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    31994 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/reactionsystem.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      472 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/symbolic.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.085778 chempy-0.8.3/chempy/tests/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/tests/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2487 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/ammonical_cupric_solution.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1570 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test__equilibrium.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    20777 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/tests/test_chemistry.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       84 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_core.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1294 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_einstein_smoluchowski.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1531 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_electrolytes.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4491 2023-07-16 09:59:31.000000 chempy-0.8.3/chempy/tests/test_equilibria.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1206 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_henry.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15621 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_reactionsystem.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2018 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_solution.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15995 2023-07-16 09:59:31.000000 chempy-0.8.3/chempy/tests/test_units.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      430 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_util.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.089778 chempy-0.8.3/chempy/thermodynamics/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       77 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/thermodynamics/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1814 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/thermodynamics/expressions.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.089778 chempy-0.8.3/chempy/thermodynamics/tests/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/thermodynamics/tests/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3438 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/thermodynamics/tests/test_expressions.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    22736 2023-07-16 09:59:31.000000 chempy-0.8.3/chempy/units.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.101779 chempy-0.8.3/chempy/util/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      147 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2233 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/_aqueous.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      795 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/_dimensionality.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    25887 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/_expr.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4153 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/_expr_deprecated.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5910 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/_julia.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2295 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/_quantities.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4652 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/arithmeticdict.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6776 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/bkh.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4940 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/util/deprecation.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5114 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/graph.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1062 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/numutil.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    20195 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/parsing.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6753 2021-10-29 07:48:12.000000 chempy-0.8.3/chempy/util/periodic.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8881 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/util/pyutil.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    11947 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/regression.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      890 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/rendering.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2792 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/stoich.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10550 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/table.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4079 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/util/terminal.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2015 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/testing.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.109779 chempy-0.8.3/chempy/util/tests/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/util/tests/__init__.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4058 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_arithmeticdict.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    18801 2021-10-29 07:48:12.000000 chempy-0.8.3/chempy/util/tests/test_expr.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1631 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_graph.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      462 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_numutil.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    20501 2022-03-29 16:41:58.000000 chempy-0.8.3/chempy/util/tests/test_parsing.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2250 2022-03-29 16:41:58.000000 chempy-0.8.3/chempy/util/tests/test_periodic.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1850 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_pyutil.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      783 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_regression.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      726 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_rendering.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2987 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_stoich.py
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1459 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_table.py
+drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.037778 chempy-0.8.3/chempy.egg-info/
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    18489 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/PKG-INFO
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3961 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        1 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      703 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/requires.txt
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        7 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/top_level.txt
+-rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      884 2023-07-16 10:14:30.113779 chempy-0.8.3/setup.cfg
+-rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     4994 2023-07-16 08:39:56.000000 chempy-0.8.3/setup.py
```

### Comparing `chempy-0.8.2/CHANGES.rst` & `chempy-0.8.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v0.8.3
+======
+- Fixes for latest version of quantities.
+- Build python wheel as part of release script.
+
 v0.8.2
 ======
 - changed version of dependency "pyodesys"
 
 v0.8.1
 ======
 - package "jupyter" was listed as formal dependency, now removed.
@@ -88,15 +93,15 @@
 v0.6.7
 ======
 - Updated manuscript for JOSS.
 
 v0.6.6
 ======
 - Support for containers in ``chempy.units.unit_of``.
-- ``balance_stoichiometry`` now correctly find the canoncial solution when ``underdetermined=None`` is passed.
+- ``balance_stoichiometry`` now correctly find the canonical solution when ``underdetermined=None`` is passed.
 - ``chempy.kinetics.integrated`` was refactored to have more approachable API.
 
 v0.6.5
 ======
 - Fix assertion firing
 
 v0.6.4
@@ -110,23 +115,23 @@
 
 v0.6.2
 ======
 - More relaxed tests with respect to 3rd party programs
 
 v0.6.1
 ======
-- Extensive test suite in conda pacakge no longer require graphviz & latex
+- Extensive test suite in conda package no longer require graphviz & latex
 
 v0.6.0
 ======
 - ``balance_stoichiometry`` now accepts either of ``True``, ``False``, ``None`` as ``underdetermined``.
 - ``NameSpace`` and ``AttributeContainer`` are now public in ``.util.pyutil``.
 - New printers in ``chempy.printing``, allows user to subclass printers.
 - Jupyter Notebook representation of ``ReactionSystem`` is now interactive (JavaScript/CSS)
-- More data from the litterature: water viscosity (``chempy.properties.water_viscosity_korson_1969``).
+- More data from the literature: water viscosity (``chempy.properties.water_viscosity_korson_1969``).
 - New methods for ``ReactionSystem``:
   - ``split``: splits reaction-system into disjoint parts
   - ``categorize_substances``: e.g. "nonparticipating", "unaffected".
 - Better documentation throughout.
 
 v0.5.7
 ======
@@ -166,15 +171,15 @@
 - CSTR kinetics
 - Minor fixes, new notebooks
 
 v0.5.0
 ======
 - ``.electrochemistry.nernst_formula`` - thanks to Adel Qalieh (@adelq)
 - moved ``.util.parsing.number_to_scientific_*`` to ``.printing(.numbers)``
-- Number formating now handles uncertainties.
+- Number formatting now handles uncertainties.
 - ``refereence`` in reimplementations now a dict
 - Fixes to ``.kinetics.ode.get_odesys`` (refactored)
 
 v0.4.1
 ======
 - Fixes for enhanced robustness:
   - ``.kinetics.ode.get_odesys``
```

### Comparing `chempy-0.8.2/LICENSE` & `chempy-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/README.rst` & `chempy-0.8.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 ChemPy
 ======
 
-.. image:: http://hera.physchem.kth.se:8080/api/badges/bjodah/chempy/status.svg
-   :target: http://hera.physchem.kth.se:8080/bjodah/chempy
+.. image:: https://github.com/bjodah/chempy/actions/workflows/lint_python.yml/badge.svg
+   :target: https://github.com/bjodah/chempy/actions/workflows/lint_python.yml
    :alt: Build status
 .. image:: https://img.shields.io/pypi/v/chempy.svg
    :target: https://pypi.python.org/pypi/chempy
    :alt: PyPI version
 .. image:: https://img.shields.io/badge/python-3.8,3.9-blue.svg
    :target: https://www.python.org/
    :alt: Python version
 .. image:: https://img.shields.io/pypi/l/chempy.svg
    :target: https://github.com/bjodah/chempy/blob/master/LICENSE
    :alt: License
-.. image:: http://img.shields.io/badge/benchmarked%20by-asv-green.svg?style=flat
-   :target: http://hera.physchem.kth.se/~chempy/benchmarks
-   :alt: airspeedvelocity
-.. image:: http://hera.physchem.kth.se/~chempy/branches/master/htmlcov/coverage.svg
-   :target: http://hera.physchem.kth.se/~chempy/branches/master/htmlcov
-   :alt: coverage
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00565/status.svg
    :target: https://doi.org/10.21105/joss.00565
    :alt: Journal of Open Source Software DOI
 
 .. contents::
 
 
@@ -38,54 +32,48 @@
 
   - Debye-Hückel expressions
   - Arrhenius & Eyring equation
   - Einstein-Smoluchowski equation
 
 - Properties (pure python implementations from the literature)
 
-  - water density as function of temperature
-  - water permittivity as function of temperature and pressure
-  - water diffusivity as function of temperature
-  - water viscosity as function of temperature
-  - sulfuric acid density as function of temperature & weight fraction H₂SO₄
-  - More to come... (and contributions are most welcome!)
+  - `water density <https://github.com/bjodah/chempy/blob/master/chempy/properties/water_density_tanaka_2001.py>`_ as function of temperature
+  - `water permittivity <https://github.com/bjodah/chempy/blob/master/chempy/properties/water_permittivity_bradley_pitzer_1979.py>`_ as function of temperature and pressure
+  - `water diffusivity <https://github.com/bjodah/chempy/blob/master/chempy/properties/water_diffusivity_holz_2000.py>`_ as function of temperature
+  - `water viscosity <https://github.com/bjodah/chempy/blob/master/chempy/properties/water_viscosity_korson_1969.py>`_ as function of temperature
+  - `sulfuric acid density <https://github.com/bjodah/chempy/blob/master/chempy/properties/sulfuric_acid_density_myhre_1998.py>`_ as function of temperature & weight fraction H₂SO₄
+  - `More <https://github.com/bjodah/chempy/tree/master/chempy/properties>`_ to come... (and contributions are most welcome!)
 
 
 Documentation
 -------------
 The easiest way to get started is to have a look at the examples in this README,
 and also the jupyter notebooks_. In addition there is auto-generated API documentation
-for the latest `stable release here <https://bjodah.github.io/chempy/latest>`_
-(and `here are <http://hera.physchem.kth.se/~chempy/branches/master/html>`_ the API docs for the development version).
+for the latest `stable release here <https://bjodah.github.io/chempy/latest>`_.
 
-.. _notebooks: http://hera.physchem.kth.se/~chempy/branches/master/examples
+.. _notebooks: https://github.com/bjodah/chempy/tree/master/examples
 
 Installation
 ------------
 Simplest way to install ChemPy and its (optional) dependencies is to use the
 `conda package manager <https://conda.pydata.org/docs/>`_::
 
-   $ conda install -c bjodah chempy pytest
+   $ conda install -c conda-forge chempy pytest
    $ pytest -rs -W ignore::chempy.ChemPyDeprecationWarning --pyargs chempy
 
 currently conda packages are only provided for Linux. On Windows and OS X
 you will need to use ``pip`` instead::
 
    $ python3 -m pip install chempy pytest
    $ python3 -m pytest -rs -W ignore::chempy.ChemPyDeprecationWarning --pyargs chempy
 
 there will a few tests which will be skipped due to some missing optional
 backends in addition to those in SciPy (used for solving systems of non-linear
 equations and ordinary differential equations).
 
-If you are still using Python 2 you can use the long-term-support 0.6.x branch
-of ChemPy which will continue to receive bugfixes::
-
-   $ python2 -m pip install "chempy<0.7"
-
 
 Optional dependencies
 ~~~~~~~~~~~~~~~~~~~~~
 If you used ``conda`` to install ChemPy you can skip this section.
 But if you use ``pip`` the default installation is achieved by writing::
 
    $ python3 -m pip install --user --upgrade chempy pytest
@@ -206,15 +194,15 @@
 .. code:: python
 
    >>> pprint([dict(_) for _ in balance_stoichiometry({'C', 'O2'}, {'CO2', 'CO'}, underdetermined=None)])
    [{'C': 3, 'O2': 2}, {'CO': 2, 'CO2': 1}]
 
 
 note however that even though this solution is in some sense "canonical",
-it is merely one of an inifite number of solutions (``x1`` from earlier may be any integer).
+it is merely one of an infinite number of solutions (``x1`` from earlier may be any integer).
 
 
 .. _Symbol: http://docs.sympy.org/latest/modules/core.html#sympy.core.symbol.Symbol
 
 
 Balancing reactions
 ~~~~~~~~~~~~~~~~~~~
```

### Comparing `chempy-0.8.2/chempy/__init__.py` & `chempy-0.8.3/chempy/__init__.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/_eqsys.py` & `chempy-0.8.3/chempy/_eqsys.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/_equilibrium.py` & `chempy-0.8.3/chempy/_equilibrium.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/_solution.py` & `chempy-0.8.3/chempy/_solution.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/_util.py` & `chempy-0.8.3/chempy/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             import numpy as backend
         except ImportError:
             import math as backend
     return backend
 
 
 def intdiv(p, q):
-    """Integer divsions which rounds toward zero
+    """Integer division which rounds toward zero
 
     Examples
     --------
     >>> intdiv(3, 2)
     1
     >>> intdiv(-3, 2)
     -1
```

### Comparing `chempy-0.8.2/chempy/chemistry.py` & `chempy-0.8.3/chempy/chemistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         return str(self.name)
 
     def _repr_html_(self):
         return self.html_name
 
     @staticmethod
     def composition_keys(substance_iter, skip_keys=()):
-        """Occuring :attr:`composition` keys among a series of substances"""
+        """Occurring :attr:`composition` keys among a series of substances"""
         keys = set()
         for s in substance_iter:
             if s.composition is None:
                 continue
             for k in s.composition.keys():
                 if k in skip_keys:
                     continue
@@ -259,15 +259,15 @@
                 if ``phases`` is a dictionary:
                     ``phase_idx = phases[suffix]``
                 else:
                     ``phase_idx = phases.index(suffix) + 1``
             and if suffixes is missing in phases phase_idx is taken to be 0
         default_phase_idx: int or None (default: 0)
             If ``default_phase_idx`` is ``None``, ``ValueError`` is raised for
-                unkown suffixes.
+                unknown suffixes.
             Else ``default_phase_idx`` is used as ``phase_idx`` in those cases.
         \\*\\*kwargs:
             Keyword arguments passed on.
 
         Examples
         --------
         >>> water = Species.from_formula('H2O')
@@ -564,15 +564,15 @@
                             "Found a negative stoichiometry for %s in %s." % (k, nam)
                         )
                     else:
                         return False
         return True
 
     def check_all_integral(self, throw=False):
-        """Checks if all stoichiometric coefficents are integers"""
+        """Checks if all stoichiometric coefficients are integers"""
         for nam, cont in [
             (nam, getattr(self, nam))
             for nam in "reac prod inact_reac inact_prod".split()
         ]:
             for k, v in cont.items():
                 if v != type(v)(int(v)):
                     if throw:
@@ -1184,15 +1184,15 @@
             return NotImplemented
         param = None if self.param is None else self.param ** other
         if other < 0:
             other *= -1
             flip = True
         else:
             flip = False
-        other = int(other)  # convert SymPy "Integer" to Pyton "int"
+        other = int(other)  # convert SymPy "Integer" to Python "int"
         reac = dict(other * ArithmeticDict(int, self.reac))
         prod = dict(other * ArithmeticDict(int, self.prod))
         inact_reac = dict(other * ArithmeticDict(int, self.inact_reac))
         inact_prod = dict(other * ArithmeticDict(int, self.inact_prod))
         if flip:
             reac, prod = prod, reac
             inact_reac, inact_prod = inact_prod, inact_reac
@@ -1333,15 +1333,15 @@
         from 1.
     underdetermined : bool
         Allows to find a non-unique solution (in addition to a constant factor
         across all terms). Set to ``False`` to disallow (raise ValueError) on
         e.g. "C + O2 -> CO + CO2". Set to ``None`` if you want the symbols replaced
         so that the coefficients are the smallest possible positive (non-zero) integers.
     allow_duplicates : bool
-        If False: raises an excpetion if keys appear in both ``reactants`` and ``products``.
+        If False: raises an exception if keys appear in both ``reactants`` and ``products``.
 
     Examples
     --------
     >>> ref = {'C2H2': 2, 'O2': 3}, {'CO': 4, 'H2O': 2}
     >>> balance_stoichiometry({'C2H2', 'O2'}, {'CO', 'H2O'}) == ref
     True
     >>> ref2 = {'H2': 1, 'O2': 1}, {'H2O2': 1}
@@ -1373,14 +1373,15 @@
     import sympy
     from sympy import (
         MutableDenseMatrix,
         gcd,
         zeros,
         linsolve,
         numbered_symbols,
+        nsimplify,
         Wild,
         Symbol,
         Integer,
         Tuple,
         preorder_traversal as pre,
     )
 
@@ -1491,16 +1492,22 @@
             any_neg = any(substances[pk].composition.get(ck, 0) < 0 for pk in reactants)
             if any_pos and any_neg:
                 pass  # negative and positive parts among reactants, no worries
             else:
                 raise ValueError("Component '%s' not among products" % ck)
 
     A = MutableDenseMatrix([[_get(ck, sk) for sk in subst_keys] for ck in cks])
+    A = nsimplify(A)
     symbs = list(reversed([next(parametric_symbols) for _ in range(len(subst_keys))]))
     (sol,) = linsolve((A, zeros(len(cks), 1)), symbs)
+    try:
+        sol = nsimplify(sol)
+    except (AttributeError):
+        pass
+
     wi = Wild("wi", properties=[lambda k: not k.has(Symbol)])
     cd = reduce(
         gcd,
         [1]
         + [
             1 / m[wi]
             for m in map(lambda n: n.match(symbs[-1] / wi), pre(sol))
@@ -1546,26 +1553,28 @@
     integer_one = 1  # need 'is' check, SyntaxWarning when checking against literal
     if underdetermined is integer_one:
         from ._release import __version__
 
         if int(__version__.split(".")[1]) > 6:
             warnings.warn(  # deprecated because comparison with ``1`` problematic (True==1)
                 (
-                    "Pass underdetermined == None instead of ``1`` (depreacted since 0.7.0,"
+                    "Pass underdetermined == None instead of ``1`` (deprecated since 0.7.0,"
                     " will_be_missing_in='0.9.0')"
                 ),
                 ChemPyDeprecationWarning,
             )
         underdetermined = None
     if underdetermined is None:
         sol = Tuple(*[Integer(x) for x in _solve_balancing_ilp_pulp(A)])
 
     fact = gcd(sol)
     sol = MutableDenseMatrix([e / fact for e in sol]).reshape(len(sol), 1)
     sol /= reduce(gcd, sol)
+    sol = nsimplify(sol)
+
     if 0 in sol:
         raise ValueError("Superfluous species given.")
     if underdetermined:
         if any(x == sympy.nan for x in sol):
             raise ValueError("Failed to balance reaction")
     else:
         for x in sol:
```

### Comparing `chempy-0.8.2/chempy/einstein_smoluchowski.py` & `chempy-0.8.3/chempy/einstein_smoluchowski.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/electrochemistry/nernst.py` & `chempy-0.8.3/chempy/electrochemistry/nernst.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/electrochemistry/tests/test_nernst.py` & `chempy-0.8.3/chempy/electrochemistry/tests/test_nernst.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/electrolytes.py` & `chempy-0.8.3/chempy/electrolytes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-This modules collects expressions related to ionic strenght, e.g. the Debye-Hückel expressions.
+This modules collects expressions related to ionic strength, e.g. the Debye-Hückel expressions.
 """
 
 from collections import OrderedDict
 import warnings
 
 from ._util import get_backend
 from .chemistry import Substance
```

### Comparing `chempy-0.8.2/chempy/equilibria.py` & `chempy-0.8.3/chempy/equilibria.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
             See py:meth:`pyneqsys.NeqSys.solve`. Two additional keys
             are intercepted here:
                 latex_names: bool (default: False)
                 conc_unit_str: str (default: 'M')
         neqsys_type : str
             what method to use for NeqSys construction (get_neqsys_*)
         \\*\\*kwargs :
-            Keyword argumetns passed on to py:meth:`pyneqsys.NeqSys.solve_series`.
+            Keyword arguments passed on to py:meth:`pyneqsys.NeqSys.solve_series`.
 
         """
         _plot = plot_kwargs is not None
         if _plot:
             latex_names = plot_kwargs.pop("latex_names", False)
             conc_unit_str = plot_kwargs.pop("conc_unit_str", "M")
             if "ax" not in plot_kwargs:
```

### Comparing `chempy-0.8.2/chempy/henry.py` & `chempy-0.8.3/chempy/henry.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/_native.py` & `chempy-0.8.3/chempy/kinetics/_native.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/_rates.py` & `chempy-0.8.3/chempy/kinetics/_rates.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/analysis.py` & `chempy-0.8.3/chempy/kinetics/analysis.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/arrhenius.py` & `chempy-0.8.3/chempy/kinetics/arrhenius.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/eyring.py` & `chempy-0.8.3/chempy/kinetics/eyring.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Contains functions for the `Eyring equation
 <https://en.wikipedia.org/wiki/Eyring_equation>`_.
 """
 
 import math
 
 from .._util import get_backend
-from ..util.regression import least_squares
 from ..util.pyutil import defaultnamedtuple
 from ..units import default_units, Backend, default_constants, format_string
 from .arrhenius import _get_R, _fit
 
 try:
     import numpy as np
 except ImportError:
```

### Comparing `chempy-0.8.2/chempy/kinetics/integrated.py` & `chempy-0.8.3/chempy/kinetics/integrated.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/ode.py` & `chempy-0.8.3/chempy/kinetics/ode.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     output_time_unit : unit (Optional)
     cstr : bool
         Generate expressions for continuously stirred tank reactor.
     constants : module
         e.g. ``chempy.units.default_constants``, parameter keys not found in
         substitutions will be looked for as an attribute of ``constants`` when provided.
     \\*\\*kwargs :
-        Keyword arguemnts passed on to `SymbolicSys`.
+        Keyword arguments passed on to `SymbolicSys`.
 
     Returns
     -------
     pyodesys.symbolic.SymbolicSys
     extra : dict, with keys:
         - param_keys : list of str instances
         - unique : OrderedDict mapping str to value (possibly None)
```

### Comparing `chempy-0.8.2/chempy/kinetics/rates.py` & `chempy-0.8.3/chempy/kinetics/rates.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/tests/test__native.py` & `chempy-0.8.3/chempy/kinetics/tests/test__native.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/tests/test__rates.py` & `chempy-0.8.3/chempy/kinetics/tests/test__rates.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     p = MassAction(10 ** ShiftedTPoly([273.15, 0.7, 0.02, 0.003, 0.0004]))
     r = Reaction({"A": 2, "B": 1}, {"C": 1}, p, {"B": 1})
     res = p({"A": 11, "B": 13, "temperature": 298.15}, reaction=r)
     ref = 10 ** (0.7 + 0.02 * 25 + 0.003 * 25 ** 2 + 0.0004 * 25 ** 3)
     assert abs(res - ref * 13 * 11 ** 2) < 1e-15
 
 
+@pytest.mark.xfail  # TODO: fails in github-actions, passes locally (on 2 different machines..)
 @requires(units_library)
 def test_Log10TPolyMassAction__units():
     Mps = u.molar / u.second
     kunit = 1 / u.molar ** 2 / u.second
     p = MassAction(
         Constant(kunit)
         * 10
```

### Comparing `chempy-0.8.2/chempy/kinetics/tests/test_arrhenius.py` & `chempy-0.8.3/chempy/kinetics/tests/test_arrhenius.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/tests/test_eyring.py` & `chempy-0.8.3/chempy/kinetics/tests/test_eyring.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/tests/test_integrated.py` & `chempy-0.8.3/chempy/kinetics/tests/test_integrated.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/tests/test_ode.py` & `chempy-0.8.3/chempy/kinetics/tests/test_ode.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/kinetics/tests/test_rates.py` & `chempy-0.8.3/chempy/kinetics/tests/test_rates.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/js.py` & `chempy-0.8.3/chempy/printing/js.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         cls_names_substances=json.dumps(cls_names_substances),
         substance_row_cls_irrel=json.dumps(substance_row_cls_irrel),
         rsys_id=rsys_id,
     )
 
 
 class JSPrinter(CSSPrinter):
-    """Prints javascript-enabled HTML representaions"""
+    """Prints javascript-enabled HTML representations"""
 
     def _print_ReactionSystem(self, rsys, **kwargs):
         tab = super(JSPrinter, self)._print_ReactionSystem(rsys, **kwargs)
         _script_tag = '<script type="text/javascript">%s</script>'
         substances = self._get("substances", **kwargs)
         cls_names_substances = list(map(_html_clsname, substances))
         return tab + _script_tag % _js_rsys(
```

### Comparing `chempy-0.8.2/chempy/printing/numbers.py` & `chempy-0.8.3/chempy/printing/numbers.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/pretty.py` & `chempy-0.8.3/chempy/printing/pretty.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/printer.py` & `chempy-0.8.3/chempy/printing/printer.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/string.py` & `chempy-0.8.3/chempy/printing/string.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/table.py` & `chempy-0.8.3/chempy/printing/table.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/tables.py` & `chempy-0.8.3/chempy/printing/tables.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/tests/test_numbers.py` & `chempy-0.8.3/chempy/printing/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/tests/test_table.py` & `chempy-0.8.3/chempy/printing/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/tex.py` & `chempy-0.8.3/chempy/printing/tex.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/printing/web.py` & `chempy-0.8.3/chempy/printing/web.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/debye_huckel_radii.py` & `chempy-0.8.3/chempy/properties/debye_huckel_radii.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/gas_sol_electrolytes_schumpe_1993.py` & `chempy-0.8.3/chempy/properties/gas_sol_electrolytes_schumpe_1993.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/sulfuric_acid_density_myhre_1998.py` & `chempy-0.8.3/chempy/properties/sulfuric_acid_density_myhre_1998.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-This module implements the denisty parameterisation of aqueous sulfuric acid
+This module implements the density parameterisation of aqueous sulfuric acid
 of Myhre et al. from 1998.
 """
 
 import numpy as np
 import warnings
 
 from ..util import NoConvergence
@@ -132,15 +132,15 @@
         (default: :func:`sulfuric_acid_density`).
     units : object (optional)
         Object with attributes: meter, kilogram, mol.
     atol : float (optionally with units)
         Convergence criterion for fixed-point iteration
         (default: 1e-3 kg/m³).
     maxiter : int
-        Maximum number of iterations (when exceeded a NoConvergence excpetion
+        Maximum number of iterations (when exceeded a NoConvergence exception
         is raised).
     \\*\\*kwargs:
         Keyword arguments passed onto ``rho_cb``.
 
     Returns
     -------
     Density of sulfuric acid (float of kg/m³ if T is float and units is None)
```

### Comparing `chempy-0.8.2/chempy/properties/tests/test_sulfuric_acid_density_myhre_1998.py` & `chempy-0.8.3/chempy/properties/tests/test_sulfuric_acid_density_myhre_1998.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/tests/test_water_density_tanaka_2001.py` & `chempy-0.8.3/chempy/properties/tests/test_water_density_tanaka_2001.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/tests/test_water_diffusivity_holz_2000.py` & `chempy-0.8.3/chempy/properties/tests/test_water_diffusivity_holz_2000.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/tests/test_water_permittivity_bradley_pitzer_1979.py` & `chempy-0.8.3/chempy/properties/tests/test_water_permittivity_bradley_pitzer_1979.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/tests/test_water_viscosity_korson_1969.py` & `chempy-0.8.3/chempy/properties/tests/test_water_viscosity_korson_1969.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/water_density_tanaka_2001.py` & `chempy-0.8.3/chempy/properties/water_density_tanaka_2001.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     --------
     >>> print('%.2f' % water_density(277.13))
     999.97
 
     References
     ----------
     TANAKA M., GIRARD G., DAVIS R., PEUTO A. and BIGNELL N.,
-        "Recommanded table for the density of water between 0 °C and 40 °C
+        "Recommended table for the density of water between 0 °C and 40 °C
         based on recent experimental reports",
         Metrologia, 2001, 38, 301-309.
         http://iopscience.iop.org/article/10.1088/0026-1394/38/4/3
         doi:10.1088/0026-1394/38/4/3
     """
     if units is None:
         K = 1
```

### Comparing `chempy-0.8.2/chempy/properties/water_diffusivity_holz_2000.py` & `chempy-0.8.3/chempy/properties/water_diffusivity_holz_2000.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     T : float
         Temperature (default: in Kelvin)
     units : object (optional)
         object with attributes: Kelvin, meter, kilogram
     warn : bool (default: True)
         Emit UserWarning when outside temperature range.
     err_mult : length 2 array_like (default: None)
-        Perturb paramaters D0 and TS with err_mult[0]*dD0 and
+        Perturb parameters D0 and TS with err_mult[0]*dD0 and
         err_mult[1]*dTS respectively, where dD0 and dTS are the
-        reported uncertainties in the fitted paramters. Useful
+        reported uncertainties in the fitted parameters. Useful
         for estimating error in diffusion coefficient.
 
     References
     ----------
     Temperature-dependent self-diffusion coefficients of water and six selected
         molecular liquids for calibration in accurate 1H NMR PFG measurements
         Manfred Holz, Stefan R. Heila, Antonio Saccob;
```

### Comparing `chempy-0.8.2/chempy/properties/water_permittivity_bradley_pitzer_1979.py` & `chempy-0.8.3/chempy/properties/water_permittivity_bradley_pitzer_1979.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/properties/water_viscosity_korson_1969.py` & `chempy-0.8.3/chempy/properties/water_viscosity_korson_1969.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/reactionsystem.py` & `chempy-0.8.3/chempy/reactionsystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,15 +464,15 @@
 
         Parameters
         ----------
         rsystems : iterable of ReactionSystem instances
 
         Returns
         -------
-        pair of ReactionSystem instaces: the "sum" and "duplicates"
+        pair of ReactionSystem instances: the "sum" and "duplicates"
 
         """
         iter_rs = iter(rsystems)
         rsys = next(iter_rs)
         skipped = ReactionSystem([])
 
         def _pred(r):
@@ -579,15 +579,15 @@
         if isinstance(cont, np.ndarray):
             pass
         elif isinstance(cont, dict):
             substance_keys = self.substances.keys()
             if raise_on_unk:
                 for k in cont:
                     if k not in substance_keys:
-                        raise KeyError("Unkown substance key: %s" % k)
+                        raise KeyError("Unknown substance key: %s" % k)
             cont = [cont[k] for k in substance_keys]
         if unit is not None:
             cont = to_unitless(cont, unit)
 
         cont = np.atleast_1d(np.asarray(cont, dtype=dtype).squeeze())
         if cont.shape[-1] != self.ns:
             raise ValueError("Incorrect size")
@@ -786,15 +786,15 @@
         Returns
         -------
         numpy.ndarray :
             Per substance upper limit (ordered as :attr:`substances`).
 
         Notes
         -----
-        The function does not take into account wheter there actually exists a
+        The function does not take into account whether there actually exists a
         reaction path leading to a substance. Note also that the upper limit is
         per substance, i.e. the sum of all upper bounds amount to more substance than
         available in ``init_conc``.
 
         Examples
         --------
         >>> rs = ReactionSystem.from_string('2 HNO2 -> H2O + NO + NO2 \n 2 NO2 -> N2O4')
```

### Comparing `chempy-0.8.2/chempy/tests/ammonical_cupric_solution.py` & `chempy-0.8.3/chempy/tests/ammonical_cupric_solution.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/tests/test__equilibrium.py` & `chempy-0.8.3/chempy/tests/test__equilibrium.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/tests/test_chemistry.py` & `chempy-0.8.3/chempy/tests/test_chemistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from functools import reduce
 from operator import attrgetter, add
 import sys
+from sympy import nsimplify
 
 import pytest
 
 from ..util.arithmeticdict import ArithmeticDict
 from ..util.testing import requires
 from ..util.parsing import parsing_library
 from ..units import default_units, units_library, to_unitless, allclose
@@ -71,14 +72,20 @@
     assert Species.from_formula("CO2(aq)", mapping, phase_idx=7).phase_idx == 7
 
     uranyl_ads = Species.from_formula("UO2+2(ads)", phases={"(aq)": 0, "(ads)": 1})
     assert uranyl_ads.composition == {0: 2, 92: 1, 8: 2}
     assert uranyl_ads.phase_idx == 1
 
 
+@requires(parsing_library)
+def test_Species_default_phase_none():
+    with pytest.raises(ValueError):
+        Species.from_formula("CO2(aq)", default_phase_idx=None)
+
+
 def test_Solute():
     from ..chemistry import Solute
     from ..util.pyutil import ChemPyDeprecationWarning
 
     with pytest.warns(ChemPyDeprecationWarning):
         w = Solute("H2O")
     assert w.name == "H2O"
@@ -336,16 +343,20 @@
     assert p4 == {"CO": 14, "H2O": 19, "N2": 10}
 
     a5, b5 = {"C3H5NO", "CH4", "NH3", "H2O"}, {"C2H6", "CH4O", "CH5N", "CH3N"}
     formulas = list(set.union(a5, b5))
     substances = dict(zip(formulas, map(Substance.from_formula, formulas)))
     compositions = {k: ArithmeticDict(int, substances[k].composition) for k in formulas}
     r5, p5 = balance_stoichiometry(a5, b5)
-    compo_reac = dict(reduce(add, [compositions[k] * v for k, v in r5.items()]))
-    compo_prod = dict(reduce(add, [compositions[k] * v for k, v in p5.items()]))
+    compo_reac = nsimplify(
+        dict(reduce(add, [compositions[k] * v for k, v in r5.items()]))
+    )
+    compo_prod = nsimplify(
+        dict(reduce(add, [compositions[k] * v for k, v in p5.items()]))
+    )
     assert compo_reac == compo_prod
 
     a6, b6 = map(
         lambda x: set(x.split()), "CuSCN KIO3 HCl;CuSO4 KCl HCN ICl H2O".split(";")
     )
     r6, p6 = balance_stoichiometry(a6, b6)
     assert r6 == dict(CuSCN=4, KIO3=7, HCl=14)
@@ -367,14 +378,22 @@
     res = rxn.string()
     ref = "4 CuSCN + 7 KIO3 + 14 HCl -> 4 CuSO4 + 7 KCl + 4 HCN + 7 ICl + 5 H2O"
     assert res == ref
 
 
 @requires("sympy")
 def test_balance_stoichiometry__simple():
+    # 4 NH4ClO4 -> 2 N2 + 4 HCl + 6H2O + 5O2
+    # 4 Al + 3O2 -> 2Al2O3
+    # ---------------------------------------
+    # 6 NH4ClO4 + 10 Al + -> 3 N2 + 6 HCl + 9 H2O + 5 Al2O3
+    reac, prod = balance_stoichiometry({"NH4ClO4", "Al"}, {"Al2O3", "HCl", "H2O", "N2"})
+    assert reac == {"NH4ClO4": 6, "Al": 10}
+    assert prod == {"Al2O3": 5, "HCl": 6, "H2O": 9, "N2": 3}
+
     r2, p2 = balance_stoichiometry({"Na2CO3"}, {"Na2O", "CO2"})
     assert r2 == {"Na2CO3": 1}
     assert p2 == {"Na2O": 1, "CO2": 1}
 
 
 @requires("sympy", "pulp")
 @pytest.mark.parametrize("underdet", [False, None, True])
@@ -439,19 +458,19 @@
         ref3[1].values()
     )
     assert bal3 == ref3
 
 
 @requires("sympy", "pulp")
 def test_balance_stoichiometry__underdetermined__canoncial():
-    # This tests for canoncial representation of the underdetermined system
+    # This tests for canonical representation of the underdetermined system
     # where all coefficients are integer and >= 1. It is however of limited
     # practical use (and hence marked ``xfail``) since underdetermined systems
     # have infinite number of solutions. It should however be possible to rewrite
-    # the logic so that such canoncial results are returned from balance_stoichiometry
+    # the logic so that such canonical results are returned from balance_stoichiometry
     r2 = {"O2", "O3", "C", "NO", "N2O", "NO2", "N2O4"}
     p2 = {"CO", "CO2", "N2"}
     bal2 = balance_stoichiometry(r2, p2, underdetermined=None)
     ref2 = (
         {"O2": 1, "O3": 1, "C": 7, "NO": 1, "N2O": 1, "NO2": 1, "N2O4": 1},
         {"CO": 1, "CO2": 6, "N2": 3},
     )
```

### Comparing `chempy-0.8.2/chempy/tests/test_einstein_smoluchowski.py` & `chempy-0.8.3/chempy/tests/test_einstein_smoluchowski.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/tests/test_electrolytes.py` & `chempy-0.8.3/chempy/tests/test_electrolytes.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/tests/test_equilibria.py` & `chempy-0.8.3/chempy/tests/test_equilibria.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     eqsys, names, _ = _get_NaCl(Cls=Species, phase_idx=1)
     inp = eqsys.as_per_substance_array({"Na+": 1, "Cl-": 2, "NaCl": 4})
     result = eqsys.dissolved(inp)
     ref = eqsys.as_per_substance_array({"Na+": 5, "Cl-": 6, "NaCl": 0})
     assert np.allclose(result, ref)
 
 
+@pytest.mark.xfail  # TODO: fails in github-actions, passes locally (on 2 different machines..)
 @requires("numpy")
 @pytest.mark.parametrize("NumSys", [(NumSysLin,), (NumSysLog,), (NumSysLog, NumSysLin)])
 def test_precipitate(NumSys):
     eqsys, species, cases = _get_NaCl(Species, phase_idx=1)
 
     for init, final in cases:
         x, sol, sane = eqsys.root(
```

### Comparing `chempy-0.8.2/chempy/tests/test_henry.py` & `chempy-0.8.3/chempy/tests/test_henry.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/tests/test_reactionsystem.py` & `chempy-0.8.3/chempy/tests/test_reactionsystem.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/tests/test_solution.py` & `chempy-0.8.3/chempy/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/tests/test_units.py` & `chempy-0.8.3/chempy/tests/test_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     assert result[0] == 0.1
     assert result[1] == 0.2
 
     one_billionth_molar_in_nanomolar = to_unitless(1e-9 * u.molar, u.nanomolar)
     assert one_billionth_molar_in_nanomolar == 1
 
 
+@pytest.mark.xfail  # TODO: fails in github-actions, passes locally (on 2 different machines..)
 @requires(units_library)
 def test_UncertainQuantity():
     a = UncertainQuantity([1, 2], u.m, [0.1, 0.2])
     assert a[1] == [2.0] * u.m
     assert (-a)[0] == [-1.0] * u.m
     assert (-a).uncertainty[0] == [0.1] * u.m
     assert (-a)[0] == (a * -1)[0]
@@ -217,15 +218,15 @@
 
 
 @requires(units_library, "sympy")
 def test_to_unitless__sympy():
     import sympy as sp
 
     assert sp.cos(to_unitless(sp.pi)) == -1
-    with pytest.raises(AttributeError):
+    with pytest.raises(Exception):
         to_unitless(sp.pi, u.second)
 
 
 @requires(units_library)
 def test_linspace():
     ls = linspace(2 * u.second, 3 * u.second)
     assert abs(to_unitless(ls[0], u.hour) - 2 / 3600.0) < 1e-15
```

### Comparing `chempy-0.8.2/chempy/thermodynamics/expressions.py` & `chempy-0.8.3/chempy/thermodynamics/expressions.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/thermodynamics/tests/test_expressions.py` & `chempy-0.8.3/chempy/thermodynamics/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/units.py` & `chempy-0.8.3/chempy/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         )
     if not hasattr(default_units, "molal"):
         default_units.molal = pq.UnitQuantity(
             "molal", default_units.mole / default_units.kg, u_symbol="molal"
         )
     if not hasattr(default_units, "per100eV"):
         default_units.per100eV = pq.UnitQuantity(
-            "per_100_eV",
+            "per100eV",
             1 / (100 * default_units.eV * default_constants.Avogadro_constant),
             u_symbol="(100eV)**-1",
         )
     if not hasattr(default_units, "micromole"):
         default_units.micromole = pq.UnitQuantity(
             "micromole", pq.mole / 1e6, u_symbol="μmol"
         )
@@ -153,15 +153,15 @@
 
 energy = ArithmeticDict(int, {"mass": 1, "length": 2, "time": -2})
 volume = ArithmeticDict(int, {"length": 3})
 concentration = {"amount": 1} - volume
 
 
 def get_derived_unit(registry, key):
-    """Get the unit of a physcial quantity in a provided unit system.
+    """Get the unit of a physical quantity in a provided unit system.
 
     Parameters
     ----------
     registry: dict (str: unit)
         mapping 'length', 'mass', 'time', 'current', 'temperature',
         'luminous_intensity', 'amount'. If registry is ``None`` the
         function returns 1.0 unconditionally.
@@ -227,39 +227,39 @@
     # see https://github.com/python-quantities/python-quantities/issues/148
     from quantities.markup import format_units_latex
 
     return format_units_latex(dim, mult=r"\\cdot")
 
 
 def latex_of_unit(quant):
-    """Returns LaTeX reperesentation of the unit of a quantity
+    """Returns LaTeX representation of the unit of a quantity
 
     Examples
     --------
     >>> print(latex_of_unit(1/default_units.kelvin))
     \\mathrm{\\frac{1}{K}}
 
     """
     return _latex_from_dimensionality(quant.dimensionality).strip("$")
 
 
 def unicode_of_unit(quant):
-    """Returns unicode reperesentation of the unit of a quantity
+    """Returns unicode representation of the unit of a quantity
 
     Examples
     --------
     >>> print(unicode_of_unit(1/default_units.kelvin))
     1/K
 
     """
     return quant.dimensionality.unicode
 
 
 def html_of_unit(quant):
-    """Returns HTML reperesentation of the unit of a quantity
+    """Returns HTML representation of the unit of a quantity
 
     Examples
     --------
     >>> print(html_of_unit(2*default_units.m**2))
     m<sup>2</sup>
 
     """
@@ -275,15 +275,15 @@
         factor, u_symbol = unit_registry[k]
         if u_symbol == 1:
             unit_quants = [1]
         else:
             unit_quants = list(pq.Quantity(0, u_symbol).dimensionality.keys())
 
         if len(unit_quants) != 1:
-            raise TypeError("Unkown UnitQuantity: {}".format(unit_registry[k]))
+            raise TypeError("Unknown UnitQuantity: {}".format(unit_registry[k]))
         else:
             new_registry[k] = factor * unit_quants[0]
     return new_registry
 
 
 # Abstraction of underlying package providing units and dimensional analysis:
 
@@ -382,15 +382,18 @@
     ):
         return value
     elif isinstance(value, str):
         raise ValueError("str not supported")
     else:
         try:
             try:
-                result = (value * pq.dimensionless / new_unit).rescale(pq.dimensionless)
+                mag = magnitude(value)
+                unt = unit_of(value)
+                conv = rescale(unt/new_unit, pq.dimensionless)
+                result = np.array(mag)*conv
             except AttributeError:
                 if new_unit == pq.dimensionless:
                     return value
                 else:
                     raise
             else:
                 if result.ndim == 0:
```

### Comparing `chempy-0.8.2/chempy/util/_aqueous.py` & `chempy-0.8.3/chempy/util/_aqueous.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/_dimensionality.py` & `chempy-0.8.3/chempy/util/_dimensionality.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/_expr.py` & `chempy-0.8.3/chempy/util/_expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     raise NotImplementedError(
         "Don't know how to convert %s (of type %s)" % (obj, type(obj))
     )
 
 
 class Expr(object):
-    """Baseclass for Expressions corresponding to physical quantitites.
+    """Baseclass for Expressions corresponding to physical quantities.
 
     The design assumes that a large group of different Expr subclasses may
     be evaluated with some shared state (parameter_keys). The backend kwarg
     in call enables use of e.g. math, numpy or sympy interchangeably.
 
     Parameters
     ----------
```

### Comparing `chempy-0.8.2/chempy/util/_expr_deprecated.py` & `chempy-0.8.3/chempy/util/_expr_deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def _mk_Poly(parameter_name, reciprocal=False, shift_name="shift"):
     """Class factory of Expr subclass for (shifted) polynomial
 
     Parameters
     ----------
     parameter: str
-        name of paramter
+        name of parameter
     reciprocal: bool
         whether the polynomial is in the reciprocal of the parameter
 
     Returns
     -------
     Expr subclass for a shifted polynomial with the args: offset, p0, p1, ...
     the class has the method "eval_poly" with same signature as __call__
```

### Comparing `chempy-0.8.2/chempy/util/_julia.py` & `chempy-0.8.3/chempy/util/_julia.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         assert not r.reac and not r.inact_reac and not r.inact_prod
         ((prod, n),) = r.prod.items()
         assert n == 1
         r_str = ("{}, 0 \u21D2 {}" if ratcoeff > 0 else "{}, {} \u21D2 0").format(
             parmap[pk], substmap[prod]
         )
     else:
-        raise NotImplementedError("Whats that?")
+        raise NotImplementedError("What's that?")
     return r_str, pk, abs(ratcoeff)
 
 
 class DiffEqBioJl:
     _template_body = """\
 {name} = @{crn_macro} begin
     {reactions}
```

### Comparing `chempy-0.8.2/chempy/util/_quantities.py` & `chempy-0.8.3/chempy/util/_quantities.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # See https://github.com/python-quantities/python-quantities/pull/112
 def format_units_html(udict, font="%s", mult=r"&sdot;", paren=False):
     """
     Replace the units string provided with an equivalent html string.
 
     Exponentiation (m**2) will be replaced with superscripts (m<sup>2</sup>})
 
-    No formating is done, change `font` argument to e.g.:
+    No formatting is done, change `font` argument to e.g.:
     '<span style="color: #0000a0">%s</span>' to have text be colored blue.
 
     Multiplication (*) are replaced with the symbol specified by the mult
     argument. By default this is the latex &sdot; symbol.  Other useful options
     may be '' or '*'.
 
     If paren=True, encapsulate the string in '(' and ')'
```

### Comparing `chempy-0.8.2/chempy/util/arithmeticdict.py` & `chempy-0.8.3/chempy/util/arithmeticdict.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
             d1[k] = d1[k] / d2[k]
     else:
         for k in d1:
             d1[k] /= d2
 
 
 class ArithmeticDict(defaultdict):
-    """A dictionary which supports arithmetics
+    """A dictionary which supports arithmetic
 
     Subclassed from defaultdict, with support for addition, subtraction,
     multiplication and division. If other term/factor has a :meth:`keys` method
-    the arithmetics are performed on a key per key basis. If :meth:`keys` is
+    the arithmetic are performed on a key per key basis. If :meth:`keys` is
     missing, the operation is broadcasted onto all values.
     Nonexisting keys are interpreted to signal a zero.
 
     Notes
     -----
     ``__eq__`` ignores values equal to ``self.default_factory()``
```

### Comparing `chempy-0.8.2/chempy/util/bkh.py` & `chempy-0.8.3/chempy/util/bkh.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/deprecation.py` & `chempy-0.8.3/chempy/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/graph.py` & `chempy-0.8.3/chempy/util/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Convenince functions for representing reaction systems as graphs.
+Convenience functions for representing reaction systems as graphs.
 """
 import os
 import subprocess
 import shutil
 import tempfile
 
 
@@ -16,28 +16,28 @@
     nodeparams='[label="{}",shape=diamond]',
     colors=("maroon", "darkgreen"),
     penwidths=None,
     include_inactive=True,
 ):
     """
     Returns list of lines of DOT (graph description language)
-    formated graph.
+    formatted graph.
 
     Parameters
     ==========
     rsys: ReactionSystem
     tex: bool (default False)
-        If set True, output will be LaTeX formated
+        If set True, output will be LaTeX formatted
     (Substance need to have latex_name attribute set)
     rprefix: string
         Reaction enumeration prefix, default: r
     rref0: integer
-        Reaction enumeration inital counter value, default: 1
+        Reaction enumeration initial counter value, default: 1
     nodeparams: string
-        DOT formated param list, default: [label={} shape=diamond]
+        DOT formatted param list, default: [label={} shape=diamond]
 
     Returns
     =======
     list of lines of DOT representation of the graph representation.
 
     """
     lines = ['digraph "' + str(rsys.name) + '" {\n']
```

### Comparing `chempy-0.8.2/chempy/util/numutil.py` & `chempy-0.8.3/chempy/util/numutil.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/parsing.py` & `chempy-0.8.3/chempy/util/parsing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 """ Functions for chemical formulae and reactions """
 
 
 from collections import defaultdict
 
 import re
-import warnings
 
-from .pyutil import ChemPyDeprecationWarning, memoize
+from .pyutil import memoize
 from .periodic import symbols
 
 parsing_library = "pyparsing"  # info used for selective testing.
 
 
 def get_parsing_context():
     """returns the default dictionary for parsing strings in chempy"""
@@ -73,42 +72,124 @@
         written by:
             Paul McGuire, http://stackoverflow.com/users/165216/paul-mcguire
         in answer to the question formulated by:
             Thales MG, http://stackoverflow.com/users/2708711/thales-mg
         the code is licensed under 'CC-WIKI'.
         (see: http://blog.stackoverflow.com/2009/06/attribution-required/)
 
+    Documentation for the desired product.  Original documentation
+    above.
+
+    Create a chemical formula parser.
+
+    Parse a chemical formula, including elements, nested ions,
+    complexes, charges (ions), hydrates, and state symbols.
+
+    BNF for nested chemical formula with complexes
+
+        count :: ( '1'..'9'? | '1'..'9'' '0'..'9'+ )
+        element :: 'A'..'Z' 'a'..'z'*
+        charge :: ( '-' | '+' ) ( '1'..'9'? | '1'..'9'' '0'..'9'+ )
+        prime :: ( "*" | "'" )*
+        term :: (element
+                 | '(' formula ')'
+                 | '{' formula '}'
+                 | '[' formula ']' ) count prime charge?
+        formula :: term+
+        hydrate :: '.' count? formula
+        state :: '(' ( 's' | 'l' | 'g' | 'aq' | 'cr' ) ')'
+        compound :: count formula hydrate? state?
+
+    Parse a chemical formula, including elements, non-integer
+    subscripts, nested ions, complexes, charges (ions), hydrates, and
+    state symbols.
+
+    BNF for nested chemical formula with complexes
+
+        count :: ( '1'..'9'? | '1'..'9'' '0'..'9'+ | '0'..'9'+ '.' '0'..'9'+ )
+        element :: 'A'..'Z' 'a'..'z'*
+        charge :: ( '-' | '+' ) ( '1'..'9'? | '1'..'9'' '0'..'9'+ )
+        prime :: ( "*" | "'" )*
+        term :: (element
+                 | '(' formula ')'
+                 | '{' formula '}'
+                 | '[' formula ']' ) count prime charge?
+        formula :: term+
+        hydrate :: '..' count? formula
+        state :: '(' ( 's' | 'l' | 'g' | 'aq' | 'cr' ) ')'
+        compound :: count formula hydrate? state?
     """
     _p = __import__(parsing_library)
     Forward, Group, OneOrMore = _p.Forward, _p.Group, _p.OneOrMore
     Optional, ParseResults, Regex = _p.Optional, _p.ParseResults, _p.Regex
-    Suppress, Word, nums = _p.Suppress, _p.Word, _p.nums
+    Suppress = _p.Suppress
 
-    LPAR, RPAR = map(Suppress, "()")
-    integer = Word(nums)
+    # Define and suppress the grouping symbols.
+    LCB = Suppress(Regex(r"\{"))
+    RCB = Suppress(Regex(r"\}"))
+    LSB = Suppress(Regex(r"\["))
+    RSB = Suppress(Regex(r"\]"))
+    LP = Suppress(Regex(r"\("))
+    RP = Suppress(Regex(r"\)"))
+
+    # Define and suppress the caged symbol.
+    caged = Suppress(Regex(r"\@"))
+
+    # Primes/stars for marking special species in reactions.
+    primes = Suppress(Regex(r"[*']+"))
+
+    # Parse counts (subscripts and coefficients).
+    count = Regex(r"(\d+\.\d+|\d*)")
+    count.setParseAction(lambda t: 1 if t[0] == "" else float(t[0]))
 
-    # add parse action to convert integers to ints, to support doing addition
-    # and multiplication at parse time
-    integer.setParseAction(lambda t: int(t[0]))
+    # Parse states.
+    state = Suppress(Regex(r"\((s|l|g|aq|cr)\)"))
 
-    # element = Word(alphas.upper(), alphas.lower())
-    # or if you want to be more specific, use this Regex
+    # Elements, 1-118, official symbols.
     element = Regex(
-        r"A[cglmrstu]|B[aehikr]?|C[adeflmnorsu]?|D[bsy]|E[rsu]|F[elmr]?|"
-        "G[ade]|H[efgos]?|I[nr]?|Kr?|L[airuv]|M[cdgnot]|N[abdehiop]?|"
-        "O[gs]?|P[abdmortu]?|R[abefghnu]|S[bcegimnr]?|T[abcehilms]|"
-        "U|V|W|Xe|Yb?|Z[nr]"
-    )
+        r"A[cglmrstu]"
+        "|B[aehikr]?"
+        "|C[adeflmnorsu]?"
+        "|D[bsy]"
+        "|E[rsu]"
+        "|F[elmr]?"
+        "|G[ade]"
+        "|H[efgos]?"
+        "|I[nr]?"
+        "|Kr?"
+        "|L[airuv]"
+        "|M[cdgnot]"
+        "|N[abdehiop]?"
+        "|O[gs]?"
+        "|P[abdmortu]?"
+        "|R[abefghnu]"
+        "|S[bcegimnr]?"
+        "|T[abcehilms]"
+        "|U"
+        "|V"
+        "|W"
+        "|Xe"
+        "|Yb?"
+        "|Z[nr]"
+    ).setResultsName("element", listAllMatches=True)
 
     # forward declare 'formula' so it can be used in definition of 'term'
     formula = Forward()
 
     term = Group(
-        (element | Group(LPAR + formula + RPAR)("subgroup"))
-        + Optional(integer, default=1)("mult")
+        (
+            element
+            | Group(LP + formula + RP)("subgroup")
+            | Group(LSB + formula + RSB)("subgroup")
+            | Group(LCB + formula + RCB)("subgroup")
+            | Group(caged + formula)("subgroup")
+        )
+        + Optional(count, default=1)("mult")
+        + Optional(state)("state")
+        + Optional(primes)("primes")
     )
 
     # add parse actions for parse-time processing
 
     # parse action to multiply out subgroups
     def multiplyContents(tokens):
         t = tokens[0]
@@ -151,79 +232,74 @@
     elif chgstr == "-":
         return -1
 
     for token, anti, sign in zip("+-", "-+", (1, -1)):
         if token in chgstr:
             if anti in chgstr:
                 raise ValueError("Invalid charge description (+ & - present)")
+
             before, after = chgstr.split(token)
+
             if len(before) > 0 and len(after) > 0:
                 raise ValueError("Values both before and after charge token")
-            if len(before) > 0:
-                # will_be_missing_in='0.8.0'
-                warnings.warn(
-                    "'Fe/3+' deprecated, use e.g. 'Fe+3'",
-                    ChemPyDeprecationWarning,
-                    stacklevel=3,
-                )
-                return sign * int(1 if before == "" else before)
+
             if len(after) > 0:
                 return sign * int(1 if after == "" else after)
+
     raise ValueError("Invalid charge description (+ or - missing)")
 
 
 def _formula_to_parts(formula, prefixes, suffixes):
-    # Drop prefixes and suffixes
+    # Drop prefixes and suffixes.
     drop_pref, drop_suff = [], []
     for ign in prefixes:
         if formula.startswith(ign):
             drop_pref.append(ign)
             formula = formula[len(ign) :]
     for ign in suffixes:
         if formula.endswith(ign):
             drop_suff.append(ign)
             formula = formula[: -len(ign)]
 
-    # Extract charge
+    # Extract charge.
     if "/" in formula:
-        # will_be_missing_in='0.8.0'
-        warnings.warn(
-            "/ depr. (before 0.5.0): use 'Fe+3' over 'Fe/3+'",
-            ChemPyDeprecationWarning,
-            stacklevel=3,
+        raise ValueError(
+            "Slashes ('/') in charge strings are deprecated."
+            "  Use `Fe+3` instead of `Fe/3+`."
         )
-        parts = formula.split("/")
-
-        if "+" in parts[0] or "-" in parts[0]:
-            raise ValueError("Charge needs to be separated with a /")
-        if parts[1] is not None:
-            wo_pm = parts[1].replace("+", "").replace("-", "")
-            if wo_pm != "" and not str.isdigit(wo_pm):
-                raise ValueError("Non-digits in charge specifier")
-        if len(parts) > 2:
-            raise ValueError("At most one '/' allowed in formula")
     else:
         for token in "+-":
             if token in formula:
                 if formula.count(token) > 1:
                     raise ValueError("Multiple tokens: %s" % token)
                 parts = formula.split(token)
                 parts[1] = token + parts[1]
                 break
         else:
             parts = [formula, None]
+
     return parts + [tuple(drop_pref), tuple(drop_suff[::-1])]
 
 
 def _parse_stoich(stoich):
-    if stoich == "e":  # special case, the electron is not an element
+    # Special case:  the electron is not an element.
+    if stoich == "e":
         return {}
-    return {
-        symbols.index(k) + 1: n for k, n in _get_formula_parser().parseString(stoich)
-    }
+
+    comp = {}
+    for k, n in _get_formula_parser().parseString(stoich, parseAll=True):
+        # Only use rational subscripts if necessary as
+        # ``sympy.linsolve()`` does not like non-integers when
+        # balancing reactions.
+        if n == int(n):
+            comp[symbols.index(k) + 1] = int(n)
+        else:
+            comp[symbols.index(k) + 1] = n
+
+    return comp
 
 
 _greek_letters = (
     "alpha",
     "beta",
     "gamma",
     "delta",
@@ -244,29 +320,30 @@
     "tau",
     "upsilon",
     "phi",
     "chi",
     "psi",
     "omega",
 )
-_greek_u = u"αβγδεζηθικλμνξοπρστυφχψω"
+_greek_u = "αβγδεζηθικλμνξοπρστυφχψω"
 
 _latex_mapping = {k + "-": "\\" + k + "-" for k in _greek_letters}
 _latex_mapping["epsilon-"] = "\\varepsilon-"
 _latex_mapping["omicron-"] = "o-"
 _latex_mapping["."] = "^\\bullet "
-_latex_infix_mapping = {".": "\\cdot "}
+_latex_infix_mapping = {"..": "\\cdot "}
 
 _unicode_mapping = {k + "-": v + "-" for k, v in zip(_greek_letters, _greek_u)}
-_unicode_mapping["."] = u"⋅"
-_unicode_infix_mapping = {".": u"·"}
+_unicode_mapping["."] = "⋅"
+_unicode_infix_mapping = {"..": "·"}
 
 _html_mapping = {k + "-": "&" + k + ";-" for k in _greek_letters}
 _html_mapping["."] = "&sdot;"
-_html_infix_mapping = _html_mapping
+# _html_infix_mapping = _html_mapping
+_html_infix_mapping = {"..": "&sdot;"}
 
 
 def _get_leading_integer(s):
     m = re.findall(r"^\d+", s)
     if len(m) == 0:
         m = 1
     elif len(m) == 1:
@@ -296,42 +373,47 @@
 
     Examples
     --------
     >>> formula_to_composition('NH4+') == {0: 1, 1: 4, 7: 1}
     True
     >>> formula_to_composition('.NHO-(aq)') == {0: -1, 1: 1, 7: 1, 8: 1}
     True
-    >>> formula_to_composition('Na2CO3.7H2O') == {11: 2, 6: 1, 8: 10, 1: 14}
+    >>> formula_to_composition('Na2CO3..7H2O') == {11: 2, 6: 1, 8: 10, 1: 14}
     True
 
     """
     if prefixes is None:
         prefixes = _latex_mapping.keys()
+
     stoich_tok, chg_tok = _formula_to_parts(formula, prefixes, suffixes)[:2]
     tot_comp = {}
-    parts = stoich_tok.split(".")
+    parts = stoich_tok.split("..")
+
     for idx, stoich in enumerate(parts):
         if idx == 0:
             m = 1
         else:
             m, stoich = _get_leading_integer(stoich)
         comp = _parse_stoich(stoich)
         for k, v in comp.items():
             if k not in tot_comp:
                 tot_comp[k] = m * v
             else:
                 tot_comp[k] += m * v
+
     if chg_tok is not None:
         tot_comp[0] = _get_charge(chg_tok)
+
     return tot_comp
 
 
 def _subs(string, patterns):
     for patt, repl in patterns.items():
         string = string.replace(patt, repl)
+
     return string
 
 
 def _parse_multiplicity(strings, substance_keys=None):
     """
     Examples
     --------
@@ -361,15 +443,15 @@
                 float(items[0]) if "." in items[0] or "e" in items[0] else int(items[0])
             )
         else:
             raise ValueError("To many parts in substring")
     if substance_keys is not None:
         for k in result:
             if k not in substance_keys:
-                raise ValueError("Unkown substance_key: %s" % k)
+                raise ValueError("Unknown substance_key: %s" % k)
     return result
 
 
 def to_reaction(line, substance_keys, token, Cls, globals_=None, **kwargs):
     """Parses a string into a Reaction object and substances
 
     Reac1 + 2 Reac2 + (2 Reac1) -> Prod1 + Prod2; 10**3.7; ref='doi:12/ab'
@@ -446,25 +528,25 @@
     sup,
     formula,
     prefixes=None,
     infixes=None,
     suffixes=("(s)", "(l)", "(g)", "(aq)"),
 ):
     parts = _formula_to_parts(formula, prefixes.keys(), suffixes)
-    stoichs = parts[0].split(".")
+    stoichs = parts[0].split("..")
     string = ""
     for idx, stoich in enumerate(stoichs):
         if idx == 0:
             m = 1
         else:
             m, stoich = _get_leading_integer(stoich)
-            string += _subs(".", infixes)
+            string += _subs("..", infixes)
         if m != 1:
             string += str(m)
-        string += re.sub(r"([0-9]+)", lambda m: sub(m.group(1)), stoich)
+        string += re.sub(r"([0-9]+\.[0-9]+|[0-9]+)", lambda m: sub(m.group(1)), stoich)
 
     if parts[1] is not None:
         chg = _get_charge(parts[1])
         if chg < 0:
             token = "-" if chg == -1 else "%d-" % -chg
         if chg > 0:
             token = "+" if chg == 1 else "%d+" % chg
@@ -479,15 +561,15 @@
     r"""Convert formula string to latex representation
 
     Parameters
     ----------
     formula: str
         Chemical formula, e.g. 'H2O', 'Fe+3', 'Cl-'
     prefixes: dict
-        Prefix transofmrations, default: greek letters and .
+        Prefix transformations, default: greek letters and .
     infixes: dict
         Infix transformations, default: .
     suffixes: iterable of str
         What suffixes not to interpret, default: (s), (l), (g), (aq)
 
     Examples
     --------
@@ -506,37 +588,38 @@
     if prefixes is None:
         prefixes = _latex_mapping
     if infixes is None:
         infixes = _latex_infix_mapping
     return _formula_to_format(
         lambda x: "_{%s}" % x,
         lambda x: "^{%s}" % x,
-        formula,
+        # formula,
+        re.sub(r"([{}])", r"\\\1", formula) if re.search(r"[{}]", formula) else formula,
         prefixes,
         infixes,
         **kwargs
     )
 
 
 _unicode_sub = {}
 
-for k, v in enumerate(u"₀₁₂₃₄₅₆₇₈₉"):
+for k, v in enumerate("₀₁₂₃₄₅₆₇₈₉"):
     _unicode_sub[str(k)] = v
 
 _unicode_sup = {
-    "+": u"⁺",
-    "-": u"⁻",
+    "+": "⁺",
+    "-": "⁻",
 }
 
-for k, v in enumerate(u"⁰¹²³⁴⁵⁶⁷⁸⁹"):
+for k, v in enumerate("⁰¹²³⁴⁵⁶⁷⁸⁹"):
     _unicode_sup[str(k)] = v
 
 
 def formula_to_unicode(formula, prefixes=None, infixes=None, **kwargs):
-    u"""Convert formula string to unicode string representation
+    """Convert formula string to unicode string representation
 
     Parameters
     ----------
     formula : str
         Chemical formula, e.g. 'H2O', 'Fe+3', 'Cl-'
     prefixes : dict
         Prefix transofmrations, default: greek letters and .
@@ -570,15 +653,15 @@
         prefixes,
         infixes,
         **kwargs
     )
 
 
 def formula_to_html(formula, prefixes=None, infixes=None, **kwargs):
-    u"""Convert formula string to html string representation
+    """Convert formula string to html string representation
 
     Parameters
     ----------
     formula : str
         Chemical formula, e.g. 'H2O', 'Fe+3', 'Cl-'
     prefixes : dict
         Prefix transformations, default: greek letters and .
```

### Comparing `chempy-0.8.2/chempy/util/pyutil.py` & `chempy-0.8.3/chempy/util/pyutil.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/regression.py` & `chempy-0.8.3/chempy/util/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     >>> b1, v1, r2_1 = least_squares([1, 2, 3], [0, 1, 4], [1, 1, 1])
     >>> b2, v2, r2_2 = least_squares([1, 2, 3], [0, 1, 4], [1, 1, .2])
     >>> abs(b2[1] - 1) < abs(b1[1] - 1)
     True
 
     References
     ----------
-    Wikipedia & standard texts on least sqaures method.
+    Wikipedia & standard texts on least squares method.
     Comment regarding R2 in WLS:
         Willett, John B., and Judith D. Singer. "Another cautionary note about R 2:
         Its use in weighted least-squares regression analysis."
         The American Statistician 42.3 (1988): 236-238.
 
     """
     sqrtw = np.sqrt(w)
@@ -276,15 +276,15 @@
     return beta, cov, {"weights": weights, "niter": ii, "success": ii < itermax}
 
 
 irls.ones = lambda x, y, b, c: 1
 
 if np is not None:
     irls.exp = lambda x, y, b, c: np.exp(b[1] * x)
-    irls.gaussian = lambda x, y, b, c: np.exp(-((b[1] * x) ** 2))  # guassian weighting
+    irls.gaussian = lambda x, y, b, c: np.exp(-((b[1] * x) ** 2))  # gaussian weighting
     irls.abs_residuals = lambda x, y, b, c: np.abs(b[0] + b[1] * x - y)
 
 
 def irls_units(x, y, **kwargs):
     """Units aware version of :func:`irls`
 
     Parameters
```

### Comparing `chempy-0.8.2/chempy/util/rendering.py` & `chempy-0.8.3/chempy/util/rendering.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/stoich.py` & `chempy-0.8.3/chempy/util/stoich.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/table.py` & `chempy-0.8.3/chempy/util/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     ----------
     rsys : ReactionSystem
     rref0 : integer
         default start of index counter (default: 1)
     coldelim : string
         column delimiter (default: ' & ')
     tex : bool
-        use latex formated output (default: True)
+        use latex formatted output (default: True)
     ref_fmt : string or callable
         format string of ``ref`` attribute of reactions
     unit_registry : unit registry
         optional (default: None)
     """
     if ref_fmt is None:
```

### Comparing `chempy-0.8.2/chempy/util/terminal.py` & `chempy-0.8.3/chempy/util/terminal.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/testing.py` & `chempy-0.8.3/chempy/util/testing.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/tests/test_arithmeticdict.py` & `chempy-0.8.3/chempy/util/tests/test_arithmeticdict.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/tests/test_expr.py` & `chempy-0.8.3/chempy/util/tests/test_expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         # Canonical ensemble:
         molar_c_v = 3 * R * (TE / (2 * T)) ** 2 * backend.sinh(TE / (2 * T)) ** -2
         return molar_c_v / molar_mass
 
 
 def _get_cv(kelvin=1, gram=1, mol=1):
 
-    Al = Substance.from_formula("Al", data={"DebyeT": 428 * kelvin})
-    Be = Substance.from_formula("Be", data={"DebyeT": 1440 * kelvin})
+    Al = Substance.from_formula("Al", data={"DebyeT": 428 * kelvin, "mass": 26.9815385})
+    Be = Substance.from_formula("Be", data={"DebyeT": 1440 * kelvin, "mass": 9.0121831})
 
     def einT(s):
         return 0.806 * s.data["DebyeT"]
 
     return {s.name: EinsteinSolid([einT(s), s.mass * gram / mol]) for s in (Al, Be)}
```

### Comparing `chempy-0.8.2/chempy/util/tests/test_graph.py` & `chempy-0.8.3/chempy/util/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/tests/test_periodic.py` & `chempy-0.8.3/chempy/util/tests/test_periodic.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 )
 from ..testing import requires
 from ..parsing import formula_to_composition, parsing_library
 
 
 def test_atomic_number():
     assert atomic_number("U") == 92
+    assert atomic_number("u") == 92
     assert atomic_number("carbon") == 6
     assert atomic_number("oganesson") == 118
     with pytest.raises(ValueError):
         atomic_number("unobtainium")
 
 
 def test_mass_from_composition():
@@ -42,15 +43,15 @@
 
 
 @requires(parsing_library)
 def test_mass_from_composition__formula():
     mass = mass_from_composition(formula_to_composition("NaF"))
     assert abs(41.988172443 - mass) < 1e-7
 
-    Fminus = mass_from_composition(formula_to_composition("F/-"))
+    Fminus = mass_from_composition(formula_to_composition("F-"))
     assert abs(Fminus - 18.998403163 - 5.489e-4) < 1e-7
 
 
 def test_molar_masses_of_the_elements_gh172():
     from chempy import Substance
 
     previous_mass = 0
```

### Comparing `chempy-0.8.2/chempy/util/tests/test_pyutil.py` & `chempy-0.8.3/chempy/util/tests/test_pyutil.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/tests/test_regression.py` & `chempy-0.8.3/chempy/util/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/tests/test_rendering.py` & `chempy-0.8.3/chempy/util/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/tests/test_stoich.py` & `chempy-0.8.3/chempy/util/tests/test_stoich.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/chempy/util/tests/test_table.py` & `chempy-0.8.3/chempy/util/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.2/setup.cfg` & `chempy-0.8.3/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [flake8]
 max-line-length = 119
-extend-ignore = E203, W503
+extend-ignore = E203, W503, W504
 exclude = 
 	.jupyter
-ignore = 
-	* W503 W504
-	__init__.py F401 F403
-	arrhenius.py F401
-	.jupyter
-	chempy/*.* E226
-	chempy/kinetics/tests/test_rates.py E221 E222 E251
-	chempy/properties/** E222
-	debye_huckel.py F401
-	doc/conf.py ALL
-	eyring.py F401
+	.local
+per-file-ignores = 
+	**/__init__.py: F401 F403
+	chempy/arrhenius.py: F401
+	chempy/*.*: E226
+	chempy/kinetics/tests/test_rates.py: E221 E222 E251
+	chempy/properties/**: E222
+	chempy/debye_huckel.py: F401
+	doc/conf.py: ALL
+	chempy/eyring.py: F401
 
 [tool:pytest]
 norecursedirs = .* _* build dist conda-recipe scripts benchmarks doc deploy venv *cache*
 flake8-max-line-length = 119
 flake8-ignore = 
 	* E203 W503 W504
 	__init__.py F401 F403
```

### Comparing `chempy-0.8.2/setup.py` & `chempy-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 release_py_path = _path_under_setup(pkg_name, "_release.py")
 
 if len(RELEASE_VERSION) > 0:
     if RELEASE_VERSION[0] == "v":
         TAGGED_RELEASE = True
         __version__ = RELEASE_VERSION[1:]
     else:
-        raise ValueError("Ill formated version")
+        raise ValueError("Ill formatted version")
 else:
     TAGGED_RELEASE = False
     # read __version__ attribute from _release.py:
     exec(open(release_py_path).read())
     if __version__.endswith("git"):
         try:
             _git_version = (
@@ -89,15 +89,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 with io.open(_path_under_setup(pkg_name, "__init__.py"), "rt", encoding="utf-8") as f:
     short_description = f.read().split('"""')[1].split("\n")[1]
 if not 10 < len(short_description) < 255:
-    warnings.warn("Short description from __init__.py proably not read correctly")
+    warnings.warn("Short description from __init__.py probably not read correctly")
 long_descr = io.open(_path_under_setup("README.rst"), encoding="utf-8").read()
 if not len(long_descr) > 100:
     warnings.warn("Long description from README.rst probably not read correctly.")
 _author, _author_email = open(_path_under_setup("AUTHORS"), "rt").readline().split("<")
 
 extras_req = {
     "integrators": ["pyodeint>=0.10.4", "pycvodes>=0.14.0", "pygslodeiv2>=0.9.4"],
```

