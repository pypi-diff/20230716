# Comparing `tmp/mispr-0.0.3.tar.gz` & `tmp/mispr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mispr-0.0.3.tar", last modified: Sat Jul 15 23:11:04 2023, max compression
+gzip compressed data, was "mispr-0.0.4.tar", last modified: Sun Jul 16 00:54:42 2023, max compression
```

## Comparing `mispr-0.0.3.tar` & `mispr-0.0.4.tar`

### file list

```diff
@@ -1,261 +1,264 @@
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.531704 mispr-0.0.3/
--rw-r--r--   0 rashatwi   (501) staff       (20)      104 2021-08-05 21:58:56.000000 mispr-0.0.3/.gitignore
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.465551 mispr-0.0.3/.idea/
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.465785 mispr-0.0.3/.idea/libraries/
--rw-r--r--   0 rashatwi   (501) staff       (20)      123 2019-11-03 21:34:51.000000 mispr-0.0.3/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 rashatwi   (501) staff       (20)      180 2019-11-03 21:34:51.000000 mispr-0.0.3/.idea/vcs.xml
--rw-r--r--   0 rashatwi   (501) staff       (20)     1088 2022-08-29 17:56:34.000000 mispr-0.0.3/LICENSE
--rw-r--r--   0 rashatwi   (501) staff       (20)     3141 2023-07-15 23:11:04.531781 mispr-0.0.3/PKG-INFO
--rw-r--r--   0 rashatwi   (501) staff       (20)     2508 2023-07-08 20:34:21.000000 mispr-0.0.3/README.md
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.465987 mispr-0.0.3/docs/
--rw-r--r--   0 rashatwi   (501) staff       (20)    71796 2022-08-29 15:56:21.000000 mispr-0.0.3/docs/logo.png
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.466572 mispr-0.0.3/mispr/
--rw-r--r--   0 rashatwi   (501) staff       (20)       21 2021-10-06 00:29:14.000000 mispr-0.0.3/mispr/__init__.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.467725 mispr-0.0.3/mispr/gaussian/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/__init__.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.468145 mispr-0.0.3/mispr/gaussian/data/
--rw-r--r--   0 rashatwi   (501) staff       (20)      302 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/data/h_pot.bib
--rw-r--r--   0 rashatwi   (501) staff       (20)      285 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/data/li_pot.bib
--rw-r--r--   0 rashatwi   (501) staff       (20)      241 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/data/mg_pot.bib
--rw-r--r--   0 rashatwi   (501) staff       (20)    17589 2023-07-15 20:36:20.000000 mispr-0.0.3/mispr/gaussian/database.py
--rw-r--r--   0 rashatwi   (501) staff       (20)      958 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/defaults.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.469153 mispr-0.0.3/mispr/gaussian/firetasks/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/firetasks/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    29470 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/firetasks/geo_transformation.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    50644 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/firetasks/parse_outputs.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    14771 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/firetasks/run_calc.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     5413 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/firetasks/write_inputs.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.469630 mispr-0.0.3/mispr/gaussian/fireworks/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/fireworks/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     5011 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/fireworks/break_mol.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    10448 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/fireworks/core.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.471127 mispr-0.0.3/mispr/gaussian/utilities/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2023-07-09 22:46:07.000000 mispr-0.0.3/mispr/gaussian/utilities/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     1191 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/db_utilities.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     5476 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/dbdoc.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     2500 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/files.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     9426 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/fw_utilities.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     5636 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/gout.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     7833 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/inputs.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     2407 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/metadata.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     3355 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/misc.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    14438 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/mol.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     5873 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/utilities/rdkit.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.471252 mispr-0.0.3/mispr/gaussian/workflows/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/workflows/__init__.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.472367 mispr-0.0.3/mispr/gaussian/workflows/base/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/gaussian/workflows/base/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     8958 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/workflows/base/bde.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     9006 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/workflows/base/binding_energy.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    14144 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/workflows/base/core.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     7255 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/workflows/base/esp.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    22767 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/workflows/base/ip_ea.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     6768 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/gaussian/workflows/base/nmr.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.472586 mispr-0.0.3/mispr/hybrid/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/hybrid/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     1106 2021-10-17 17:07:37.000000 mispr-0.0.3/mispr/hybrid/defaults.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.472845 mispr-0.0.3/mispr/hybrid/firetasks/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-10-15 21:06:01.000000 mispr-0.0.3/mispr/hybrid/firetasks/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     2868 2021-10-26 14:05:58.000000 mispr-0.0.3/mispr/hybrid/firetasks/nmr_from_md.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.473250 mispr-0.0.3/mispr/hybrid/workflows/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/hybrid/workflows/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     5494 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/hybrid/workflows/core.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    12531 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/hybrid/workflows/nmr.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.473636 mispr-0.0.3/mispr/lammps/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/__init__.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.473872 mispr-0.0.3/mispr/lammps/data/
--rw-r--r--   0 rashatwi   (501) staff       (20)     2145 2023-07-09 22:46:24.000000 mispr-0.0.3/mispr/lammps/data/masses.json
--rw-r--r--   0 rashatwi   (501) staff       (20)     8713 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/lammps/database.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     6967 2021-10-21 18:52:06.000000 mispr-0.0.3/mispr/lammps/defaults.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.474507 mispr-0.0.3/mispr/lammps/firetasks/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/firetasks/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    27523 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/lammps/firetasks/parse_outputs.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    10672 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/lammps/firetasks/run.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    16308 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/lammps/firetasks/write_inputs.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.474731 mispr-0.0.3/mispr/lammps/fireworks/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/fireworks/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    11696 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/lammps/fireworks/core.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.475515 mispr-0.0.3/mispr/lammps/templates/
--rw-r--r--   0 rashatwi   (501) staff       (20)      909 2021-10-11 17:34:11.000000 mispr-0.0.3/mispr/lammps/templates/emin_gaff
--rw-r--r--   0 rashatwi   (501) staff       (20)      843 2021-10-11 17:34:11.000000 mispr-0.0.3/mispr/lammps/templates/emin_general
--rw-r--r--   0 rashatwi   (501) staff       (20)      168 2021-08-05 18:59:45.000000 mispr-0.0.3/mispr/lammps/templates/gaff_tleap
--rw-r--r--   0 rashatwi   (501) staff       (20)     1304 2023-07-09 22:46:35.000000 mispr-0.0.3/mispr/lammps/templates/npt
--rw-r--r--   0 rashatwi   (501) staff       (20)     1339 2023-07-09 22:46:35.000000 mispr-0.0.3/mispr/lammps/templates/nvt
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.477939 mispr-0.0.3/mispr/lammps/tests/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)      966 2021-08-24 18:37:19.000000 mispr-0.0.3/mispr/lammps/tests/antechamber.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    13544 2021-08-24 18:40:54.000000 mispr-0.0.3/mispr/lammps/tests/base_test.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     4922 2021-08-24 18:45:32.000000 mispr-0.0.3/mispr/lammps/tests/control.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     5887 2021-08-24 18:45:33.000000 mispr-0.0.3/mispr/lammps/tests/custom_data_workflow.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     9852 2021-08-24 18:27:05.000000 mispr-0.0.3/mispr/lammps/tests/data.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.479185 mispr-0.0.3/mispr/lammps/tests/database/
--rw-r--r--   0 rashatwi   (501) staff       (20)      349 2021-08-24 18:29:49.000000 mispr-0.0.3/mispr/lammps/tests/database/delete_data.py
--rw-r--r--   0 rashatwi   (501) staff       (20)      319 2021-08-24 18:30:22.000000 mispr-0.0.3/mispr/lammps/tests/database/first_connection.py
--rw-r--r--   0 rashatwi   (501) staff       (20)      429 2021-08-24 18:30:23.000000 mispr-0.0.3/mispr/lammps/tests/database/insert_one.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     1234 2021-08-24 18:31:36.000000 mispr-0.0.3/mispr/lammps/tests/database/operators-compound_queries.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     1768 2021-08-24 18:35:57.000000 mispr-0.0.3/mispr/lammps/tests/database/query_data.py
--rw-r--r--   0 rashatwi   (501) staff       (20)      402 2021-08-24 18:35:59.000000 mispr-0.0.3/mispr/lammps/tests/database/read_data.py
--rw-r--r--   0 rashatwi   (501) staff       (20)      673 2021-08-24 18:36:18.000000 mispr-0.0.3/mispr/lammps/tests/database/update_data.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     7133 2021-08-24 18:48:06.000000 mispr-0.0.3/mispr/lammps/tests/electrolyte_wf.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     6091 2021-08-24 18:50:26.000000 mispr-0.0.3/mispr/lammps/tests/esp_to_ff_dict_custom.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     6869 2021-08-24 18:52:54.000000 mispr-0.0.3/mispr/lammps/tests/esp_to_ff_dict_function.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     7137 2021-08-24 18:54:27.000000 mispr-0.0.3/mispr/lammps/tests/liquid_wf_local.py
--rw-r--r--   0 rashatwi   (501) staff       (20)      959 2021-08-24 18:55:47.000000 mispr-0.0.3/mispr/lammps/tests/parmchk.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     3594 2021-08-24 18:56:21.000000 mispr-0.0.3/mispr/lammps/tests/prmtop.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     2674 2021-08-24 18:57:21.000000 mispr-0.0.3/mispr/lammps/tests/run_lammps.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.483871 mispr-0.0.3/mispr/lammps/tests/test_files/
--rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:45.000000 mispr-0.0.3/mispr/lammps/tests/test_files/Na.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:45.000000 mispr-0.0.3/mispr/lammps/tests/test_files/SPC_E.pdb
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.492849 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/
--rw-r--r--   0 rashatwi   (501) staff       (20)  3431877 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/complex.data
--rw-r--r--   0 rashatwi   (501) staff       (20)     1953 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/d__diff.txt
--rw-r--r--   0 rashatwi   (501) staff       (20)      351 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/diffusion.csv
--rw-r--r--   0 rashatwi   (501) staff       (20)      934 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/in.emin_complex.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)     1953 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/n__diff.txt
--rw-r--r--   0 rashatwi   (501) staff       (20)     1953 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/o__diff.txt
--rw-r--r--   0 rashatwi   (501) staff       (20)     5708 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/rdf.csv
--rw-r--r--   0 rashatwi   (501) staff       (20)     1953 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/analysis/w__diff.txt
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.493013 mispr-0.0.3/mispr/lammps/tests/test_files/antechamber/
--rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:45.000000 mispr-0.0.3/mispr/lammps/tests/test_files/antechamber/dhps.esp
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.494304 mispr-0.0.3/mispr/lammps/tests/test_files/control/
--rw-r--r--   0 rashatwi   (501) staff       (20)      720 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/control/case_1.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      720 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/control/case_2.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      911 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/control/case_2_npt.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      921 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/control/case_2_npt_group_list.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      720 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/control/case_3.lammpsin
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.498674 mispr-0.0.3/mispr/lammps/tests/test_files/data/
--rw-r--r--   0 rashatwi   (501) staff       (20)     7659 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/H2O2.prmtop
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.499830 mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5/
--rw-r--r--   0 rashatwi   (501) staff       (20)     7380 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5/ff.json
--rw-r--r--   0 rashatwi   (501) staff       (20)     2974 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5/leap.log
--rw-r--r--   0 rashatwi   (501) staff       (20)      548 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5/tleap.in
--rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5.prmtop
--rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:45.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/Na.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:45.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/SPC_E.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)   192616 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/complex.data
--rw-r--r--   0 rashatwi   (501) staff       (20)   176562 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/complex_from_concentration.data
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.510176 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/
--rw-r--r--   0 rashatwi   (501) staff       (20)    17891 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER.ESP
--rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_AC.AC
--rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_AC.AC0
--rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_BOND_TYPE.AC
--rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_BOND_TYPE.AC0
--rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP.AC
--rw-r--r--   0 rashatwi   (501) staff       (20)      181 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP1.IN
--rw-r--r--   0 rashatwi   (501) staff       (20)     2690 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP1.OUT
--rw-r--r--   0 rashatwi   (501) staff       (20)      194 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP2.IN
--rw-r--r--   0 rashatwi   (501) staff       (20)     2747 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP2.OUT
--rw-r--r--   0 rashatwi   (501) staff       (20)     1355 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ATOMTYPE.INF
--rw-r--r--   0 rashatwi   (501) staff       (20)       67 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.frcmod
--rw-r--r--   0 rashatwi   (501) staff       (20)       84 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.inpcrd
--rw-r--r--   0 rashatwi   (501) staff       (20)      365 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.mol2
--rw-r--r--   0 rashatwi   (501) staff       (20)     7659 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.prmtop
--rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.frcmod
--rw-r--r--   0 rashatwi   (501) staff       (20)      924 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.inpcrd
--rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.mol2
--rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.prmtop
--rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:45.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/Na.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:45.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/SPC_E.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/dhps.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/dhps.out
--rw-r--r--   0 rashatwi   (501) staff       (20)    18347 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/esout
--rw-r--r--   0 rashatwi   (501) staff       (20)   108780 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/leap.log
--rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/oh.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/oh.out
--rw-r--r--   0 rashatwi   (501) staff       (20)    79039 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/packed.xyz
--rw-r--r--   0 rashatwi   (501) staff       (20)      808 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/punch
--rw-r--r--   0 rashatwi   (501) staff       (20)       21 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/qout
--rw-r--r--   0 rashatwi   (501) staff       (20)      544 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/tleap.in
--rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/dhps.out
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.512215 mispr-0.0.3/mispr/lammps/tests/test_files/data/emin/
--rw-r--r--   0 rashatwi   (501) staff       (20)      698 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/emin/complex.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      458 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/emin/run_file.json
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.512636 mispr-0.0.3/mispr/lammps/tests/test_files/data/melt/
--rw-r--r--   0 rashatwi   (501) staff       (20)      921 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/melt/complex.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      452 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/melt/run_file.json
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.512964 mispr-0.0.3/mispr/lammps/tests/test_files/data/npt/
--rw-r--r--   0 rashatwi   (501) staff       (20)      976 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/npt/complex.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      451 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/npt/run_file.json
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.513255 mispr-0.0.3/mispr/lammps/tests/test_files/data/nvt_0-20/
--rw-r--r--   0 rashatwi   (501) staff       (20)     1064 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/nvt_0-20/complex.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      456 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/nvt_0-20/run_file.json
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.513537 mispr-0.0.3/mispr/lammps/tests/test_files/data/nvt_20-40/
--rw-r--r--   0 rashatwi   (501) staff       (20)     1062 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/nvt_20-40/complex.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      457 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/nvt_20-40/run_file.json
--rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/oh.out
--rw-r--r--   0 rashatwi   (501) staff       (20)    89455 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/packed.xyz
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.513826 mispr-0.0.3/mispr/lammps/tests/test_files/data/quench/
--rw-r--r--   0 rashatwi   (501) staff       (20)      934 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/quench/complex.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      454 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/data/quench/run_file.json
--rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/dhps.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/dhps.frcmod
--rw-r--r--   0 rashatwi   (501) staff       (20)      924 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/dhps.inpcrd
--rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/dhps.mol2
--rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/dhps.out
--rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/dhps.prmtop
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.517653 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.519028 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/
--rw-r--r--   0 rashatwi   (501) staff       (20)       67 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.frcmod
--rw-r--r--   0 rashatwi   (501) staff       (20)       84 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.inpcrd
--rw-r--r--   0 rashatwi   (501) staff       (20)      365 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.mol2
--rw-r--r--   0 rashatwi   (501) staff       (20)     7659 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.prmtop
--rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/oh.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)      544 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/tleap.in
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.520108 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/
--rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.frcmod
--rw-r--r--   0 rashatwi   (501) staff       (20)      924 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.inpcrd
--rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.mol2
--rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.prmtop
--rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/dhps.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)      592 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/tleap.in
--rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/Na.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/SPC_E.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)   176562 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/complex_from_concentration.data
--rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/dhps.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/dhps.out
--rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/oh.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/oh.out
--rw-r--r--   0 rashatwi   (501) staff       (20)     4293 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/leap.log
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.526652 mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/
--rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/Na.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/SPC_E.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/dhps.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/dhps.out
--rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/oh.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/oh.out
--rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/oh.esp
--rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/oh.out
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.527102 mispr-0.0.3/mispr/lammps/tests/test_files/parmchk/
--rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/parmchk/dhps.frcmod
--rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/parmchk/dhps.mol2
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.529341 mispr-0.0.3/mispr/lammps/tests/test_files/prmtop/
--rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/prmtop/Na.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/prmtop/SPC_E.pdb
--rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/prmtop/dhps.out
--rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/prmtop/dhps.prmtop
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.529885 mispr-0.0.3/mispr/lammps/tests/test_files/run_lammps/
--rw-r--r--   0 rashatwi   (501) staff       (20)      911 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/run_lammps/test.lammpsin
--rw-r--r--   0 rashatwi   (501) staff       (20)      911 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/run_lammps/test_npt.lammpsin
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.530698 mispr-0.0.3/mispr/lammps/tests/test_files/tleap/
--rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/tleap/dhps.frcmod
--rw-r--r--   0 rashatwi   (501) staff       (20)      924 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/tleap/dhps.inpcrd
--rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/tleap/dhps.mol2
--rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 18:59:44.000000 mispr-0.0.3/mispr/lammps/tests/test_files/tleap/dhps.prmtop
--rw-r--r--   0 rashatwi   (501) staff       (20)      500 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/tleap/tleap.in
--rw-r--r--   0 rashatwi   (501) staff       (20)      476 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/tests/test_files/tleap.in
--rw-r--r--   0 rashatwi   (501) staff       (20)     1311 2021-08-24 18:57:31.000000 mispr-0.0.3/mispr/lammps/tests/tleap.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.531281 mispr-0.0.3/mispr/lammps/utilities/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/utilities/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    18470 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/lammps/utilities/opls.py
--rw-r--r--   0 rashatwi   (501) staff       (20)     5397 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/lammps/utilities/utilities.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.531524 mispr-0.0.3/mispr/lammps/workflows/
--rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 21:11:00.000000 mispr-0.0.3/mispr/lammps/workflows/__init__.py
--rw-r--r--   0 rashatwi   (501) staff       (20)    15679 2023-07-15 20:33:13.000000 mispr-0.0.3/mispr/lammps/workflows/base.py
-drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-15 23:11:04.467139 mispr-0.0.3/mispr.egg-info/
--rw-r--r--   0 rashatwi   (501) staff       (20)     3141 2023-07-15 23:11:04.000000 mispr-0.0.3/mispr.egg-info/PKG-INFO
--rw-r--r--   0 rashatwi   (501) staff       (20)     9736 2023-07-15 23:11:04.000000 mispr-0.0.3/mispr.egg-info/SOURCES.txt
--rw-r--r--   0 rashatwi   (501) staff       (20)        1 2023-07-15 23:11:04.000000 mispr-0.0.3/mispr.egg-info/dependency_links.txt
--rw-r--r--   0 rashatwi   (501) staff       (20)      164 2023-07-15 23:11:04.000000 mispr-0.0.3/mispr.egg-info/requires.txt
--rw-r--r--   0 rashatwi   (501) staff       (20)        6 2023-07-15 23:11:04.000000 mispr-0.0.3/mispr.egg-info/top_level.txt
--rw-r--r--   0 rashatwi   (501) staff       (20)       79 2023-07-15 23:11:04.532015 mispr-0.0.3/setup.cfg
--rw-r--r--   0 rashatwi   (501) staff       (20)     1244 2023-07-15 20:33:13.000000 mispr-0.0.3/setup.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.893555 mispr-0.0.4/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      104 2021-08-05 21:58:56.000000 mispr-0.0.4/.gitignore
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.857554 mispr-0.0.4/.idea/
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.857713 mispr-0.0.4/.idea/libraries/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      123 2019-11-03 21:34:51.000000 mispr-0.0.4/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 rashatwi   (501) staff       (20)      180 2019-11-03 21:34:51.000000 mispr-0.0.4/.idea/vcs.xml
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1088 2022-08-29 17:56:34.000000 mispr-0.0.4/LICENSE
+-rw-r--r--   0 rashatwi   (501) staff       (20)     3141 2023-07-16 00:54:42.893674 mispr-0.0.4/PKG-INFO
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2508 2023-07-08 20:34:21.000000 mispr-0.0.4/README.md
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.857839 mispr-0.0.4/docs/
+-rw-r--r--   0 rashatwi   (501) staff       (20)    71796 2022-08-29 15:56:21.000000 mispr-0.0.4/docs/logo.png
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.858007 mispr-0.0.4/mispr/
+-rw-r--r--   0 rashatwi   (501) staff       (20)       21 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/__init__.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.858951 mispr-0.0.4/mispr/common/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:48:24.000000 mispr-0.0.4/mispr/common/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     3266 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/common/pubchem.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.859298 mispr-0.0.4/mispr/gaussian/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/__init__.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.859654 mispr-0.0.4/mispr/gaussian/data/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      302 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/data/h_pot.bib
+-rw-r--r--   0 rashatwi   (501) staff       (20)      285 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/data/li_pot.bib
+-rw-r--r--   0 rashatwi   (501) staff       (20)      241 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/data/mg_pot.bib
+-rw-r--r--   0 rashatwi   (501) staff       (20)    17589 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/database.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)      958 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/defaults.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.860271 mispr-0.0.4/mispr/gaussian/firetasks/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/firetasks/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    29470 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/firetasks/geo_transformation.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    50644 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/firetasks/parse_outputs.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    14771 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/firetasks/run_calc.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5413 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/firetasks/write_inputs.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.860641 mispr-0.0.4/mispr/gaussian/fireworks/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/fireworks/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5011 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/fireworks/break_mol.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    10448 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/fireworks/core.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.862258 mispr-0.0.4/mispr/gaussian/utilities/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2023-07-09 22:46:07.000000 mispr-0.0.4/mispr/gaussian/utilities/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1191 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/db_utilities.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5476 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/dbdoc.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2500 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/files.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     9426 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/fw_utilities.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5636 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/gout.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     7833 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/inputs.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2407 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/metadata.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     3355 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/misc.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    14438 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/mol.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5873 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/utilities/rdkit.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.862377 mispr-0.0.4/mispr/gaussian/workflows/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/workflows/__init__.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.863228 mispr-0.0.4/mispr/gaussian/workflows/base/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/gaussian/workflows/base/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     8958 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/workflows/base/bde.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     9006 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/workflows/base/binding_energy.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    14144 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/workflows/base/core.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     7255 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/workflows/base/esp.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    22767 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/workflows/base/ip_ea.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     6768 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/gaussian/workflows/base/nmr.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.863435 mispr-0.0.4/mispr/hybrid/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/hybrid/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1106 2021-10-17 17:07:37.000000 mispr-0.0.4/mispr/hybrid/defaults.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.863700 mispr-0.0.4/mispr/hybrid/firetasks/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-10-15 21:06:01.000000 mispr-0.0.4/mispr/hybrid/firetasks/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2868 2021-10-26 14:05:58.000000 mispr-0.0.4/mispr/hybrid/firetasks/nmr_from_md.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.864018 mispr-0.0.4/mispr/hybrid/workflows/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/hybrid/workflows/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5494 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/hybrid/workflows/core.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    12531 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/hybrid/workflows/nmr.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.864344 mispr-0.0.4/mispr/lammps/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/__init__.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.864462 mispr-0.0.4/mispr/lammps/data/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2145 2023-07-09 22:46:24.000000 mispr-0.0.4/mispr/lammps/data/masses.json
+-rw-r--r--   0 rashatwi   (501) staff       (20)     8713 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/lammps/database.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     6967 2021-10-21 18:52:06.000000 mispr-0.0.4/mispr/lammps/defaults.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.864918 mispr-0.0.4/mispr/lammps/firetasks/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/firetasks/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    27523 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/lammps/firetasks/parse_outputs.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    10672 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/lammps/firetasks/run.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    16308 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/lammps/firetasks/write_inputs.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.865134 mispr-0.0.4/mispr/lammps/fireworks/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/fireworks/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    11696 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/lammps/fireworks/core.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.865695 mispr-0.0.4/mispr/lammps/templates/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      909 2021-10-11 17:34:11.000000 mispr-0.0.4/mispr/lammps/templates/emin_gaff
+-rw-r--r--   0 rashatwi   (501) staff       (20)      843 2021-10-11 17:34:11.000000 mispr-0.0.4/mispr/lammps/templates/emin_general
+-rw-r--r--   0 rashatwi   (501) staff       (20)      168 2021-08-05 18:59:45.000000 mispr-0.0.4/mispr/lammps/templates/gaff_tleap
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1304 2023-07-09 22:46:35.000000 mispr-0.0.4/mispr/lammps/templates/npt
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1339 2023-07-09 22:46:35.000000 mispr-0.0.4/mispr/lammps/templates/nvt
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.867275 mispr-0.0.4/mispr/lammps/tests/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)      966 2021-08-24 18:37:19.000000 mispr-0.0.4/mispr/lammps/tests/antechamber.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    13544 2021-08-24 18:40:54.000000 mispr-0.0.4/mispr/lammps/tests/base_test.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     4922 2021-08-24 18:45:32.000000 mispr-0.0.4/mispr/lammps/tests/control.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5887 2021-08-24 18:45:33.000000 mispr-0.0.4/mispr/lammps/tests/custom_data_workflow.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     9852 2021-08-24 18:27:05.000000 mispr-0.0.4/mispr/lammps/tests/data.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.868359 mispr-0.0.4/mispr/lammps/tests/database/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      349 2021-08-24 18:29:49.000000 mispr-0.0.4/mispr/lammps/tests/database/delete_data.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)      319 2021-08-24 18:30:22.000000 mispr-0.0.4/mispr/lammps/tests/database/first_connection.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)      429 2021-08-24 18:30:23.000000 mispr-0.0.4/mispr/lammps/tests/database/insert_one.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1234 2021-08-24 18:31:36.000000 mispr-0.0.4/mispr/lammps/tests/database/operators-compound_queries.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1768 2021-08-24 18:35:57.000000 mispr-0.0.4/mispr/lammps/tests/database/query_data.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)      402 2021-08-24 18:35:59.000000 mispr-0.0.4/mispr/lammps/tests/database/read_data.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)      673 2021-08-24 18:36:18.000000 mispr-0.0.4/mispr/lammps/tests/database/update_data.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     7133 2021-08-24 18:48:06.000000 mispr-0.0.4/mispr/lammps/tests/electrolyte_wf.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     6091 2021-08-24 18:50:26.000000 mispr-0.0.4/mispr/lammps/tests/esp_to_ff_dict_custom.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     6869 2021-08-24 18:52:54.000000 mispr-0.0.4/mispr/lammps/tests/esp_to_ff_dict_function.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     7137 2021-08-24 18:54:27.000000 mispr-0.0.4/mispr/lammps/tests/liquid_wf_local.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)      959 2021-08-24 18:55:47.000000 mispr-0.0.4/mispr/lammps/tests/parmchk.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     3594 2021-08-24 18:56:21.000000 mispr-0.0.4/mispr/lammps/tests/prmtop.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2674 2021-08-24 18:57:21.000000 mispr-0.0.4/mispr/lammps/tests/run_lammps.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.870606 mispr-0.0.4/mispr/lammps/tests/test_files/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:45.000000 mispr-0.0.4/mispr/lammps/tests/test_files/Na.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:45.000000 mispr-0.0.4/mispr/lammps/tests/test_files/SPC_E.pdb
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.873128 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/
+-rw-r--r--   0 rashatwi   (501) staff       (20)  3431877 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/complex.data
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1953 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/d__diff.txt
+-rw-r--r--   0 rashatwi   (501) staff       (20)      351 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/diffusion.csv
+-rw-r--r--   0 rashatwi   (501) staff       (20)      934 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/in.emin_complex.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1953 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/n__diff.txt
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1953 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/o__diff.txt
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5708 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/rdf.csv
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1953 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/analysis/w__diff.txt
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.873247 mispr-0.0.4/mispr/lammps/tests/test_files/antechamber/
+-rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:45.000000 mispr-0.0.4/mispr/lammps/tests/test_files/antechamber/dhps.esp
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.873898 mispr-0.0.4/mispr/lammps/tests/test_files/control/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      720 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/control/case_1.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      720 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/control/case_2.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      911 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/control/case_2_npt.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      921 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/control/case_2_npt_group_list.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      720 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/control/case_3.lammpsin
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.875832 mispr-0.0.4/mispr/lammps/tests/test_files/data/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     7659 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/H2O2.prmtop
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.876242 mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     7380 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5/ff.json
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2974 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5/leap.log
+-rw-r--r--   0 rashatwi   (501) staff       (20)      548 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5/tleap.in
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5.prmtop
+-rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:45.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/Na.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:45.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/SPC_E.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)   192616 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/complex.data
+-rw-r--r--   0 rashatwi   (501) staff       (20)   176562 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/complex_from_concentration.data
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.881338 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/
+-rw-r--r--   0 rashatwi   (501) staff       (20)    17891 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER.ESP
+-rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_AC.AC
+-rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_AC.AC0
+-rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_BOND_TYPE.AC
+-rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_BOND_TYPE.AC0
+-rw-r--r--   0 rashatwi   (501) staff       (20)      227 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP.AC
+-rw-r--r--   0 rashatwi   (501) staff       (20)      181 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP1.IN
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2690 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP1.OUT
+-rw-r--r--   0 rashatwi   (501) staff       (20)      194 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP2.IN
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2747 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP2.OUT
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1355 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ATOMTYPE.INF
+-rw-r--r--   0 rashatwi   (501) staff       (20)       67 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.frcmod
+-rw-r--r--   0 rashatwi   (501) staff       (20)       84 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.inpcrd
+-rw-r--r--   0 rashatwi   (501) staff       (20)      365 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.mol2
+-rw-r--r--   0 rashatwi   (501) staff       (20)     7659 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.prmtop
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.frcmod
+-rw-r--r--   0 rashatwi   (501) staff       (20)      924 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.inpcrd
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.mol2
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.prmtop
+-rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:45.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/Na.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:45.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/SPC_E.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/dhps.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/dhps.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18347 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/esout
+-rw-r--r--   0 rashatwi   (501) staff       (20)   108780 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/leap.log
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/oh.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/oh.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)    79039 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/packed.xyz
+-rw-r--r--   0 rashatwi   (501) staff       (20)      808 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/punch
+-rw-r--r--   0 rashatwi   (501) staff       (20)       21 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/qout
+-rw-r--r--   0 rashatwi   (501) staff       (20)      544 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/tleap.in
+-rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/dhps.out
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.881583 mispr-0.0.4/mispr/lammps/tests/test_files/data/emin/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      698 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/emin/complex.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      458 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/emin/run_file.json
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.881835 mispr-0.0.4/mispr/lammps/tests/test_files/data/melt/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      921 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/melt/complex.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      452 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/melt/run_file.json
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.882084 mispr-0.0.4/mispr/lammps/tests/test_files/data/npt/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      976 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/npt/complex.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      451 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/npt/run_file.json
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.882333 mispr-0.0.4/mispr/lammps/tests/test_files/data/nvt_0-20/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1064 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/nvt_0-20/complex.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      456 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/nvt_0-20/run_file.json
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.882591 mispr-0.0.4/mispr/lammps/tests/test_files/data/nvt_20-40/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1062 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/nvt_20-40/complex.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      457 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/nvt_20-40/run_file.json
+-rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/oh.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)    89455 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/packed.xyz
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.882831 mispr-0.0.4/mispr/lammps/tests/test_files/data/quench/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      934 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/quench/complex.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      454 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/data/quench/run_file.json
+-rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/dhps.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/dhps.frcmod
+-rw-r--r--   0 rashatwi   (501) staff       (20)      924 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/dhps.inpcrd
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/dhps.mol2
+-rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/dhps.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/dhps.prmtop
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.885176 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.886102 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/
+-rw-r--r--   0 rashatwi   (501) staff       (20)       67 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.frcmod
+-rw-r--r--   0 rashatwi   (501) staff       (20)       84 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.inpcrd
+-rw-r--r--   0 rashatwi   (501) staff       (20)      365 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.mol2
+-rw-r--r--   0 rashatwi   (501) staff       (20)     7659 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.prmtop
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/oh.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)      544 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/tleap.in
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.887169 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.frcmod
+-rw-r--r--   0 rashatwi   (501) staff       (20)      924 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.inpcrd
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.mol2
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.prmtop
+-rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/dhps.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)      592 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/tleap.in
+-rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/Na.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/SPC_E.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)   176562 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/complex_from_concentration.data
+-rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/dhps.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/dhps.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/oh.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/oh.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)     4293 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/leap.log
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.889487 mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/Na.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/SPC_E.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)    90594 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/dhps.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/dhps.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/oh.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/oh.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18325 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/oh.esp
+-rw-r--r--   0 rashatwi   (501) staff       (20)    28374 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/oh.out
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.889776 mispr-0.0.4/mispr/lammps/tests/test_files/parmchk/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/parmchk/dhps.frcmod
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/parmchk/dhps.mol2
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.891893 mispr-0.0.4/mispr/lammps/tests/test_files/prmtop/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      215 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/prmtop/Na.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)      590 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/prmtop/SPC_E.pdb
+-rw-r--r--   0 rashatwi   (501) staff       (20)  1488557 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/prmtop/dhps.out
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/prmtop/dhps.prmtop
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.892201 mispr-0.0.4/mispr/lammps/tests/test_files/run_lammps/
+-rw-r--r--   0 rashatwi   (501) staff       (20)      911 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/run_lammps/test.lammpsin
+-rw-r--r--   0 rashatwi   (501) staff       (20)      911 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/run_lammps/test_npt.lammpsin
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.892834 mispr-0.0.4/mispr/lammps/tests/test_files/tleap/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1110 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/tleap/dhps.frcmod
+-rw-r--r--   0 rashatwi   (501) staff       (20)      924 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/tleap/dhps.inpcrd
+-rw-r--r--   0 rashatwi   (501) staff       (20)     2875 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/tleap/dhps.mol2
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18484 2021-08-05 18:59:44.000000 mispr-0.0.4/mispr/lammps/tests/test_files/tleap/dhps.prmtop
+-rw-r--r--   0 rashatwi   (501) staff       (20)      500 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/tleap/tleap.in
+-rw-r--r--   0 rashatwi   (501) staff       (20)      476 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/tests/test_files/tleap.in
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1311 2021-08-24 18:57:31.000000 mispr-0.0.4/mispr/lammps/tests/tleap.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.893195 mispr-0.0.4/mispr/lammps/utilities/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/utilities/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    18470 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/lammps/utilities/opls.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)     5397 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/lammps/utilities/utilities.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.893410 mispr-0.0.4/mispr/lammps/workflows/
+-rw-r--r--   0 rashatwi   (501) staff       (20)        0 2021-08-05 21:11:00.000000 mispr-0.0.4/mispr/lammps/workflows/__init__.py
+-rw-r--r--   0 rashatwi   (501) staff       (20)    15679 2023-07-16 00:52:19.000000 mispr-0.0.4/mispr/lammps/workflows/base.py
+drwxr-xr-x   0 rashatwi   (501) staff       (20)        0 2023-07-16 00:54:42.858720 mispr-0.0.4/mispr.egg-info/
+-rw-r--r--   0 rashatwi   (501) staff       (20)     3141 2023-07-16 00:54:42.000000 mispr-0.0.4/mispr.egg-info/PKG-INFO
+-rw-r--r--   0 rashatwi   (501) staff       (20)     9785 2023-07-16 00:54:42.000000 mispr-0.0.4/mispr.egg-info/SOURCES.txt
+-rw-r--r--   0 rashatwi   (501) staff       (20)        1 2023-07-16 00:54:42.000000 mispr-0.0.4/mispr.egg-info/dependency_links.txt
+-rw-r--r--   0 rashatwi   (501) staff       (20)      164 2023-07-16 00:54:42.000000 mispr-0.0.4/mispr.egg-info/requires.txt
+-rw-r--r--   0 rashatwi   (501) staff       (20)        6 2023-07-16 00:54:42.000000 mispr-0.0.4/mispr.egg-info/top_level.txt
+-rw-r--r--   0 rashatwi   (501) staff       (20)       79 2023-07-16 00:54:42.893927 mispr-0.0.4/setup.cfg
+-rw-r--r--   0 rashatwi   (501) staff       (20)     1244 2023-07-16 00:52:19.000000 mispr-0.0.4/setup.py
```

### Comparing `mispr-0.0.3/LICENSE` & `mispr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/PKG-INFO` & `mispr-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mispr
-Version: 0.0.3
+Version: 0.0.4
 Summary: mispr contains FireWorks workflows for Materials Science
 Home-page: https://github.com/molmd/mispr
 Author: Rasha Atwi, Matthew Bliss
 Author-email: rasha.atwi@stonybrook.edu, matthew.bliss@stonybrook.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mispr-0.0.3/README.md` & `mispr-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/docs/logo.png` & `mispr-0.0.4/docs/logo.png`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/gaussian/database.py` & `mispr-0.0.4/mispr/gaussian/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from mispr.gaussian.utilities.metadata import get_chem_schema
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger()
 ch = logging.StreamHandler(stream=sys.stdout)
 logger.addHandler(ch)
 logger.setLevel(20)
```

### Comparing `mispr-0.0.3/mispr/gaussian/defaults.py` & `mispr-0.0.4/mispr/gaussian/defaults.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/gaussian/firetasks/geo_transformation.py` & `mispr-0.0.4/mispr/gaussian/firetasks/geo_transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from mispr.gaussian.utilities.db_utilities import get_db
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_KEY = "gout_key"
 
 
 @explicit_serialize
```

### Comparing `mispr-0.0.3/mispr/gaussian/firetasks/parse_outputs.py` & `mispr-0.0.4/mispr/gaussian/firetasks/parse_outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from mispr.gaussian.utilities.db_utilities import get_db
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_KEY = "gout_key"
 HARTREE_TO_EV = 27.2114
 HARTREE_TO_KJ = 2600
 FARAD = 96.5
```

### Comparing `mispr-0.0.3/mispr/gaussian/firetasks/run_calc.py` & `mispr-0.0.4/mispr/gaussian/firetasks/run_calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from mispr.gaussian.defaults import CUSTODIAN_MAX_ERRORS
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 @explicit_serialize
 class RunGaussianDirect(FiretaskBase):
     """
```

### Comparing `mispr-0.0.3/mispr/gaussian/firetasks/write_inputs.py` & `mispr-0.0.4/mispr/gaussian/firetasks/write_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pymatgen.analysis.local_env import OpenBabelNN
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 @explicit_serialize
 class WriteInput(FiretaskBase):
     """
     Write Gaussian input file for a molecule/cluster in the current
     working directory.
```

### Comparing `mispr-0.0.3/mispr/gaussian/fireworks/break_mol.py` & `mispr-0.0.4/mispr/gaussian/fireworks/break_mol.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 FIREWORK_KWARGS = Firework.__init__.__code__.co_varnames
 
 
 class BreakMolFW(Firework):
```

### Comparing `mispr-0.0.3/mispr/gaussian/fireworks/core.py` & `mispr-0.0.4/mispr/gaussian/fireworks/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from mispr.gaussian.firetasks.geo_transformation import ProcessMoleculeInput
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 FIREWORK_KWARGS = Firework.__init__.__code__.co_varnames
 
 
 def common_tasks(
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/db_utilities.py` & `mispr-0.0.4/mispr/gaussian/utilities/db_utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from mispr.gaussian.database import GaussianCalcDb
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def get_db(input_db=None):
     """
     Helper function to create a GaussianCalcDb instance from a file or
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/dbdoc.py` & `mispr-0.0.4/mispr/gaussian/utilities/dbdoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from mispr.gaussian.utilities.metadata import get_chem_schema
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def _job_types(gin):
     """
     Determines the type of the Gaussian job (e.g. opt, freq, etc.)
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/files.py` & `mispr-0.0.4/mispr/gaussian/utilities/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def bibtex_parser(bib_file, working_dir):
     """
     Parses a bibtex file and returns a dictionary of the entries.
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/fw_utilities.py` & `mispr-0.0.4/mispr/gaussian/utilities/fw_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __credits__ = "Anubhav Jain, Kiran Mathew"
 
 logger = logging.getLogger(__name__)
 
 
 def get_list_fireworks_and_tasks(
     workflow, firework_substring=None, task_substring=None
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/gout.py` & `mispr-0.0.4/mispr/gaussian/utilities/gout.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from mispr.gaussian.utilities.db_utilities import get_db
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def process_run(operation_type, run, input_file=None, **kwargs):
     """
     Processes a Gaussian run and returns a dictionary of the results.
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/inputs.py` & `mispr-0.0.4/mispr/gaussian/utilities/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from mispr.gaussian.defaults import STANDARD_OPT_GUASSIAN_INPUT
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def _add_solvent_inputs(
     gaussian_inputs, solvent_gaussian_inputs, solvent_properties=None
 ):
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/metadata.py` & `mispr-0.0.4/mispr/gaussian/utilities/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pymatgen.core.structure import Molecule
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def get_chem_schema(mol):
     """
     Returns a dictionary of chemical schema for a given molecule to use
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/misc.py` & `mispr-0.0.4/mispr/gaussian/utilities/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def pass_gout_dict(fw_spec, key):
     """
     Helper function used in the Gaussian Fireworks to pass Gaussian
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/mol.py` & `mispr-0.0.4/mispr/gaussian/utilities/mol.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from mispr.common.pubchem import PubChemRunner
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def process_mol(operation_type, mol, local_opt=False, **kwargs):
     """
     Processes a molecule. Used for handling different molecule formats
```

### Comparing `mispr-0.0.3/mispr/gaussian/utilities/rdkit.py` & `mispr-0.0.4/mispr/gaussian/utilities/rdkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from mispr.gaussian.utilities.mol import get_bond_order_str
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def get_rdkit_mol(mol, sanitize=True, remove_h=False):
     """
     Converts a pymatgen mol object to RDKit rdmol object. Uses RDKit to perform
```

### Comparing `mispr-0.0.3/mispr/gaussian/workflows/base/bde.py` & `mispr-0.0.4/mispr/gaussian/workflows/base/bde.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from mispr.gaussian.firetasks.parse_outputs import BDEtoDB
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 def get_bde(
     mol_operation_type,
     mol,
     ref_charge=0,
     fragment_charges=None,
```

### Comparing `mispr-0.0.3/mispr/gaussian/workflows/base/binding_energy.py` & `mispr-0.0.4/mispr/gaussian/workflows/base/binding_energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from mispr.gaussian.firetasks.parse_outputs import BindingEnergytoDB
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 logger = logging.getLogger(__name__)
 
 
 def get_binding_energies(
     mol_operation_type,
```

### Comparing `mispr-0.0.3/mispr/gaussian/workflows/base/core.py` & `mispr-0.0.4/mispr/gaussian/workflows/base/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from mispr.gaussian.firetasks.parse_outputs import ProcessRun
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 WORKFLOW_KWARGS = Workflow.__init__.__code__.co_varnames
 
 
 class GoutTypeError(Exception):
```

### Comparing `mispr-0.0.3/mispr/gaussian/workflows/base/esp.py` & `mispr-0.0.4/mispr/gaussian/workflows/base/esp.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from mispr.gaussian.firetasks.parse_outputs import ESPtoDB
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 def get_esp_charges(
     mol_operation_type,
     mol,
```

### Comparing `mispr-0.0.3/mispr/gaussian/workflows/base/ip_ea.py` & `mispr-0.0.4/mispr/gaussian/workflows/base/ip_ea.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from mispr.gaussian.firetasks.parse_outputs import IPEAtoDB
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 
 class Node:
     """
     Generates the fireworks corresponding to different molecule states
```

### Comparing `mispr-0.0.3/mispr/gaussian/workflows/base/nmr.py` & `mispr-0.0.4/mispr/gaussian/workflows/base/nmr.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from mispr.gaussian.firetasks.parse_outputs import NMRtoDB
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Jan 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 logger = logging.getLogger(__name__)
 
 
 def get_nmr_tensors(
     mol_operation_type,
```

### Comparing `mispr-0.0.3/mispr/hybrid/defaults.py` & `mispr-0.0.4/mispr/hybrid/defaults.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/hybrid/firetasks/nmr_from_md.py` & `mispr-0.0.4/mispr/hybrid/firetasks/nmr_from_md.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/hybrid/workflows/core.py` & `mispr-0.0.4/mispr/hybrid/workflows/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from mispr.gaussian.workflows.base.core import common_fw, WORKFLOW_KWARGS
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Oct 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 def run_hybrid_calcs(
     mol_operation_type,
     mol,
     mol_type,
     mol_data,
```

### Comparing `mispr-0.0.3/mispr/hybrid/workflows/nmr.py` & `mispr-0.0.4/mispr/hybrid/workflows/nmr.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from mispr.hybrid.firetasks.nmr_from_md import NMRFromMD
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Oct 2021"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 def get_solvation_structures_nmr(
     mol_operation_type,
     mol,
     mol_type,
     mol_data,
```

### Comparing `mispr-0.0.3/mispr/lammps/data/masses.json` & `mispr-0.0.4/mispr/lammps/data/masses.json`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/database.py` & `mispr-0.0.4/mispr/lammps/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from mispr.lammps.utilities.utilities import process_ff_doc
 
 __author__ = "Matthew Bliss"
 __maintainer__ = "Matthew Bliss"
 __email__ = "matthew.bliss@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Apr 2020"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger()
 ch = logging.StreamHandler(stream=sys.stdout)
 logger.addHandler(ch)
 logger.setLevel(20)
```

### Comparing `mispr-0.0.3/mispr/lammps/defaults.py` & `mispr-0.0.4/mispr/lammps/defaults.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/firetasks/parse_outputs.py` & `mispr-0.0.4/mispr/lammps/firetasks/parse_outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from mispr.gaussian.utilities.metadata import get_mol_formula
 
 __author__ = "Matthew Bliss"
 __maintainer__ = "Matthew Bliss"
 __email__ = "matthew.bliss@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Apr 2020"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 GAFF_DOI = "https://doi.org/10.1002/jcc.20035"
 
 
 @explicit_serialize
```

### Comparing `mispr-0.0.3/mispr/lammps/firetasks/run.py` & `mispr-0.0.4/mispr/lammps/firetasks/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from mispr.lammps.utilities.utilities import get_db, process_ff_doc, add_ff_labels_to_dict
 
 __author__ = "Matthew Bliss"
 __maintainer__ = "Matthew Bliss"
 __email__ = "matthew.bliss@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Apr 2020"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 CONFIG_PATH = os.path.normpath(
     os.path.join(
         os.path.dirname(os.path.abspath(__file__)), "..", "config", "config.ini"
     )
```

### Comparing `mispr-0.0.3/mispr/lammps/firetasks/write_inputs.py` & `mispr-0.0.4/mispr/lammps/firetasks/write_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from mispr.gaussian.utilities.metadata import get_chem_schema, get_mol_formula
 
 __author__ = "Matthew Bliss"
 __maintainer__ = "Matthew Bliss"
 __email__ = "matthew.bliss@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Apr 2020"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 TEMPLATE_DIR = os.path.normpath(
     os.path.join(os.path.dirname(os.path.abspath(__file__)), "..", "templates")
 )
 DEFAULT_KEY = "lammpsin_key"
```

### Comparing `mispr-0.0.3/mispr/lammps/fireworks/core.py` & `mispr-0.0.4/mispr/lammps/fireworks/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from mispr.lammps.firetasks.parse_outputs import GetRDF, CalcDiff, ProcessPrmtop
 
 __author__ = "Matthew Bliss"
 __maintainer__ = "Matthew Bliss"
 __email__ = "matthew.bliss@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Apr 2020"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 FIREWORK_KWARGS = Firework.__init__.__code__.co_varnames
 
 
 def ambertools_tasks(**kwargs):
```

### Comparing `mispr-0.0.3/mispr/lammps/templates/emin_gaff` & `mispr-0.0.4/mispr/lammps/templates/emin_gaff`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/templates/emin_general` & `mispr-0.0.4/mispr/lammps/templates/emin_general`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/templates/npt` & `mispr-0.0.4/mispr/lammps/templates/npt`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/templates/nvt` & `mispr-0.0.4/mispr/lammps/templates/nvt`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/antechamber.py` & `mispr-0.0.4/mispr/lammps/tests/antechamber.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/base_test.py` & `mispr-0.0.4/mispr/lammps/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/control.py` & `mispr-0.0.4/mispr/lammps/tests/control.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/custom_data_workflow.py` & `mispr-0.0.4/mispr/lammps/tests/custom_data_workflow.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/data.py` & `mispr-0.0.4/mispr/lammps/tests/data.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/database/operators-compound_queries.py` & `mispr-0.0.4/mispr/lammps/tests/database/operators-compound_queries.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/database/query_data.py` & `mispr-0.0.4/mispr/lammps/tests/database/query_data.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/database/update_data.py` & `mispr-0.0.4/mispr/lammps/tests/database/update_data.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/electrolyte_wf.py` & `mispr-0.0.4/mispr/lammps/tests/electrolyte_wf.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/esp_to_ff_dict_custom.py` & `mispr-0.0.4/mispr/lammps/tests/esp_to_ff_dict_custom.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/esp_to_ff_dict_function.py` & `mispr-0.0.4/mispr/lammps/tests/esp_to_ff_dict_function.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/liquid_wf_local.py` & `mispr-0.0.4/mispr/lammps/tests/liquid_wf_local.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/parmchk.py` & `mispr-0.0.4/mispr/lammps/tests/parmchk.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/prmtop.py` & `mispr-0.0.4/mispr/lammps/tests/prmtop.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/run_lammps.py` & `mispr-0.0.4/mispr/lammps/tests/run_lammps.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/SPC_E.pdb` & `mispr-0.0.4/mispr/lammps/tests/test_files/SPC_E.pdb`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/analysis/complex.data` & `mispr-0.0.4/mispr/lammps/tests/test_files/analysis/complex.data`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/analysis/d__diff.txt` & `mispr-0.0.4/mispr/lammps/tests/test_files/analysis/d__diff.txt`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/analysis/in.emin_complex.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/analysis/in.emin_complex.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/analysis/n__diff.txt` & `mispr-0.0.4/mispr/lammps/tests/test_files/analysis/n__diff.txt`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/analysis/o__diff.txt` & `mispr-0.0.4/mispr/lammps/tests/test_files/analysis/o__diff.txt`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/analysis/rdf.csv` & `mispr-0.0.4/mispr/lammps/tests/test_files/analysis/rdf.csv`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/analysis/w__diff.txt` & `mispr-0.0.4/mispr/lammps/tests/test_files/analysis/w__diff.txt`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/antechamber/dhps.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/antechamber/dhps.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/control/case_1.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/control/case_1.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/control/case_2.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/control/case_2.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/control/case_2_npt.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/control/case_2_npt.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/control/case_2_npt_group_list.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/control/case_2_npt_group_list.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/control/case_3.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/control/case_3.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/H2O2.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/H2O2.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5/ff.json` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5/ff.json`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5/leap.log` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5/leap.log`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5/tleap.in` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5/tleap.in`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/H5C12SN2O5.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/H5C12SN2O5.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/SPC_E.pdb` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/SPC_E.pdb`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/complex.data` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/complex.data`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/complex_from_concentration.data` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/complex_from_concentration.data`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER.ESP` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER.ESP`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP1.OUT` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP1.OUT`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP2.OUT` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ANTECHAMBER_RESP2.OUT`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/ATOMTYPE.INF` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/ATOMTYPE.INF`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H2O2.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.frcmod` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.frcmod`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.inpcrd` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.inpcrd`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.mol2` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.mol2`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/H5C12SN2O5.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/SPC_E.pdb` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/SPC_E.pdb`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/dhps.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/dhps.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/dhps.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/dhps.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/esout` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/esout`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/leap.log` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/leap.log`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/oh.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/oh.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/oh.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/oh.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/packed.xyz` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/packed.xyz`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/punch` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/punch`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/custom_workflow/tleap.in` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/custom_workflow/tleap.in`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/dhps.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/dhps.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/emin/complex.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/emin/complex.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/melt/complex.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/melt/complex.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/npt/complex.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/npt/complex.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/nvt_0-20/complex.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/nvt_0-20/complex.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/nvt_20-40/complex.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/nvt_20-40/complex.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/oh.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/oh.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/packed.xyz` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/packed.xyz`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/data/quench/complex.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/data/quench/complex.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/dhps.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/dhps.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/dhps.frcmod` & `mispr-0.0.4/mispr/lammps/tests/test_files/dhps.frcmod`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/dhps.inpcrd` & `mispr-0.0.4/mispr/lammps/tests/test_files/dhps.inpcrd`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/dhps.mol2` & `mispr-0.0.4/mispr/lammps/tests/test_files/dhps.mol2`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/dhps.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/dhps.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/dhps.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/dhps.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/H2O2.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/oh.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/oh.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H2O2/tleap.in` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H2O2/tleap.in`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.frcmod` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.frcmod`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.inpcrd` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.inpcrd`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.mol2` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.mol2`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/H5C12SN2O5.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/dhps.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/dhps.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/tleap.in` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/H5C12SN2O5/tleap.in`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/SPC_E.pdb` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/SPC_E.pdb`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/complex_from_concentration.data` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/complex_from_concentration.data`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/dhps.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/dhps.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/dhps.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/dhps.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/oh.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/oh.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/esp_to_data/oh.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/esp_to_data/oh.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/leap.log` & `mispr-0.0.4/mispr/lammps/tests/test_files/leap.log`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/SPC_E.pdb` & `mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/SPC_E.pdb`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/dhps.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/dhps.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/dhps.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/dhps.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/oh.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/oh.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/liquid_workflow/oh.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/liquid_workflow/oh.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/oh.esp` & `mispr-0.0.4/mispr/lammps/tests/test_files/oh.esp`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/oh.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/oh.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/parmchk/dhps.frcmod` & `mispr-0.0.4/mispr/lammps/tests/test_files/parmchk/dhps.frcmod`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/parmchk/dhps.mol2` & `mispr-0.0.4/mispr/lammps/tests/test_files/parmchk/dhps.mol2`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/prmtop/SPC_E.pdb` & `mispr-0.0.4/mispr/lammps/tests/test_files/prmtop/SPC_E.pdb`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/prmtop/dhps.out` & `mispr-0.0.4/mispr/lammps/tests/test_files/prmtop/dhps.out`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/prmtop/dhps.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/prmtop/dhps.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/run_lammps/test.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/run_lammps/test.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/run_lammps/test_npt.lammpsin` & `mispr-0.0.4/mispr/lammps/tests/test_files/run_lammps/test_npt.lammpsin`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/tleap/dhps.frcmod` & `mispr-0.0.4/mispr/lammps/tests/test_files/tleap/dhps.frcmod`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/tleap/dhps.inpcrd` & `mispr-0.0.4/mispr/lammps/tests/test_files/tleap/dhps.inpcrd`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/tleap/dhps.mol2` & `mispr-0.0.4/mispr/lammps/tests/test_files/tleap/dhps.mol2`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/test_files/tleap/dhps.prmtop` & `mispr-0.0.4/mispr/lammps/tests/test_files/tleap/dhps.prmtop`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/tests/tleap.py` & `mispr-0.0.4/mispr/lammps/tests/tleap.py`

 * *Files identical despite different names*

### Comparing `mispr-0.0.3/mispr/lammps/utilities/opls.py` & `mispr-0.0.4/mispr/lammps/utilities/opls.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from pymatgen.core.structure import Molecule
 
 __author__ = "Rasha Atwi"
 __maintainer__ = "Rasha Atwi"
 __email__ = "rasha.atwi@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Aug 2022"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 logger = logging.getLogger(__name__)
 
 NONBONDED_HEADER = "OPLSAA FORCE FIELD TYPE ASSIGNED\n"
 BONDS_HEADER = " Stretch            k            r0    quality         bt        comment\n"
 ANGLES_HEADER = " Bending                      k       theta0    quality   at  comment\n"
 DIHEDRALS_HEADER = " proper Torsion                     V1      V2      V3      V4    quality  tt  comment\n"
```

### Comparing `mispr-0.0.3/mispr/lammps/utilities/utilities.py` & `mispr-0.0.4/mispr/lammps/utilities/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from mispr.gaussian.utilities.fw_utilities import get_list_fireworks_and_tasks
 
 __author__ = "Matthew Bliss"
 __maintainer__ = "Matthew Bliss"
 __email__ = "matthew.bliss@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Apr 2020"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 def add_ff_labels_to_BADI_lists(ff_list, label):
     """
     Adds extra string to the end of all atom type labels in lists containing
     information about Bonds, Angles, Dihedrals, or Impropers (BADI). This
     function is intended to be used through the add_ff_labels_to_dict()
```

### Comparing `mispr-0.0.3/mispr/lammps/workflows/base.py` & `mispr-0.0.4/mispr/lammps/workflows/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 )
 
 __author__ = "Matthew Bliss"
 __maintainer__ = "Matthew Bliss"
 __email__ = "matthew.bliss@stonybrook.edu"
 __status__ = "Development"
 __date__ = "Apr 2020"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 
 def lammps_data_fws(
     system_species_data,
     system_mixture_type,
     box_data,
     box_data_type="cubic",
```

### Comparing `mispr-0.0.3/mispr.egg-info/PKG-INFO` & `mispr-0.0.4/mispr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mispr
-Version: 0.0.3
+Version: 0.0.4
 Summary: mispr contains FireWorks workflows for Materials Science
 Home-page: https://github.com/molmd/mispr
 Author: Rasha Atwi, Matthew Bliss
 Author-email: rasha.atwi@stonybrook.edu, matthew.bliss@stonybrook.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mispr-0.0.3/mispr.egg-info/SOURCES.txt` & `mispr-0.0.4/mispr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 docs/logo.png
 mispr/__init__.py
 mispr.egg-info/PKG-INFO
 mispr.egg-info/SOURCES.txt
 mispr.egg-info/dependency_links.txt
 mispr.egg-info/requires.txt
 mispr.egg-info/top_level.txt
+mispr/common/__init__.py
+mispr/common/pubchem.py
 mispr/gaussian/__init__.py
 mispr/gaussian/database.py
 mispr/gaussian/defaults.py
 mispr/gaussian/data/h_pot.bib
 mispr/gaussian/data/li_pot.bib
 mispr/gaussian/data/mg_pot.bib
 mispr/gaussian/firetasks/__init__.py
```

### Comparing `mispr-0.0.3/setup.py` & `mispr-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 module_dir = os.path.dirname(os.path.abspath(__file__))
 
 setuptools.setup(
     name="mispr",
-    version="0.0.3",
+    version="0.0.4",
     author="Rasha Atwi, Matthew Bliss",
     author_email="rasha.atwi@stonybrook.edu, matthew.bliss@stonybrook.edu",
     description="mispr contains FireWorks workflows for Materials Science",
     long_description=open(os.path.join(module_dir, "README.md")).read(),
     url="https://github.com/molmd/mispr",
     install_requires=[
         "numpy >= 1.21.1",
```

