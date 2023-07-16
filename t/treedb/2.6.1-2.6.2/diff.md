# Comparing `tmp/treedb-2.6.1.zip` & `tmp/treedb-2.6.2.zip`

## zipinfo {}

```diff
@@ -1,81 +1,81 @@
-Zip file size: 520336 bytes, number of entries: 79
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/treedb/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/treedb.egg-info/
--rw-rw-rw-  2.0 fat     1010 b- defN 23-Mar-20 19:04 treedb-2.6.1/fix-spaces.py
--rw-rw-rw-  2.0 fat     1107 b- defN 23-Mar-20 19:04 treedb-2.6.1/LICENSE.txt
--rw-rw-rw-  2.0 fat      728 b- defN 23-Mar-20 19:04 treedb-2.6.1/lint-code.py
--rw-rw-rw-  2.0 fat      232 b- defN 23-Mar-20 19:04 treedb-2.6.1/MANIFEST.in
--rw-rw-rw-  2.0 fat     8262 b- defN 23-Mar-20 19:16 treedb-2.6.1/PKG-INFO
--rw-rw-rw-  2.0 fat     6977 b- defN 23-Mar-20 19:04 treedb-2.6.1/README.rst
--rw-rw-rw-  2.0 fat       86 b- defN 23-Mar-20 19:04 treedb-2.6.1/requirements.txt
--rw-rw-rw-  2.0 fat     1577 b- defN 23-Mar-20 19:04 treedb-2.6.1/run-tests.py
--rw-rw-rw-  2.0 fat      450 b- defN 23-Mar-20 19:16 treedb-2.6.1/setup.cfg
--rw-rw-rw-  2.0 fat     1807 b- defN 23-Mar-20 19:16 treedb-2.6.1/setup.py
--rw-rw-rw-  2.0 fat   753223 b- defN 23-Mar-20 19:13 treedb-2.6.1/Stats.ipynb
--rw-rw-rw-  2.0 fat      165 b- defN 23-Mar-20 19:04 treedb-2.6.1/tox.ini
--rw-rw-rw-  2.0 fat     1129 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb.ini
--rw-rw-rw-  2.0 fat     1118 b- defN 23-Mar-20 19:04 treedb-2.6.1/try-treedb.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/tests/bare/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/tests/empty/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/tests/reads_repo/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/tests/writes_repo/
--rw-rw-rw-  2.0 fat     6662 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/conftest.py
--rw-rw-rw-  2.0 fat     1328 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/helpers.py
--rw-rw-rw-  2.0 fat      425 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/bare/test_backend_basics.py
--rw-rw-rw-  2.0 fat     2840 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/bare/test_backend_export_bare.py
--rw-rw-rw-  2.0 fat     2225 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/bare/test_fields.py
--rw-rw-rw-  2.0 fat     1007 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/bare/test_records.py
--rw-rw-rw-  2.0 fat     1162 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/empty/test_backend_sqlite_master.py
--rw-rw-rw-  2.0 fat     3606 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_backend_export_reads.py
--rw-rw-rw-  2.0 fat      163 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_backend_load.py
--rw-rw-rw-  2.0 fat     2325 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_backend_pandas.py
--rw-rw-rw-  2.0 fat      237 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_checks.py
--rw-rw-rw-  2.0 fat    12566 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_export_reads.py
--rw-rw-rw-  2.0 fat     7738 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_models.py
--rw-rw-rw-  2.0 fat     2738 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_queries.py
--rw-rw-rw-  2.0 fat     3855 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_raw_export.py
--rw-rw-rw-  2.0 fat      229 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/reads_repo/test_raw_records.py
--rw-rw-rw-  2.0 fat     1297 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/writes_repo/test_export_writes.py
--rw-rw-rw-  2.0 fat      688 b- defN 23-Mar-20 19:04 treedb-2.6.1/tests/writes_repo/test_files.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/treedb/backend/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/treedb/languoids/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-20 19:16 treedb-2.6.1/treedb/raw/
--rw-rw-rw-  2.0 fat     9244 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/checks.py
--rw-rw-rw-  2.0 fat      965 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/config.py
--rw-rw-rw-  2.0 fat    13507 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/export.py
--rw-rw-rw-  2.0 fat     3598 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/glottolog.py
--rw-rw-rw-  2.0 fat    13516 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/import_models.py
--rw-rw-rw-  2.0 fat     3458 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/logging_.py
--rw-rw-rw-  2.0 fat    45912 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/models.py
--rw-rw-rw-  2.0 fat    31207 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/queries.py
--rw-rw-rw-  2.0 fat     3241 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/settings.py
--rw-rw-rw-  2.0 fat     2965 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/_globals.py
--rw-rw-rw-  2.0 fat     4979 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/_proxies.py
--rw-rw-rw-  2.0 fat    17187 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/_tools.py
--rw-rw-rw-  2.0 fat     3143 b- defN 23-Mar-20 19:16 treedb-2.6.1/treedb/__init__.py
--rw-rw-rw-  2.0 fat    10786 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/backend/export.py
--rw-rw-rw-  2.0 fat     9885 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/backend/load.py
--rw-rw-rw-  2.0 fat     6110 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/backend/models.py
--rw-rw-rw-  2.0 fat     2436 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/backend/pandas.py
--rw-rw-rw-  2.0 fat     3942 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/backend/sqlite_master.py
--rw-rw-rw-  2.0 fat     2799 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/backend/views.py
--rw-rw-rw-  2.0 fat     5941 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/backend/_basics.py
--rw-rw-rw-  2.0 fat      560 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/backend/__init__.py
--rw-rw-rw-  2.0 fat     5321 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/languoids/fields.py
--rw-rw-rw-  2.0 fat     7761 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/languoids/files.py
--rw-rw-rw-  2.0 fat    25731 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/languoids/records.py
--rw-rw-rw-  2.0 fat     1124 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/languoids/_root.py
--rw-rw-rw-  2.0 fat      620 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/languoids/__init__.py
--rw-rw-rw-  2.0 fat     4520 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/raw/export.py
--rw-rw-rw-  2.0 fat     2886 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/raw/import_models.py
--rw-rw-rw-  2.0 fat     3006 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/raw/models.py
--rw-rw-rw-  2.0 fat     5149 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/raw/records.py
--rw-rw-rw-  2.0 fat      475 b- defN 23-Mar-20 19:04 treedb-2.6.1/treedb/raw/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Mar-20 19:16 treedb-2.6.1/treedb.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat     8262 b- defN 23-Mar-20 19:16 treedb-2.6.1/treedb.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      175 b- defN 23-Mar-20 19:16 treedb-2.6.1/treedb.egg-info/requires.txt
--rw-rw-rw-  2.0 fat     1611 b- defN 23-Mar-20 19:16 treedb-2.6.1/treedb.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-Mar-20 19:16 treedb-2.6.1/treedb.egg-info/top_level.txt
-79 files, 1090992 bytes uncompressed, 508890 bytes compressed:  53.4%
+Zip file size: 527193 bytes, number of entries: 79
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/treedb/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/treedb.egg-info/
+-rw-rw-rw-  2.0 fat     1010 b- defN 23-Jul-05 19:14 treedb-2.6.2/fix-spaces.py
+-rw-rw-rw-  2.0 fat     1107 b- defN 23-Jul-05 19:14 treedb-2.6.2/LICENSE.txt
+-rw-rw-rw-  2.0 fat      728 b- defN 23-Jul-05 19:14 treedb-2.6.2/lint-code.py
+-rw-rw-rw-  2.0 fat      232 b- defN 23-Jul-05 19:14 treedb-2.6.2/MANIFEST.in
+-rw-rw-rw-  2.0 fat     8249 b- defN 23-Jul-16 15:20 treedb-2.6.2/PKG-INFO
+-rw-rw-rw-  2.0 fat     6977 b- defN 23-Jul-05 19:14 treedb-2.6.2/README.rst
+-rw-rw-rw-  2.0 fat       86 b- defN 23-Jul-05 19:14 treedb-2.6.2/requirements.txt
+-rw-rw-rw-  2.0 fat     1577 b- defN 23-Jul-05 19:14 treedb-2.6.2/run-tests.py
+-rw-rw-rw-  2.0 fat      451 b- defN 23-Jul-16 15:20 treedb-2.6.2/setup.cfg
+-rw-rw-rw-  2.0 fat     1806 b- defN 23-Jul-16 15:20 treedb-2.6.2/setup.py
+-rw-rw-rw-  2.0 fat   769798 b- defN 23-Jul-16 15:14 treedb-2.6.2/Stats.ipynb
+-rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-16 13:22 treedb-2.6.2/tox.ini
+-rw-rw-rw-  2.0 fat     1129 b- defN 23-Jul-05 19:14 treedb-2.6.2/treedb.ini
+-rw-rw-rw-  2.0 fat     1118 b- defN 23-Jul-05 19:14 treedb-2.6.2/try-treedb.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/tests/bare/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/tests/empty/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/tests/reads_repo/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/tests/writes_repo/
+-rw-rw-rw-  2.0 fat     6662 b- defN 23-Jul-16 14:48 treedb-2.6.2/tests/conftest.py
+-rw-rw-rw-  2.0 fat     1349 b- defN 23-Jul-16 13:22 treedb-2.6.2/tests/helpers.py
+-rw-rw-rw-  2.0 fat      425 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/bare/test_backend_basics.py
+-rw-rw-rw-  2.0 fat     2840 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/bare/test_backend_export_bare.py
+-rw-rw-rw-  2.0 fat     2225 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/bare/test_fields.py
+-rw-rw-rw-  2.0 fat     1007 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/bare/test_records.py
+-rw-rw-rw-  2.0 fat     1162 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/empty/test_backend_sqlite_master.py
+-rw-rw-rw-  2.0 fat     3604 b- defN 23-Jul-16 14:48 treedb-2.6.2/tests/reads_repo/test_backend_export_reads.py
+-rw-rw-rw-  2.0 fat      163 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/reads_repo/test_backend_load.py
+-rw-rw-rw-  2.0 fat     2325 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/reads_repo/test_backend_pandas.py
+-rw-rw-rw-  2.0 fat      237 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/reads_repo/test_checks.py
+-rw-rw-rw-  2.0 fat    13111 b- defN 23-Jul-16 14:48 treedb-2.6.2/tests/reads_repo/test_export_reads.py
+-rw-rw-rw-  2.0 fat     7738 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/reads_repo/test_models.py
+-rw-rw-rw-  2.0 fat     2738 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/reads_repo/test_queries.py
+-rw-rw-rw-  2.0 fat     4171 b- defN 23-Jul-16 14:48 treedb-2.6.2/tests/reads_repo/test_raw_export.py
+-rw-rw-rw-  2.0 fat      229 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/reads_repo/test_raw_records.py
+-rw-rw-rw-  2.0 fat     1297 b- defN 23-Jul-05 19:14 treedb-2.6.2/tests/writes_repo/test_export_writes.py
+-rw-rw-rw-  2.0 fat      916 b- defN 23-Jul-16 14:48 treedb-2.6.2/tests/writes_repo/test_files.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/treedb/backend/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/treedb/languoids/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jul-16 15:20 treedb-2.6.2/treedb/raw/
+-rw-rw-rw-  2.0 fat     9262 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/checks.py
+-rw-rw-rw-  2.0 fat      974 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/config.py
+-rw-rw-rw-  2.0 fat    13505 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/export.py
+-rw-rw-rw-  2.0 fat     3629 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/glottolog.py
+-rw-rw-rw-  2.0 fat    13543 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/import_models.py
+-rw-rw-rw-  2.0 fat     3496 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/logging_.py
+-rw-rw-rw-  2.0 fat    45984 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/models.py
+-rw-rw-rw-  2.0 fat    31256 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/queries.py
+-rw-rw-rw-  2.0 fat     3247 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/settings.py
+-rw-rw-rw-  2.0 fat     2974 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/_globals.py
+-rw-rw-rw-  2.0 fat     5013 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/_proxies.py
+-rw-rw-rw-  2.0 fat    17247 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/_tools.py
+-rw-rw-rw-  2.0 fat     3143 b- defN 23-Jul-16 15:14 treedb-2.6.2/treedb/__init__.py
+-rw-rw-rw-  2.0 fat    10819 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/backend/export.py
+-rw-rw-rw-  2.0 fat     9924 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/backend/load.py
+-rw-rw-rw-  2.0 fat     6155 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/backend/models.py
+-rw-rw-rw-  2.0 fat     2445 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/backend/pandas.py
+-rw-rw-rw-  2.0 fat     3954 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/backend/sqlite_master.py
+-rw-rw-rw-  2.0 fat     2825 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/backend/views.py
+-rw-rw-rw-  2.0 fat     5956 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/backend/_basics.py
+-rw-rw-rw-  2.0 fat      560 b- defN 23-Jul-05 19:14 treedb-2.6.2/treedb/backend/__init__.py
+-rw-rw-rw-  2.0 fat     5350 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/languoids/fields.py
+-rw-rw-rw-  2.0 fat     7654 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/languoids/files.py
+-rw-rw-rw-  2.0 fat    25808 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/languoids/records.py
+-rw-rw-rw-  2.0 fat     1138 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/languoids/_root.py
+-rw-rw-rw-  2.0 fat      620 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/languoids/__init__.py
+-rw-rw-rw-  2.0 fat     4526 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/raw/export.py
+-rw-rw-rw-  2.0 fat     2898 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/raw/import_models.py
+-rw-rw-rw-  2.0 fat     3012 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/raw/models.py
+-rw-rw-rw-  2.0 fat     5147 b- defN 23-Jul-16 13:22 treedb-2.6.2/treedb/raw/records.py
+-rw-rw-rw-  2.0 fat      475 b- defN 23-Jul-05 19:14 treedb-2.6.2/treedb/raw/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jul-16 15:20 treedb-2.6.2/treedb.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat     8249 b- defN 23-Jul-16 15:20 treedb-2.6.2/treedb.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      175 b- defN 23-Jul-16 15:20 treedb-2.6.2/treedb.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat     1611 b- defN 23-Jul-16 15:20 treedb-2.6.2/treedb.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-16 15:20 treedb-2.6.2/treedb.egg-info/top_level.txt
+79 files, 1109215 bytes uncompressed, 515747 bytes compressed:  53.5%
```

## zipnote {}

```diff
@@ -1,238 +1,238 @@
-Filename: treedb-2.6.1/
+Filename: treedb-2.6.2/
 Comment: 
 
-Filename: treedb-2.6.1/tests/
+Filename: treedb-2.6.2/tests/
 Comment: 
 
-Filename: treedb-2.6.1/treedb/
+Filename: treedb-2.6.2/treedb/
 Comment: 
 
-Filename: treedb-2.6.1/treedb.egg-info/
+Filename: treedb-2.6.2/treedb.egg-info/
 Comment: 
 
-Filename: treedb-2.6.1/fix-spaces.py
+Filename: treedb-2.6.2/fix-spaces.py
 Comment: 
 
-Filename: treedb-2.6.1/LICENSE.txt
+Filename: treedb-2.6.2/LICENSE.txt
 Comment: 
 
-Filename: treedb-2.6.1/lint-code.py
+Filename: treedb-2.6.2/lint-code.py
 Comment: 
 
-Filename: treedb-2.6.1/MANIFEST.in
+Filename: treedb-2.6.2/MANIFEST.in
 Comment: 
 
-Filename: treedb-2.6.1/PKG-INFO
+Filename: treedb-2.6.2/PKG-INFO
 Comment: 
 
-Filename: treedb-2.6.1/README.rst
+Filename: treedb-2.6.2/README.rst
 Comment: 
 
-Filename: treedb-2.6.1/requirements.txt
+Filename: treedb-2.6.2/requirements.txt
 Comment: 
 
-Filename: treedb-2.6.1/run-tests.py
+Filename: treedb-2.6.2/run-tests.py
 Comment: 
 
-Filename: treedb-2.6.1/setup.cfg
+Filename: treedb-2.6.2/setup.cfg
 Comment: 
 
-Filename: treedb-2.6.1/setup.py
+Filename: treedb-2.6.2/setup.py
 Comment: 
 
-Filename: treedb-2.6.1/Stats.ipynb
+Filename: treedb-2.6.2/Stats.ipynb
 Comment: 
 
-Filename: treedb-2.6.1/tox.ini
+Filename: treedb-2.6.2/tox.ini
 Comment: 
 
-Filename: treedb-2.6.1/treedb.ini
+Filename: treedb-2.6.2/treedb.ini
 Comment: 
 
-Filename: treedb-2.6.1/try-treedb.py
+Filename: treedb-2.6.2/try-treedb.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/bare/
+Filename: treedb-2.6.2/tests/bare/
 Comment: 
 
-Filename: treedb-2.6.1/tests/empty/
+Filename: treedb-2.6.2/tests/empty/
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/
+Filename: treedb-2.6.2/tests/reads_repo/
 Comment: 
 
-Filename: treedb-2.6.1/tests/writes_repo/
+Filename: treedb-2.6.2/tests/writes_repo/
 Comment: 
 
-Filename: treedb-2.6.1/tests/conftest.py
+Filename: treedb-2.6.2/tests/conftest.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/helpers.py
+Filename: treedb-2.6.2/tests/helpers.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/bare/test_backend_basics.py
+Filename: treedb-2.6.2/tests/bare/test_backend_basics.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/bare/test_backend_export_bare.py
+Filename: treedb-2.6.2/tests/bare/test_backend_export_bare.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/bare/test_fields.py
+Filename: treedb-2.6.2/tests/bare/test_fields.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/bare/test_records.py
+Filename: treedb-2.6.2/tests/bare/test_records.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/empty/test_backend_sqlite_master.py
+Filename: treedb-2.6.2/tests/empty/test_backend_sqlite_master.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_backend_export_reads.py
+Filename: treedb-2.6.2/tests/reads_repo/test_backend_export_reads.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_backend_load.py
+Filename: treedb-2.6.2/tests/reads_repo/test_backend_load.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_backend_pandas.py
+Filename: treedb-2.6.2/tests/reads_repo/test_backend_pandas.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_checks.py
+Filename: treedb-2.6.2/tests/reads_repo/test_checks.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_export_reads.py
+Filename: treedb-2.6.2/tests/reads_repo/test_export_reads.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_models.py
+Filename: treedb-2.6.2/tests/reads_repo/test_models.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_queries.py
+Filename: treedb-2.6.2/tests/reads_repo/test_queries.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_raw_export.py
+Filename: treedb-2.6.2/tests/reads_repo/test_raw_export.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/reads_repo/test_raw_records.py
+Filename: treedb-2.6.2/tests/reads_repo/test_raw_records.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/writes_repo/test_export_writes.py
+Filename: treedb-2.6.2/tests/writes_repo/test_export_writes.py
 Comment: 
 
-Filename: treedb-2.6.1/tests/writes_repo/test_files.py
+Filename: treedb-2.6.2/tests/writes_repo/test_files.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/
+Filename: treedb-2.6.2/treedb/backend/
 Comment: 
 
-Filename: treedb-2.6.1/treedb/languoids/
+Filename: treedb-2.6.2/treedb/languoids/
 Comment: 
 
-Filename: treedb-2.6.1/treedb/raw/
+Filename: treedb-2.6.2/treedb/raw/
 Comment: 
 
-Filename: treedb-2.6.1/treedb/checks.py
+Filename: treedb-2.6.2/treedb/checks.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/config.py
+Filename: treedb-2.6.2/treedb/config.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/export.py
+Filename: treedb-2.6.2/treedb/export.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/glottolog.py
+Filename: treedb-2.6.2/treedb/glottolog.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/import_models.py
+Filename: treedb-2.6.2/treedb/import_models.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/logging_.py
+Filename: treedb-2.6.2/treedb/logging_.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/models.py
+Filename: treedb-2.6.2/treedb/models.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/queries.py
+Filename: treedb-2.6.2/treedb/queries.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/settings.py
+Filename: treedb-2.6.2/treedb/settings.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/_globals.py
+Filename: treedb-2.6.2/treedb/_globals.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/_proxies.py
+Filename: treedb-2.6.2/treedb/_proxies.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/_tools.py
+Filename: treedb-2.6.2/treedb/_tools.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/__init__.py
+Filename: treedb-2.6.2/treedb/__init__.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/export.py
+Filename: treedb-2.6.2/treedb/backend/export.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/load.py
+Filename: treedb-2.6.2/treedb/backend/load.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/models.py
+Filename: treedb-2.6.2/treedb/backend/models.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/pandas.py
+Filename: treedb-2.6.2/treedb/backend/pandas.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/sqlite_master.py
+Filename: treedb-2.6.2/treedb/backend/sqlite_master.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/views.py
+Filename: treedb-2.6.2/treedb/backend/views.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/_basics.py
+Filename: treedb-2.6.2/treedb/backend/_basics.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/backend/__init__.py
+Filename: treedb-2.6.2/treedb/backend/__init__.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/languoids/fields.py
+Filename: treedb-2.6.2/treedb/languoids/fields.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/languoids/files.py
+Filename: treedb-2.6.2/treedb/languoids/files.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/languoids/records.py
+Filename: treedb-2.6.2/treedb/languoids/records.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/languoids/_root.py
+Filename: treedb-2.6.2/treedb/languoids/_root.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/languoids/__init__.py
+Filename: treedb-2.6.2/treedb/languoids/__init__.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/raw/export.py
+Filename: treedb-2.6.2/treedb/raw/export.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/raw/import_models.py
+Filename: treedb-2.6.2/treedb/raw/import_models.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/raw/models.py
+Filename: treedb-2.6.2/treedb/raw/models.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/raw/records.py
+Filename: treedb-2.6.2/treedb/raw/records.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb/raw/__init__.py
+Filename: treedb-2.6.2/treedb/raw/__init__.py
 Comment: 
 
-Filename: treedb-2.6.1/treedb.egg-info/dependency_links.txt
+Filename: treedb-2.6.2/treedb.egg-info/dependency_links.txt
 Comment: 
 
-Filename: treedb-2.6.1/treedb.egg-info/PKG-INFO
+Filename: treedb-2.6.2/treedb.egg-info/PKG-INFO
 Comment: 
 
-Filename: treedb-2.6.1/treedb.egg-info/requires.txt
+Filename: treedb-2.6.2/treedb.egg-info/requires.txt
 Comment: 
 
-Filename: treedb-2.6.1/treedb.egg-info/SOURCES.txt
+Filename: treedb-2.6.2/treedb.egg-info/SOURCES.txt
 Comment: 
 
-Filename: treedb-2.6.1/treedb.egg-info/top_level.txt
+Filename: treedb-2.6.2/treedb.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `treedb-2.6.1/fix-spaces.py` & `treedb-2.6.2/fix-spaces.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/LICENSE.txt` & `treedb-2.6.2/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/lint-code.py` & `treedb-2.6.2/lint-code.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/PKG-INFO` & `treedb-2.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treedb
-Version: 2.6.1
+Version: 2.6.2
 Summary: Glottolog languoid tree as SQLite database
 Home-page: https://github.com/glottolog/treedb
 Author: Sebastian Bank
 Author-email: sebastian.bank@uni-leipzig.de
 License: MIT
 Project-URL: Changelog, https://github.com/glottolog/treedb/blob/master/CHANGES.rst
 Project-URL: Issue Tracker, https://github.com/glottolog/treedb/issues
@@ -14,20 +14,20 @@
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: pretty
 Provides-Extra: pandas
 License-File: LICENSE.txt
 
 Glottolog ``treedb``
```

## Comparing `treedb-2.6.1/README.rst` & `treedb-2.6.2/README.rst`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/run-tests.py` & `treedb-2.6.2/run-tests.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/setup.py` & `treedb-2.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import pathlib
 from setuptools import setup, find_packages
 
 setup(
     name='treedb',
-    version='2.6.1',
+    version='2.6.2',
     author='Sebastian Bank',
     author_email='sebastian.bank@uni-leipzig.de',
     description='Glottolog languoid tree as SQLite database',
     keywords='glottolog languoids sqlite3 database',
     license='MIT',
     url='https://github.com/glottolog/treedb',
     project_urls={
         'Changelog': 'https://github.com/glottolog/treedb/blob/master/CHANGES.rst',
         'Issue Tracker': 'https://github.com/glottolog/treedb/issues',
         'CI': 'https://github.com/glottolog/treedb/actions',
         'Coverage': 'https://codecov.io/gh/glottolog/treedb',
     },
     packages=find_packages(),
     platforms='any',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'csv23~=0.3',
         'pycountry==22.3.5',  # date-based versioning scheme
         'sqlalchemy>=1.4.24',
     ],
     extras_require={
         'dev': ['tox>=3', 'flake8', 'pep8-naming', 'wheel', 'twine'],
         'test': ['pytest>=6', 'pytest-cov', 'coverage'],
         'pretty': ['sqlparse>=0.3'],
         'pandas': ['pandas>=1'],
     },
     long_description=pathlib.Path('README.rst').read_text(encoding='utf-8'),
+    long_description_content_type='text/x-rst',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
```

## Comparing `treedb-2.6.1/treedb.ini` & `treedb-2.6.2/treedb.ini`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/try-treedb.py` & `treedb-2.6.2/try-treedb.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/tests/conftest.py` & `treedb-2.6.2/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """``pytest`` command-line options and fixtures."""
 
 import os
 import string
 
 import pytest
 
-DEFAULT_GLOTTOLOG_TAG = 'v4.7'
+DEFAULT_GLOTTOLOG_TAG = 'v4.8'
 
 RUN_WRITES = '--run-writes'
 
 SKIP_SLOW = '--skip-slow'
 
 SKIP_PANDAS = '--skip-pandas'
```

## Comparing `treedb-2.6.1/tests/helpers.py` & `treedb-2.6.2/tests/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import itertools
 
 MB = 2**20
 
 
-def pairwise(iterable):
+def pairwise(iterable, /):
     a, b = itertools.tee(iterable)
     next(b, None)
     return zip(a, b)
 
 
-def get_assert_head(items, *, n):
+def get_assert_head(items, /, *, n):
     head = list(itertools.islice(items, n))
 
     assert head
     assert len(head) == n
 
     return head
 
 
-def assert_nonempty_string(obj):
+def assert_nonempty_string(obj, /):
     assert obj is not None
     assert isinstance(obj, str)
 
 
-def assert_nonempty_string_tuple(obj):
+def assert_nonempty_string_tuple(obj, /):
     assert obj is not None
     assert isinstance(obj, tuple)
     assert all(isinstance(o, str) for o in obj)
     assert obj
     assert all(obj)
 
 
-def assert_nonempty_dict(obj):
+def assert_nonempty_dict(obj, /):
     assert obj is not None
     assert isinstance(obj, dict)
     assert obj
 
 
-def assert_file_size_between(path, min, max, *, unit=MB):
+def assert_file_size_between(path, /, min, max, *, unit=MB):
     assert path is not None
     assert path.exists()
     assert path.is_file()
     assert min * unit <= path.stat().st_size <= max * unit
 
 
-def assert_valid_languoids(items, *, n):
+def assert_valid_languoids(items, /, *, n):
     for path, languoid in get_assert_head(items, n=n):
         assert_nonempty_string_tuple(path)
         assert_nonempty_dict(languoid)
 
         for key in ('id', 'level', 'name'):
             assert_nonempty_string(languoid[key])
```

## Comparing `treedb-2.6.1/tests/bare/test_backend_export_bare.py` & `treedb-2.6.2/tests/bare/test_backend_export_bare.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/tests/bare/test_fields.py` & `treedb-2.6.2/tests/bare/test_fields.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/tests/bare/test_records.py` & `treedb-2.6.2/tests/bare/test_records.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/tests/empty/test_backend_sqlite_master.py` & `treedb-2.6.2/tests/empty/test_backend_sqlite_master.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/tests/reads_repo/test_backend_export_reads.py` & `treedb-2.6.2/tests/reads_repo/test_backend_export_reads.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import sys
-
 import pytest
 import sqlalchemy as sa
 
 from helpers import assert_file_size_between
 
 QUERY_HASH = {'master': None,
+              'v4.8': '705b1e4e30c35c659e536f0b41dc2c4197c72037b2c8eec7af20c3bf9ef4c992',
               'v4.7': 'e1054be01c4e17150e875d1cab40c754c0e1aeb3b5343a36c5771d3587115537',
               'v4.6': '4479476b397fa7dfbfd560a4bef5be06513ddc54f7c103d1f565e3a26404a90f',
               'v4.5': 'b36b5cdc7508b8c2843a3c93ff536ead9b4b63cdf80679f70993a5dd524a8926',
               'v4.4': '224691678e1f2e18406d6dd1a278e062c683ac12ec2acf57d501931d3661142e',
               'v4.3-treedb-fixes': 'bf8af9e4840642f4622cec41bf3156afac75317740ff0eef1ac75ec1998d4f78',
               'v4.2.1': '25222b4feb2d89b4edaeecc546280a059ae6ba69da961d56ee4a387ba3b81fc0',
               'v4.1': '55e9cab42b012048ae9f6c08353752fded7054bf531039979c6803ede54b95ac'}
@@ -21,15 +20,14 @@
     out, err = capsys.readouterr()
     assert not err
 
     assert out.startswith("git describe '")
 
 
 @pytest.mark.slow
-@pytest.mark.skipif(sys.version_info < (3, 7), reason='requires Python 3.7+')
 def test_backup(treedb):
     path = treedb.engine.file_with_suffix('.backup.sqlite3')
 
     engine = treedb.backup(path.name)
 
     assert engine.url.database == path.name
     assert_file_size_between(path, 10, 200)
```

## Comparing `treedb-2.6.1/tests/reads_repo/test_backend_pandas.py` & `treedb-2.6.2/tests/reads_repo/test_backend_pandas.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/tests/reads_repo/test_export_reads.py` & `treedb-2.6.2/tests/reads_repo/test_export_reads.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,43 @@
                      assert_valid_languoids)
 
 PREFIX = 'path_languoid:path:sha256:'
 
 PREFIX_ID = 'path_languoid:id:sha256:'
 
 CHECKSUM = {'master': None,
+            'v4.8': '66b901e25048a86758798657f4a940b29208b971f4384314c07f8c574788bee8',
             'v4.7': 'bd2be4c0a0463c85a01e287cf12f1d73041cc775f26d6a5d69a419ed0f7aad09',
             'v4.6': '3e07ebd1d58f84604dab5f717dfcd2745b8dd37adbecab61a6bfdcb4b9e85d1c',
             'v4.5': '308e0e142683b5365d36dacb57cc22926d60c9d4b061eba6d58829b75b8843cb',
             'v4.4': '289247f73d5bf57f0a7dc8e0e2473b5625ace605dbad57b3c06fe93063d47599',
             'v4.3-treedb-fixes': '54b468c7310fdd958b2b17fe439ee47c00d211498b405a5bd74b2920f68e3969',
             'v4.2.1': '9e19d66c95a43f595a8ea0b72ba6e7e293e02faf66978b63dda8ddba7d37e3f6',
             'v4.1': '9b795566bd7f5ccb10e0cb4f5e5be10b5ccce496d9816728b904f41b75cdd55a'}
 
 STATS = {'master': None,
+         'v4.8': '''\
+26,669 languoids
+   245 families
+   184 isolates
+   429 roots
+ 8,595 languages
+ 4,467 subfamilies
+13,362 dialects
+ 7,654 Spoken L1 Languages
+   223 Sign Language
+   121 Unclassifiable
+    84 Pidgin
+    68 Unattested
+    31 Artificial Language
+     9 Mixed Language
+    15 Speech Register
+ 8,205 All
+   390 Bookkeeping
+''',
          'v4.7': '''\
 26,416 languoids
    245 families
    184 isolates
    429 roots
  8,572 languages
  4,425 subfamilies
@@ -286,48 +306,59 @@
         assert not df.empty
         assert df.index.name == 'id'
         assert list(df.columns) == ['path', 'languoid']
         assert df.index.is_unique
         df.info(memory_usage='deep')
 
 
-xfail_master_unnormalized = pytest.mark.xfail_glottolog_tag('master', reason='possibly unnormalized master',
-                                                            raises=AssertionError)
+xfail_master_unnormalized = pytest.mark.xfail_glottolog_tag(
+    'master', reason='possibly unnormalized master',
+    raises=AssertionError)
+
+
+xfail_4_8_empty_altnames_elcat = pytest.mark.xfail_glottolog_tag(
+    'v4.8', reason='empty v4.8 altnames',
+    # https://github.com/glottolog/glottolog/pull/980
+    raises=AssertionError)
 
 
-xfail_empty_altnames_elcat = pytest.mark.xfail_glottolog_tag('v4.5', reason='empty altnames',
-                                                             # https://github.com/glottolog/glottolog/pull/79
-                                                             raises=AssertionError)
+xfail_4_5_empty_altnames_elcat = pytest.mark.xfail_glottolog_tag(
+    'v4.5', reason='empty v4.4 altnames',
+    # https://github.com/glottolog/glottolog/pull/795
+    raises=AssertionError)
 
 
-xfail_float_normalization = pytest.mark.xfail_glottolog_tag('v4.1', reason='float normalization',
-                                                            # https://github.com/glottolog/glottolog/pull/495
-                                                            raises=AssertionError)
+xfail_4_1_float_normalization = pytest.mark.xfail_glottolog_tag(
+    'v4.1', reason='missing v4.1 float normalization',
+    # https://github.com/glottolog/glottolog/pull/495
+    raises=AssertionError)
 
 
 @pytest.mark.parametrize(
     'kwargs',
     [pytest.param([{'source': 'files'},
                    {'source': 'raw'},
                    {'source': 'tables'}],
                   id='files, raw, tables',
                   marks=[xfail_master_unnormalized,
-                         xfail_empty_altnames_elcat,
-                         xfail_float_normalization]),
+                         xfail_4_8_empty_altnames_elcat,
+                         xfail_4_5_empty_altnames_elcat,
+                         xfail_4_1_float_normalization]),
      pytest.param([{'source': 'raw', 'order_by': 'id'},
                    {'source': 'tables', 'order_by': 'id'}],
                   id='raw(order_by=id), tables(order_by=id)',
                   marks=[xfail_master_unnormalized,
-                         xfail_float_normalization]),
+                         xfail_4_8_empty_altnames_elcat,
+                         xfail_4_1_float_normalization]),
      pytest.param([{'source': 'files', 'limit': 100,
                     'expected_prefix': 'path_languoid:path[limit=100]:sha256:'},
                    {'source': 'raw', 'order_by': 'file', 'limit': 100,
                     'expected_prefix': 'path_languoid:file[limit=100]:sha256:'}],
                   id='files(limit=100), raw(order_by=file, limit=100)',
-                  marks=[xfail_empty_altnames_elcat])])
+                  marks=[xfail_4_5_empty_altnames_elcat])])
 def test_checksum_equivalence(pytestconfig, treedb, kwargs):
     """Test for equivalence of the serialization from different sources.
 
     - from the md.ini files ('files')
     - from the file lines loaded into raw tables  ('raw')
     - from the parsed table contents ('tables')
```

## Comparing `treedb-2.6.1/tests/reads_repo/test_models.py` & `treedb-2.6.2/tests/reads_repo/test_models.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/tests/reads_repo/test_queries.py` & `treedb-2.6.2/tests/reads_repo/test_queries.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/tests/reads_repo/test_raw_export.py` & `treedb-2.6.2/tests/reads_repo/test_raw_export.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 
 from helpers import assert_file_size_between
 
-CHECKSUM = {('v4.7', False): 'strong:sha256:a54b735866b496fa5d508d2037d7a6a6452680eb0fc04f4c564f188a8e847def',
+CHECKSUM = {('v4.8', False): 'strong:sha256:f7f31bc8e8e6087bb64d24d7e88fa1c9dc3570ec279174b2c78c0fd91011168e',
+            ('v4.8', True): 'weak:sha256:fd231ffb2a44ac6ed979d5e8050aafe6fd49f8e6d53e0499755d1f81a2194f5d',
+            ('v4.7', False): 'strong:sha256:a54b735866b496fa5d508d2037d7a6a6452680eb0fc04f4c564f188a8e847def',
             ('v4.7', True): 'weak:sha256:838d735b87dc23da491e89f76fddd7766e9b392963f581788fcc9c5e4ed51161',
             ('v4.6', False): 'strong:sha256:fcc129dbfedc77a8238565e4e12eb53198e70dda9f6613c7f467e5b057dc04ca',
             ('v4.6', True): 'weak:sha256:1610520f11227a5489b44693b14a5d8db423d66d7ace391c2db221a56036457a',
             ('v4.5', False): 'strong:sha256:dda5285990cf8818c217a3dfc03799f2f7a091139a2de6ba08cd0fd18b8f3b94',
             ('v4.5', True): 'weak:sha256:8e56dab63dacb3d1b44e85c55ec3ea04dee8754d8a89e9542fd69df2a0e2f28b',
             ('v4.4', False): 'strong:sha256:3c95e5081c8d689980637506e363f99904798aa1a5ceb69eb1187b8eaff53709',
             ('v4.4', True): 'weak:sha256:690dd35d5de6a0841f3d3f8cc8c9853382797c73e082a418c1b9ad77bd7495bb',
@@ -15,14 +17,15 @@
             ('v4.2.1', False): 'strong:sha256:03ae265f46c79a5fd9ae44ada3ed50840dbdb897384b7ac57456ba12b6206a71',  # noqa: E501
             ('v4.2.1', True): 'weak:sha256:9cf661e51d8cd6d8ef1f5e93dbbf4612a8a7e06712c56747d7a280b2d83f503b',
             ('v4.1', False): 'strong:sha256:1d5a043b6cff9b2adb073e94eb67f5d4789b3b8f215c1eb7a3f26d0d1858d90a',
             ('v4.1', True): 'weak:sha256:2380ef917237713ac2d6710c05bb62648f9dafa40024550906674a5135d05e3b',
             ('v4.1', 'unordered'): 'unordered:sha256:dc6ed1762d47dec12432b09e0d1a1159153f062893bd884e8f21ec6b9e42d6c8'}  # noqa: E501
 
 RAW_CSV_SHA256 = {'master': None,
+                  'v4.8': '0f1b646c5bc9f3a454e8516d9a0288b086bb8acba673b94c1a4942d3a5d1bdaa',
                   'v4.7': '2b03bfdc8226e0cd0736a227fd74b7e04a511a198b102b70920af3c9f6194529',
                   'v4.6': '5a792c56de62db2695ef29d2344b60196d40d6307acab2a8b72f2b73681ec0b9',
                   'v4.5': '7c8a101b40c41629e6dfd6f5e5bfb627d3b8bc0e85a4444c7f9cff0ad4dbf1c9',
                   'v4.4': 'ad0c5a84f36815d25d053649bf2362097283e04b80d336bf4edb1c5ff1795bf6',
                   'v4.3-treedb-fixes': '1ef6923a94d19c708fd0e7ae87b6ee24c69d1d82fa9f81b16eaa5067e61ab1b6',
                   'v4.2.1': 'ab9d4339f3c0fa3acb0faf0f7306dc5409640ecd46e451de9a76445519f5157e',
                   'v4.1': '963163852e7f4ee34b516bc459bdbb908f2f4aab64bda58087a1a23a731921fd'}
```

## Comparing `treedb-2.6.1/tests/writes_repo/test_export_writes.py` & `treedb-2.6.2/tests/writes_repo/test_export_writes.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/treedb/checks.py` & `treedb-2.6.2/treedb/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 __all__ = ['check',
            'compare_languoids']
 
 
 log = logging.getLogger(__name__)
 
 
-def check(func=None, *, bind=_globals.ENGINE):
+def check(func=None, /, *, bind=_globals.ENGINE):
     """Run consistency/sanity checks on database."""
     if func is not None:
         try:
             check.registered.append(func)
         except AttributeError:
             check.registered = [func]
         return func
@@ -54,19 +54,19 @@
     return passed
 
 
 class Check(object):
 
     detail = True
 
-    def __init__(self, session, **kwargs):
+    def __init__(self, session, /, **kwargs):
         self.session = session
         self.query = self.invalid_query(**kwargs)
 
-    def invalid_query(self, **kwargs):  # pragma: no cover
+    def invalid_query(self, /, **kwargs):  # pragma: no cover
         raise NotImplementedError
 
     def validate(self):
         query = (self.query
                  .with_only_columns(sa.func.count().label('invalid_count'))
                  .order_by(None))
 
@@ -90,15 +90,15 @@
             msg = (f'{self.invalid_count:d} invalid\n'
                    f'    (violating {self.__doc__})')
         else:
             msg = 'OK'
         return f'{self.__class__.__name__}: {msg}'
 
     @staticmethod
-    def show_detail(invalid, invalid_count, number=25):  # pragma: no cover
+    def show_detail(invalid, invalid_count, /, *, number=25):  # pragma: no cover
         ids = (i.id for i in itertools.islice(invalid, number))
         cont = ', ...' if number < invalid_count else ''
         print(f"    {', '.join(ids)}{cont}")
 
 
 def docformat(func):
     sig = inspect.signature(func)
@@ -269,15 +269,15 @@
     from .raw import File, Value
 
     return (sa.select(File)
             .select_from(File)
             .where(~sa.exists().where(Value.file_id == File.id)))
 
 
-def compare_languoids(left_source: str = 'files', right_source: str = 'raw',
+def compare_languoids(left_source: str = 'files', right_source: str = 'raw', /,
                       *, order_by: str = _globals.LANGUOID_ORDER):  # pragma: no cover
     from . import export
 
     def compare(left, right):
         same = True
         for lt, rt in itertools.zip_longest(left, right):
             if lt != rt:
```

## Comparing `treedb-2.6.1/treedb/config.py` & `treedb-2.6.2/treedb/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 
 CONFIG_IN_ROOT = _tools.path_from_filename('config')
 
 
 log = logging.getLogger(__name__)
 
 
-def get_config_path(root=_globals.ROOT,
-                    *, configpath=CONFIG_IN_ROOT):
+def get_config_path(root=_globals.ROOT, /, *,
+                    configpath=CONFIG_IN_ROOT):
     return _languoids.get_repo_root(root) / configpath
 
 
-def iterconfigs(root=_globals.ROOT, *, glob='*.ini'):
+def iterconfigs(root=_globals.ROOT, /, *, glob='*.ini'):
     for path in get_config_path().glob(glob):
         yield path.name, load_config(path)
 
 
-def load_config(filepath, *, sort_sections: bool = False
+def load_config(filepath, /, *, sort_sections: bool = False
                 ) -> typing.Dict[str, typing.Dict[str, str]]:
     log.debug('open config file from path: %r', filepath)
     cfg = _tools.ConfigParser.from_file(filepath)
 
     log.debug('parsed %d section: %r', len(cfg), cfg)
     return cfg.to_dict(sort_sections=sort_sections)
```

## Comparing `treedb-2.6.1/treedb/export.py` & `treedb-2.6.2/treedb/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         parts_sum = sum(values)
         term = ' + '.join(f'{v:,d} {p}' for p, v in zip(parts, values))
         log.debug('verify %s == %d %s', term, counts[total], total)
         if counts[total] != parts_sum:  # pragma: no cover
             warnings.warn(f'{term} = {parts_sum:,d}')
 
 
-def iterlanguoids(source: str = 'files',
-                  *, limit: typing.Optional[int] = None,
+def iterlanguoids(source: str = 'files', /, *,
+                  limit: typing.Optional[int] = None,
                   offset: typing.Optional[int] = 0,
                   order_by: str = _globals.LANGUOID_ORDER,
                   progress_after: int = _tools.PROGRESS_AFTER,
                   root=_globals.ROOT, bind=_globals.ENGINE,
                   ) -> typing.Iterable[_globals.LanguoidItem]:
     """Yield (path, languoid) pairs from diffferent sources."""
     log.info('generate languoids from %r', source)
@@ -96,16 +96,16 @@
                                order_by=order_by,
                                progress_after=progress_after,
                                bind=bind)
     else:  # pragma: no cover
         raise ValueError(f'unknown source: {source!r}')
 
 
-def checksum(source: str = 'tables',
-             *, limit: typing.Optional[int] = None,
+def checksum(source: str = 'tables', *,
+             limit: typing.Optional[int] = None,
              offset: typing.Optional[int] = 0,
              order_by: str = _globals.LANGUOID_ORDER,
              hash_name: str = _globals.DEFAULT_HASH,
              bind=_globals.ENGINE):
     """Return checksum over source."""
     log.info('hash languoids json lines from %r ordered by %r with %r',
              source, order_by, hash_name)
@@ -115,25 +115,25 @@
                                             source=source,
                                             limit=limit,
                                             offset=offset,
                                             order_by=order_by,
                                             sort_keys=True, bind=bind)
     log.info('%s json lines written', f'{total_lines:_d}')
 
-    offset = f'offset={offset!r}' if offset else ''
-    limit = f'limit={limit!r}' if limit is not None else ''
+    offset = f'{offset=!r}' if offset else ''
+    limit = f'{limit=!r}' if limit is not None else ''
     sliced = ','.join(s for s in (offset, limit) if s)
     sliced = f'[{sliced}]' if sliced else ''
     result = (f'{CHECKSUM_NAME}:{order_by}{sliced}'
               f':{hashobj.name}:{hashobj.hexdigest()}')
     log.info('%s: %r', hashobj.name, result)
     return result
 
 
-def write_json_lines(file=None, *, suffix: str = '.jsonl',
+def write_json_lines(file=None, /, *, suffix: str = '.jsonl',
                      delete_present: bool = True,
                      autocompress: bool = True,
                      source: str = 'tables',
                      limit: typing.Optional[int] = None,
                      offset: typing.Optional[int] = 0,
                      order_by: str = _globals.LANGUOID_ORDER,
                      sort_keys: bool = True,
@@ -269,15 +269,15 @@
 
         if not (n % progress_after):
             log.info('%s languoids fetched', f'{n:_d}')
 
     log.info('%s languoids total', f'{n:_d}')
 
 
-def write_files(root=_globals.ROOT, *, replace: bool = False,
+def write_files(root=_globals.ROOT, /, *, replace: bool = False,
                 dry_run: bool = False,
                 require_nwritten: typing.Optional[int] = None,
                 source: str = 'tables',
                 limit: typing.Optional[int] = None,
                 offset: typing.Optional[int] = 0,
                 progress_after: int = _tools.PROGRESS_AFTER,
                 bind=_globals.ENGINE) -> int:
```

## Comparing `treedb-2.6.1/treedb/glottolog.py` & `treedb-2.6.2/treedb/glottolog.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,100 +16,100 @@
 
 REPO_URL = 'https://github.com/glottolog/glottolog.git'
 
 
 log = logging.getLogger(__name__)
 
 
-def glottolog_version(root=_globals.ROOT) -> argparse.Namespace:
+def glottolog_version(*, root=_globals.ROOT) -> argparse.Namespace:
     return GlottologVersion.from_root(root)
 
 
 class GlottologVersion(argparse.Namespace):
 
     @classmethod
-    def from_root(cls, root) -> GlottologVersion:
+    def from_root(cls, root, /) -> GlottologVersion:
         return cls.from_commit_describe(git_rev_parse(root),
                                         git_describe(root))
 
     @classmethod
-    def from_commit_describe(cls, commit: str, describe: str
+    def from_commit_describe(cls, commit: str, describe: str, /,
                              ) -> GlottologVersion:
         return cls(commit=commit, describe=describe)
 
     def __str__(self) -> str:
         return f'Glottolog {self.describe} ({self.commit})'
 
 
-def checkout_or_clone(tag_or_branch: str, *, target=None):
+def checkout_or_clone(tag_or_branch: str, /, *, target=None):
     if target is None:
         target = _languoids.get_repo_root()
 
     target = _tools.path_from_filename(target)
 
     if not target.exists():
         clone = git_clone(tag_or_branch, target=target)
     else:
         clone = None
 
     checkout = git_checkout(tag_or_branch, target=target)
     return clone, checkout
 
 
-def git_clone(tag_or_branch: str, *, target,
+def git_clone(tag_or_branch: str, /, *, target,
               depth: int = 1):
     log.info('clone Glottolog master repo at %r into %r', tag_or_branch, target)
     cmd = ['git', 'clone',
            '-c', 'advice.detachedHead=false',
            '--single-branch',
            '--branch', tag_or_branch,
            '--depth', f'{depth:d}',
            REPO_URL, target]
     return _tools.run(cmd, check=True)
 
 
-def git_checkout(tag_or_branch: str, *, target,
+def git_checkout(tag_or_branch: str, /, *, target,
                  set_branch: str = __package__):
     log.info('checkout %r and (re)set branch %r', tag_or_branch, set_branch)
     cmd = ['git', 'checkout']
     if set_branch is not None:
         cmd += ['-B', set_branch]
     cmd.append(tag_or_branch)
     return _tools.run(cmd, cwd=target, check=True)
 
 
-def git_rev_parse(repo_root, revision: str = 'HEAD',
-                  *, verify: bool = True) -> str:
+def git_rev_parse(repo_root, /, *, revision: str = 'HEAD',
+                  verify: bool = True) -> str:
     log.info('get %r git_commit from %r', revision, repo_root)
     cmd = ['git', 'rev-parse']
     if verify:
         cmd.append('--verify')
     cmd.append(revision)
     commit = _tools.run(cmd, cwd=repo_root, check=True,
                         capture_output=True, unpack=True)
     log.info('git_commit: %r', commit)
     return commit
 
 
-def git_describe(repo_root) -> str:
+def git_describe(repo_root, /) -> str:
     log.info('get git_describe from %r', repo_root)
     cmd = ['git', 'describe', '--tags', '--always']
     describe = _tools.run(cmd, cwd=repo_root, check=True,
                           capture_output=True, unpack=True)
     log.info('git_describe: %r', describe)
     return describe
 
 
-def git_status(repo_root) -> str:
+def git_status(repo_root, /) -> str:
     log.debug('get status from %r', repo_root)
     cmd = ['git', 'status', '--porcelain']
     return _tools.run(cmd, cwd=repo_root, check=True,
                       capture_output=True, unpack=True)
 
 
-def git_status_is_clean(repo_root) -> bool:
+def git_status_is_clean(repo_root, /) -> bool:
     """Return if there are neither changes in the index nor untracked files."""
     log.info('get clean from %r', repo_root)
     status = git_status(repo_root)
     clean = not status
     log.info('clean: %r', clean)
     return clean
```

## Comparing `treedb-2.6.1/treedb/import_models.py` & `treedb-2.6.2/treedb/import_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,40 +33,40 @@
 
     model = None
 
     @staticmethod
     def key_to_params(key):
         return {'name': key}
 
-    def __init__(self, items=(),
-                 *, conn,
+    def __init__(self, items=(), /, *,
+                 conn,
                  model=None, key_to_params=None,
                  log_insert=True):
         super().__init__(items)
         if model is not None:
             self.model = model
         if key_to_params is not None:
             self.key_to_params = key_to_params
         self.log_insert = log_insert
 
         self.conn = conn
         self.insert = functools.partial(conn.execute, sa.insert(self.model))
 
-    def __missing__(self, key):
+    def __missing__(self, key, /):
         if self.log_insert:
             log.debug('insert new %s: %r', self.model.__tablename__, key)
         params = self.key_to_params(key)
 
         pk, = self.insert(params).inserted_primary_key
 
         self[key] = pk
         return pk
 
 
-def main(languoids, *, conn):
+def main(languoids, /, *, conn):
 
     bibfile_ids = ModelMap(conn=conn, model=Bibfile)
 
     class BibitemMap(ModelMap):
         # using closure over bibfile_ids
 
         model = Bibitem
@@ -109,15 +109,15 @@
     insert_languoids(conn,
                      languoids=languoids,
                      bibitem_ids=bibitem_ids, es_ids=es_ids)
 
     insert_pseudofamilies(conn)
 
 
-def insert_languoid_levels(conn, *, config_file='languoid_levels.ini'):
+def insert_languoid_levels(conn, /, *, config_file='languoid_levels.ini'):
     log.info('insert languoid levels from: %r', config_file)
     levels = Config.load(config_file, bind=conn)
     levels = dict(sorted(levels.items(), key=lambda x: int(x[1]['ordinal'])))
 
     assert set(levels) >= set(LEVEL)
     extra_levels = sorted(set(levels) - set(LEVEL))
     if extra_levels:
@@ -128,15 +128,15 @@
     params = [{'name': section,
                'description': l['description'].strip(),
                'ordinal': int(l['ordinal'])}
               for section, l in levels.items()]
     conn.execute(sa.insert(LanguoidLevel), params)
 
 
-def insert_pseudofamilies(conn, *, config_file='language_types.ini'):
+def insert_pseudofamilies(conn, /, *, config_file='language_types.ini'):
     log.info('insert pseudofamilies from: %r', config_file)
     languagetypes = Config.load(config_file, bind=conn)
     pseudofamilies = {section: l for section, l in languagetypes.items()
                       if l.get('pseudo_family_id', '').strip()}
 
     log.debug('insert %d pseudofamilies: %r', len(pseudofamilies),
               list(pseudofamilies))
@@ -164,27 +164,27 @@
                       f' {missing_special_families!r}')
     inserted_bookkeeping = {p['name'] for p in params if p['bookkeeping']}
     if inserted_bookkeeping != {BOOKKEEPING}:
         warnings.warn(f'inserted bookkeeping: {inserted_bookkeeping!r}'
                       f' expected bookkeeping: {BOOKKEEPING!r}')
 
 
-def insert_macroareas(conn, *, config_file='macroareas.ini'):
+def insert_macroareas(conn, /, *, config_file='macroareas.ini'):
     log.info('insert macroareas from: %r', config_file)
     macroareas = Config.load(config_file, bind=conn)
 
     log.debug('insert %d macroareas: %r', len(macroareas), list(macroareas))
     params = [{'name': m['name'].strip(),
                'config_section': section,
                'description': m['description'].strip()}
               for section, m in macroareas.items()]
     conn.execute(sa.insert(Macroarea), params)
 
 
-def insert_endangermentstatus(conn, *, bibitem_ids,
+def insert_endangermentstatus(conn, /, *, bibitem_ids,
                               config_file='aes_status.ini'):
     log.info('insert endangermentstatus from %r:', config_file)
     status = Config.load(config_file, bind=conn)
 
     log.debug('insert %d endangermentstatus: %r', len(status), list(status))
     params = [{'name': s['name'].strip(),
                'config_section': section,
@@ -195,15 +195,15 @@
                'icon': s['icon'].strip(),
                'bibitem_id': bibitem_ids[s['reference_id'].strip()
                                          .partition(':')[::2]]}
               for section, s in status.items()]
     conn.execute(sa.insert(EndangermentStatus), params)
 
 
-def insert_languoids(conn, *, languoids, bibitem_ids, es_ids):
+def insert_languoids(conn, /, *, languoids, bibitem_ids, es_ids):
     log.info('insert languoids')
 
     def unseen_countries(countries, _seen={}):
         for c in countries:
             id_, name = (c[k] for k in ('id', 'name'))
             try:
                 assert _seen[id_] == name
@@ -220,15 +220,15 @@
               'identifiersite_ids': ModelMap(conn=conn, model=IdentifierSite),
               'es_ids': es_ids}
 
     for _, l in languoids:
         insert_languoid(l, **kwargs)
 
 
-def insert_languoid(languoid, *, conn,
+def insert_languoid(languoid, /, *, conn,
                     insert_lang,
                     unseen_countries,
                     sourceprovider_ids,
                     bibitem_ids,
                     altnameprovider_ids,
                     identifiersite_ids,
                     es_ids):
```

## Comparing `treedb-2.6.1/treedb/logging_.py` & `treedb-2.6.2/treedb/logging_.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 FORMAT = '[%(levelname)s@%(name)s] %(message)s'
 
 
 log = logging.getLogger(__name__)
 
 
-def configure_logging_from_file(path, *,
+def configure_logging_from_file(path, /, *,
                                 level=None,
                                 log_sql=None,
-                                capture_warnings=True,
-                                reset=True):
+                                capture_warnings: bool = True,
+                                reset: bool = True):
     if reset:
         reset_logging()
 
     log.debug('logging.config.fileConfig(%r)', path)
     logging.config.fileConfig(path, disable_existing_loggers=reset)
 
     package_logger = logging.getLogger(__package__)
@@ -55,25 +55,25 @@
     root_logger = logging.getLogger()
     for h in list(root_logger.handlers):
         log.debug('%r.removeHandler(%r)', root_logger, h)
         root_logger.removeHandler(h)
         h.close()
 
 
-def log_version(*, also_print=False, print_file=None):
+def log_version(*, also_print: bool = False, print_file=None):
     import treedb
 
     log.info('%s version: %s', __package__, treedb.__version__)
     log.debug('%r', treedb)
     if also_print or print_file is not None:
         print(f'{__package__} version: {treedb.__version__}',
               file=print_file)
 
 
-def set_capture_warnings(value=True):
+def set_capture_warnings(value: bool = True, /):
     log.debug('set logging.captureWarnings(%r)', value)
     logging.captureWarnings(value)
 
 
 def configure_logging(*,
                       level='WARNING',
                       log_sql=False,
```

## Comparing `treedb-2.6.1/treedb/models.py` & `treedb-2.6.2/treedb/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,26 +162,26 @@
                                       back_populates='languoid')
 
     iso_retirement = relationship('IsoRetirement',
                                   uselist=False,
                                   back_populates='languoid')
 
     @classmethod
-    def _aliased_child_parent(cls, *,
+    def _aliased_child_parent(cls, /, *,
                               child_root: bool = False,
                               parent_root: bool = False):
         if child_root and parent_root:  # pragma: no cover
             raise ValueError('child_root and parent_root are mutually exclusive')
 
         Child = aliased(cls, name='root' if child_root else 'child')  # noqa: N806
         Parent = aliased(cls, name='root' if parent_root else 'parent')  # noqa: N806
         return Child, Parent
 
     @classmethod
-    def _tree(cls, *, from_parent: bool = False,
+    def _tree(cls, /, *, from_parent: bool = False,
               innerjoin=False,
               child_root=None, parent_root=None, node_level=None,
               with_steps: bool = False,
               with_terminal: bool = False):
         if innerjoin not in (False, True, 'reflexive'):  # pragma: no cover
             raise ValueError(f'invalid innerjoin: {innerjoin!r}')
 
@@ -263,23 +263,23 @@
         tree_2 = tree_2.select_from(tree_2_fromclause)
 
         tree = tree_1.union_all(tree_2)
 
         return tree
 
     @classmethod
-    def tree(cls, *, include_self: bool = False,
+    def tree(cls, /, *, include_self: bool = False,
              with_steps: bool = False,
              with_terminal: bool = False):
         return cls._tree(from_parent=False,
                          innerjoin='reflexive' if include_self else True,
                          with_steps=with_steps, with_terminal=with_terminal)
 
     @classmethod
-    def _path_part(cls, label: str = 'path_part',
+    def _path_part(cls, /, *, label: str = 'path_part',
                    include_self: bool = True,
                    bottomup: bool = False,
                    _tree=None):
         if _tree is None:
             tree = cls.tree(include_self=include_self, with_steps=True)
         else:
             tree = _tree
@@ -290,26 +290,26 @@
                             .order_by(tree.c.steps if bottomup
                                       else tree.c.steps.desc())
                             .alias('parent_path'))
 
         return select_path_part
 
     @classmethod
-    def path(cls, *, label: str = 'path',
+    def path(cls, /, *, label: str = 'path',
              delimiter: str = _globals.FILE_PATH_SEP,
              include_self: bool = True,
              bottomup: bool = False,
              _tree=None):
         squery = cls._path_part(include_self=include_self, bottomup=bottomup,
                                 _tree=_tree)
         path = sa.func.group_concat(squery.c.path_part, delimiter).label(label)
         return sa.select(path).label(label)
 
     @classmethod
-    def node_relative(cls, *, from_parent: bool = False,
+    def node_relative(cls, /, *, from_parent: bool = False,
                       innerjoin=False,
                       child_root=None, parent_root=None, node_level=None,
                       with_steps: bool = False,
                       with_terminal: bool = False):
         tree = cls._tree(from_parent=from_parent, innerjoin=innerjoin,
                          child_root=child_root, parent_root=parent_root,
                          node_level=node_level,
@@ -333,32 +333,32 @@
         node_relative = (tree.join(Node, is_node)
                          .join(Relative, is_relative,
                                isouter=not innerjoin))
 
         return Node, Relative, tree, node_relative
 
     @classmethod
-    def child_ancestor(cls, *, innerjoin=False,
+    def child_ancestor(cls, /, *, innerjoin=False,
                        child_level=None):
         Child, Parent, _, child_parent = cls.node_relative(from_parent=False,  # noqa: N806
                                                            innerjoin=innerjoin,
                                                            node_level=child_level)
         return Child, Parent, _, child_parent
 
     @classmethod
-    def parent_descendant(cls, *, innerjoin=False,
+    def parent_descendant(cls, /, *, innerjoin=False,
                           parent_root=None, parent_level=None):
         Parent, Child, _, parent_child = cls.node_relative(from_parent=True,  # noqa: N806
                                                            innerjoin=innerjoin,
                                                            parent_root=parent_root,
                                                            node_level=parent_level)
         return Parent, Child, parent_child
 
     @classmethod
-    def path_family_language(cls, *, path_label: str = 'path',
+    def path_family_language(cls, /, *, path_label: str = 'path',
                              path_delimiter: str = _globals.FILE_PATH_SEP,
                              include_self: bool = True,
                              bottomup: bool = False,
                              family_label: str = 'family_id',
                              language_label: str = 'language_id'):
         tree = cls.tree(include_self=include_self, with_steps=True, with_terminal=True)
 
@@ -497,20 +497,20 @@
 
     languoids = relationship('Languoid',
                              secondary='languoid_country',
                              order_by='Languoid.id',
                              back_populates='countries')
 
     @classmethod
-    def printf(cls, *, minimal: bool = True, label: str = 'printf'):
+    def printf(cls, /, *, minimal: bool = True, label: str = 'printf'):
         return (sa.func.printf('%s (%s)', cls.name, cls.id)
                 if not minimal else cls.id).label(label)
 
     @classmethod
-    def jsonf(cls, *, sort_keys: bool, label: str = 'jsonf'):
+    def jsonf(cls, /, *, sort_keys: bool, label: str = 'jsonf'):
         return json_object(id=cls.id,
                            name=cls.name,
                            sort_keys_=sort_keys,
                            label_=label,)
 
 
 languoid_country = Table('languoid_country', registry.metadata,
@@ -550,21 +550,21 @@
                 f' scheme={self.scheme!r}>')
 
     languoid = relationship('Languoid',
                             innerjoin=True,
                             back_populates='links')
 
     @classmethod
-    def printf(cls, *, label: str = 'printf'):
+    def printf(cls, /, *, label: str = 'printf'):
         return sa.case((cls.title != sa.null(),
                         sa.func.printf('[%s](%s)', cls.title, cls.url)),
                        else_=cls.url).label(label)
 
     @classmethod
-    def jsonf(cls, *, sort_keys: bool, label: str = 'jsonf'):
+    def jsonf(cls, /, *, sort_keys: bool, label: str = 'jsonf'):
         return json_object(scheme=cls.scheme,
                            url=cls.url,
                            title=cls.title,
                            sort_keys_=sort_keys,
                            label_=label)
 
 
@@ -608,21 +608,21 @@
                 f' end_day={self.end_day!r}>')
 
     languoid = relationship('Languoid',
                             innerjoin=True,
                             back_populates='timespan')
 
     @classmethod
-    def printf(cls, *, label: str = 'printf'):
+    def printf(cls, /, *, label: str = 'printf'):
         return sa.func.printf('%s-%s-%s/%s-%s-%s',
                               cls.start_year, cls.start_month, cls.start_day,
                               cls.end_year, cls.end_month, cls.end_day)
 
     @classmethod
-    def jsonf(cls, *, sort_keys: bool, label: str = 'jsonf'):
+    def jsonf(cls, /, *, sort_keys: bool, label: str = 'jsonf'):
         return json_object(start_year=cls.start_year,
                            start_month=cls.start_month,
                            start_day=cls.start_day,
                            end_year=cls.end_year,
                            end_month=cls.end_month,
                            end_day=cls.end_day,
                            sort_keys_=sort_keys,
@@ -658,16 +658,16 @@
                             back_populates='sources')
 
     bibitem = relationship('Bibitem',
                            innerjoin=True,
                            back_populates='sources')
 
     @classmethod
-    def printf(cls, bibfile, bibitem,
-               *, label: str = 'printf'):
+    def printf(cls, bibfile, bibitem, /, *,
+               label: str = 'printf'):
         return sa.case((sa.and_(cls.pages != sa.null(), cls.trigger != sa.null()),
                         sa.func.printf('**%s:%s**:%s<trigger "%s">',
                                        bibfile.name, bibitem.bibkey,
                                        cls.pages, cls.trigger)),
                        (cls.pages != sa.null(),
                         sa.func.printf('**%s:%s**:%s',
                                        bibfile.name, bibitem.bibkey,
@@ -677,16 +677,16 @@
                                        bibfile.name, bibitem.bibkey,
                                        cls.trigger)),
                        else_=sa.func.printf('**%s:%s**',
                                             bibfile.name, bibitem.bibkey)
                        ).label(label)
 
     @classmethod
-    def jsonf(cls, bibfile, bibitem,
-              *, sort_keys: bool, label: str = 'jsonf'):
+    def jsonf(cls, bibfile, bibitem, /, *,
+              sort_keys: bool, label: str = 'jsonf'):
         return json_object(bibfile=bibfile.name,
                            bibkey=bibitem.bibkey,
                            pages=cls.pages,
                            trigger=cls.trigger,
                            sort_keys_=sort_keys,
                            label_=label)
 
@@ -783,20 +783,20 @@
                             back_populates='altnames')
 
     provider = relationship('AltnameProvider',
                             innerjoin=True,
                             back_populates='altnames')
 
     @classmethod
-    def printf(cls, *, label: str = 'printf'):
+    def printf(cls, /, *, label: str = 'printf'):
         full = sa.func.printf('%s [%s]', cls.name, cls.lang)
         return sa.case((cls.lang == '', cls.name), else_=full).label(label)
 
     @classmethod
-    def jsonf(cls, *, sort_keys: bool, label: str = 'jsonf'):
+    def jsonf(cls, /, *, sort_keys: bool, label: str = 'jsonf'):
         half = json_object(name=cls.name,
                            lang=None,
                            sort_keys_=sort_keys)
         full = json_object(name=cls.name,
                            lang=cls.lang,
                            sort_keys_=sort_keys)
         return sa.case((cls.lang == '', half), else_=full).label(label)
@@ -935,23 +935,23 @@
     languoid = relationship('Languoid', innerjoin=True)
 
     bibitem = relationship('Bibitem',
                            innerjoin=True,
                            back_populates='classificationrefs')
 
     @classmethod
-    def printf(cls, bibfile, bibitem,
-               *, label: str = 'printf'):
+    def printf(cls, bibfile, bibitem, /, *,
+               label: str = 'printf'):
         return sa.func.printf(sa.case((cls.pages != sa.null(), '**%s:%s**:%s'),
                                       else_='**%s:%s**'),
                               bibfile.name, bibitem.bibkey, cls.pages).label(label)
 
     @classmethod
-    def jsonf(cls, bibfile, bibitem,
-              *, sort_keys: bool, label: str = 'jsonf'):
+    def jsonf(cls, bibfile, bibitem, /, *,
+              sort_keys: bool, label: str = 'jsonf'):
         return json_object(bibfile=bibfile.name,
                            bibkey=bibitem.bibkey,
                            pages=cls.pages,
                            trigger=None,
                            sort_keys_=sort_keys,
                            label_=label)
 
@@ -987,16 +987,16 @@
                                       back_populates='endangerments')
 
     source = relationship('EndangermentSource',
                           innerjoin=True,
                           back_populates='endangerment')
 
     @classmethod
-    def jsonf(cls, source, bibfile, bibitem,
-              *, sort_keys: bool, label: str = 'jsonf'):
+    def jsonf(cls, source, bibfile, bibitem, /, *,
+              sort_keys: bool, label: str = 'jsonf'):
         source = json_object(name=source.name,
                              bibfile=bibfile.name,
                              bibkey=bibitem.bibkey,
                              pages=source.pages,
                              sort_keys_=sort_keys)
         return json_object(status=cls.status,
                            source=source,
@@ -1059,16 +1059,16 @@
                            back_populates='endangermentsources')
 
     endangerment = relationship('Endangerment',
                                 uselist=False,
                                 back_populates='source')
 
     @classmethod
-    def printf(cls, bibfile, bibitem,
-               *, label: str = 'printf'):
+    def printf(cls, bibfile, bibitem, /, *,
+               label: str = 'printf'):
         return sa.case((cls.bibitem_id == sa.null(), cls.name),
                        else_=sa.func.printf('**%s:%s**:%s',
                                             bibfile.name, bibitem.bibkey,
                                             cls.pages)).label(label)
 
 
 @registry.mapped
@@ -1094,15 +1094,15 @@
                 f' ethnologue_versions={self.ethnologue_versions!r}>')
 
     languoid = relationship('Languoid',
                             innerjoin=True,
                             back_populates='ethnologue_comment')
 
     @classmethod
-    def jsonf(cls, *, sort_keys: bool, optional: bool = False,
+    def jsonf(cls, /, *, sort_keys: bool, optional: bool = False,
               label: str = 'jsonf'):
         mapping = json_object(isohid=cls.isohid,
                               comment_type=cls.comment_type,
                               ethnologue_versions=cls.ethnologue_versions,
                               comment=cls.comment,
                               sort_keys_=sort_keys)
         if optional:
@@ -1128,15 +1128,15 @@
 
     remedy = Column(Text, CheckConstraint("remedy != ''"))
     comment = Column(Text, CheckConstraint("comment != ''"))
 
     __table_args__ = (
         # TODO: fix disagreement
         Index('change_request_key', sa.func.coalesce(change_request, effective)),
-        CheckConstraint("remedy IS NOT NULL OR reason = 'non-existent'"),
+        CheckConstraint("reason != 'split' or remedy IS NOT NULL"),
         {'info': {'without_rowid': True}},
     )
 
     def __repr__(self):
         return (f'<{self.__class__.__name__}'
                 f' languoid_id={self.languoid_id!r}'
                 f' code={self.code!r}'
@@ -1151,15 +1151,15 @@
                             back_populates='iso_retirement')
 
     change_to = relationship('IsoRetirementChangeTo',
                              order_by='IsoRetirementChangeTo.ord',
                              back_populates='iso_retirement')
 
     @classmethod
-    def jsonf(cls, *, sort_keys: bool,
+    def jsonf(cls, /, *, sort_keys: bool,
               change_to=None, optional: bool = False,
               label: str = 'jsonf'):
         mapping = json_object(code=cls.code,
                               name=cls.name,
                               change_request=cls.change_request,
                               change_to=change_to,
                               effective=json_datetime(cls.effective),
```

## Comparing `treedb-2.6.1/treedb/queries.py` & `treedb-2.6.2/treedb/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,70 +156,70 @@
     select_languoid = add_order_by(select_languoid,
                                    order_by=order_by,
                                    column_for_path_order=path)
 
     return select_languoid
 
 
-def add_order_by(select_languoid: sa.sql.Select,
-                 *, order_by: str, column_for_path_order) -> sa.sql.Select:
+def add_order_by(select_languoid: sa.sql.Select, /, *,
+                 order_by: str, column_for_path_order) -> sa.sql.Select:
     if order_by in (True, None, 'id'):
         return select_languoid.order_by(Languoid.id)
     elif order_by == 'path':
         return select_languoid.order_by(column_for_path_order)
     elif order_by is False:  # pragma: no cover
         return select_languoid
-    raise ValueError(f'order_by={order_by!r} not implemented')  # pragma: no cover
+    raise ValueError(f'{order_by=!r} not implemented')  # pragma: no cover
 
 
-def add_model_columns(select_languoid: sa.sql.Select, model,
-                      *, add_outerjoin=None, label: str = '{name}',
+def add_model_columns(select_languoid: sa.sql.Select, model, /, *,
+                      add_outerjoin=None, label: str = '{name}',
                       ignore: str = 'id') -> sa.sql.Select:
     columns = model.__table__.columns
     if ignore:
         ignore_suffix = f'_{ignore}'
         columns = [c for c in columns
                    if c.name != ignore and not c.name.endswith(ignore_suffix)]
 
     columns = [c.label(label.format(name=c.name)) for c in columns]
     select_languoid = select_languoid.add_columns(*columns)
     if add_outerjoin is not None:
         select_languoid = select_languoid.outerjoin(add_outerjoin)
     return select_languoid
 
 
-def group_concat(x, *, separator: str = ', '):
+def group_concat(x, /, *, separator: str = ', '):
     return sa.func.group_concat(x, separator)
 
 
-def add_identifier(select_languoid: sa.sql.Select, site_name: str,
-                   *, label: str) -> sa.sql.Select:
+def add_identifier(select_languoid: sa.sql.Select, site_name: str, /, *,
+                   label: str) -> sa.sql.Select:
     identifier = aliased(Identifier, name=f'ident_{site_name}')
     site = aliased(IdentifierSite, name=f'ident_{site_name}_site')
     label = label.format(site_name=site_name)
 
     return (select_languoid.add_columns(identifier.identifier.label(label))
             .outerjoin(sa.join(identifier, site, identifier.site_id == site.id),
                        sa.and_(site.name == site_name,
                                identifier.languoid_id == Languoid.id)))
 
 
-def add_classification_comment(select_languoid: sa.sql.Select, kind: str,
-                               *, label: str,
+def add_classification_comment(select_languoid: sa.sql.Select, kind: str, /, *,
+                               label: str,
                                bib_suffix: str = '_cr') -> sa.sql.Select:
     comment = aliased(ClassificationComment, name=f'cc_{kind}')
     label = label.format(kind=kind)
 
     return (select_languoid.add_columns(comment.comment.label(label))
             .outerjoin(comment, sa.and_(comment.kind == kind,
                                         comment.languoid_id == Languoid.id)))
 
 
-def add_classification_refs(select_languoid: sa.sql.Select, kind: str,
-                            *, label: str,
+def add_classification_refs(select_languoid: sa.sql.Select, kind: str, /, *,
+                            label: str,
                             bib_suffix: str = '_cr') -> sa.sql.Select:
     ref = aliased(ClassificationRef, name=f'cr_{kind}')
     bibfile = aliased(Bibfile, name=f'bibfile{bib_suffix}_{kind}')
     bibitem = aliased(Bibitem, name=f'bibitem{bib_suffix}_{kind}')
     label = label.format(kind=kind)
 
     ref = (select(ref.printf(bibfile, bibitem))
@@ -232,16 +232,16 @@
            .order_by(ref.ord)
            .alias(f'lang_cref_{kind}'))
 
     refs = select(group_concat(ref.c.printf).label(label)).label(label)
     return select_languoid.add_columns(refs)
 
 
-def add_endangermentsource(select_languoid: sa.sql.Select,
-                           *, label: str,
+def add_endangermentsource(select_languoid: sa.sql.Select, /, *,
+                           label: str,
                            bib_suffix: str = '_e') -> sa.sql.Select:
     bibfile = aliased(Bibfile, name=f'bibfile{bib_suffix}')
     bibitem = aliased(Bibitem, name=f'bibitem{bib_suffix}')
 
     endangermentsource = (EndangermentSource.printf(bibfile, bibitem)
                           .label(label))
 
@@ -320,15 +320,15 @@
     if offset:
         select_json = select_json.offset(offset)
     if limit is not None:
         select_json = select_json.limit(limit)
     return select_json
 
 
-def select_languoid_macroareas(languoid=Languoid, *, as_json: bool,
+def select_languoid_macroareas(languoid=Languoid, /, *, as_json: bool,
                                label: str = 'macroareas',
                                alias: str = 'lang_ma') -> sa.sql.Select:
     name = languoid_macroarea.c.macroarea_name
 
     macroarea = (select(name)
                  .select_from(languoid_macroarea)
                  .filter_by(languoid_id=languoid.id)
@@ -339,15 +339,15 @@
     aggregate = group_array if as_json else group_concat
 
     macroareas = aggregate(macroarea.c.macroarea_name)
 
     return select(macroareas.label(label)).label(label)
 
 
-def select_languoid_countries(languoid=Languoid, *, as_json: bool,
+def select_languoid_countries(languoid=Languoid, /, *, as_json: bool,
                               label: str = 'countries',
                               sort_keys: bool = False,
                               alias: str = 'lang_country') -> sa.sql.Select:
     value = (Country.jsonf(sort_keys=sort_keys) if as_json else
              languoid_country.c.country_id)
 
     country = (select(value)
@@ -384,26 +384,26 @@
             .alias(alias))
 
     links = group_array(sa.func.json(link.c.jsonf)) if as_json else group_concat(link.c.printf)
 
     return select(links.label(label)).label(label)
 
 
-def select_languoid_timespan(languoid=Languoid, *, as_json: bool,
+def select_languoid_timespan(languoid=Languoid, /, *, as_json: bool,
                              label: str = 'timespan',
                              sort_keys: bool = False) -> sa.sql.Select:
     return (select(Timespan.jsonf(sort_keys=sort_keys) if as_json else
                    Timespan.printf())
             .select_from(Timespan)
             .filter_by(languoid_id=languoid.id)
             .correlate(languoid)
             .label(label))
 
 
-def select_languoid_sources(languoid=Languoid, *, as_json: bool,
+def select_languoid_sources(languoid=Languoid, /, *, as_json: bool,
                             provider_name: typing.Optional[str] = None,
                             label: str = 'sources',
                             sort_keys: bool = False,
                             alias: str = 'lang_source',
                             bib_prefix: str = 'source_') -> sa.sql.Select:
     source = (aliased(Source, name=f'source_{provider_name}')
               if provider_name is not None else Source)
@@ -457,15 +457,15 @@
                                  '{}')
     else:  # pragma: no cover
         raise NotImplementedError
 
     return select(sources.label(label)).label(label)
 
 
-def select_languoid_altnames(languoid=Languoid, *, as_json: bool,
+def select_languoid_altnames(languoid=Languoid, /, *, as_json: bool,
                              provider_name: typing.Optional[str] = None,
                              label: str = 'altnames',
                              sort_keys: bool = False,
                              alias: str = 'lang_altname') -> sa.sql.Select:
     if provider_name is not None:
         altname = aliased(Altname, name=f'altname_{provider_name}')
         provider = aliased(AltnameProvider, name=f'altname_{provider_name}_provider')
@@ -511,15 +511,15 @@
                                   '{}')
     else:  # pragma: no cover
         raise NotImplementedError
 
     return select(altnames.label(label)).label(label)
 
 
-def select_languoid_triggers(languoid=Languoid, *, as_json: bool,
+def select_languoid_triggers(languoid=Languoid, /, *, as_json: bool,
                              field_name: typing.Optional[str] = None,
                              label: str = 'triggers',
                              alias: str = 'lang_trigger') -> sa.sql.Select:
     if field_name is not None:
         trigger = aliased(Trigger, name=f'trigger_{field_name}')
         columns = [trigger.trigger]
         order_by = [trigger.ord]
@@ -558,16 +558,16 @@
                                   '{}')
     else:  # pragma no cover
         raise NotImplementedError
 
     return select(triggers.label(label)).label(label)
 
 
-def select_languoid_identifier(languoid=Languoid,
-                               *, label: str = 'identifiers') -> sa.sql.Select:
+def select_languoid_identifier(languoid=Languoid, /, *,
+                               label: str = 'identifiers') -> sa.sql.Select:
     identifier = (select(IdentifierSite.name.label('site'),
                          Identifier.identifier.label('identifier'))
                   .select_from(Identifier)
                   .filter_by(languoid_id=languoid.id)
                   .correlate(languoid)
                   .join(Identifier.site.of_type(IdentifierSite))
                   .alias('lang_identifiers'))
@@ -581,16 +581,16 @@
     identifier = sa.func.nullif(group_object(identifier.c.site,
                                              identifier.c.identifier),
                                 '{}')
 
     return select(identifier.label(label)).label(label)
 
 
-def select_languoid_classification(languoid=Languoid,
-                                   *, label: str = 'classification',
+def select_languoid_classification(languoid=Languoid, /, *,
+                                   label: str = 'classification',
                                    sort_keys: bool = False,
                                    bib_suffix: str = '_cr') -> sa.sql.Select:
     classification_comment = (select(ClassificationComment.kind.label('key'),
                                      sa.func.json_quote(ClassificationComment.comment).label('value'))
                               .select_from(ClassificationComment)
                               .filter_by(languoid_id=languoid.id)
                               .correlate(languoid)
@@ -632,16 +632,16 @@
                                    '{}')
 
     return (select(nullification.label(label))
             .select_from(classification)
             .label(label))
 
 
-def select_languoid_endangerment(languoid=Languoid,
-                                 *, label: str = 'endangerment',
+def select_languoid_endangerment(languoid=Languoid, /, *,
+                                 label: str = 'endangerment',
                                  sort_keys: bool = False,
                                  bib_suffix: str = '_e') -> sa.sql.Select:
     bibitem = aliased(Bibitem, name=f'bibitem{bib_suffix}')
     bibfile = aliased(Bibfile, name=f'bibfile{bib_suffix}')
 
     return (select(Endangerment.jsonf(EndangermentSource,
                                       bibfile, bibitem,
@@ -651,27 +651,27 @@
             .filter_by(languoid_id=languoid.id)
             .correlate(languoid)
             .join(Endangerment.source)
             .outerjoin(sa.join(bibitem, bibfile))
             .label(label))
 
 
-def select_languoid_hh_ethnologue_comment(languoid=Languoid,
-                                          *, label: str = 'hh_ethnologue_comment',
+def select_languoid_hh_ethnologue_comment(languoid=Languoid, /, *,
+                                          label: str = 'hh_ethnologue_comment',
                                           sort_keys: bool = False) -> sa.sql.Select:
     return (select(EthnologueComment
                    .jsonf(sort_keys=sort_keys, label=label))
             .select_from(EthnologueComment)
             .filter_by(languoid_id=languoid.id)
             .correlate(languoid)
             .label(label))
 
 
-def select_languoid_iso_retirement(languoid=Languoid,
-                                   *, label: str = 'iso_retirement',
+def select_languoid_iso_retirement(languoid=Languoid, /, *,
+                                   label: str = 'iso_retirement',
                                    sort_keys: bool = False,
                                    alias: str = 'lang_irct',
                                    alias_label: str = 'change_to') -> sa.sql.Select:
     codes = select_iso_retirement_change_to(as_json=True,
                                             label=alias_label)
 
     return (select(IsoRetirement.jsonf(change_to=codes,
@@ -680,15 +680,15 @@
                                        label=label))
             .select_from(IsoRetirement)
             .filter_by(languoid_id=languoid.id)
             .correlate(languoid)
             .label(label))
 
 
-def select_iso_retirement_change_to(iso_retirement=IsoRetirement, *,
+def select_iso_retirement_change_to(iso_retirement=IsoRetirement, /, *,
                                     as_json: bool, label: str,
                                     alias: str = 'lang_irct') -> sa.sql.Select:
     code = (select(IsoRetirementChangeTo.code)
             .select_from(IsoRetirementChangeTo)
             .filter_by(languoid_id=iso_retirement.languoid_id)
             .correlate(IsoRetirement)
             .order_by(IsoRetirementChangeTo.ord)
@@ -698,16 +698,16 @@
 
     codes = aggregate(code.c.code)
 
     return select(codes.label(label)).label(label)
 
 
 def iterdescendants(parent_level: typing.Optional[str] = None,
-                    child_level: typing.Optional[str] = None,
-                    *, bind=_globals.ENGINE) -> typing.Iterator[typing.Tuple[str, typing.List[str]]]:
+                    child_level: typing.Optional[str] = None, *,
+                    bind=_globals.ENGINE) -> typing.Iterator[typing.Tuple[str, typing.List[str]]]:
     """Yield pairs of (parent id, sorted list of their descendant ids)."""
     # TODO: implement ancestors/descendants as sa.orm.relationship()
     # see https://bitbucket.org/zzzeek/sqlalchemy/issues/4165
     parent_root = None
     if parent_level is None:
         pass
     elif parent_level == 'top':
```

## Comparing `treedb-2.6.1/treedb/settings.py` & `treedb-2.6.2/treedb/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 log = logging.getLogger(__name__)
 
 
 class ConfigParser(configparser.ConfigParser):
 
     @classmethod
-    def from_file(cls, path, *, required=False, default_repo_root):
+    def from_file(cls, path, /, *, required=False, default_repo_root):
         path = _tools.path_from_filename(path).resolve()
 
         defaults = {'here': path.parent.as_posix()}
         inst = cls(defaults=defaults)
         inst.set_default_repo_root(default_repo_root)
 
         found = inst.read([path])
@@ -41,16 +41,16 @@
         return inst
 
     def set_default_repo_root(self, repo_root):
         self.add_section(ROOT_OPTION[0])
         self.set(*ROOT_OPTION, repo_root)
 
 
-def configure(config_path=_globals.CONFIG,
-              *, engine=NOT_SET, root=NOT_SET,
+def configure(config_path=_globals.CONFIG, /, *,
+              engine=NOT_SET, root=NOT_SET,
               loglevel=None, log_sql: bool = None,
               default_repo_root=_globals.DEFAULT_ROOT,
               title: typing.Optional[str] = None,
               title_memory_tag: str = _globals.MEMORY_TAG) -> None:
     """Set root, and engine and configure logging from the given .ini file."""
     log.info('configure from %r, title=%r', config_path, title)
     log.debug('default repo root: %r', default_repo_root)
```

## Comparing `treedb-2.6.1/treedb/_globals.py` & `treedb-2.6.2/treedb/_globals.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 
 RecordValueType = typing.Union[str, typing.List[str]]
 
 
 RecordType = typing.Mapping[str, typing.Mapping[str, RecordValueType]]
 
 
-def filepath_tuple(file_path: str,
-                   *, sep=FILE_PATH_SEP) -> typing.Tuple[str]:
+def filepath_tuple(file_path: str, /, *,
+                   sep=FILE_PATH_SEP) -> typing.Tuple[str]:
     path_parts = file_path.split(sep)
     return tuple(path_parts)
 
 
 class RecordItem(typing.NamedTuple):
     """Pair of path and record.
 
@@ -74,15 +74,15 @@
     """
 
     path: PathType
 
     record: RecordType
 
     @classmethod
-    def from_filepath_record(cls, file_path: str, languoid):
+    def from_filepath_record(cls, file_path: str, languoid, /):
         return cls(filepath_tuple(file_path), languoid)
 
 
 ValueType = typing.Union[str,
                          int, float,
                          bool,
                          None,
@@ -117,9 +117,9 @@
     """
 
     path: PathType
 
     languoid: LanguoidType
 
     @classmethod
-    def from_filepath_languoid(cls, file_path: str, languoid):
+    def from_filepath_languoid(cls, file_path: str, languoid, /):
         return cls(filepath_tuple(file_path), languoid)
```

## Comparing `treedb-2.6.1/treedb/_proxies.py` & `treedb-2.6.2/treedb/_proxies.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     >>> import pathlib
     >>> PathProxy(pathlib.Path())
     <treedb._proxies.PathProxy path='.' inode=...>
     >>> print(PathProxy(pathlib.Path()))
     .
     """
 
-    def __init__(self, path=None):
+    def __init__(self, path=None, /):
         self.path = path
 
     def __fspath__(self):
         return self._delegate.__fspath__()
 
     def __str__(self):
         if self._delegate is None:
@@ -74,23 +74,23 @@
 
 class EngineProxy(Proxy, sa.engine.Engine):
     """
 
     >>> EngineProxy(future=True)
     <treedb._proxies.EngineProxy>
     """
-    def __init__(self, engine=None, *, future):
+    def __init__(self, engine=None, /, *, future):
         self.engine = engine
         self.future = future
 
-    def _create_engine(self, url):
+    def _create_engine(self, url, /):
         log.debug('sqlalchemy.create_engine(%r)', url)
         self.engine = sa.create_engine(url, future=self.future)
 
-    def connect(self, close_with_result=False, **kwargs):
+    def connect(self, *, close_with_result: bool = False, **kwargs):
         return self.engine.connect(**kwargs)
 
     def dispose(self):
         if self._delegate is not None:
             log.debug('dispose %s.%r', self._delegate.__module__, self._delegate)
             self._delegate.dispose()
 
@@ -153,28 +153,28 @@
             parent = f' parent={self.file.parent.name!r}'
             name = self.file.name
 
         return (f'<{self.__module__}.{self.__class__.__name__}'
                 f' filename={name!r}{parent}'
                 f' size={self.file_size()!r}>')
 
-    def file_with_suffix(self, suffix):
+    def file_with_suffix(self, suffix, /):
         if self.file is None:
             name = f'{self.memory_write_path.name}{suffix}'
             return self.memory_write_path.with_name(name)
         return self.file.with_suffix(suffix)
 
     def file_exists(self):
         return self.file is not None and self.file.exists()
 
     def file_mtime(self):
         return (datetime.datetime.fromtimestamp(self.file.stat().st_mtime)
                 if self.file_exists() else None)
 
-    def file_size(self, as_megabytes=False):
+    def file_size(self, *, as_megabytes: bool = False):
         if self.file_exists():
             result = self.file.stat().st_size
             if as_megabytes:
                 result /= 2**20
             return result
         return None
```

## Comparing `treedb-2.6.1/treedb/_tools.py` & `treedb-2.6.2/treedb/_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,28 @@
            'Ordering',
            'ConfigParser']
 
 
 log = logging.getLogger(__name__)
 
 
-def uniqued(iterable):
+def uniqued(iterable, /):
     """Return list of unique hashable elements preserving order.
 
     >>> uniqued('spamham')
     ['s', 'p', 'a', 'm', 'h']
     """
     seen = set()
     return [i for i in iterable if i not in seen and not seen.add(i)]
 
 
-def next_count(start: int = 0, step: int = 1):
+def next_count(*, start: int = 0, step: int = 1):
     """Return a callable returning descending ints.
 
-    >>> nxt = next_count(1)
+    >>> nxt = next_count(start=1)
 
     >>> nxt()
     1
 
     >>> nxt()
     2
     """
@@ -111,16 +111,16 @@
     >>> {knight: [g.name for g in grp] for knight, grp in groupby_knight(people_sorted)}
     {False: ['Brian'], True: ['Sir Robin', 'Sir Lancelot']}
     """
     key = operator.attrgetter(*attrnames)
     return functools.partial(itertools.groupby, key=key)
 
 
-def islice_limit(iterable,
-                 *, limit: typing.Optional[int] = None,
+def islice_limit(iterable, /, *,
+                 limit: typing.Optional[int] = None,
                  offset: typing.Optional[int] = 0):
     """Return a slice from iterable applying limit and offset.
 
     >>> list(islice_limit('spam', limit=3))
     ['s', 'p', 'a']
 
     >>> list(islice_limit('spam', offset=3))
@@ -138,26 +138,26 @@
     elif limit is not None:
         return itertools.islice(iterable, limit)
     elif offset:
         return itertools.islice(iterable, offset, None)
     return iterable
 
 
-def iterslices(iterable, *, size: int):
+def iterslices(iterable, /, *, size: int):
     """Yield iterable in chunks of maximal size.
 
     >>> [tuple(chunk) for chunk in iterslices('bacon', size=2)]
     [('b', 'a'), ('c', 'o'), ('n',)]
     """
     iterable = iter(iterable)
     next_slice = functools.partial(itertools.islice, iterable, size)
     return iter(lambda: list(next_slice()), [])
 
 
-def walk_scandir(top, *,
+def walk_scandir(top, /, *,
                  verbose: bool = False,
                  sortkey=operator.attrgetter('name')) -> typing.Iterator[os.DirEntry]:
     """Yield os.DirEntry objects for all files under top."""
     # NOTE: os.walk() ignores errors and this can be more efficient
     top = path_from_filename(top)
     if not top.is_absolute():
         top = pathlib.Path.cwd().joinpath(top).resolve()
@@ -184,16 +184,17 @@
                 dirs.append(dentry.path)
             else:
                 yield dentry
 
         stack.extend(reversed(dirs))
 
 
-def pipe_json_lines(file, documents=None, *,
-                    delete_present: bool = True, autocompress: bool = True,
+def pipe_json_lines(file, documents=None, /, *,
+                    delete_present: bool = True,
+                    autocompress: bool = True,
                     newline: typing.Optional[str] = '\n',
                     sort_keys: bool = True,
                     compact: bool = True,
                     indent: typing.Optional[int] = None,
                     ensure_ascii: bool = False):
     r"""Load/dump json lines as endpoint pipe.
 
@@ -226,15 +227,15 @@
         lines = pipe_json(documents, dump=True, **json_kwargs)
         return pipe_lines(file, lines, **lines_kwargs)
 
     lines = pipe_lines(file, **lines_kwargs)
     return pipe_json(lines, dump=False, **json_kwargs)
 
 
-def pipe_json(documents, *, dump: bool,
+def pipe_json(documents, /, *, dump: bool,
               sort_keys: bool = True,
               compact: bool = False,
               indent: typing.Optional[int] = None,
               ensure_ascii: bool = False):
     """Bidirectional codec between a generator and a consumer."""
     codec = json.dumps if dump else json.loads
 
@@ -242,16 +243,15 @@
         dump_kwargs = {'sort_keys': sort_keys,
                        'indent': indent,
                        'ensure_ascii': ensure_ascii,
                        # json-serialize datetime.datetime
                        'default': operator.methodcaller('isoformat')}
         if compact:
             if indent:  # pragma: no cover
-                warnings.warn(f'indent={indent!r} overridden'
-                              f' by compact={compact}')
+                warnings.warn(f'{indent=!r} overridden by {compact=}')
             dump_kwargs.update(indent=None,
                                separators=(',', ':'))
         elif indent:
             warnings.warn('non-canonical JSON Lines format from indent %r' % indent)
 
         codec = functools.partial(codec, **dump_kwargs)
 
@@ -262,15 +262,15 @@
         assert next(itercodec([None])) == 'null'
     else:
         assert next(itercodec(['null'])) is None
 
     return itercodec(documents)
 
 
-def pipe_lines(file, lines=None, *, newline: typing.Optional[str] = None,
+def pipe_lines(file, lines=None, /, *, newline: typing.Optional[str] = None,
                delete_present: bool = False, autocompress: bool = True):
     open_func, result, hashobj = get_open_result(file,
                                                  write=lines is not None,
                                                  delete_present=delete_present,
                                                  autocompress=autocompress,
                                                  newline=newline)
 
@@ -288,30 +288,30 @@
     def iterlines():
         with open_func() as f:
             yield from f
 
     return iterlines()
 
 
-def write_wrapped(hashsum, f, lines, *, buflines: int = 1_000):
+def write_wrapped(hashsum, f, lines, /, *, buflines: int = 1_000):
     write_line = functools.partial(print, file=f)
     buf = f.buffer
     total = 0
     for lines in iterslices(lines, size=buflines):
         for line in lines:
             write_line(line)
         total += len(lines)
         hashsum.update(buf.getbuffer())
         # NOTE: f.truncate(0) would prepend zero-bytes
         f.seek(0)
         f.truncate()
     return total
 
 
-def write_lines(file, lines):
+def write_lines(file, lines, /):
     r"""
 
     >>> with io.StringIO() as f:
     ...    write_lines(f, ['spam', 'eggs'])
     ...    text = f.getvalue()
     2
 
@@ -321,27 +321,27 @@
     write_line = functools.partial(print, file=file)
     total = 0
     for total, line in enumerate(lines, start=1):
         write_line(line)
     return total
 
 
-def path_from_filename(filename, *args, expanduser: bool = True):
+def path_from_filename(filename, /, *args, expanduser: bool = True):
     if hasattr(filename, 'open'):
         assert not args
         result = filename
     else:
         result = pathlib.Path(filename, *args)
 
     if expanduser:
         result = result.expanduser()
     return result
 
 
-def get_open_result(file, *, write: bool = False,
+def get_open_result(file, /, *, write: bool = False,
                     delete_present: bool = False, autocompress: bool = False,
                     newline: typing.Optional[str] = None,
                     _encoding: str = 'utf-8'):
     open_kwargs = {'mode': 'wt' if write else 'rt',
                    'encoding': _encoding,
                    'newline': newline}
     textio_kwargs = {'write_through': True, 'encoding': _encoding}
@@ -386,29 +386,29 @@
             path.unlink()
 
     assert result is not None
 
     return open_func, result, hashobj
 
 
-def get_open_module(filepath, autocompress: bool = False):
+def get_open_module(filepath, /, *, autocompress: bool = False):
     file = path_from_filename(filepath)
 
     suffix = file.suffix.lower()
     if autocompress:
         result = SUFFIX_OPEN_MODULE.get(suffix, builtins)
     else:
         result = builtins
         if suffix in SUFFIX_OPEN_MODULE:  # pragma: no cover
             warnings.warn(f'file {file!r} has suffix {suffix!r}'
                           ' but autocompress=False')
     return result
 
 
-def sha256sum(file, *, raw: bool = False, autocompress: bool = True,
+def sha256sum(file, /, *, raw: bool = False, autocompress: bool = True,
               hash_file_string: bool = False,
               file_string_encoding: str = ENCODING):
     """
 
     >>> sha256sum('', hash_file_string=True)
     'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'
     """
@@ -423,20 +423,20 @@
 
         with open_module.open(file, 'rb') as f:
             update_hashobj(hashobj, f)
 
     return hashobj if raw else hashobj.hexdigest()
 
 
-def update_hashobj(hashobj, file, *, chunksize: int = 2**16):  # 64 KiB
+def update_hashobj(hashobj, file, /, *, chunksize: int = 2**16):  # 64 KiB
     for chunk in iter(functools.partial(file.read, chunksize), b''):
         hashobj.update(chunk)
 
 
-def run(cmd, *, capture_output: bool = False,
+def run(cmd, /, *, capture_output: bool = False,
         unpack: bool = False, cwd=None, check: bool = False,
         encoding: str = ENCODING):
     log.info('subprocess.run(%r)', cmd)
 
     if platform.system() == 'Windows':
         startupinfo = subprocess.STARTUPINFO()
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
@@ -477,27 +477,27 @@
     >>> list(o.sorted_enumerate(['ham', 'bacon', 'eggs'], start=1))
     [(1, 'eggs'), (2, 'bacon'), (3, 'ham')]
     """
 
     _missing = float('inf')
 
     @classmethod
-    def fromlist(cls, keys, *, start_index: int = 0):
+    def fromlist(cls, keys, /, *, start_index: int = 0):
         return cls((k, i) for i, k in enumerate(uniqued(keys), start=start_index))
 
-    def __missing__(self, key):
+    def __missing__(self, key, /):
         return self._missing
 
-    def _sortkey(self, key):
+    def _sortkey(self, key, /):
         return self[key], key
 
-    def sorted(self, keys):
+    def sorted(self, keys, /):
         return sorted(keys, key=self._sortkey)
 
-    def sorted_enumerate(self, keys, start: int = 0):
+    def sorted_enumerate(self, keys, /, *, start: int = 0):
         keyed = sorted((self[key], key) for key in keys)
         return ((i, key) for i, (_, key) in enumerate(keyed, start=start))
 
 
 class ConfigParser(configparser.ConfigParser):
     """Conservative ConfigParser with optional encoding header."""
 
@@ -508,35 +508,35 @@
                       'interpolation': None}
 
     _newline = None
 
     _header = None
 
     @classmethod
-    def from_file(cls, filename, *, encoding=ENCODING, **kwargs):
+    def from_file(cls, filename, /, *, encoding=ENCODING, **kwargs):
         path = path_from_filename(filename)
         if cls._basename is not None and path.name != cls._basename:
             raise RuntimeError(f'unexpected filename {path!r}'
                                f' (must end with {cls._basename})')
 
         inst = cls(**kwargs)
         with path.open(encoding=encoding) as f:
             inst.read_file(f)
         return inst
 
-    def __init__(self, *, defaults=None, **kwargs):
+    def __init__(self, /, *, defaults=None, **kwargs):
         for k, v in self._init_defaults.items():
             kwargs.setdefault(k, v)
         super().__init__(defaults=defaults, **kwargs)
 
-    def to_dict(self, *, sort_sections: bool = False,
+    def to_dict(self, /, *, sort_sections: bool = False,
                 _default_section: str = configparser.DEFAULTSECT):
         items = sorted(self.items()) if sort_sections else self.items()
         return {name: dict(section) for name, section in items
                 if name != _default_section}
 
-    def to_file(self, filename, *, encoding=ENCODING):
+    def to_file(self, filename, /, *, encoding=ENCODING):
         path = path_from_filename(filename)
         with path.open('wt', encoding=encoding, newline=self._newline) as f:
             if self._header is not None:
                 f.write(self._header.format(encoding=encoding))
             self.write(f)
```

## Comparing `treedb-2.6.1/treedb/__init__.py` & `treedb-2.6.2/treedb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
            'get_example_query',
            'get_languoids_query',
            'iterdescendants',
            'configure',
            'engine', 'root']
 
 __title__ = 'treedb'
-__version__ = '2.6.1'
+__version__ = '2.6.2'
 __author__ = 'Sebastian Bank <sebastian.bank@uni-leipzig.de>'
 __license__ = 'MIT, see LICENSE.txt'
 __copyright__ = 'Copyright (c) 2017-2023 Sebastian Bank'
 
 
 # default engine: in-memory database
 engine = set_engine(None)
```

## Comparing `treedb-2.6.1/treedb/backend/export.py` & `treedb-2.6.2/treedb/backend/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,36 +48,36 @@
                     .one())
     Dataset.log_dataset(dataset, ignore_dirty=ignore_dirty,
                         also_print=True, print_file=file)
     Producer.log_producer(producer,
                           also_print=True, print_file=file)
 
 
-def print_schema(metadata=_globals.REGISTRY.metadata,
-                 *, file=None,
+def print_schema(metadata=_globals.REGISTRY.metadata, /, *,
+                 file=None,
                  engine=_globals.ENGINE):
     """Print the SQL from metadata.create_all() without executing."""
     def print_sql(sql, *_, **__):
         print(sql.compile(dialect=engine.dialect),
               file=file)
 
     mock_engine = sa.create_mock_engine(engine.url, executor=print_sql)
 
     metadata.create_all(mock_engine, checkfirst=False)
 
 
-def print_query_sql(query=None, *, literal_binds: bool = True,
+def print_query_sql(query=None, /, *, literal_binds: bool = True,
                     pretty: bool = True,
                     file=None, flush: bool = True):
     """Print the literal SQL for the given query."""
     sql = get_query_sql(query, literal_binds=literal_binds, pretty=pretty)
     print(sql, file=file, flush=flush)
 
 
-def get_query_sql(query=None, *, literal_binds: bool = True,
+def get_query_sql(query=None, /, *, literal_binds: bool = True,
                   pretty: bool = False):
     """Return the literal SQL for the given query."""
     if query is None:
         from .. import queries
 
         query = queries.get_example_query()
 
@@ -85,15 +85,15 @@
     result = compiled.string
 
     if pretty and _backend.sqlparse is not None:
         result = _backend.sqlparse.format(result, reindent=True)
     return result
 
 
-def backup(filename=None, *, as_new_engine: bool = False,
+def backup(filename=None, /, *, as_new_engine: bool = False,
            pages: int = 0,
            engine=_globals.ENGINE):
     """Write the database into another .sqlite3 file and return its engine."""
     log.info('backup database')
     log.info('source: %r', engine)
 
     url = 'sqlite://'
@@ -125,16 +125,16 @@
 
     log.info('database backup complete')
     if as_new_engine:
         _backend.set_engine(result)
     return result
 
 
-def dump_sql(filename=None,
-             *, progress_after: int = 100_000,
+def dump_sql(filename=None, /, *,
+             progress_after: int = 100_000,
              encoding: str = _tools.ENCODING,
              engine=_globals.ENGINE):
     """Dump the engine database into a plain-text SQL file."""
     if filename is None:
         filename = engine.file_with_suffix('.sql.gz').name
     path = _tools.path_from_filename(filename)
     log.info('dump sql to %r', path)
@@ -156,15 +156,15 @@
             if not (n % progress_after):
                 log.info('%s lines written', f'{n:_d}')
 
     log.info('%s lines total', f'{n:_d}')
     return path
 
 
-def csv_zipfile(filename=None, *, exclude_raw: bool = False,
+def csv_zipfile(filename=None, /, *, exclude_raw: bool = False,
                 metadata=_globals.REGISTRY.metadata,
                 dialect=csv23.DIALECT, encoding: str = csv23.ENCODING,
                 engine=_globals.ENGINE):
     """Write all tables to <tablename>.csv in <databasename>.zip."""
     log.info('export database')
     log.debug('engine: %r', engine)
 
@@ -202,15 +202,15 @@
                 csv23.write_csv(f, rows, header=header,
                                 dialect=dialect, encoding=encoding)
 
     log.info('database export complete.')
     return _tools.path_from_filename(filename)
 
 
-def print_rows(query=None, *, file=None,
+def print_rows(query=None, /, *, file=None,
                pretty: bool = False,
                format_: typing.Optional[str] = None,
                verbose: bool = False,
                mappings: bool = True,
                bind=_globals.ENGINE):
     if query is None:
         from .. import queries as _queries
@@ -237,30 +237,30 @@
 
     for r in rows:
         print_func(r)
 
 
 class PrettyPrinter(pprint.PrettyPrinter):
 
-    def __init__(self, stream, *,
+    def __init__(self, stream, /, *,
                  sort_dicts: bool = False,
                  **kwargs) -> None:
         if sys.version_info < (3, 8):
             if not sort_dicts:
                 warnings.warn(f'sort_dicts={sort_dicts!r} not available')
             del sort_dicts
         else:
             kwargs['sort_dicts'] = sort_dicts
         if sys.version_info >= (3, 10):
             kwargs.setdefault('underscore_numbers', True)
         super().__init__(stream=stream, **kwargs)
 
 
-def write_csv(query=None, filename=None,
-              *, verbose: bool = False,
+def write_csv(query=None, /, filename=None, *,
+              verbose: bool = False,
               dialect=csv23.DIALECT, encoding: str = csv23.ENCODING,
               bind=_globals.ENGINE):
     """Write get__example_query() query (or given query) to CSV, return filename."""
     if query is None:
         from .. import queries as _queries
 
         query = _queries.get_example_query()
@@ -284,15 +284,15 @@
         header = list(result.keys())
         log.info('csv header: %r', header)
         return csv23.write_csv(filename, result, header=header,
                                dialect=dialect, encoding=encoding,
                                autocompress=True)
 
 
-def hash_csv(query=None, *, hash_name: str = _globals.DEFAULT_HASH,
+def hash_csv(query=None, /, *, hash_name: str = _globals.DEFAULT_HASH,
              dialect=csv23.DIALECT, encoding: str = csv23.ENCODING,
              raw: bool = False,
              bind=_globals.ENGINE):
     if query is None:
         from .. import queries as _queries
 
         query = _queries.get_example_query()
@@ -301,15 +301,15 @@
         result = conn.execute(query)
 
         header = list(result.keys())
         return hash_rows(result, header=header, hash_name=hash_name, raw=raw,
                          dialect=dialect, encoding=encoding)
 
 
-def hash_rows(rows, *, hash_name: str = _globals.DEFAULT_HASH,
+def hash_rows(rows, /, *, hash_name: str = _globals.DEFAULT_HASH,
               header=None,
               dialect=csv23.DIALECT, encoding=csv23.ENCODING,
               raw: bool = False):
     if hash_name is None:
         hash_name = _globals.DEFAULT_HASH
 
     log.info('hash rows with %r, csv header: %r', hash_name, header)
```

## Comparing `treedb-2.6.1/treedb/backend/load.py` & `treedb-2.6.2/treedb/backend/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,44 +20,44 @@
 
 __all__ = ['main']
 
 
 log = logging.getLogger(__name__)
 
 
-def get_root(repo_root, *, default,
+def get_root(repo_root, /, *, default,
              treepath=_languoids.TREE_IN_ROOT):
     if repo_root is not None:
         root = _languoids.set_root(repo_root, treepath=treepath)
     else:
         root = default
 
     log.info('load database from %r', root)
     if not root.exists():
         log.error('root does not exist')
         raise RuntimeError(f'tree root not found: {root!r}')
     return root
 
 
-def get_from_raw(from_raw, *, exclude_raw: bool):
+def get_from_raw(from_raw, /, *, exclude_raw: bool):
     if exclude_raw and from_raw:  # pragma: no cover
         log.error('incompatible exclude_raw=%r and from_raw=%r', exclude_raw, from_raw)
         raise ValueError('exclude_raw and from_raw cannot both be True')
     elif from_raw is None:
         from_raw = not exclude_raw
     return from_raw
 
 
-def get_engine(filename_or_engine, *, require: bool):
+def get_engine(filename_or_engine, /, *, require: bool):
     if hasattr(filename_or_engine, 'execute'):
         return filename_or_engine
     return _backend.set_engine(filename_or_engine, require=require)
 
 
-def get_dataset(engine, *, exclude_raw: bool, strict: bool):
+def get_dataset(engine, /, *, exclude_raw: bool, strict: bool):
     dataset = None
 
     if engine.file is None:
         log.warning('connected to a transient in-memory database')
         dataset = _models.Dataset.get_dataset(bind=engine, strict=True)
     elif engine.file_size():
         dataset = _models.Dataset.get_dataset(bind=engine, strict=strict)
@@ -67,16 +67,16 @@
         elif dataset.exclude_raw != bool(exclude_raw):  # pragma: no cover
             dataset = None
             log.warning('rebuild needed from exclude_raw mismatch')
 
     return dataset
 
 
-def main(filename=_globals.ENGINE, repo_root=None,
-         *, treepath=_languoids.TREE_IN_ROOT,
+def main(filename=_globals.ENGINE, repo_root=None, /, *,
+         treepath=_languoids.TREE_IN_ROOT,
          metadata=_globals.REGISTRY.metadata,
          require: bool = False,
          rebuild: bool = False,
          from_raw: bool = None,
          exclude_raw: bool = False,
          exclude_views: bool = False,
          force_rebuild: bool = False,
@@ -126,15 +126,15 @@
     _models.Dataset.log_dataset(dataset)
     pdc = _models.Producer.get_producer(bind=engine)
     _models.Producer.log_producer(pdc)
 
     return engine
 
 
-def create_tables(metadata, *, conn,
+def create_tables(metadata, /, *, conn,
                   exclude_raw: bool, exclude_views: bool):
     # import here to register models for create_all()
     log.debug('import module %s.models', __package__)
     from .. import models
 
     assert models is not None
 
@@ -160,15 +160,15 @@
     log.debug('set application_id = %r', application_id)
     conn.execute(sa.text(f'PRAGMA application_id = {application_id:d}'))
 
     log.debug('run create_all')
     metadata.create_all(bind=conn)
 
 
-def load(metadata, *, conn, root,
+def load(metadata, /, *, conn, root,
          from_raw: bool, exclude_raw: bool):
     log.info('record git commit in %r', root)
     # pre-create dataset to added as final item marking completeness
     dataset = make_dataset(root, exclude_raw=exclude_raw)
     _models.Dataset.log_dataset(dataset)
 
     log.info('write %r', _models.Producer.__tablename__)
@@ -204,15 +204,15 @@
 
     log.info('COMMIT dataset: %r', conn)
     conn.commit()
 
     return dataset
 
 
-def import_configs(conn, *, root):
+def import_configs(conn, /, *, root):
     insert_config = functools.partial(conn.execute, sa.insert(_models.Config))
     for filename, cfg in _config.iterconfigs(root):
         get_line = _tools.next_count(start=1)
         params = [{'filename': filename, 'section': section, 'option': option,
                    'value': value.strip(), 'line': get_line()}
                   for section, sec in cfg.items()
                   for option, value in sec.items()
@@ -223,15 +223,15 @@
 
     select_version = (sa.select(_models.Config.value)
                       .filter_by(filename='publication.ini',
                                  section='zenodo', option='version'))
     return conn.execute(select_version).scalar_one_or_none()
 
 
-def make_dataset(root, *, exclude_raw: bool):
+def make_dataset(root, /, *, exclude_raw: bool):
     try:
         dataset = {'title': 'Glottolog treedb',
                    'git_commit': _glottolog.git_rev_parse(root),
                    'git_describe': _glottolog.git_describe(root),
                    # clean = neither changes in index nor untracked files
                    'clean': _glottolog.git_status_is_clean(root),
                    'exclude_raw': exclude_raw}
@@ -239,38 +239,38 @@
         log.exception('error running git command in %r', str(root))
         raise RuntimeError(f'failed to get info for dataset: {e}') from e
     else:
         log.info('identified dataset')
         return dataset
 
 
-def write_dataset(conn, *, dataset):
+def write_dataset(conn, /, *, dataset):
     log.debug('dataset: %r', dataset)
     conn.execute(sa.insert(_models.Dataset), dataset)
 
 
-def write_producer(conn, *, name: str):
+def write_producer(conn, /, *, name: str):
     from .. import __version__
 
     params = {'name': name, 'version': __version__}
     _models.Producer.log_producer(params)
     conn.execute(sa.insert(_models.Producer), params)
 
 
-def import_raw(conn, *, root):
+def import_raw(conn, /, *, root):
     log.debug('import target module %s.raw.import_models', __package__)
 
     from ..raw import import_models
 
     log.debug('root: %r', root)
 
     import_models.main(root, conn=conn)
 
 
-def import_languoids(conn, *, root, source: str):
+def import_languoids(conn, /, *, root, source: str):
     log.debug('import source module %s.languoids', __package__)
 
     from .. import export
 
     log.debug('import target module %s.import_models', __package__)
 
     from .. import import_models
```

## Comparing `treedb-2.6.1/treedb/backend/models.py` & `treedb-2.6.2/treedb/backend/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     clean = sa.Column(sa.Boolean(create_constraint=True), nullable=False)
 
     version = sa.Column(sa.Text, sa.CheckConstraint("version != ''"))
 
     exclude_raw = sa.Column(sa.Boolean(create_constraint=True), nullable=False)
 
     @classmethod
-    def get_dataset(cls, *, bind, strict, fallback=None):
+    def get_dataset(cls, /, *, bind, strict, fallback=None):
         table = cls.__tablename__
         log.debug('read %r from %r', table, bind)
 
         try:
             result, = _backend.iterrows(sa.select(cls), mappings=True, bind=bind)
         except sa.exc.OperationalError as e:
             if 'no such table' in e.orig.args[0]:
@@ -60,15 +60,15 @@
         except Exception as e:  # pragma: no cover
             log.exception('error selecting %r', table)
             raise RuntimeError('failed to select %r from %r', table, bind) from e
         else:
             return result
 
     @classmethod
-    def log_dataset(cls, params, *,
+    def log_dataset(cls, params, /, *,
                     ignore_dirty: bool = False,
                     also_print: bool = False, print_file=None):
         name = cls.__tablename__
         log.info('git describe %(git_describe)r clean: %(clean)r', params)
         log.debug('%s.title: %r', name, params['title'])
         log.info('%s.git_commit: %r', name, params['git_commit'])
         if 'version' in params:
@@ -104,20 +104,21 @@
     name = sa.Column(sa.Text, sa.CheckConstraint("name != ''"),
                      unique=True, nullable=False)
 
     version = sa.Column(sa.Text, sa.CheckConstraint("version != ''"),
                         nullable=False)
 
     @classmethod
-    def get_producer(cls, *, bind):
+    def get_producer(cls, /, *, bind):
         result, = _backend.iterrows(sa.select(cls), mappings=True, bind=bind)
         return result
 
     @classmethod
-    def log_producer(cls, params, *, also_print=False, print_file=None):
+    def log_producer(cls, params, /, *,
+                     also_print: bool = False, print_file=None):
         name = cls.__tablename__
         log.info('%s.name: %s', name, params['name'])
         log.info('%s.version: %s', name, params['version'])
         if also_print or print_file is not None:
             print(f"{name}.name: {params['name']}", file=print_file)
             print(f"{name}.version: {params['version']}", file=print_file)
 
@@ -141,15 +142,15 @@
     line = sa.Column(sa.Integer, sa.CheckConstraint('line > 0'),
                      nullable=False)
 
     __table_args__ = (sa.UniqueConstraint(filename, line),
                       {'info': {'without_rowid': True}})
 
     @classmethod
-    def load(cls, filename: str, *, bind,
+    def load(cls, filename: str, /, *, bind,
              _groupby_section=_tools.groupby_itemgetter(0)):
         select_values = (sa.select(Config.section, Config.option, Config.value)
                         .filter_by(filename=filename)
                         .order_by('section', 'option'))
         result = _backend.iterrows(select_values, bind=bind)
         return {section: {option: value for _, option, value in grp}
                 for section, grp in _groupby_section(result)}
```

## Comparing `treedb-2.6.1/treedb/backend/pandas.py` & `treedb-2.6.2/treedb/backend/pandas.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,46 +29,46 @@
             import pandas as PANDAS  # noqa: N812
         except ImportError as e:  # pragma: no cover
             warnings.warn(f'failed to import pandas: {e}')
         else:
             log.info('pandas version: %s', PANDAS.__version__)
 
 
-def pd_read_sql(sql=None, *args, con=_globals.ENGINE, **kwargs):
+def pd_read_sql(sql=None, /, *args, con=_globals.ENGINE, **kwargs):
     _import_pandas()
 
     if PANDAS is None:
         return None
 
     if sql is None:
         from .. import queries
 
         sql = queries.get_example_query()
 
     with _backend.connect(bind=con) as conn:
         return PANDAS.read_sql_query(sql, *args, con=conn, **kwargs)
 
 
-def pd_read_json_lines(query,
-                       *, buflines: int = JSON_BUFLINES,
+def pd_read_json_lines(query, /, *,
+                       buflines: int = JSON_BUFLINES,
                        bind=_globals.ENGINE,
                        **kwargs):
     _import_pandas()
 
     if PANDAS is None:
         return None
 
     with _backend.connect(bind=bind) as conn:
         result = conn.execute(query)
         json_lines = result.scalars()
         return _pd_read_json_lines(json_lines, **kwargs)
 
 
-def _pd_read_json_lines(json_lines: typing.Iterable[str],
-                        *, buflines: int = JSON_BUFLINES,
+def _pd_read_json_lines(json_lines: typing.Iterable[str], /, *,
+                        buflines: int = JSON_BUFLINES,
                         concat_ignore_index: bool = False,
                         **kwargs):
     _import_pandas()
 
     if PANDAS is None:
         return None
```

## Comparing `treedb-2.6.1/treedb/backend/sqlite_master.py` & `treedb-2.6.2/treedb/backend/sqlite_master.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                               sa.column('type', sa.Text),
                               sa.column('name', sa.Text),
                               sa.column('tbl_name', sa.Text),
                               sa.column('rootpage', sa.Integer),
                               sa.column('sql', sa.Text))
 
 
-def print_table_sql(model_or_table, *, include_nrows: bool = True,
+def print_table_sql(model_or_table, /, *, include_nrows: bool = True,
                     file=None, flush: bool = True,
                     bind=_globals.ENGINE):
     """Print CREATE TABLE for the given table and its number of rows."""
     with bind.connect() as conn:
         result = conn.execute(select_table_sql(model_or_table))
         sql = result.scalar_one_or_none()
 
@@ -44,36 +44,36 @@
             nrows = None
 
     print(sql, file=file, flush=flush)
     if nrows is not None:
         print(nrows, file=file, flush=flush)
 
 
-def _get_table_name(model_or_table):
+def _get_table_name(model_or_table, /):
     if hasattr(model_or_table, '__tablename__'):
         return model_or_table.__tablename__
     elif hasattr(model_or_table, 'name'):
         return model_or_table.name
     return model_or_table
 
 
-def select_table_sql(model_or_table):
+def select_table_sql(model_or_table, /):
     """Select CREATE_TABLE of the given table from sqlite_master."""
     select = (sa.select(sqlite_master.c.sql)
               .select_from(sqlite_master)
               .filter_by(type='table')
               .filter_by(name=sa.bindparam('table_name')))
 
     if model_or_table is not None:
         table_name = _get_table_name(model_or_table)
         select = select.params(table_name=table_name)
     return select
 
 
-def select_table_nrows(model_or_table, *, label: str = 'n_rows'):
+def select_table_nrows(model_or_table, /, *, label: str = 'n_rows'):
     """Select the number of rows for the given table."""
     table_name = _get_table_name(model_or_table)
     return (sa.select(sa.func.count().label(label))
            .select_from(sa.table(table_name)))
 
 
 def select_tables_nrows(*, table_label: str = 'table_name',
```

## Comparing `treedb-2.6.1/treedb/backend/views.py` & `treedb-2.6.2/treedb/backend/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,36 +31,36 @@
     def decorator(func):
         REGISTERED[name] = functools.partial(func, **kwargs)
         return func
 
     return decorator
 
 
-def create_all_views(*, clear=False):
+def create_all_views(*, clear: bool = False):
     log.debug('run create_view() for %d views in REGISTERED', len(REGISTERED))
     for name, func in REGISTERED.items():
         table = view(name, selectable=func(), clear=clear)
         setattr(TABLES, name, table)
 
 
-def view(name, selectable, *, clear=False):
+def view(name, selectable, *, clear: bool = False):
     """Register a CREATE and DROP VIEW DDL for the given selectable."""
     log.debug('view(%r, clear=%r)', name, clear)
 
     if clear:
         DDL[name] = None, None
         return None
 
     DDL[name] = (CreateView(name, selectable),
                  DropView(name))
 
     return make_table(selectable, name=name)
 
 
-def make_table(selectable, *, name='view_table'):
+def make_table(selectable, /, *, name: str = 'view_table'):
     table = sa.table(name)
     for c in selectable.alias().c:
         _, col = c._make_proxy(table)
         table.append_column(col)
     return table
```

## Comparing `treedb-2.6.1/treedb/backend/_basics.py` & `treedb-2.6.2/treedb/backend/_basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 def print_versions(*, engine=ENGINE, file=None) -> None:
     logging_.log_version(also_print=True, print_file=file)
     log_versions(also_print=True, print_file=file,
                  engine=engine)
 
 
-def set_engine(filename, *,
+def set_engine(filename, /, *,
                resolve: bool = False,
                require: bool = False,
                title: typing.Optional[str] = None,
                title_memory_tag: str = _globals.MEMORY_TAG):
     """Return new sqlite3 engine and set it as default engine for treedb."""
     log.info('set_engine: %r', filename)
 
@@ -141,30 +141,30 @@
     if pragma_bulk_insert:
         conn.execute(sa.text('PRAGMA synchronous = OFF'))
         conn.execute(sa.text('PRAGMA journal_mode = MEMORY'))
 
     return conn
 
 
-def scalar(statement, *args, bind=ENGINE, **kwargs):
+def scalar(statement, /, *args, bind=ENGINE, **kwargs):
     with connect(bind=bind) as conn:
         return conn.scalar(statement, *args, **kwargs)
 
 
-def iterrows(query, *, mappings=False, bind=ENGINE):
+def iterrows(query, /, *, mappings=False, bind=ENGINE):
     with connect(bind=bind) as conn:
         result = conn.execute(query)
 
         if mappings:
             result = result.mappings()
 
         yield from result
 
 
-def expression_compile(expression, *, literal_binds=True):
+def expression_compile(expression, /, *, literal_binds=True):
     """Return literal compiled expression."""
     return expression.compile(compile_kwargs={'literal_binds': literal_binds})
 
 
 # Windows, Python < 3.9: https://www.sqlite.org/download.html
 def json_object(*, sort_keys_: bool,
                 label_: typing.Optional[str] = None,
@@ -172,10 +172,10 @@
     items = sorted(kwargs.items()) if sort_keys_ else kwargs.items()
     obj = sa.func.json_object(*[x for kv in items for x in kv])
     if label_ is not None:
         obj = obj.label(label_)
     return sa.type_coerce(obj, sa.JSON) if load_json_ else obj
 
 
-def json_datetime(date):
+def json_datetime(date, /):
     date = sa.func.replace(date, ' ', 'T')
     return sa.func.replace(date, '.000000', '')
```

## Comparing `treedb-2.6.1/treedb/backend/__init__.py` & `treedb-2.6.2/treedb/backend/__init__.py`

 * *Files identical despite different names*

## Comparing `treedb-2.6.1/treedb/languoids/fields.py` & `treedb-2.6.2/treedb/languoids/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,25 +96,25 @@
                                 (SOURCES, 'glottolog'),
                                 (ISO_RETIREMENT, 'change_to')})
 
 
 log = logging.getLogger(__name__)
 
 
-def is_known(section, option):
+def is_known(section, option, /):
     """Retun True if the section option is known or in an ALL_OPTIONS section."""
     return (section, ALL_OPTIONS) in FIELDS or (section, option) in FIELDS
 
 
-def is_all_options(section, option):
+def is_all_options(section, option, /):
     """Retun True if the section option is in an ALL_OPTIONS section."""
     return (section, ALL_OPTIONS) in FIELDS
 
 
-def is_lines(section, option, *, unknown_as_scalar=True):
+def is_lines(section, option, /, *, unknown_as_scalar: bool = True):
     """Return True if the section option is treated as list of lines."""
     result = FIELDS.get((section, ALL_OPTIONS))
 
     if result is None:
         try:
             return FIELDS[section, option]
         except KeyError:
@@ -129,35 +129,35 @@
 
     return result
 
 
 sorted_sections = SECTION_ORDER.sorted
 
 
-def sorted_options(section, options):
+def sorted_options(section, options, /):
     """Return the given section options as sorted list in canonical order."""
     fields = FIELD_ORDER.sorted((section, o) for o in options)
     return [o for _, o in fields]
 
 
-def parse_lines(value):
+def parse_lines(value, /):
     r"""
 
     >>> parse_lines(None)
     []
 
     >>> parse_lines(' spam\neggs\n  ')
     ['spam', 'eggs']
     """
     if value is None:
         return []
     return value.strip().splitlines()
 
 
-def format_lines(value):
+def format_lines(value, /):
     r"""
 
     >>> format_lines(['spam', 'eggs'])
     '\nspam\neggs'
 
     >>> format_lines([])
     ''
@@ -168,15 +168,15 @@
 
 RawRecordType = typing.Mapping[str, typing.Mapping[str, str]]
 
 
 RawRecordItem = typing.Tuple[typing.Optional[_globals.PathType], RawRecordType]
 
 
-def join_lines_inplace(record_item: _globals.RecordItem) -> RawRecordItem:
+def join_lines_inplace(record_item: _globals.RecordItem, /) -> RawRecordItem:
     path, record = record_item
     for name, section in record.items():
         for option in section:
             if is_lines(name, option):
                 lines = format_lines(section[option])
                 section[option] = lines
     return path, record
```

## Comparing `treedb-2.6.1/treedb/languoids/files.py` & `treedb-2.6.2/treedb/languoids/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     _basename = BASENAME
 
     _newline = '\r\n'
 
     _header = '# -*- coding: {encoding} -*-\n'
 
-    def update_config(self, raw_record: _fields.RawRecordType,
-                      *, replace: bool = False,
+    def update_config(self, raw_record: _fields.RawRecordType, /, *,
+                      replace: bool = False,
                       quiet: bool = False,
                       is_lines=_fields.is_lines,
                       core_sections=_fields.CORE_SECTIONS,
                       omit_empty_core_options=_fields.OMIT_EMPTY_CORE_OPTIONS,
                       keep_empty_sections=_fields.KEEP_EMPTY_SECTIONS,
                       keep_empty_options=_fields.KEEP_EMPTY_OPTIONS,
                       sorted_sections=_fields.sorted_sections,
@@ -124,23 +124,23 @@
     path: _globals.PathType
 
     dentry: os.DirEntry
 
     config: ConfigParser
 
     @classmethod
-    def from_dentry(cls, dentry: os.DirEntry,
-                    *, path_slice: slice = slice(None)):
+    def from_dentry(cls, dentry: os.DirEntry, /, *,
+                    path_slice: slice = slice(None)):
         path = _tools.path_from_filename(dentry)
         config = ConfigParser.from_file(path)
         return cls(path.parts[path_slice], dentry, config)
 
 
-def iterfiles(root=_globals.ROOT,
-              *, progress_after: int = _tools.PROGRESS_AFTER
+def iterfiles(root=_globals.ROOT, /, *,
+              progress_after: int = _tools.PROGRESS_AFTER
               ) -> typing.Iterator[FileInfo]:
     """Yield triples of ((<path_part>, ...), <ConfigParser object>, <DirEntry object>)."""
     root = _tools.path_from_filename(root).resolve()
     log.info(f'start parsing {BASENAME} files from %r', root)
     msg = f'%s {BASENAME} files parsed'
 
     kwargs = {'path_slice': slice(len(root.parts), -1)}
@@ -152,23 +152,23 @@
 
         if not (n % progress_after):
             log.info(msg, f'{n:_d}')
 
     log.info(f'%s {BASENAME} files total', f'{n:_d}')
 
 
-def roundtrip(root=_globals.ROOT,
-              *, progress_after: int = _tools.PROGRESS_AFTER) -> None:
+def roundtrip(root=_globals.ROOT, /, *,
+              progress_after: int = _tools.PROGRESS_AFTER) -> None:
     """Load/save all config files (drops leading/trailing whitespace)."""
     log.info(f'start roundtripping {BASENAME} files in %r', root)
     for path_tuple, dentry, cfg in iterfiles(root, progress_after=progress_after):
         cfg.to_file(dentry.path)
 
 
-def write_files(records: typing.Iterable[_globals.RecordItem],
+def write_files(records: typing.Iterable[_globals.RecordItem], /,
                 root=_globals.ROOT, *, replace: bool = False,
                 dry_run: bool = False, quiet: typing.Optional[bool] = None,
                 require_nwritten: typing.Optional[int] = None,
                 progress_after: typing.Optional[int] = _tools.PROGRESS_AFTER,
                 basename: str = BASENAME) -> int:
     """Write ((<path_part>, ...), <dict of dicts>) pairs to root."""
     if replace:  # pragma: no cover
@@ -200,15 +200,13 @@
 
             files_written += 1
 
             if not dry_run and (files_written % progress_after):
                 log.info(f'%s {basename} files written', f'{files_written:_d}')
 
         if require_nwritten is not None and files_written > require_nwritten:
-            raise ValueError(f'files_written={files_written}'
-                             f' over require_nwritten={require_nwritten}')
+            raise ValueError(f'{files_written=} over {require_nwritten=}')
 
     log.info(f'%s {basename} files written total', f'{files_written:_d}')
     if require_nwritten is not None and files_written < require_nwritten:
-        raise ValueError(f'files_written={files_written}'
-                         f' under require_nwritten={require_nwritten}')
+        raise ValueError(f'{files_written=} under {require_nwritten=}')
     return files_written
```

## Comparing `treedb-2.6.1/treedb/languoids/records.py` & `treedb-2.6.2/treedb/languoids/records.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 (?P<end_date>\d{1,4}-\d{2}-\d{2})
 '''.strip(), flags=(re.ASCII | re.VERBOSE))
 
 
 log = logging.getLogger(__name__)
 
 
-def pipe(items, *, dump: bool,
+def pipe(items, /, *, dump: bool,
          convert_lines: bool):
     codec = _dump if dump else _parse
     return codec(items, convert_lines=convert_lines)
 
 
-def _parse(records: typing.Iterable[_globals.RecordItem],
-           *, convert_lines: bool) -> typing.Iterator[_globals.LanguoidItem]:
+def _parse(records: typing.Iterable[_globals.RecordItem], /, *,
+           convert_lines: bool) -> typing.Iterator[_globals.LanguoidItem]:
     r"""Yield languoid items from given record ítems (from raw).
 
     >>> dict(pipe({('abin1243',):
     ...            {'core': {'name': 'Abinomn',
     ...                      'hid': 'bsa',
     ...                      'level': 'language',
     ...                      'iso639-3': 'bsa',
@@ -130,16 +130,16 @@
     make_item = _globals.LanguoidItem
     for n, (path, cfg) in enumerate(records, start=1):
         languoid = make_languoid(path, cfg, convert_lines=convert_lines)
         yield make_item(path, languoid)
     log.info('%s languoids extracted from records', f'{n:_d}')
 
 
-def _dump(languoids: typing.Iterable[_globals.LanguoidItem],
-          *, convert_lines: bool) -> typing.Iterator[_globals.RecordItem]:
+def _dump(languoids: typing.Iterable[_globals.LanguoidItem], /, *,
+          convert_lines: bool) -> typing.Iterator[_globals.RecordItem]:
     r"""
 
     >>> dict(pipe({('abin1243',): {
     ...             'id': 'abin1243',
     ...             'parent_id': None,
     ...             'name': 'Abinomn',
     ...             'level': 'language',
@@ -222,16 +222,16 @@
       'iso_retirement': {}}}
     """  # noqa: E501
     for path, l in languoids:
         record = make_record(l, convert_lines=convert_lines)
         yield path, record
 
 
-def make_languoid(path_tuple: _globals.PathType, cfg: _globals.RecordType,
-                  *, convert_lines: bool) -> _globals.LanguoidType:
+def make_languoid(path_tuple: _globals.PathType, cfg: _globals.RecordType, /, *,
+                  convert_lines: bool) -> _globals.LanguoidType:
     _make_lines = _fields.parse_lines if convert_lines else make_lines_raw
 
     core = cfg[CORE]
 
     languoid = {'id': path_tuple[-1],
                 'parent_id': path_tuple[-2] if len(path_tuple) > 1 else None,
                 'name': core['name'],
@@ -313,16 +313,16 @@
                                     'change_to': _make_lines(sct.get('change_to')),
                                     'remedy': sct.get('remedy'),
                                     'comment': sct.get('comment')}
 
     return languoid
 
 
-def make_record(languoid: _globals.LanguoidType,
-                *, convert_lines: bool,
+def make_record(languoid: _globals.LanguoidType, /, *,
+                convert_lines: bool,
                 is_lines=_fields.is_lines) -> _globals.RecordType:
     core = {'name': languoid['name'],
             'hid': languoid['hid'],
             'level': languoid['level'],
             'iso639-3': languoid['iso639_3'],
             'latitude': format_float(languoid['latitude']),
             'longitude': format_float(languoid['longitude']),
@@ -385,115 +385,114 @@
 
     if convert_lines:
         _, record = _fields.join_lines_inplace((None, record))
 
     return record
 
 
-def make_lines_raw(value):
+def make_lines_raw(value, /):
     """No-op.
 
     >>> make_lines_raw(None)
     []
 
     >>> make_lines_raw(['spam', 'eggs'])
     ['spam', 'eggs']
     """
     if value is None:
         return []
     return value
 
 
-def skip_empty(mapping):
+def skip_empty(mapping, /):
     """
 
     >>> skip_empty({'spam': None, 'eggs': [], 'bacon': 'ham'})
     {'bacon': 'ham'}
     """
     return {k: v for k, v in mapping.items() if v}
 
 
-def get_float(mapping, key, format_=FLOAT_FORMAT):
+def get_float(mapping, key, /, *, format_=FLOAT_FORMAT):
     """
 
     >>> get_float({'spam': '1.42'}, 'spam')
     1.42
 
     >>> assert get_float({}, 'spam') is None
     >>> assert get_float({'eggs': 42}, 'spam') is None
     """
     result = mapping.get(key)
     if result is not None:
         result = float(format_ % float(result))
     return result
 
 
-def format_float(value, format_=FLOAT_FORMAT):
+def format_float(value, /, *, format_=FLOAT_FORMAT):
     """
 
     >>> format_float(1.42)
     '1.42'
 
     >>> assert format_float(None) is None
     """
     if value is None:
         return None
     return str(float(format_ % value))
 
 
-def make_date(value, *, format_=DATE_FORMAT):
+def make_date(value, /, *, format_=DATE_FORMAT):
     """
 
     >>> make_date('2001-12-31')
     datetime.date(2001, 12, 31)
     """
     return datetime.datetime.strptime(value, format_).date()
 
 
-def format_date(value, *, format_=DATE_FORMAT):
+def format_date(value, /, *, format_=DATE_FORMAT):
     """
 
     >>> format_date(datetime.date(2001, 12, 31))
     '2001-12-31'
     """
     return value.strftime(format_)
 
 
-def make_datetime(value, *, format_=DATETIME_FORMAT):
+def make_datetime(value, /, *, format_=DATETIME_FORMAT):
     """
 
     >>> make_datetime('2001-12-31T23:59:59')
     datetime.datetime(2001, 12, 31, 23, 59, 59)
     """
     return datetime.datetime.strptime(value, format_)
 
 
-def format_datetime(value, *, format_=DATETIME_FORMAT):
+def format_datetime(value, /, *, format_=DATETIME_FORMAT):
     """
 
     >>> format_datetime(datetime.datetime(2001, 12, 31, 23, 59, 59))
     '2001-12-31T23:59:59'
     """
     return value.strftime(format_)
 
 
-def make_interval(value, date_format=DATE_FORMAT, fix_year=True,
+def make_interval(value, /, *, date_format=DATE_FORMAT, fix_year=True,
                   _match=ISO_8601_INTERVAL.fullmatch, strict=False):
     """
 
     >>> make_interval('-9999-01-01/+9999-12-31')
     {'start_year': -9999, 'start_month': 1, 'start_day': 1, 'end_year': 9999, 'end_month': 12, 'end_day': 31}
 
     >>> assert make_interval(None) is None
     """
     if value is None:
         return None
     value = value.strip()
-    ma = _match(value)
-    if ma is None:
+    if (ma := _match(value)) is None:
         warnings.warn(f'unmatched interval: {value!r}')
 
         if strict:  # pragma: no cover
             log.error('invalid interval', value)
             raise ValueError('invalid interval', value)
 
         log.warning('ignoring interval value %r', value)
@@ -519,15 +518,15 @@
             'start_month': start.month,
             'start_day': start.day,
             'end_year': end.year * end_sign,
             'end_month': end.month,
             'end_day': end.day}
 
 
-def format_interval(value, year_tmpl='{: 05d}'):
+def format_interval(value, /, *, year_tmpl='{: 05d}'):
     """
 
     >>> format_interval({'start_year': -9999,
     ...                  'start_month': 1,
     ...                  'start_day': 1,
     ...                  'end_year': 9999,
     ...                  'end_month': 12,
@@ -561,29 +560,29 @@
     \(
         (?P<id>[^)]+)
     \)
 )
 '''.strip(), flags=re.VERBOSE)
 
 
-def splitcountry(name, *, _match=_COUNTRY_PATTERN.fullmatch):
+def splitcountry(name, /, *, _match=_COUNTRY_PATTERN.fullmatch):
     """
 
     >>> splitcountry('The Union of the Comoros (KM)')
     {'name': 'The Union of the Comoros', 'id': 'KM'}
     """
     groups = _match(name).groupdict()
     id_only = groups.pop('id_only')
     if id_only:
         country = pycountry.countries.get(alpha_2=id_only)
         return {'id': id_only, 'name': country.name}
     return groups
 
 
-def formatcountry(value, minimal=True):
+def formatcountry(value, /, *, minimal=True):
     """
 
     >>> formatcountry({'name': 'The Kingdom of Norway', 'id': 'NO'})
     'NO'
 
     >>> formatcountry({'name': 'The Kingdom of Norway', 'id': 'NO'},
     ...               minimal=False)
@@ -598,31 +597,30 @@
 \]
 \(
     (?P<url>[^)]+)
 \)
 '''.strip(), flags=re.VERBOSE)
 
 
-def splitlink(markdown, *, _match=_LINK_PATTERN.fullmatch):
+def splitlink(markdown, /, *, _match=_LINK_PATTERN.fullmatch):
     """
 
     >>> splitlink('https://www.example.com')
     {'url': 'https://www.example.com', 'title': None, 'scheme': 'https'}
 
     >>> splitlink('http://www.example.com')
     {'url': 'http://www.example.com', 'title': None, 'scheme': 'http'}
 
     >>> splitlink('[Example](https://www.example.com)')
     {'url': 'https://www.example.com', 'title': 'Example', 'scheme': 'https'}
 
     >>> splitlink('www.example.com')
     {'url': 'www.example.com', 'title': None, 'scheme': None}
     """
-    ma = _match(markdown)
-    if ma is not None:
+    if (ma := _match(markdown)) is not None:
         title, url = ma.groups()
     else:
         title = None
         url = markdown
 
     scheme, sep, rest = url.partition('://')
     if sep:
@@ -630,15 +628,15 @@
         scheme = scheme.lower()
     else:
         scheme = None
 
     return {'url': url, 'title': title, 'scheme': scheme}
 
 
-def formatlink(value):
+def formatlink(value, /):
     """
 
     >>> formatlink({'url': 'https://example.com'})
     'https://example.com'
 
     >>> formatlink({'url': 'https://example.com', 'title': 'Example'})
     '[Example](https://example.com)'
@@ -665,15 +663,15 @@
     <trigger[ ]"
         (?P<trigger>[^\"]+)
     ">
 )?
 '''.strip(), flags=re.VERBOSE)
 
 
-def splitsource(s, *, _match=_SOURCE_PATTERN.match,  # pre v4.1 compat
+def splitsource(s, /, *, _match=_SOURCE_PATTERN.match,  # pre v4.1 compat
                 endangerment=False):
     """
 
     >>> splitsource('**hh:42**')
     {'bibfile': 'hh', 'bibkey': '42', 'pages': None, 'trigger': None}
 
     >>> splitsource('**hh:42**:23-55')
@@ -691,15 +689,15 @@
     result = _match(s).groupdict()
     if endangerment:
         result['name'] = s
         result.pop('trigger', None)
     return result
 
 
-def formatsource(value, endangerment=False):
+def formatsource(value, /, *, endangerment=False):
     """
 
     >>> formatsource({'bibfile': 'hh', 'bibkey': '23'})
     '**hh:23**'
 
     >>> formatsource({'bibfile': 'hh', 'bibkey': '23', 'pages': '1-23'})
     '**hh:23**:1-23'
@@ -729,30 +727,30 @@
      \[
          (?P<lang>[a-z]{2,3})
      \]
 )?
 '''.strip(), flags=re.VERBOSE)
 
 
-def splitaltname(s, *, _match=_ALTNAME_PATTERN.fullmatch):
+def splitaltname(s, /, *, _match=_ALTNAME_PATTERN.fullmatch):
     """
 
     >>> splitaltname('Spam')
     {'name': 'Spam', 'lang': None}
 
     >>> splitaltname('Späm [de]')
     {'name': 'Späm', 'lang': 'de'}
 
     >>> splitaltname('Späm [deu]')
     {'name': 'Späm', 'lang': 'deu'}
     """
     return _match(s).groupdict()
 
 
-def formataltname(value):
+def formataltname(value, /):
     """
 
     >>> formataltname({'name': 'Spam'})
     'Spam'
 
     >>> formataltname({'name': 'Spam', 'lang': None})
     'Spam'
```

## Comparing `treedb-2.6.1/treedb/languoids/_root.py` & `treedb-2.6.2/treedb/languoids/_root.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 TREE_IN_ROOT = _tools.path_from_filename('languoids', 'tree')
 
 
 log = logging.getLogger(__name__)
 
 
-def set_root(repo_root, *, resolve=False,
+def set_root(repo_root, /, *, resolve: bool = False,
              treepath=TREE_IN_ROOT):
     """Set and return default root for glottolog lanugoid directory tree."""
     log.info('set_root: %r', repo_root)
     if repo_root is None:
         raise ValueError(f'missing repo_root path: {repo_root!r}')
 
     repo_path = _tools.path_from_filename(repo_root)
@@ -25,14 +25,14 @@
         repo_path = repo_path.resolve(strict=False)
 
     ROOT = _globals.ROOT  # noqa: N806
     ROOT.path = repo_path / _tools.path_from_filename(treepath)
     return ROOT
 
 
-def get_repo_root(root=_globals.ROOT,
-                  *, treepath=TREE_IN_ROOT):
+def get_repo_root(root=_globals.ROOT, /, *,
+                  treepath=TREE_IN_ROOT):
     assert root.parts[-len(treepath.parts):] == treepath.parts
     repo_root = _tools.path_from_filename(root)
     for _ in treepath.parts:
         repo_root = repo_root.parent
     return repo_root
```

## Comparing `treedb-2.6.1/treedb/languoids/__init__.py` & `treedb-2.6.2/treedb/languoids/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 from .files import iterfiles
 
 __all__ = ['TREE_IN_ROOT', 'set_root', 'get_repo_root',
            'iterfiles',
            'iterrecords']
 
 
-def iterrecords(root=_globals.ROOT,
-                *, progress_after: int = _tools.PROGRESS_AFTER
+def iterrecords(*, root=_globals.ROOT,
+                progress_after: int = _tools.PROGRESS_AFTER
                 ) -> typing.Iterable[_globals.RecordItem]:
     for path_tuple, _, cfg in iterfiles(root, progress_after=progress_after):
         yield path_tuple, cfg
```

## Comparing `treedb-2.6.1/treedb/raw/export.py` & `treedb-2.6.2/treedb/raw/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                                        dialect=dialect, encoding=encoding,
                                        raw=True)
 
     logging.info('%s: %r', hashobj.name, hashobj.hexdigest())
     return f'{kind}:{hashobj.name}:{hashobj.hexdigest()}'
 
 
-def write_raw_csv(filename=None, *,
+def write_raw_csv(filename=None, /, *,
                   dialect: str = csv23.DIALECT, encoding: str = csv23.ENCODING):
     """Write (path, section, option, line, value) rows to filename."""
     if filename is None:
         filename = _globals.ENGINE.file_with_suffix('.raw.csv.gz').name
     else:
         filename = _tools.path_from_filename(filename)
 
@@ -96,15 +96,15 @@
                      .join_from(File, Value).join(Option)
                      .order_by('path', 'section', 'option', 'line'))
 
     return _backend_export.write_csv(select_values, filename,
                                      dialect=dialect, encoding=encoding)
 
 
-def write_files(root=_globals.ROOT, *, replace: bool = False,
+def write_files(root=_globals.ROOT, /, *, replace: bool = False,
                 dry_run: bool = False,
                 require_nwritten: typing.Optional[int] = None,
                 limit: typing.Optional[int] = None,
                 offset: typing.Optional[int] = 0,
                 progress_after: int = _tools.PROGRESS_AFTER,
                 bind=_globals.ENGINE):
     """Write (path, section, option, line, value) rows back into config files."""
```

## Comparing `treedb-2.6.1/treedb/raw/import_models.py` & `treedb-2.6.2/treedb/raw/import_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
 
 class OptionMap(dict):
     """Insert option on demand, add ``(section, option) -> (pk, is_lines)`` to map."""
 
     model = Option
 
-    def __init__(self, items=(), *, conn):
+    def __init__(self, items=(), /, *, conn):
         super().__init__(items)
         self.insert = functools.partial(conn.execute, sa.insert(self.model))
 
-    def __missing__(self, key):
+    def __missing__(self, key, /):
         log.debug('insert option: %r', key)
         section, option = key
         is_lines = _fields.is_lines(section, option)
 
         params = {'section': section, 'option': option,
                   'is_lines': is_lines}
 
@@ -52,26 +52,26 @@
 
         pk, = self.insert(params).inserted_primary_key
 
         self[key] = result = (pk, is_lines)
         return result
 
 
-def itervalues(cfg, file_id, *, option_map):
+def itervalues(cfg, file_id, /, *, option_map):
     get_line = _tools.next_count(start=1)
     for section, sec in cfg.items():
         for option, text in sec.items():
             option_id, is_lines = option_map[section, option]
             values = text.strip().splitlines() if is_lines else [text]
             for v in values:
                 yield {'file_id': file_id, 'option_id': option_id,
                        'line': get_line(), 'value': v}
 
 
-def main(root, *, conn):
+def main(root, /, *, conn):
     insert_file = functools.partial(conn.execute, sa.insert(File))
 
     option_id_is_lines = OptionMap(conn=conn)
 
     insert_value = functools.partial(conn.execute, sa.insert(Value))
 
     for path_tuple, dentry, cfg in _languoids.iterfiles(root):
```

## Comparing `treedb-2.6.1/treedb/raw/models.py` & `treedb-2.6.2/treedb/raw/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     sha256 = Column(String(64), CheckConstraint('length(sha256) = 64'),
                     unique=True, nullable=False)
 
     __table_args__ = (CheckConstraint('substr(path, -length(glottocode))'
                                       ' = glottocode'),)
 
     @classmethod
-    def path_depth(cls, label='path_depth'):
+    def path_depth(cls, /, *, label='path_depth'):
         return sa.func.floor((sa.func.length(cls.path) + 1) / 9).label(label)
 
 
 @registry.mapped
 class Option:
     """Unique (section, option) key of the values with lines config."""
```

## Comparing `treedb-2.6.1/treedb/raw/records.py` & `treedb-2.6.2/treedb/raw/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         select_values = select_values.join(File)
         if order_by == 'path':
             key_column = File.path
         else:
             key_column = File.glottocode
         value_key = key_column
     else:  # pragma: no cover
-        raise ValueError(f'order_by={order_by!r} not implememted')
+        raise ValueError(f'{order_by=!r} not implememted')
 
     log.info('order_by: %r', order_by)
     select_files = (sa.select(File.path)
                     .order_by(key_column))
     select_values = (select_values
                      .order_by(value_key,
                                'section', Value.line, 'option'))
@@ -92,15 +92,15 @@
             n += count
             if not (n % progress_after):
                 log.info('%s raw records generated', f'{n:_d}')
 
     log.info('%s raw records total', f'{n:_d}')
 
 
-def window_slices(key_column, *, size: int = WINDOWSIZE,
+def window_slices(key_column, /, *, size: int = WINDOWSIZE,
                   bind=_globals.ENGINE):
     """Yield where clause making function for key_column windows of size.
 
     adapted from https://github.com/sqlalchemy/sqlalchemy/wiki/RangeQuery-and-WindowedRangeQuery
     """
     log.info('fetch %r slices for window of %d', str(key_column.expression), size)
     keys = iterkeys(key_column, size=size, bind=bind)
@@ -118,15 +118,15 @@
     for end in keys:
         yield lambda c, last=last, end=end: sa.and_(c > last, c <= end)
         last = end
 
     yield lambda c, end=end: (c > end)
 
 
-def iterkeys(key_column, *, size: int = WINDOWSIZE,
+def iterkeys(key_column, /, *, size: int = WINDOWSIZE,
              bind=_globals.ENGINE):
     row_num = sa.func.row_number().over(order_by=key_column).label('row_num')
     select_all_keys = (sa.select(key_column.label('key'), row_num)
                        .alias('key_ord'))
 
     select_keys = (sa.select(select_all_keys.c.key)
                    .where((select_all_keys.c.row_num % size) == 0))
```

## Comparing `treedb-2.6.1/treedb.egg-info/PKG-INFO` & `treedb-2.6.2/treedb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treedb
-Version: 2.6.1
+Version: 2.6.2
 Summary: Glottolog languoid tree as SQLite database
 Home-page: https://github.com/glottolog/treedb
 Author: Sebastian Bank
 Author-email: sebastian.bank@uni-leipzig.de
 License: MIT
 Project-URL: Changelog, https://github.com/glottolog/treedb/blob/master/CHANGES.rst
 Project-URL: Issue Tracker, https://github.com/glottolog/treedb/issues
@@ -14,20 +14,20 @@
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: pretty
 Provides-Extra: pandas
 License-File: LICENSE.txt
 
 Glottolog ``treedb``
```

## Comparing `treedb-2.6.1/treedb.egg-info/SOURCES.txt` & `treedb-2.6.2/treedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

