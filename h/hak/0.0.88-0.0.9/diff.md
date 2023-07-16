# Comparing `tmp/hak-0.0.88.tar.gz` & `tmp/hak-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hak-0.0.88.tar", last modified: Sun Jul 16 04:05:54 2023, max compression
+gzip compressed data, was "hak-0.0.9.tar", last modified: Wed Apr 19 10:43:20 2023, max compression
```

## Comparing `hak-0.0.88.tar` & `hak-0.0.9.tar`

### file list

```diff
@@ -1,530 +1,369 @@
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/
--rw-rw-r--   0 q         (1000) q         (1000)     1068 2023-07-07 13:22:08.000000 hak-0.0.88/LICENSE
--rw-rw-r--   0 q         (1000) q         (1000)     1212 2023-07-16 04:05:54.949642 hak-0.0.88/PKG-INFO
--rw-rw-r--   0 q         (1000) q         (1000)      583 2023-07-10 13:04:07.000000 hak-0.0.88/README.md
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 04:34:17.000000 hak-0.0.88/hak/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/data/
--rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-04 23:50:58.000000 hak-0.0.88/hak/data/months.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/fake/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.88/hak/fake/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/fake/os/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.88/hak/fake/os/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      418 2023-04-23 03:18:31.000000 hak-0.0.88/hak/fake/os/system.py
--rw-rw-r--   0 q         (1000) q         (1000)      424 2023-04-23 03:18:31.000000 hak-0.0.88/hak/fake/printer.py
--rw-rw-r--   0 q         (1000) q         (1000)       45 2023-04-23 03:18:31.000000 hak-0.0.88/hak/fake/sleep.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/fake/subprocess/
--rw-rw-r--   0 q         (1000) q         (1000)     5858 2023-07-06 06:52:44.000000 hak-0.0.88/hak/fake/subprocess/run.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.925642 hak-0.0.88/hak/many/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/bools/
--rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 06:52:37.000000 hak-0.0.88/hak/many/bools/count_true.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/dicts/
--rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 06:52:47.000000 hak-0.0.88/hak/many/dicts/a_into_b.py
--rw-rw-r--   0 q         (1000) q         (1000)     1136 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/dicts/compare.py
--rw-rw-r--   0 q         (1000) q         (1000)      911 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/dicts/compare_relevant_only.py
--rw-rw-r--   0 q         (1000) q         (1000)      797 2023-07-10 13:05:10.000000 hak-0.0.88/hak/many/dicts/convert_date_strings_to_dates.py
--rw-rw-r--   0 q         (1000) q         (1000)      363 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/dicts/get_all_keys.py
--rw-rw-r--   0 q         (1000) q         (1000)      712 2023-07-16 01:20:35.000000 hak-0.0.88/hak/many/dicts/get_datatypes.py
--rw-rw-r--   0 q         (1000) q         (1000)      493 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/dicts/get_first_and_last_dates.py
--rw-rw-r--   0 q         (1000) q         (1000)     1429 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/dicts/get_keys_with_none_or_zero_vals.py
--rw-rw-r--   0 q         (1000) q         (1000)      199 2023-07-06 06:53:17.000000 hak-0.0.88/hak/many/dicts/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      663 2023-07-06 06:53:28.000000 hak-0.0.88/hak/many/dicts/merge_freq_dicts.py
--rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 06:53:38.000000 hak-0.0.88/hak/many/dicts/reindex.py
--rw-rw-r--   0 q         (1000) q         (1000)      203 2023-07-06 06:53:48.000000 hak-0.0.88/hak/many/dicts/sort_by_key.py
--rw-rw-r--   0 q         (1000) q         (1000)      384 2023-07-10 13:05:47.000000 hak-0.0.88/hak/many/dicts/sum_by_key.py
--rw-rw-r--   0 q         (1000) q         (1000)     9805 2023-07-16 03:09:19.000000 hak-0.0.88/hak/many/dicts/to_table.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/directories/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/directories/empty/
--rw-rw-r--   0 q         (1000) q         (1000)      701 2023-07-10 13:07:02.000000 hak-0.0.88/hak/many/directories/empty/find.py
--rw-rw-r--   0 q         (1000) q         (1000)      649 2023-07-10 13:07:36.000000 hak-0.0.88/hak/many/directories/empty/remove.py
--rw-rw-r--   0 q         (1000) q         (1000)      579 2023-07-06 06:54:08.000000 hak-0.0.88/hak/many/directories/exist.py
--rw-rw-r--   0 q         (1000) q         (1000)      606 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/directories/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      440 2023-07-07 05:17:37.000000 hak-0.0.88/hak/many/directories/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.925642 hak-0.0.88/hak/many/files/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/files/pyfiles/
--rw-rw-r--   0 q         (1000) q         (1000)     1789 2023-07-06 06:54:28.000000 hak-0.0.88/hak/many/files/pyfiles/dismantle.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/lists/
--rw-rw-r--   0 q         (1000) q         (1000)      216 2023-07-06 06:54:38.000000 hak-0.0.88/hak/many/lists/merge.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/numbers/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 02:09:58.000000 hak-0.0.88/hak/many/numbers/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/numbers/ints/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 02:11:47.000000 hak-0.0.88/hak/many/numbers/ints/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/numbers/ints/mode/
--rw-rw-r--   0 q         (1000) q         (1000)      405 2023-07-10 13:08:08.000000 hak-0.0.88/hak/many/numbers/ints/mode/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      148 2023-07-10 12:30:14.000000 hak-0.0.88/hak/many/numbers/ints/remove_zeroes.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/many/pyfiles/
--rw-rw-r--   0 q         (1000) q         (1000)      161 2023-07-06 06:54:46.000000 hak-0.0.88/hak/many/pyfiles/format.py
--rw-rw-r--   0 q         (1000) q         (1000)      847 2023-07-06 06:54:53.000000 hak-0.0.88/hak/many/pyfiles/format_and_commit.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/strings/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:55:00.000000 hak-0.0.88/hak/many/strings/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      130 2023-07-06 06:55:08.000000 hak-0.0.88/hak/many/strings/add_src_funks_prefix.py
--rw-rw-r--   0 q         (1000) q         (1000)      586 2023-07-06 06:55:15.000000 hak-0.0.88/hak/many/strings/compare.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/strings/contain/
--rw-rw-r--   0 q         (1000) q         (1000)      145 2023-07-06 06:55:23.000000 hak-0.0.88/hak/many/strings/contain/version.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/strings/date_pieces/
--rw-rw-r--   0 q         (1000) q         (1000)      676 2023-07-10 13:09:01.000000 hak-0.0.88/hak/many/strings/date_pieces/get.py
--rw-rw-r--   0 q         (1000) q         (1000)     3832 2023-07-10 13:10:37.000000 hak-0.0.88/hak/many/strings/date_pieces/separate_day.py
--rw-rw-r--   0 q         (1000) q         (1000)      834 2023-07-10 13:12:11.000000 hak-0.0.88/hak/many/strings/date_pieces/separate_year.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/strings/dates/
--rw-rw-r--   0 q         (1000) q         (1000)     3259 2023-07-10 13:12:55.000000 hak-0.0.88/hak/many/strings/dates/detect_format.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/strings/filepaths/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:55:30.000000 hak-0.0.88/hak/many/strings/filepaths/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1238 2023-07-10 13:15:48.000000 hak-0.0.88/hak/many/strings/filepaths/get_least_recently_modified.py
--rw-rw-r--   0 q         (1000) q         (1000)     1196 2023-07-10 13:16:18.000000 hak-0.0.88/hak/many/strings/filepaths/get_most_recently_modified.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/strings/filepaths/py/
--rw-rw-r--   0 q         (1000) q         (1000)     1009 2023-07-06 06:55:37.000000 hak-0.0.88/hak/many/strings/filepaths/py/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/strings/filepaths/py/testables/
--rw-rw-r--   0 q         (1000) q         (1000)     2077 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/strings/filepaths/py/testables/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      660 2023-07-06 06:55:52.000000 hak-0.0.88/hak/many/strings/filepaths/py/to_filepath_file_content_dict.py
--rw-rw-r--   0 q         (1000) q         (1000)     2234 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/strings/find_first_diff.py
--rw-rw-r--   0 q         (1000) q         (1000)      291 2023-07-10 13:16:37.000000 hak-0.0.88/hak/many/strings/get_index_of_first_difference.py
--rw-rw-r--   0 q         (1000) q         (1000)      444 2023-07-06 06:56:07.000000 hak-0.0.88/hak/many/strings/make_patch_version_change_to_py.py
--rw-rw-r--   0 q         (1000) q         (1000)      297 2023-07-06 06:56:14.000000 hak-0.0.88/hak/many/strings/module_names_from_py_filenames.py
--rw-rw-r--   0 q         (1000) q         (1000)      416 2023-07-06 06:56:22.000000 hak-0.0.88/hak/many/strings/patch_setup_cfg.py
--rw-rw-r--   0 q         (1000) q         (1000)      632 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/strings/patch_setup_py.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/strings/pyfiles/
--rw-rw-r--   0 q         (1000) q         (1000)     1514 2023-07-06 06:56:37.000000 hak-0.0.88/hak/many/strings/pyfiles/filter_out_items.py
--rw-rw-r--   0 q         (1000) q         (1000)      782 2023-07-10 13:03:40.000000 hak-0.0.88/hak/many/strings/show_diff.py
--rw-rw-r--   0 q         (1000) q         (1000)      667 2023-07-06 06:56:51.000000 hak-0.0.88/hak/many/strings/to_dict.py
--rw-rw-r--   0 q         (1000) q         (1000)      357 2023-07-06 06:56:59.000000 hak-0.0.88/hak/many/strings/two_char_combinations.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/tuples/
--rw-rw-r--   0 q         (1000) q         (1000)      261 2023-07-10 13:16:50.000000 hak-0.0.88/hak/many/tuples/to_dict.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/many/values/
--rw-rw-r--   0 q         (1000) q         (1000)     2150 2023-07-16 01:20:55.000000 hak-0.0.88/hak/many/values/get_datatype.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/none/
--rw-rw-r--   0 q         (1000) q         (1000)       84 2023-07-06 06:57:14.000000 hak-0.0.88/hak/none/nop.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/bool/
--rw-rw-r--   0 q         (1000) q         (1000)       86 2023-07-06 06:57:21.000000 hak-0.0.88/hak/one/bool/fake.py
--rw-rw-r--   0 q         (1000) q         (1000)      103 2023-07-06 06:57:28.000000 hak-0.0.88/hak/one/bool/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/bool/or_none/
--rw-rw-r--   0 q         (1000) q         (1000)      164 2023-07-06 06:57:36.000000 hak-0.0.88/hak/one/bool/or_none/fake.py
--rw-rw-r--   0 q         (1000) q         (1000)      125 2023-07-06 06:57:43.000000 hak-0.0.88/hak/one/bool/or_none/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      762 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/check_if_ok_to_proceed.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/date/
--rw-rw-r--   0 q         (1000) q         (1000)      143 2023-07-06 06:57:58.000000 hak-0.0.88/hak/one/date/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      347 2023-07-06 06:58:06.000000 hak-0.0.88/hak/one/date/is_first_second_or_third_day_of_month.py
--rw-rw-r--   0 q         (1000) q         (1000)      414 2023-07-06 06:58:13.000000 hak-0.0.88/hak/one/date/is_first_week_of_quarter.py
--rw-rw-r--   0 q         (1000) q         (1000)      208 2023-07-06 06:58:20.000000 hak-0.0.88/hak/one/date/is_monday.py
--rw-rw-r--   0 q         (1000) q         (1000)      462 2023-07-06 06:58:28.000000 hak-0.0.88/hak/one/date/is_weekday.py
--rw-rw-r--   0 q         (1000) q         (1000)      467 2023-07-06 06:58:35.000000 hak-0.0.88/hak/one/date/is_weekend.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/date/public_holiday/
--rw-rw-r--   0 q         (1000) q         (1000)     4981 2023-07-10 13:17:27.000000 hak-0.0.88/hak/one/date/public_holiday/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      385 2023-07-06 06:58:50.000000 hak-0.0.88/hak/one/date/select_from_last_n_days.py
--rw-rw-r--   0 q         (1000) q         (1000)      146 2023-07-06 06:58:57.000000 hak-0.0.88/hak/one/date/to_dd_mm_yyyy_str.py
--rw-rw-r--   0 q         (1000) q         (1000)     1216 2023-07-10 13:17:49.000000 hak-0.0.88/hak/one/date/to_financial_year.py
--rw-rw-r--   0 q         (1000) q         (1000)      609 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/date/to_utc_timestamp.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.925642 hak-0.0.88/hak/one/date/year/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/date/year/easter_sunday/
--rw-rw-r--   0 q         (1000) q         (1000)      940 2023-07-10 13:18:07.000000 hak-0.0.88/hak/one/date/year/easter_sunday/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/datetime/
--rw-rw-r--   0 q         (1000) q         (1000)      149 2023-07-06 06:59:20.000000 hak-0.0.88/hak/one/datetime/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      272 2023-07-06 06:59:27.000000 hak-0.0.88/hak/one/datetime/select_from_last_n_days.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/dict/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:59:34.000000 hak-0.0.88/hak/one/dict/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/dict/cell/
--rw-rw-r--   0 q         (1000) q         (1000)     2230 2023-07-16 03:14:47.000000 hak-0.0.88/hak/one/dict/cell/get_width.py
--rw-rw-r--   0 q         (1000) q         (1000)     2575 2023-07-16 03:38:59.000000 hak-0.0.88/hak/one/dict/cell/make.py
--rw-rw-r--   0 q         (1000) q         (1000)     1475 2023-07-16 03:39:04.000000 hak-0.0.88/hak/one/dict/cell/to_str.py
--rw-rw-r--   0 q         (1000) q         (1000)      219 2023-07-06 06:59:42.000000 hak-0.0.88/hak/one/dict/convert_to_sql_insertable.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/dict/custom_order/
--rw-rw-r--   0 q         (1000) q         (1000)      445 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/dict/custom_order/apply.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/dict/durations/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:59:49.000000 hak-0.0.88/hak/one/dict/durations/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1147 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/dict/durations/load.py
--rw-rw-r--   0 q         (1000) q         (1000)      800 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/dict/durations/save.py
--rw-rw-r--   0 q         (1000) q         (1000)      134 2023-07-06 07:00:12.000000 hak-0.0.88/hak/one/dict/durations/to_tuple_list_sorted_by_duration.py
--rw-rw-r--   0 q         (1000) q         (1000)      769 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/dict/durations/update_one.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/dict/frequencies/
--rw-rw-r--   0 q         (1000) q         (1000)      519 2023-07-06 07:00:27.000000 hak-0.0.88/hak/one/dict/frequencies/choose.py
--rw-rw-r--   0 q         (1000) q         (1000)      385 2023-07-06 07:00:35.000000 hak-0.0.88/hak/one/dict/frequencies/make_from_strings.py
--rw-rw-r--   0 q         (1000) q         (1000)      187 2023-07-06 07:00:42.000000 hak-0.0.88/hak/one/dict/get_or_default.py
--rw-rw-r--   0 q         (1000) q         (1000)      616 2023-07-10 13:19:02.000000 hak-0.0.88/hak/one/dict/get_or_zero.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/dict/header/
--rw-rw-r--   0 q         (1000) q         (1000)     2423 2023-07-14 05:14:28.000000 hak-0.0.88/hak/one/dict/header/to_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/dict/hidden_fields/
--rw-rw-r--   0 q         (1000) q         (1000)      301 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/dict/hidden_fields/hide.py
--rw-rw-r--   0 q         (1000) q         (1000)      190 2023-07-06 07:00:57.000000 hak-0.0.88/hak/one/dict/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      116 2023-07-06 07:01:05.000000 hak-0.0.88/hak/one/dict/make_from_key_value_lists.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.933642 hak-0.0.88/hak/one/dict/period/
--rw-rw-r--   0 q         (1000) q         (1000)     1016 2023-07-10 14:58:58.000000 hak-0.0.88/hak/one/dict/period/contains_date.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/period/financial_year/
--rw-rw-r--   0 q         (1000) q         (1000)      896 2023-07-10 14:58:56.000000 hak-0.0.88/hak/one/dict/period/financial_year/contains_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      866 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/dict/period/financial_year/ge.py
--rw-rw-r--   0 q         (1000) q         (1000)      317 2023-07-10 14:58:55.000000 hak-0.0.88/hak/one/dict/period/financial_year/get_end_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      589 2023-07-10 14:58:54.000000 hak-0.0.88/hak/one/dict/period/financial_year/get_start_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/dict/period/financial_year/gt.py
--rw-rw-r--   0 q         (1000) q         (1000)      388 2023-07-10 13:04:13.000000 hak-0.0.88/hak/one/dict/period/financial_year/increment.py
--rw-rw-r--   0 q         (1000) q         (1000)     1415 2023-07-10 13:06:36.000000 hak-0.0.88/hak/one/dict/period/financial_year/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      866 2023-07-10 13:07:10.000000 hak-0.0.88/hak/one/dict/period/financial_year/le.py
--rw-rw-r--   0 q         (1000) q         (1000)      856 2023-07-10 13:07:47.000000 hak-0.0.88/hak/one/dict/period/financial_year/leq.py
--rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-10 13:08:14.000000 hak-0.0.88/hak/one/dict/period/financial_year/lt.py
--rw-rw-r--   0 q         (1000) q         (1000)     1733 2023-07-10 14:58:59.000000 hak-0.0.88/hak/one/dict/period/financial_year/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      255 2023-07-10 13:11:06.000000 hak-0.0.88/hak/one/dict/period/financial_year/to_str.py
--rw-rw-r--   0 q         (1000) q         (1000)     1307 2023-07-10 14:58:54.000000 hak-0.0.88/hak/one/dict/period/get_end.py
--rw-rw-r--   0 q         (1000) q         (1000)     1457 2023-07-10 15:00:35.000000 hak-0.0.88/hak/one/dict/period/get_start.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/period/month/
--rw-rw-r--   0 q         (1000) q         (1000)      460 2023-07-10 14:58:53.000000 hak-0.0.88/hak/one/dict/period/month/contains_date.py
--rw-rw-r--   0 q         (1000) q         (1000)     1179 2023-07-10 14:58:51.000000 hak-0.0.88/hak/one/dict/period/month/get_end_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      996 2023-07-10 14:58:50.000000 hak-0.0.88/hak/one/dict/period/month/get_start_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      283 2023-07-10 13:20:49.000000 hak-0.0.88/hak/one/dict/pick_by_keys.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/proposed_dismantlement/
--rw-rw-r--   0 q         (1000) q         (1000)     1544 2023-07-06 07:01:20.000000 hak-0.0.88/hak/one/dict/proposed_dismantlement/show.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/rate/
--rw-rw-r--   0 q         (1000) q         (1000)      733 2023-07-16 01:21:18.000000 hak-0.0.88/hak/one/dict/rate/abs.py
--rw-rw-r--   0 q         (1000) q         (1000)     1405 2023-07-16 04:02:13.000000 hak-0.0.88/hak/one/dict/rate/add.py
--rw-rw-r--   0 q         (1000) q         (1000)     1010 2023-07-16 01:21:27.000000 hak-0.0.88/hak/one/dict/rate/div_number_by_rate.py
--rw-rw-r--   0 q         (1000) q         (1000)      947 2023-07-16 03:39:08.000000 hak-0.0.88/hak/one/dict/rate/div_rate_by_rate.py
--rw-rw-r--   0 q         (1000) q         (1000)     1362 2023-07-16 03:39:13.000000 hak-0.0.88/hak/one/dict/rate/eq.py
--rw-rw-r--   0 q         (1000) q         (1000)      632 2023-07-16 03:34:20.000000 hak-0.0.88/hak/one/dict/rate/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)     3264 2023-07-16 01:21:47.000000 hak-0.0.88/hak/one/dict/rate/make.py
--rw-rw-r--   0 q         (1000) q         (1000)     1165 2023-07-16 03:39:18.000000 hak-0.0.88/hak/one/dict/rate/mult_rate_by_number.py
--rw-rw-r--   0 q         (1000) q         (1000)     1409 2023-07-16 03:39:23.000000 hak-0.0.88/hak/one/dict/rate/mult_rate_by_rate.py
--rw-rw-r--   0 q         (1000) q         (1000)     1410 2023-07-16 03:39:28.000000 hak-0.0.88/hak/one/dict/rate/sub.py
--rw-rw-r--   0 q         (1000) q         (1000)      636 2023-07-16 03:30:41.000000 hak-0.0.88/hak/one/dict/rate/to_float.py
--rw-rw-r--   0 q         (1000) q         (1000)      664 2023-07-16 01:20:47.000000 hak-0.0.88/hak/one/dict/rate/to_num.py
--rw-rw-r--   0 q         (1000) q         (1000)      365 2023-07-16 03:39:33.000000 hak-0.0.88/hak/one/dict/rate/to_str.py
--rw-rw-r--   0 q         (1000) q         (1000)      283 2023-07-16 03:39:37.000000 hak-0.0.88/hak/one/dict/rate/to_str_frac.py
--rw-rw-r--   0 q         (1000) q         (1000)      852 2023-07-16 01:22:11.000000 hak-0.0.88/hak/one/dict/remove_zeroes.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/table/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 05:28:26.000000 hak-0.0.88/hak/one/dict/table/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1222 2023-07-16 03:09:12.000000 hak-0.0.88/hak/one/dict/table/get_field_widths.py
--rw-rw-r--   0 q         (1000) q         (1000)     4031 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/dict/to_max_line_width_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/values/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:43.000000 hak-0.0.88/hak/one/dict/values/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/values/numbers/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:50.000000 hak-0.0.88/hak/one/dict/values/numbers/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/values/numbers/negative/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:58.000000 hak-0.0.88/hak/one/dict/values/numbers/negative/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      281 2023-07-10 13:21:57.000000 hak-0.0.88/hak/one/dict/values/numbers/negative/count.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/dict/values/numbers/positive/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:03:13.000000 hak-0.0.88/hak/one/dict/values/numbers/positive/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      281 2023-07-10 13:22:10.000000 hak-0.0.88/hak/one/dict/values/numbers/positive/count.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/directory/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:03:28.000000 hak-0.0.88/hak/one/directory/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1568 2023-07-06 07:03:35.000000 hak-0.0.88/hak/one/directory/compress_to_tar.py
--rw-rw-r--   0 q         (1000) q         (1000)      728 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/directory/empty.py
--rw-rw-r--   0 q         (1000) q         (1000)       88 2023-07-06 07:03:51.000000 hak-0.0.88/hak/one/directory/exists.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/directory/filepaths/
--rw-rw-r--   0 q         (1000) q         (1000)     1463 2023-07-10 13:28:32.000000 hak-0.0.88/hak/one/directory/filepaths/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/directory/filepaths/packages/
--rw-rw-r--   0 q         (1000) q         (1000)     1311 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/directory/filepaths/packages/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      641 2023-07-10 13:22:24.000000 hak-0.0.88/hak/one/directory/is_empty.py
--rw-rw-r--   0 q         (1000) q         (1000)      662 2023-07-06 07:04:36.000000 hak-0.0.88/hak/one/directory/is_module.py
--rw-rw-r--   0 q         (1000) q         (1000)      763 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/directory/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      810 2023-07-07 01:06:11.000000 hak-0.0.88/hak/one/directory/remove.py
--rw-rw-r--   0 q         (1000) q         (1000)     3737 2023-07-06 07:04:58.000000 hak-0.0.88/hak/one/duration.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/file/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:05:06.000000 hak-0.0.88/hak/one/file/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      793 2023-07-06 07:05:13.000000 hak-0.0.88/hak/one/file/decrypt.py
--rw-rw-r--   0 q         (1000) q         (1000)      945 2023-07-06 07:05:20.000000 hak-0.0.88/hak/one/file/encrypt.py
--rw-rw-r--   0 q         (1000) q         (1000)      586 2023-07-10 13:22:54.000000 hak-0.0.88/hak/one/file/get_next_line_as_int.py
--rw-rw-r--   0 q         (1000) q         (1000)      705 2023-07-06 07:05:35.000000 hak-0.0.88/hak/one/file/load.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/file/pickle/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:05:42.000000 hak-0.0.88/hak/one/file/pickle/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1265 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/file/pickle/load_if_exists.py
--rw-rw-r--   0 q         (1000) q         (1000)      922 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/file/pickle/save.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/file/py/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:06:05.000000 hak-0.0.88/hak/one/file/py/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      566 2023-07-06 07:06:12.000000 hak-0.0.88/hak/one/file/py/create.py
--rw-rw-r--   0 q         (1000) q         (1000)     2645 2023-07-06 07:06:19.000000 hak-0.0.88/hak/one/file/py/dismantle.py
--rw-rw-r--   0 q         (1000) q         (1000)     3827 2023-07-06 07:06:27.000000 hak-0.0.88/hak/one/file/py/extract_fn.py
--rw-rw-r--   0 q         (1000) q         (1000)       84 2023-07-06 07:06:34.000000 hak-0.0.88/hak/one/file/py/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-06 07:06:42.000000 hak-0.0.88/hak/one/file/remove.py
--rw-rw-r--   0 q         (1000) q         (1000)      963 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/file/save.py
--rw-rw-r--   0 q         (1000) q         (1000)      770 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/file/save_lines.py
--rw-rw-r--   0 q         (1000) q         (1000)      324 2023-07-06 07:07:04.000000 hak-0.0.88/hak/one/file/save_lines_or_string.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.925642 hak-0.0.88/hak/one/file/secret/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/file/secret/password/
--rw-rw-r--   0 q         (1000) q         (1000)      696 2023-07-06 07:07:12.000000 hak-0.0.88/hak/one/file/secret/password/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/file/secret/username/
--rw-rw-r--   0 q         (1000) q         (1000)      737 2023-07-06 07:07:19.000000 hak-0.0.88/hak/one/file/secret/username/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/file/tar/
--rw-rw-r--   0 q         (1000) q         (1000)     1574 2023-07-06 07:07:26.000000 hak-0.0.88/hak/one/file/tar/extract.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/file/zip/
--rw-rw-r--   0 q         (1000) q         (1000)      507 2023-07-06 07:07:35.000000 hak-0.0.88/hak/one/file/zip/extract.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.937642 hak-0.0.88/hak/one/function/
--rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-06 08:33:41.000000 hak-0.0.88/hak/one/function/function.py
--rw-rw-r--   0 q         (1000) q         (1000)      439 2023-07-06 08:33:48.000000 hak-0.0.88/hak/one/function/write_to_file.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/list/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:33:56.000000 hak-0.0.88/hak/one/list/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      116 2023-07-06 08:34:03.000000 hak-0.0.88/hak/one/list/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      115 2023-07-06 08:34:11.000000 hak-0.0.88/hak/one/list/to_comma_separated_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/duration_ms/
--rw-rw-r--   0 q         (1000) q         (1000)     2120 2023-07-06 08:34:18.000000 hak-0.0.88/hak/one/number/duration_ms/to_bar.py
--rw-rw-r--   0 q         (1000) q         (1000)      296 2023-07-06 08:34:26.000000 hak-0.0.88/hak/one/number/duration_ms/to_bar_width.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/float/
--rw-rw-r--   0 q         (1000) q         (1000)       70 2023-07-06 08:34:33.000000 hak-0.0.88/hak/one/number/float/epsilon.py
--rw-rw-r--   0 q         (1000) q         (1000)      106 2023-07-06 08:34:41.000000 hak-0.0.88/hak/one/number/float/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      106 2023-07-06 08:34:48.000000 hak-0.0.88/hak/one/number/float/is_not.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/float/nan/
--rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 08:34:55.000000 hak-0.0.88/hak/one/number/float/nan/to_none.py
--rw-rw-r--   0 q         (1000) q         (1000)      740 2023-07-10 13:23:05.000000 hak-0.0.88/hak/one/number/float/snap_to_zero.py
--rw-rw-r--   0 q         (1000) q         (1000)      477 2023-07-16 00:13:38.000000 hak-0.0.88/hak/one/number/float/to_rate.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/days/
--rw-rw-r--   0 q         (1000) q         (1000)      227 2023-07-06 08:35:11.000000 hak-0.0.88/hak/one/number/int/days/a_to_b_inclusive.py
--rw-rw-r--   0 q         (1000) q         (1000)      104 2023-07-06 08:35:18.000000 hak-0.0.88/hak/one/number/int/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      434 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/number/int/is_prime.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/polarity/
--rw-rw-r--   0 q         (1000) q         (1000)      499 2023-07-10 13:23:20.000000 hak-0.0.88/hak/one/number/int/polarity/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/primes/
--rw-rw-r--   0 q         (1000) q         (1000)      867 2023-07-06 08:35:40.000000 hak-0.0.88/hak/one/number/int/primes/download_prime_10.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/primes/prime_factors/
--rw-rw-r--   0 q         (1000) q         (1000)     2200 2023-07-15 10:34:36.000000 hak-0.0.88/hak/one/number/int/primes/prime_factors/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/width/
--rw-rw-r--   0 q         (1000) q         (1000)      579 2023-07-06 08:35:55.000000 hak-0.0.88/hak/one/number/int/width/to_text_colour.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/year/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/year/days/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/year/days/count/
--rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 08:36:03.000000 hak-0.0.88/hak/one/number/int/year/days/count/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/number/int/year/days/first/
--rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:36:10.000000 hak-0.0.88/hak/one/number/int/year/days/first/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      431 2023-07-06 08:36:18.000000 hak-0.0.88/hak/one/number/int/year/days/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      916 2023-07-10 13:23:34.000000 hak-0.0.88/hak/one/number/int/year/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      153 2023-07-06 08:36:26.000000 hak-0.0.88/hak/one/number/int/year/now.py
--rw-rw-r--   0 q         (1000) q         (1000)      824 2023-07-14 04:32:30.000000 hak-0.0.88/hak/one/number/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      123 2023-07-06 08:36:33.000000 hak-0.0.88/hak/one/number/log_2.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/period/
--rw-rw-r--   0 q         (1000) q         (1000)      333 2023-07-06 08:36:40.000000 hak-0.0.88/hak/one/period/contains_day.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/schedule/
--rw-rw-r--   0 q         (1000) q         (1000)     3465 2023-07-06 08:36:48.000000 hak-0.0.88/hak/one/schedule/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/session/
--rw-rw-r--   0 q         (1000) q         (1000)      146 2023-07-06 08:36:55.000000 hak-0.0.88/hak/one/session/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/set/
--rw-rw-r--   0 q         (1000) q         (1000)      114 2023-07-06 08:37:03.000000 hak-0.0.88/hak/one/set/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/string/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:37:10.000000 hak-0.0.88/hak/one/string/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/string/alphanumeric/
--rw-rw-r--   0 q         (1000) q         (1000)      264 2023-07-06 08:37:18.000000 hak-0.0.88/hak/one/string/alphanumeric/fake.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/string/append/
--rw-rw-r--   0 q         (1000) q         (1000)       54 2023-07-06 08:37:25.000000 hak-0.0.88/hak/one/string/append/new_line.py
--rw-rw-r--   0 q         (1000) q         (1000)      549 2023-07-06 08:37:33.000000 hak-0.0.88/hak/one/string/camel_to_snake.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/string/char/
--rw-rw-r--   0 q         (1000) q         (1000)      326 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/char/find_all_indices.py
--rw-rw-r--   0 q         (1000) q         (1000)      128 2023-07-06 08:37:47.000000 hak-0.0.88/hak/one/string/char/is_digit.py
--rw-rw-r--   0 q         (1000) q         (1000)      207 2023-07-06 08:37:55.000000 hak-0.0.88/hak/one/string/char/is_upper.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/string/char/last/
--rw-rw-r--   0 q         (1000) q         (1000)      177 2023-07-06 08:38:02.000000 hak-0.0.88/hak/one/string/char/last/find.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.941642 hak-0.0.88/hak/one/string/chars/
--rw-rw-r--   0 q         (1000) q         (1000)      561 2023-07-06 08:38:10.000000 hak-0.0.88/hak/one/string/chars/remove.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/colour/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:38:17.000000 hak-0.0.88/hak/one/string/colour/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/colour/bright/
--rw-rw-r--   0 q         (1000) q         (1000)      166 2023-07-06 08:38:25.000000 hak-0.0.88/hak/one/string/colour/bright/blue.py
--rw-rw-r--   0 q         (1000) q         (1000)      166 2023-07-06 08:38:32.000000 hak-0.0.88/hak/one/string/colour/bright/cyan.py
--rw-rw-r--   0 q         (1000) q         (1000)      168 2023-07-06 08:38:40.000000 hak-0.0.88/hak/one/string/colour/bright/green.py
--rw-rw-r--   0 q         (1000) q         (1000)      172 2023-07-06 08:38:47.000000 hak-0.0.88/hak/one/string/colour/bright/magenta.py
--rw-rw-r--   0 q         (1000) q         (1000)      164 2023-07-06 08:38:55.000000 hak-0.0.88/hak/one/string/colour/bright/red.py
--rw-rw-r--   0 q         (1000) q         (1000)      168 2023-07-06 08:39:02.000000 hak-0.0.88/hak/one/string/colour/bright/white.py
--rw-rw-r--   0 q         (1000) q         (1000)      170 2023-07-06 08:39:10.000000 hak-0.0.88/hak/one/string/colour/bright/yellow.py
--rw-rw-r--   0 q         (1000) q         (1000)      134 2023-07-06 08:39:17.000000 hak-0.0.88/hak/one/string/colour/danger.py
--rw-rw-r--   0 q         (1000) q         (1000)      178 2023-07-06 08:39:25.000000 hak-0.0.88/hak/one/string/colour/danger_if_zero.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/colour/dark/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:39:32.000000 hak-0.0.88/hak/one/string/colour/dark/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      152 2023-07-06 08:39:40.000000 hak-0.0.88/hak/one/string/colour/dark/blue.py
--rw-rw-r--   0 q         (1000) q         (1000)      152 2023-07-06 08:39:47.000000 hak-0.0.88/hak/one/string/colour/dark/cyan.py
--rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-06 08:39:55.000000 hak-0.0.88/hak/one/string/colour/dark/default.py
--rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:40:03.000000 hak-0.0.88/hak/one/string/colour/dark/green.py
--rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-06 08:40:10.000000 hak-0.0.88/hak/one/string/colour/dark/magenta.py
--rw-rw-r--   0 q         (1000) q         (1000)      150 2023-07-06 08:40:18.000000 hak-0.0.88/hak/one/string/colour/dark/red.py
--rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:40:25.000000 hak-0.0.88/hak/one/string/colour/dark/white.py
--rw-rw-r--   0 q         (1000) q         (1000)      156 2023-07-06 08:40:33.000000 hak-0.0.88/hak/one/string/colour/dark/yellow.py
--rw-rw-r--   0 q         (1000) q         (1000)       64 2023-07-06 08:40:40.000000 hak-0.0.88/hak/one/string/colour/data.py
--rw-rw-r--   0 q         (1000) q         (1000)     3430 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/colour/decolour.py
--rw-rw-r--   0 q         (1000) q         (1000)      135 2023-07-06 08:40:47.000000 hak-0.0.88/hak/one/string/colour/info.py
--rw-rw-r--   0 q         (1000) q         (1000)      135 2023-07-06 08:40:55.000000 hak-0.0.88/hak/one/string/colour/primary.py
--rw-rw-r--   0 q         (1000) q         (1000)     2321 2023-07-06 08:41:02.000000 hak-0.0.88/hak/one/string/colour/rainbow.py
--rw-rw-r--   0 q         (1000) q         (1000)      138 2023-07-06 08:41:10.000000 hak-0.0.88/hak/one/string/colour/secondary.py
--rw-rw-r--   0 q         (1000) q         (1000)      275 2023-07-06 08:41:17.000000 hak-0.0.88/hak/one/string/colour/tgfr.py
--rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 08:41:25.000000 hak-0.0.88/hak/one/string/colour/warning.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/contains/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:41:32.000000 hak-0.0.88/hak/one/string/contains/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/contains/function/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:41:40.000000 hak-0.0.88/hak/one/string/contains/function/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-06 08:41:47.000000 hak-0.0.88/hak/one/string/contains/function/run.py
--rw-rw-r--   0 q         (1000) q         (1000)      192 2023-07-07 05:12:17.000000 hak-0.0.88/hak/one/string/contains/function/test.py
--rw-rw-r--   0 q         (1000) q         (1000)      224 2023-07-06 08:42:02.000000 hak-0.0.88/hak/one/string/contains/l.py
--rw-rw-r--   0 q         (1000) q         (1000)       76 2023-07-06 08:42:10.000000 hak-0.0.88/hak/one/string/contains/version.py
--rw-rw-r--   0 q         (1000) q         (1000)      105 2023-07-06 08:42:17.000000 hak-0.0.88/hak/one/string/count_x_in_y.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/date/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/date/separator/
--rw-rw-r--   0 q         (1000) q         (1000)      923 2023-07-10 13:23:48.000000 hak-0.0.88/hak/one/string/date/separator/get.py
--rw-rw-r--   0 q         (1000) q         (1000)     1924 2023-07-10 14:58:52.000000 hak-0.0.88/hak/one/string/date/to_date.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/day/
--rw-rw-r--   0 q         (1000) q         (1000)     1076 2023-07-10 13:25:17.000000 hak-0.0.88/hak/one/string/day/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      996 2023-07-06 08:42:32.000000 hak-0.0.88/hak/one/string/delete_character_safely.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/digits/
--rw-rw-r--   0 q         (1000) q         (1000)      206 2023-07-06 08:42:40.000000 hak-0.0.88/hak/one/string/digits/remove.py
--rw-rw-r--   0 q         (1000) q         (1000)      111 2023-07-06 08:42:47.000000 hak-0.0.88/hak/one/string/double_single_quotes.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/family_name/
--rw-rw-r--   0 q         (1000) q         (1000)   121166 2023-07-07 04:10:06.000000 hak-0.0.88/hak/one/string/family_name/fake.py
--rw-rw-r--   0 q         (1000) q         (1000)      303 2023-07-06 08:43:10.000000 hak-0.0.88/hak/one/string/family_name/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/filename/
--rw-rw-r--   0 q         (1000) q         (1000)      126 2023-07-06 08:43:25.000000 hak-0.0.88/hak/one/string/filename/to_module_name.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/filepath/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:43:32.000000 hak-0.0.88/hak/one/string/filepath/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/filepath/py/
--rw-rw-r--   0 q         (1000) q         (1000)      720 2023-07-06 08:43:39.000000 hak-0.0.88/hak/one/string/filepath/py/get_t.py
--rw-rw-r--   0 q         (1000) q         (1000)      100 2023-07-06 08:43:47.000000 hak-0.0.88/hak/one/string/find_first_parenthesis.py
--rw-rw-r--   0 q         (1000) q         (1000)      213 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/find_last_comma_index.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/fn_name/
--rw-rw-r--   0 q         (1000) q         (1000)      226 2023-07-06 08:44:02.000000 hak-0.0.88/hak/one/string/fn_name/is_ignorable.py
--rw-rw-r--   0 q         (1000) q         (1000)     5035 2023-07-06 08:44:09.000000 hak-0.0.88/hak/one/string/format.py
--rw-rw-r--   0 q         (1000) q         (1000)       73 2023-07-06 08:44:17.000000 hak-0.0.88/hak/one/string/has_at_symbol.py
--rw-rw-r--   0 q         (1000) q         (1000)      132 2023-07-06 08:44:24.000000 hak-0.0.88/hak/one/string/has_digit.py
--rw-rw-r--   0 q         (1000) q         (1000)      131 2023-07-06 08:44:32.000000 hak-0.0.88/hak/one/string/has_lowercase.py
--rw-rw-r--   0 q         (1000) q         (1000)      263 2023-07-06 08:44:39.000000 hak-0.0.88/hak/one/string/has_other_char.py
--rw-rw-r--   0 q         (1000) q         (1000)      176 2023-07-06 08:44:47.000000 hak-0.0.88/hak/one/string/has_seven_digits.py
--rw-rw-r--   0 q         (1000) q         (1000)      132 2023-07-06 08:44:54.000000 hak-0.0.88/hak/one/string/has_uppercase.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/hbar/
--rw-rw-r--   0 q         (1000) q         (1000)      122 2023-07-06 08:45:02.000000 hak-0.0.88/hak/one/string/hbar/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.925642 hak-0.0.88/hak/one/string/header/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/header/python_file/
--rw-rw-r--   0 q         (1000) q         (1000)      322 2023-07-06 08:45:09.000000 hak-0.0.88/hak/one/string/header/python_file/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/header/test_table/
--rw-rw-r--   0 q         (1000) q         (1000)      461 2023-07-06 08:45:17.000000 hak-0.0.88/hak/one/string/header/test_table/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/indent/
--rw-rw-r--   0 q         (1000) q         (1000)      137 2023-07-06 08:45:25.000000 hak-0.0.88/hak/one/string/indent/run_if_class_method.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/insert/
--rw-rw-r--   0 q         (1000) q         (1000)      602 2023-07-06 08:45:32.000000 hak-0.0.88/hak/one/string/insert/new_line_after_last_import_line.py
--rw-rw-r--   0 q         (1000) q         (1000)      278 2023-07-06 08:45:40.000000 hak-0.0.88/hak/one/string/insert/new_line_before_comment.py
--rw-rw-r--   0 q         (1000) q         (1000)      584 2023-07-06 08:45:48.000000 hak-0.0.88/hak/one/string/insert/new_line_before_def.py
--rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 08:45:56.000000 hak-0.0.88/hak/one/string/insert/new_line_before_if_main.py
--rw-rw-r--   0 q         (1000) q         (1000)      670 2023-07-06 08:46:04.000000 hak-0.0.88/hak/one/string/insert/new_line_before_lambda.py
--rw-rw-r--   0 q         (1000) q         (1000)      292 2023-07-06 08:46:12.000000 hak-0.0.88/hak/one/string/insert/new_line_before_new_line_and_cea_.py
--rw-rw-r--   0 q         (1000) q         (1000)      102 2023-07-06 08:46:20.000000 hak-0.0.88/hak/one/string/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      124 2023-07-06 08:46:27.000000 hak-0.0.88/hak/one/string/is_or_none.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/json/
--rw-rw-r--   0 q         (1000) q         (1000)      179 2023-07-06 08:46:35.000000 hak-0.0.88/hak/one/string/json/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      552 2023-07-06 08:46:42.000000 hak-0.0.88/hak/one/string/lambdarise.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/one/string/line/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/one/string/line/last/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/line/last/length/
--rw-rw-r--   0 q         (1000) q         (1000)      423 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/line/last/length/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      368 2023-07-06 08:46:58.000000 hak-0.0.88/hak/one/string/make_content_without_function.py
--rw-rw-r--   0 q         (1000) q         (1000)      333 2023-07-06 08:47:06.000000 hak-0.0.88/hak/one/string/make_function_text.py
--rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-06 08:47:13.000000 hak-0.0.88/hak/one/string/make_initial_content.py
--rw-rw-r--   0 q         (1000) q         (1000)      327 2023-07-06 08:47:21.000000 hak-0.0.88/hak/one/string/make_new_function_text.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/money/
--rw-rw-r--   0 q         (1000) q         (1000)      541 2023-07-10 13:25:31.000000 hak-0.0.88/hak/one/string/money/to_float.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/month/
--rw-rw-r--   0 q         (1000) q         (1000)     1009 2023-07-10 13:25:45.000000 hak-0.0.88/hak/one/string/month/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      559 2023-07-10 14:58:57.000000 hak-0.0.88/hak/one/string/month/to_number.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/nest_level/
--rw-rw-r--   0 q         (1000) q         (1000)      688 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/nest_level/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/password/
--rw-rw-r--   0 q         (1000) q         (1000)     1187 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/password/create.py
--rw-rw-r--   0 q         (1000) q         (1000)      555 2023-07-06 08:47:50.000000 hak-0.0.88/hak/one/string/password/has_chars_from_3_sets.py
--rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/pop_left.py
--rw-rw-r--   0 q         (1000) q         (1000)      223 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/pop_right.py
--rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 08:48:13.000000 hak-0.0.88/hak/one/string/prepend_import.py
--rw-rw-r--   0 q         (1000) q         (1000)      756 2023-07-06 08:48:20.000000 hak-0.0.88/hak/one/string/print_and_return_false.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/refactor/
--rw-rw-r--   0 q         (1000) q         (1000)     1218 2023-07-06 08:48:28.000000 hak-0.0.88/hak/one/string/refactor/by_two_char_combinations.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/remove/
--rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-06 08:48:35.000000 hak-0.0.88/hak/one/string/remove/empty_line_spaces.py
--rw-rw-r--   0 q         (1000) q         (1000)      162 2023-07-06 08:48:42.000000 hak-0.0.88/hak/one/string/remove/empty_lines.py
--rw-rw-r--   0 q         (1000) q         (1000)      441 2023-07-06 08:48:50.000000 hak-0.0.88/hak/one/string/remove/extra_new_line_following_class_definition.py
--rw-rw-r--   0 q         (1000) q         (1000)      210 2023-07-06 08:48:57.000000 hak-0.0.88/hak/one/string/remove/first_new_line_if_starts_with_new_line.py
--rw-rw-r--   0 q         (1000) q         (1000)       81 2023-07-06 08:49:04.000000 hak-0.0.88/hak/one/string/remove/whitespace_between_newlines.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/replace/
--rw-rw-r--   0 q         (1000) q         (1000)      241 2023-07-06 08:49:12.000000 hak-0.0.88/hak/one/string/replace/double_new_line_with_single_new_line.py
--rw-rw-r--   0 q         (1000) q         (1000)      129 2023-07-06 08:49:20.000000 hak-0.0.88/hak/one/string/replace/single_new_line_with_empty_string.py
--rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 08:49:27.000000 hak-0.0.88/hak/one/string/replace/triple_new_line_with_double_new_line.py
--rw-rw-r--   0 q         (1000) q         (1000)      487 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/string/replace_unprintable.py
--rw-rw-r--   0 q         (1000) q         (1000)     3365 2023-07-06 08:49:42.000000 hak-0.0.88/hak/one/string/separate_function_from_context.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/single_line_function/
--rw-rw-r--   0 q         (1000) q         (1000)      432 2023-07-06 08:49:49.000000 hak-0.0.88/hak/one/string/single_line_function/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      467 2023-07-06 08:49:57.000000 hak-0.0.88/hak/one/string/single_line_function/to_lambda_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.945642 hak-0.0.88/hak/one/string/spaces/
--rw-rw-r--   0 q         (1000) q         (1000)      111 2023-07-06 08:50:05.000000 hak-0.0.88/hak/one/string/spaces/count.py
--rw-rw-r--   0 q         (1000) q         (1000)      331 2023-07-06 08:50:12.000000 hak-0.0.88/hak/one/string/split_fn_name_and_text.py
--rw-rw-r--   0 q         (1000) q         (1000)      344 2023-07-06 08:50:20.000000 hak-0.0.88/hak/one/string/strip_unprintable.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/string/table/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 05:28:43.000000 hak-0.0.88/hak/one/string/table/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/string/table/bar/
--rw-rw-r--   0 q         (1000) q         (1000)      366 2023-07-14 05:27:26.000000 hak-0.0.88/hak/one/string/table/bar/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      265 2023-07-06 08:50:27.000000 hak-0.0.88/hak/one/string/to_cond_freq_dict.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/string/token/
--rw-rw-r--   0 q         (1000) q         (1000)     1263 2023-07-06 08:50:35.000000 hak-0.0.88/hak/one/string/token/substitute.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/string/year/
--rw-rw-r--   0 q         (1000) q         (1000)      177 2023-07-10 13:26:13.000000 hak-0.0.88/hak/one/string/year/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/string/yyyymmdd/
--rw-rw-r--   0 q         (1000) q         (1000)      238 2023-07-06 08:50:42.000000 hak-0.0.88/hak/one/string/yyyymmdd/to_date.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/one/subprocess/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/subprocess/completed_process/
--rw-rw-r--   0 q         (1000) q         (1000)      647 2023-07-07 01:06:09.000000 hak-0.0.88/hak/one/subprocess/completed_process/to_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/system/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:50:57.000000 hak-0.0.88/hak/one/system/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/system/git/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/system/git/commit/
--rw-rw-r--   0 q         (1000) q         (1000)     2527 2023-07-06 08:51:35.000000 hak-0.0.88/hak/one/system/git/commit/run.py
--rw-rw-r--   0 q         (1000) q         (1000)      393 2023-07-06 08:51:42.000000 hak-0.0.88/hak/one/system/git/commit_if_test_and_app_ok.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/system/git/gitignore/
--rw-rw-r--   0 q         (1000) q         (1000)      647 2023-07-06 08:51:51.000000 hak-0.0.88/hak/one/system/git/gitignore/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      485 2023-07-07 01:09:02.000000 hak-0.0.88/hak/one/system/git/init.py
--rw-rw-r--   0 q         (1000) q         (1000)      745 2023-07-06 08:52:07.000000 hak-0.0.88/hak/one/system/git/log_oneline.py
--rw-rw-r--   0 q         (1000) q         (1000)      870 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/system/git/push_after_delay.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/system/screen/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:52:21.000000 hak-0.0.88/hak/one/system/screen/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      786 2023-07-06 08:52:29.000000 hak-0.0.88/hak/one/system/screen/clear.py
--rw-rw-r--   0 q         (1000) q         (1000)     3127 2023-07-10 13:03:40.000000 hak-0.0.88/hak/one/terminal.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/one/tup/
--rw-rw-r--   0 q         (1000) q         (1000)      176 2023-07-06 08:52:44.000000 hak-0.0.88/hak/one/tup/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/
--rw-rw-r--   0 q         (1000) q         (1000)      430 2023-07-07 01:09:29.000000 hak-0.0.88/hak/other/l.py
--rw-rw-r--   0 q         (1000) q         (1000)       91 2023-07-06 08:52:59.000000 hak-0.0.88/hak/other/nop_state_x.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/patch/
--rw-rw-r--   0 q         (1000) q         (1000)     7954 2023-07-10 13:03:40.000000 hak-0.0.88/hak/other/patch/do.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/pip/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/pip/dist_tar/
--rw-rw-r--   0 q         (1000) q         (1000)     3093 2023-07-10 13:27:41.000000 hak-0.0.88/hak/other/pip/dist_tar/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      805 2023-07-10 13:03:40.000000 hak-0.0.88/hak/other/pip/dist_tar/remove.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/pip/setup/
--rw-rw-r--   0 q         (1000) q         (1000)     1321 2023-07-06 08:53:29.000000 hak-0.0.88/hak/other/pip/setup/update.py
--rw-rw-r--   0 q         (1000) q         (1000)     1808 2023-07-10 13:03:40.000000 hak-0.0.88/hak/other/pip/upload.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/pip/version/
--rw-rw-r--   0 q         (1000) q         (1000)      897 2023-07-10 13:03:40.000000 hak-0.0.88/hak/other/pip/version/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      120 2023-07-06 22:28:42.000000 hak-0.0.88/hak/other/pip/version/to_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/report/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/report/fail/
--rw-rw-r--   0 q         (1000) q         (1000)      822 2023-07-06 22:28:49.000000 hak-0.0.88/hak/other/report/fail/no_xyz.py
--rw-rw-r--   0 q         (1000) q         (1000)     1936 2023-07-06 22:28:57.000000 hak-0.0.88/hak/other/report/fail/xyz.py
--rw-rw-r--   0 q         (1000) q         (1000)     1462 2023-07-06 22:29:04.000000 hak-0.0.88/hak/other/report/fail/z_return_neq_y_return.py
--rw-rw-r--   0 q         (1000) q         (1000)     1623 2023-07-06 22:29:12.000000 hak-0.0.88/hak/other/report/fail/z_stdo_neq_y_stdo.py
--rw-rw-r--   0 q         (1000) q         (1000)      895 2023-07-06 22:29:19.000000 hak-0.0.88/hak/other/report/property_failure.py
--rw-rw-r--   0 q         (1000) q         (1000)      737 2023-07-06 22:29:27.000000 hak-0.0.88/hak/other/report/success.py
--rw-rw-r--   0 q         (1000) q         (1000)      394 2023-07-06 22:29:34.000000 hak-0.0.88/hak/other/report/summarise_file.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak/other/setup/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/setup/cfg/
--rw-rw-r--   0 q         (1000) q         (1000)     1547 2023-07-06 22:29:41.000000 hak-0.0.88/hak/other/setup/cfg/update.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/other/setup/py/
--rw-rw-r--   0 q         (1000) q         (1000)     1653 2023-07-10 13:03:40.000000 hak-0.0.88/hak/other/setup/py/update.py
--rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-10 13:03:40.000000 hak-0.0.88/hak/other/ternary.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/pair/
--rw-rw-r--   0 q         (1000) q         (1000)      140 2023-07-06 22:30:04.000000 hak-0.0.88/hak/pair/eq.py
--rw-rw-r--   0 q         (1000) q         (1000)      150 2023-07-10 13:03:46.000000 hak-0.0.88/hak/pxyz.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/test/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.88/hak/test/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     2658 2023-07-06 06:52:54.000000 hak-0.0.88/hak/test/do.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/test/failed/
--rw-rw-r--   0 q         (1000) q         (1000)     1112 2023-07-06 06:53:05.000000 hak-0.0.88/hak/test/failed/handle.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/test/final_line/
--rw-rw-r--   0 q         (1000) q         (1000)     2531 2023-07-10 13:03:40.000000 hak-0.0.88/hak/test/final_line/check.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/test/line_lengths/
--rw-rw-r--   0 q         (1000) q         (1000)     2717 2023-07-10 13:03:40.000000 hak-0.0.88/hak/test/line_lengths/check.py
--rw-rw-r--   0 q         (1000) q         (1000)      790 2023-07-10 13:03:40.000000 hak-0.0.88/hak/test/line_lengths_check.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/test/oldest_file/
--rw-rw-r--   0 q         (1000) q         (1000)     4789 2023-07-10 13:03:40.000000 hak-0.0.88/hak/test/oldest_file/print.py
--rw-rw-r--   0 q         (1000) q         (1000)      937 2023-07-06 06:53:55.000000 hak-0.0.88/hak/test/oldest_file_print.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.949642 hak-0.0.88/hak/test/passed/
--rw-rw-r--   0 q         (1000) q         (1000)      961 2023-07-06 06:54:05.000000 hak-0.0.88/hak/test/passed/handle.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-16 04:05:54.929642 hak-0.0.88/hak.egg-info/
--rw-rw-r--   0 q         (1000) q         (1000)     1212 2023-07-16 04:05:54.000000 hak-0.0.88/hak.egg-info/PKG-INFO
--rw-rw-r--   0 q         (1000) q         (1000)    12798 2023-07-16 04:05:54.000000 hak-0.0.88/hak.egg-info/SOURCES.txt
--rw-rw-r--   0 q         (1000) q         (1000)        1 2023-07-16 04:05:54.000000 hak-0.0.88/hak.egg-info/dependency_links.txt
--rw-rw-r--   0 q         (1000) q         (1000)     3372 2023-07-16 04:05:54.000000 hak-0.0.88/hak.egg-info/top_level.txt
--rw-rw-r--   0 q         (1000) q         (1000)      537 2023-07-16 04:05:54.949642 hak-0.0.88/setup.cfg
--rw-rw-r--   0 q         (1000) q         (1000)      576 2023-07-16 04:05:54.000000 hak-0.0.88/setup.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/
+-rw-rw-r--   0 a         (1009) a         (1010)     1068 2023-04-19 01:55:38.000000 hak-0.0.9/LICENSE
+-rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:43:20.718405 hak-0.0.9/PKG-INFO
+-rw-rw-r--   0 a         (1009) a         (1010)      406 2023-04-19 03:24:53.000000 hak-0.0.9/README.md
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      140 2023-04-19 01:55:38.000000 hak-0.0.9/hak/a_equals_b.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/bool/
+-rw-rw-r--   0 a         (1009) a         (1010)       86 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bool/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      103 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bool/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/bool/or_none/
+-rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bool/or_none/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      125 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bool/or_none/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/bools/
+-rw-rw-r--   0 a         (1009) a         (1010)      139 2023-04-19 01:55:38.000000 hak-0.0.9/hak/bools/count_true.py
+-rw-rw-r--   0 a         (1009) a         (1010)      249 2023-04-19 01:55:38.000000 hak-0.0.9/hak/calculate_duration_bar_width.py
+-rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.9/hak/check_if_ok_to_proceed.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/date/
+-rw-rw-r--   0 a         (1009) a         (1010)      143 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      347 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_first_second_or_third_day_of_month.py
+-rw-rw-r--   0 a         (1009) a         (1010)      414 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_first_week_of_quarter.py
+-rw-rw-r--   0 a         (1009) a         (1010)      208 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_monday.py
+-rw-rw-r--   0 a         (1009) a         (1010)      462 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_weekday.py
+-rw-rw-r--   0 a         (1009) a         (1010)      467 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/is_weekend.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/date/public_holiday/
+-rw-rw-r--   0 a         (1009) a         (1010)     5617 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/public_holiday/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      385 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/select_from_last_n_days.py
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/to_dd_mm_yyyy_str.py
+-rw-rw-r--   0 a         (1009) a         (1010)      605 2023-04-19 03:01:25.000000 hak-0.0.9/hak/date/to_utc_timestamp.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/date/year/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/date/year/easter_sunday/
+-rw-rw-r--   0 a         (1009) a         (1010)     1006 2023-04-19 01:55:38.000000 hak-0.0.9/hak/date/year/easter_sunday/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/datetime/
+-rw-rw-r--   0 a         (1009) a         (1010)      149 2023-04-19 01:55:38.000000 hak-0.0.9/hak/datetime/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      272 2023-04-19 01:55:38.000000 hak-0.0.9/hak/datetime/select_from_last_n_days.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dict/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      215 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/convert_to_sql_insertable.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dict/frequencies/
+-rw-rw-r--   0 a         (1009) a         (1010)      356 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/frequencies/choose.py
+-rw-rw-r--   0 a         (1009) a         (1010)      376 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/frequencies/make_from_strings.py
+-rw-rw-r--   0 a         (1009) a         (1010)      187 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/get_or_default.py
+-rw-rw-r--   0 a         (1009) a         (1010)      190 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/make_from_key_value_lists.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dict/proposed_dismantlement/
+-rw-rw-r--   0 a         (1009) a         (1010)     1520 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/proposed_dismantlement/show.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dict/test_durations/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/test_durations/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/test_durations/to_tuple_list_sorted_by_duration.py
+-rw-rw-r--   0 a         (1009) a         (1010)     4011 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dict/to_max_line_width_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/dicts/
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/a_into_b.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1200 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/compare.py
+-rw-rw-r--   0 a         (1009) a         (1010)      195 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      663 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/merge_freq_dicts.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/reindex.py
+-rw-rw-r--   0 a         (1009) a         (1010)      203 2023-04-19 01:55:38.000000 hak-0.0.9/hak/dicts/sort_by_key.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/directories/
+-rw-rw-r--   0 a         (1009) a         (1010)      567 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directories/exist.py
+-rw-rw-r--   0 a         (1009) a         (1010)      432 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directories/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/directory/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1548 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/compress_to_tar.py
+-rw-rw-r--   0 a         (1009) a         (1010)      674 2023-04-19 05:28:56.000000 hak-0.0.9/hak/directory/empty.py
+-rw-rw-r--   0 a         (1009) a         (1010)       88 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1239 2023-04-19 10:43:13.000000 hak-0.0.9/hak/directory/get_most_recently_modified.py
+-rw-rw-r--   0 a         (1009) a         (1010)      650 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/is_module.py
+-rw-rw-r--   0 a         (1009) a         (1010)      667 2023-04-19 10:09:51.000000 hak-0.0.9/hak/directory/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      782 2023-04-19 01:55:38.000000 hak-0.0.9/hak/directory/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3692 2023-04-19 01:55:38.000000 hak-0.0.9/hak/duration.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2021 2023-04-19 01:55:38.000000 hak-0.0.9/hak/duration_bar.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/fake/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/fake/os/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/os/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      418 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/os/system.py
+-rw-rw-r--   0 a         (1009) a         (1010)      424 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/printer.py
+-rw-rw-r--   0 a         (1009) a         (1010)       45 2023-04-19 01:55:38.000000 hak-0.0.9/hak/fake/sleep.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/fake/subprocess/
+-rw-rw-r--   0 a         (1009) a         (1010)     5854 2023-04-19 04:41:24.000000 hak-0.0.9/hak/fake/subprocess/run.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 10:16:12.000000 hak-0.0.9/hak/file/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      785 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/decrypt.py
+-rw-rw-r--   0 a         (1009) a         (1010)      929 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/encrypt.py
+-rw-rw-r--   0 a         (1009) a         (1010)      697 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/load.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/pickle/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/pickle/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1253 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/pickle/load_if_exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      906 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/pickle/save.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/py/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      546 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/create.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2644 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/dismantle.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3819 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/extract_fn.py
+-rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/py/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)      956 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/save.py
+-rw-rw-r--   0 a         (1009) a         (1010)      761 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/save_lines.py
+-rw-rw-r--   0 a         (1009) a         (1010)      308 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/save_lines_or_string.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/file/secret/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/secret/password/
+-rw-rw-r--   0 a         (1009) a         (1010)      680 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/secret/password/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/secret/username/
+-rw-rw-r--   0 a         (1009) a         (1010)      713 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/secret/username/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/tar/
+-rw-rw-r--   0 a         (1009) a         (1010)     1562 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/tar/extract.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/file/zip/
+-rw-rw-r--   0 a         (1009) a         (1010)      487 2023-04-19 01:55:38.000000 hak-0.0.9/hak/file/zip/extract.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/files/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/files/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)     1765 2023-04-19 04:43:12.000000 hak-0.0.9/hak/files/pyfiles/dismantle.py
+-rw-rw-r--   0 a         (1009) a         (1010)      100 2023-04-19 01:55:38.000000 hak-0.0.9/hak/find_first_parenthesis.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/float/
+-rw-rw-r--   0 a         (1009) a         (1010)       70 2023-04-19 01:55:38.000000 hak-0.0.9/hak/float/epsilon.py
+-rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.9/hak/float/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      106 2023-04-19 01:55:38.000000 hak-0.0.9/hak/float/is_not.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/float/nan/
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.9/hak/float/nan/to_none.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/function/
+-rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.9/hak/function/function.py
+-rw-rw-r--   0 a         (1009) a         (1010)      423 2023-04-19 01:55:38.000000 hak-0.0.9/hak/function/write_to_file.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/days/
+-rw-rw-r--   0 a         (1009) a         (1010)      227 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/days/a_to_b_inclusive.py
+-rw-rw-r--   0 a         (1009) a         (1010)      661 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/get_prime_factorisation.py
+-rw-rw-r--   0 a         (1009) a         (1010)      104 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      426 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/is_prime.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/year/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/year/days/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/year/days/count/
+-rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/year/days/count/get.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/int/year/days/first/
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/year/days/first/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      420 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/year/days/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      153 2023-04-19 01:55:38.000000 hak-0.0.9/hak/int/year/now.py
+-rw-rw-r--   0 a         (1009) a         (1010)      448 2023-04-19 01:55:38.000000 hak-0.0.9/hak/l.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      116 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/strings/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/strings/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 04:41:08.000000 hak-0.0.9/hak/list/strings/add_src_funks_prefix.py
+-rw-rw-r--   0 a         (1009) a         (1010)      586 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/strings/compare.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/strings/contain/
+-rw-rw-r--   0 a         (1009) a         (1010)      145 2023-04-19 04:43:23.000000 hak-0.0.9/hak/list/strings/contain/version.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/strings/filepaths/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/strings/filepaths/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1228 2023-04-19 04:38:09.000000 hak-0.0.9/hak/list/strings/filepaths/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2222 2023-04-19 04:44:27.000000 hak-0.0.9/hak/list/strings/find_first_diff.py
+-rw-rw-r--   0 a         (1009) a         (1010)      434 2023-04-19 04:45:12.000000 hak-0.0.9/hak/list/strings/make_patch_version_change_to_py.py
+-rw-rw-r--   0 a         (1009) a         (1010)      293 2023-04-19 04:47:46.000000 hak-0.0.9/hak/list/strings/module_names_from_py_filenames.py
+-rw-rw-r--   0 a         (1009) a         (1010)      410 2023-04-19 04:48:58.000000 hak-0.0.9/hak/list/strings/patch_setup_cfg.py
+-rw-rw-r--   0 a         (1009) a         (1010)      622 2023-04-19 04:51:45.000000 hak-0.0.9/hak/list/strings/patch_setup_py.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/list/strings/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)     1514 2023-04-19 04:52:08.000000 hak-0.0.9/hak/list/strings/pyfiles/filter_out_items.py
+-rw-rw-r--   0 a         (1009) a         (1010)      766 2023-04-19 05:00:37.000000 hak-0.0.9/hak/list/strings/show_diff.py
+-rw-rw-r--   0 a         (1009) a         (1010)      647 2023-04-19 05:00:56.000000 hak-0.0.9/hak/list/strings/to_dict.py
+-rw-rw-r--   0 a         (1009) a         (1010)      357 2023-04-19 05:01:35.000000 hak-0.0.9/hak/list/strings/two_char_combinations.py
+-rw-rw-r--   0 a         (1009) a         (1010)      115 2023-04-19 01:55:38.000000 hak-0.0.9/hak/list/to_comma_separated_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/lists/
+-rw-rw-r--   0 a         (1009) a         (1010)      216 2023-04-19 01:55:38.000000 hak-0.0.9/hak/lists/merge.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1131 2023-04-19 01:55:38.000000 hak-0.0.9/hak/load_durations_if_exists.py
+-rw-rw-r--   0 a         (1009) a         (1010)      123 2023-04-19 01:55:38.000000 hak-0.0.9/hak/log_2.py
+-rw-rw-r--   0 a         (1009) a         (1010)       84 2023-04-19 01:55:38.000000 hak-0.0.9/hak/nop.py
+-rw-rw-r--   0 a         (1009) a         (1010)       91 2023-04-19 01:55:38.000000 hak-0.0.9/hak/nop_state_x.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/patch/
+-rw-rw-r--   0 a         (1009) a         (1010)     7860 2023-04-19 09:15:38.000000 hak-0.0.9/hak/patch/do.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/period/
+-rw-rw-r--   0 a         (1009) a         (1010)      333 2023-04-19 01:55:38.000000 hak-0.0.9/hak/period/contains_day.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pip/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pip/dist_tar/
+-rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 07:21:09.000000 hak-0.0.9/hak/pip/dist_tar/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      804 2023-04-19 07:34:45.000000 hak-0.0.9/hak/pip/dist_tar/remove.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pip/setup/
+-rw-rw-r--   0 a         (1009) a         (1010)     1305 2023-04-19 04:43:59.000000 hak-0.0.9/hak/pip/setup/update.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1792 2023-04-19 08:32:41.000000 hak-0.0.9/hak/pip/upload.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pip/version/
+-rw-rw-r--   0 a         (1009) a         (1010)      837 2023-04-19 01:55:38.000000 hak-0.0.9/hak/pip/version/get.py
+-rw-rw-r--   0 a         (1009) a         (1010)      120 2023-04-19 01:55:38.000000 hak-0.0.9/hak/pip/version/to_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/pyfiles/
+-rw-rw-r--   0 a         (1009) a         (1010)      157 2023-04-19 01:55:38.000000 hak-0.0.9/hak/pyfiles/format.py
+-rw-rw-r--   0 a         (1009) a         (1010)      838 2023-04-19 04:33:37.000000 hak-0.0.9/hak/pyfiles/format_and_commit.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.710405 hak-0.0.9/hak/report/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/report/fail/
+-rw-rw-r--   0 a         (1009) a         (1010)      814 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/fail/no_xyz.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1914 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/fail/xyz.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1440 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/fail/z_return_neq_y_return.py
+-rw-rw-r--   0 a         (1009) a         (1010)     1601 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/fail/z_stdo_neq_y_stdo.py
+-rw-rw-r--   0 a         (1009) a         (1010)      887 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/property_failure.py
+-rw-rw-r--   0 a         (1009) a         (1010)      729 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/success.py
+-rw-rw-r--   0 a         (1009) a         (1010)      394 2023-04-19 01:55:38.000000 hak-0.0.9/hak/report/summarise_file.py
+-rw-rw-r--   0 a         (1009) a         (1010)      758 2023-04-19 01:55:38.000000 hak-0.0.9/hak/save_durations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/schedule/
+-rw-rw-r--   0 a         (1009) a         (1010)     3465 2023-04-19 01:55:38.000000 hak-0.0.9/hak/schedule/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      559 2023-04-19 01:55:38.000000 hak-0.0.9/hak/select_text_colour_from_width.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/session/
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.9/hak/session/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/set/
+-rw-rw-r--   0 a         (1009) a         (1010)      114 2023-04-19 01:55:38.000000 hak-0.0.9/hak/set/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/setup/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/setup/cfg/
+-rw-rw-r--   0 a         (1009) a         (1010)     1531 2023-04-19 07:22:45.000000 hak-0.0.9/hak/setup/cfg/update.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/setup/py/
+-rw-rw-r--   0 a         (1009) a         (1010)     1633 2023-04-19 07:24:59.000000 hak-0.0.9/hak/setup/py/update.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/alphanumeric/
+-rw-rw-r--   0 a         (1009) a         (1010)      264 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/alphanumeric/fake.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/append/
+-rw-rw-r--   0 a         (1009) a         (1010)       54 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/append/new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      541 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/camel_to_snake.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/char/
+-rw-rw-r--   0 a         (1009) a         (1010)      322 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/char/find_all_indices.py
+-rw-rw-r--   0 a         (1009) a         (1010)      128 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/char/is_digit.py
+-rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/char/is_upper.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/chars/
+-rw-rw-r--   0 a         (1009) a         (1010)      561 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/chars/remove.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/colour/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/colour/bright/
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/blue.py
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/cyan.py
+-rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/green.py
+-rw-rw-r--   0 a         (1009) a         (1010)      168 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/magenta.py
+-rw-rw-r--   0 a         (1009) a         (1010)      160 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/red.py
+-rw-rw-r--   0 a         (1009) a         (1010)      164 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/white.py
+-rw-rw-r--   0 a         (1009) a         (1010)      166 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/bright/yellow.py
+-rw-rw-r--   0 a         (1009) a         (1010)      130 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/danger.py
+-rw-rw-r--   0 a         (1009) a         (1010)      174 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/danger_if_zero.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/colour/dark/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/blue.py
+-rw-rw-r--   0 a         (1009) a         (1010)      148 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/cyan.py
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/default.py
+-rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/green.py
+-rw-rw-r--   0 a         (1009) a         (1010)      154 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/magenta.py
+-rw-rw-r--   0 a         (1009) a         (1010)      146 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/red.py
+-rw-rw-r--   0 a         (1009) a         (1010)      150 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/white.py
+-rw-rw-r--   0 a         (1009) a         (1010)      152 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/dark/yellow.py
+-rw-rw-r--   0 a         (1009) a         (1010)       64 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/data.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/info.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/primary.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2261 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/rainbow.py
+-rw-rw-r--   0 a         (1009) a         (1010)      134 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/secondary.py
+-rw-rw-r--   0 a         (1009) a         (1010)      267 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/tgfr.py
+-rw-rw-r--   0 a         (1009) a         (1010)      135 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/colour/warning.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/contains/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/contains/function/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/function/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      341 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/function/run.py
+-rw-rw-r--   0 a         (1009) a         (1010)      192 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/function/test.py
+-rw-rw-r--   0 a         (1009) a         (1010)      224 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/l.py
+-rw-rw-r--   0 a         (1009) a         (1010)       76 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/contains/version.py
+-rw-rw-r--   0 a         (1009) a         (1010)      105 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/count_x_in_y.py
+-rw-rw-r--   0 a         (1009) a         (1010)      996 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/delete_character_safely.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/digits/
+-rw-rw-r--   0 a         (1009) a         (1010)      202 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/digits/remove.py
+-rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/double_single_quotes.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/family_name/
+-rw-rw-r--   0 a         (1009) a         (1010)   115522 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/family_name/fake.py
+-rw-rw-r--   0 a         (1009) a         (1010)      303 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/family_name/is_a.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/filename/
+-rw-rw-r--   0 a         (1009) a         (1010)      126 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/filename/to_module_name.py
+-rw-rw-r--   0 a         (1009) a         (1010)      209 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/find_last_comma_index.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/fn_name/
+-rw-rw-r--   0 a         (1009) a         (1010)      226 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/fn_name/is_ignorable.py
+-rw-rw-r--   0 a         (1009) a         (1010)     5035 2023-04-19 05:00:49.000000 hak-0.0.9/hak/string/format.py
+-rw-rw-r--   0 a         (1009) a         (1010)       73 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_at_symbol.py
+-rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_digit.py
+-rw-rw-r--   0 a         (1009) a         (1010)      131 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_lowercase.py
+-rw-rw-r--   0 a         (1009) a         (1010)      259 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_other_char.py
+-rw-rw-r--   0 a         (1009) a         (1010)      172 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_seven_digits.py
+-rw-rw-r--   0 a         (1009) a         (1010)      132 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/has_uppercase.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/hbar/
+-rw-rw-r--   0 a         (1009) a         (1010)      122 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/hbar/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/string/header/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/header/python_file/
+-rw-rw-r--   0 a         (1009) a         (1010)      314 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/header/python_file/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/header/test_table/
+-rw-rw-r--   0 a         (1009) a         (1010)      461 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/header/test_table/make.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/indent/
+-rw-rw-r--   0 a         (1009) a         (1010)      137 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/indent/run_if_class_method.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/insert/
+-rw-rw-r--   0 a         (1009) a         (1010)      602 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_after_last_import_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      278 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_comment.py
+-rw-rw-r--   0 a         (1009) a         (1010)      584 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_def.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_if_main.py
+-rw-rw-r--   0 a         (1009) a         (1010)      666 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_lambda.py
+-rw-rw-r--   0 a         (1009) a         (1010)      292 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/insert/new_line_before_new_line_and_cea_.py
+-rw-rw-r--   0 a         (1009) a         (1010)      102 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      124 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/is_or_none.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/json/
+-rw-rw-r--   0 a         (1009) a         (1010)      179 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/json/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      548 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/lambdarise.py
+-rw-rw-r--   0 a         (1009) a         (1010)      360 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/make_content_without_function.py
+-rw-rw-r--   0 a         (1009) a         (1010)      325 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/make_function_text.py
+-rw-rw-r--   0 a         (1009) a         (1010)      338 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/make_initial_content.py
+-rw-rw-r--   0 a         (1009) a         (1010)      319 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/make_new_function_text.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/password/
+-rw-rw-r--   0 a         (1009) a         (1010)     1179 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/password/create.py
+-rw-rw-r--   0 a         (1009) a         (1010)      534 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/password/has_chars_from_3_sets.py
+-rw-rw-r--   0 a         (1009) a         (1010)      207 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/pop_left.py
+-rw-rw-r--   0 a         (1009) a         (1010)      219 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/pop_right.py
+-rw-rw-r--   0 a         (1009) a         (1010)      151 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/prepend_import.py
+-rw-rw-r--   0 a         (1009) a         (1010)      756 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/print_and_return_false.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/refactor/
+-rw-rw-r--   0 a         (1009) a         (1010)     1218 2023-04-19 05:01:09.000000 hak-0.0.9/hak/string/refactor/by_two_char_combinations.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.714405 hak-0.0.9/hak/string/remove/
+-rw-rw-r--   0 a         (1009) a         (1010)      211 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/empty_line_spaces.py
+-rw-rw-r--   0 a         (1009) a         (1010)      162 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/empty_lines.py
+-rw-rw-r--   0 a         (1009) a         (1010)      441 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/extra_new_line_following_class_definition.py
+-rw-rw-r--   0 a         (1009) a         (1010)      210 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/first_new_line_if_starts_with_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)       81 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/remove/whitespace_between_newlines.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/replace/
+-rw-rw-r--   0 a         (1009) a         (1010)      241 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/replace/double_new_line_with_single_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      129 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/replace/single_new_line_with_empty_string.py
+-rw-rw-r--   0 a         (1009) a         (1010)      251 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/replace/triple_new_line_with_double_new_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)      483 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/replace_unprintable.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3361 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/separate_function_from_context.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/single_line_function/
+-rw-rw-r--   0 a         (1009) a         (1010)      428 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/single_line_function/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      463 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/single_line_function/to_lambda_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/spaces/
+-rw-rw-r--   0 a         (1009) a         (1010)      111 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/spaces/count.py
+-rw-rw-r--   0 a         (1009) a         (1010)      320 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/split_fn_name_and_text.py
+-rw-rw-r--   0 a         (1009) a         (1010)      344 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/strip_unprintable.py
+-rw-rw-r--   0 a         (1009) a         (1010)      265 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/to_cond_freq_dict.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/token/
+-rw-rw-r--   0 a         (1009) a         (1010)     1263 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/token/substitute.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/string/yyyymmdd/
+-rw-rw-r--   0 a         (1009) a         (1010)      238 2023-04-19 01:55:38.000000 hak-0.0.9/hak/string/yyyymmdd/to_date.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak/subprocess/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/subprocess/completed_process/
+-rw-rw-r--   0 a         (1009) a         (1010)      655 2023-04-19 01:55:38.000000 hak-0.0.9/hak/subprocess/completed_process/to_str.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/__init__.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/git/
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/git/commit/
+-rw-rw-r--   0 a         (1009) a         (1010)     2515 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/commit/run.py
+-rw-rw-r--   0 a         (1009) a         (1010)      384 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/commit_if_test_and_app_ok.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/git/gitignore/
+-rw-rw-r--   0 a         (1009) a         (1010)      631 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/gitignore/make.py
+-rw-rw-r--   0 a         (1009) a         (1010)      486 2023-04-19 03:03:56.000000 hak-0.0.9/hak/system/git/init.py
+-rw-rw-r--   0 a         (1009) a         (1010)      725 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/log_oneline.py
+-rw-rw-r--   0 a         (1009) a         (1010)      866 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/git/push_after_delay.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/system/screen/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/screen/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)      786 2023-04-19 01:55:38.000000 hak-0.0.9/hak/system/screen/clear.py
+-rw-rw-r--   0 a         (1009) a         (1010)     3119 2023-04-19 01:55:38.000000 hak-0.0.9/hak/terminal.py
+-rw-rw-r--   0 a         (1009) a         (1010)      337 2023-04-19 01:55:38.000000 hak-0.0.9/hak/ternary.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/test/
+-rw-rw-r--   0 a         (1009) a         (1010)        0 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/__init__.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2578 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/check_final_line.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2689 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/check_line_lengths.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2843 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/do.py
+-rw-rw-r--   0 a         (1009) a         (1010)     2450 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/final_line_check.py
+-rw-rw-r--   0 a         (1009) a         (1010)      774 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/line_lengths_check.py
+-rw-rw-r--   0 a         (1009) a         (1010)      926 2023-04-19 01:55:38.000000 hak-0.0.9/hak/test/oldest_file_print.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.718405 hak-0.0.9/hak/tup/
+-rw-rw-r--   0 a         (1009) a         (1010)      176 2023-04-19 01:55:38.000000 hak-0.0.9/hak/tup/is_a.py
+-rw-rw-r--   0 a         (1009) a         (1010)      617 2023-04-19 01:55:38.000000 hak-0.0.9/hak/update_duration.py
+drwxrwxr-x   0 a         (1009) a         (1010)        0 2023-04-19 10:43:20.706405 hak-0.0.9/hak.egg-info/
+-rw-rw-r--   0 a         (1009) a         (1010)      994 2023-04-19 10:43:20.000000 hak-0.0.9/hak.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1009) a         (1010)     7947 2023-04-19 10:43:20.000000 hak-0.0.9/hak.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1009) a         (1010)        1 2023-04-19 10:43:20.000000 hak-0.0.9/hak.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1009) a         (1010)     1633 2023-04-19 10:43:20.000000 hak-0.0.9/hak.egg-info/top_level.txt
+-rw-rw-r--   0 a         (1009) a         (1010)      536 2023-04-19 10:43:20.718405 hak-0.0.9/setup.cfg
+-rw-rw-r--   0 a         (1009) a         (1010)     2781 2023-04-19 10:43:20.000000 hak-0.0.9/setup.py
```

### Comparing `hak-0.0.88/LICENSE` & `hak-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/fake/subprocess/run.py` & `hak-0.0.9/hak/fake/subprocess/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ignore_overlength_lines
 from subprocess import CompletedProcess
-from hak.one.file.load import f as load
+from hak.file.load import f as load
 
 _username = load('username.secret').split('\n')[0]
 _password = load('password.secret').split('\n')[0]
 
 def f(args, cwd, capture_output):
   if args == ['pwd']:
     return CompletedProcess(
```

### Comparing `hak-0.0.88/hak/many/dicts/compare.py` & `hak-0.0.9/hak/dicts/compare.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.print_and_return_false import f as pf
 
 def f(u, v):
   u_only = {}
   v_only = {}
-  in_u_and_v_same_vals = {}
-  in_u_and_v_diff_vals = {'u': {}, 'v': {}}
+  in_u_and_v_same_values = {}
+  in_u_and_v_different_values = {'u': {}, 'v': {}}
 
   for k in u:
     if k in v:
       if u[k] == v[k]:
-        in_u_and_v_same_vals[k] = u[k]
+        in_u_and_v_same_values[k] = u[k]
       else:
-        in_u_and_v_diff_vals['u'][k] = u[k]
-        in_u_and_v_diff_vals['v'][k] = v[k]
+        in_u_and_v_different_values['u'][k] = u[k]
+        in_u_and_v_different_values['v'][k] = v[k]
     else:
       u_only[k] = u[k]
 
   for k in v:
     if k not in u_only:
-      if k not in in_u_and_v_same_vals:
+      if k not in in_u_and_v_same_values:
         v_only[k] = v[k]
 
   return {
     'u_only': u_only,
     'v_only': v_only,
-    'in_u_and_v_same_vals': in_u_and_v_same_vals,
-    'in_u_and_v_diff_vals': in_u_and_v_diff_vals
+    'in_u_and_v_same_values': in_u_and_v_same_values,
+    'in_u_and_v_different_values': in_u_and_v_different_values
   }
 
 def t():
   u = {'a': 0, 'b': 1, 'c': 2, 'd': 2}
   v = {                'c': 2, 'd': 3, 'e': 4, 'f': 5}
   y = {
     'u_only': {'a': 0, 'b': 1},
     'v_only': {'d': 3, 'e': 4, 'f': 5},
-    'in_u_and_v_same_vals': {'c': 2},
-    'in_u_and_v_diff_vals': {'u': {'d': 2}, 'v': {'d': 3}}
+    'in_u_and_v_same_values': {'c': 2},
+    'in_u_and_v_different_values': {'u': {'d': 2}, 'v': {'d': 3}}
   }
   z = f(u, v)
   return y == z or pf([
+    'y != z',
     f"y['u_only']: {y['u_only']}",
     f"z['u_only']: {z['u_only']}",
     '',
     f"y['v_only']: {y['v_only']}",
     f"z['v_only']: {z['v_only']}",
   ])
```

### Comparing `hak-0.0.88/hak/many/dicts/merge_freq_dicts.py` & `hak-0.0.9/hak/dicts/merge_freq_dicts.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/many/directories/exist.py` & `hak-0.0.9/hak/directories/exist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdir
-from hak.one.directory.exists import f as directory_exists
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdir
+from hak.directory.exists import f as directory_exists
 
 f = lambda directories: all([directory_exists(d) for d in directories])
 
 root = './temp'
 directories = [f'{root}/{directory}' for directory in ['abc', 'ghi', 'jkl']]
 up = lambda: [mkdirine(d) for d in [root, *directories]]
 dn = lambda: rmdir(root)
```

### Comparing `hak-0.0.88/hak/many/files/pyfiles/dismantle.py` & `hak-0.0.9/hak/files/pyfiles/dismantle.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from hak.one.directory.make import f as mkdir
-from hak.one.file.save import f as save
-from hak.many.strings.filepaths.py.get import f as list_py_files
-from hak.many.strings.pyfiles.filter_out_items import f as ignore_protected
-from hak.one.file.py.dismantle import f as dismantle
-from hak.one.file.load import f as load
-from hak.one.directory.remove import f as rmdir
-from hak.one.directory.exists import f as exists
+from hak.directory.make import f as mkdir
+from hak.file.save import f as save
+from hak.list.strings.filepaths.py.get import f as list_py_files
+from hak.list.strings.pyfiles.filter_out_items import f as ignore_protected
+from hak.file.py.dismantle import f as dismantle
+from hak.file.load import f as load
+from hak.directory.remove import f as rmdir
+from hak.directory.exists import f as exists
 
 ignorable = [f'./hak/{_}.py' for _ in [
   'hak',
   'file/load',
   'terminal',
   'refactor_recommender'
 ]]
```

### Comparing `hak-0.0.88/hak/many/pyfiles/format_and_commit.py` & `hak-0.0.9/hak/pyfiles/format_and_commit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from hak.one.system.git.push_after_delay import f as push_commits_after_delay
-from hak.many.strings.filepaths.py.get import f as list_py_files
-from hak.many.strings.pyfiles.filter_out_items import f as filter_out_items
-from hak.many.pyfiles.format import f as auto_format_py_filenames
+from hak.system.git.push_after_delay import f as push_commits_after_delay
+from hak.list.strings.filepaths.py.get import f as list_py_files
+from hak.list.strings.pyfiles.filter_out_items import f as filter_out_items
+from hak.pyfiles.format import f as auto_format_py_filenames
 
 def f(_L_pi, fn_a=auto_format_py_filenames, fn_b=push_commits_after_delay):
   a = fn_a(_L_pi)
   b = fn_b(5)
   return a, b
 
 t = lambda: f(list('abc'), lambda x: x, lambda x: x)==(list('abc'), 5)
```

### Comparing `hak-0.0.88/hak/many/strings/compare.py` & `hak-0.0.9/hak/list/strings/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/many/strings/filepaths/get_least_recently_modified.py` & `hak-0.0.9/hak/directory/get_most_recently_modified.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+from hak.directory.make import f as mkdirine
+from hak.file.save import f as save
+from hak.directory.remove import f as rmdir
+from hak.string.print_and_return_false import f as pf
 from os.path import getmtime
+from hak.list.strings.filepaths.get import f as get_filepaths
 from time import sleep
 
-from hak.one.directory.filepaths.get import f as get_filepaths
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdir
-from hak.one.file.save import f as save
-from hak.pxyz import f as pxyz
-
 def f(x):
-  oldest = {'filepath': '', 'time': float('inf')}
-  # for filepath in filepaths:
-  for filepath in x:
+  filepaths = get_filepaths(x, [])
+  latest = {'filepath': '', 'time': 0}
+  for filepath in filepaths:
     last_modified_time = getmtime(filepath)
-    if last_modified_time < oldest['time']:
-      oldest = {'filepath': filepath, 'time': last_modified_time}
-  return oldest['filepath']
+    if last_modified_time > latest['time']:
+      latest = {'filepath': filepath, 'time': last_modified_time}
+  return latest['filepath']
 
 def up():
   x = {}
   x['dir_name'] = './test_directory_get_most_recently_modified'
   
   # Create test directory
   mkdirine(x['dir_name'])
@@ -37,12 +36,11 @@
 
   return x
 
 dn = lambda x: rmdir(x['dir_name'])
 
 def t():
   x = up()
-  y = x['old_file_path']
-  filepaths = get_filepaths(x['dir_name'], [])
-  z = f(filepaths)
+  y = x['new_file_path']
+  z = f(x['dir_name'])
   dn(x)
-  return pxyz(x, y, z)
+  return y == z or pf([f'x: {x}', f'y: {y}', f'z: {z}'])
```

### Comparing `hak-0.0.88/hak/many/strings/filepaths/py/to_filepath_file_content_dict.py` & `hak-0.0.9/hak/list/strings/to_dict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from hak.one.file.load import f as load
-from hak.one.file.save import f as save
-from hak.one.directory.make import f as mkdir
-from hak.one.file.remove import f as remove
-from hak.one.directory.remove import f as remove_dir
+from hak.file.load import f as load
+from hak.file.save import f as save
+from hak.directory.make import f as mkdir
+from hak.file.remove import f as remove
+from hak.directory.remove import f as remove_dir
 
 f = lambda x: {φ: load(φ) for φ in x}
 
 _root = '../temp_pyfiles_to_dict'
 _Pi = [(f'{_root}/foo.py', 'foo'), (f'{_root}/bar.py', 'bar')]
 
 dn = lambda: [*[remove(_pi_f) for (_pi_f, _) in _Pi], remove_dir(_root)]
-
 up = lambda: [mkdir(_root), *[save(_pi_f, _pi_d) for _pi_f, _pi_d in _Pi]]
 
 def t():
   up()
+  x = [f'{_root}/foo.py', f'{_root}/bar.py']
   y = {f'{_root}/foo.py': 'foo', f'{_root}/bar.py': 'bar'}
-  z = f([f'{_root}/foo.py', f'{_root}/bar.py'])
+  z = f(x)
   dn()
   return y == z
```

### Comparing `hak-0.0.88/hak/many/strings/find_first_diff.py` & `hak-0.0.9/hak/list/strings/find_first_diff.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from hak.one.string.colour.bright.magenta import f as mg
-from hak.one.string.colour.bright.cyan import f as cy
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.colour.bright.magenta import f as mg
+from hak.string.colour.bright.cyan import f as cy
+from hak.string.print_and_return_false import f as pf
 
 _f = lambda u_i, v_i, i: {'u_i': u_i, 'v_i': v_i, 'i': i}
 
 def f(u, v):
   if u == v: return None
   if len(u) < len(v): return f(u, v[:len(u)]) or _f(None, v[len(u)], len(u))
   if len(u) > len(v): return f(u[:len(v)], v) or _f(u[len(v)], None, len(v))
```

### Comparing `hak-0.0.88/hak/many/strings/patch_setup_py.py` & `hak-0.0.9/hak/list/strings/patch_setup_py.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from hak.many.strings.contain.version import f as k
-from hak.other.pip.version.to_str import f as make_v_str
-from hak.one.string.print_and_return_false import f as pf
+from hak.list.strings.contain.version import f as k
+from hak.pip.version.to_str import f as make_v_str
+from hak.string.print_and_return_false import f as pf
 
 def _k(x): return 'hak/pip/version' not in x
 
 f = lambda v, _L: [
   (f"  version='{make_v_str(v)}'," if k(_l) and _k(_l) else _l) for _l in _L
 ]
```

### Comparing `hak-0.0.88/hak/many/strings/pyfiles/filter_out_items.py` & `hak-0.0.9/hak/list/strings/pyfiles/filter_out_items.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/many/strings/show_diff.py` & `hak-0.0.9/hak/list/strings/show_diff.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.one.string.colour.bright.cyan import f as cy
-from hak.one.string.colour.bright.magenta import f as mg
-from hak.one.string.colour.bright.yellow import f as yl
-from hak.many.strings.find_first_diff import f as find_first_diff
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.colour.bright.cyan import f as cy
+from hak.string.colour.bright.magenta import f as mg
+from hak.string.colour.bright.yellow import f as yl
+from hak.list.strings.find_first_diff import f as find_first_diff
+from hak.string.print_and_return_false import f as pf
 
 # show_diff
 
 def f(u, v, w=64):
   u = str(u)
   v = str(v)
   i = find_first_diff(u, v)['i']
```

### Comparing `hak-0.0.88/hak/one/check_if_ok_to_proceed.py` & `hak-0.0.9/hak/check_if_ok_to_proceed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from queue import Queue as Q
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.print_and_return_false import f as pf
 
 def t_proceed():
   try: f(FakeInput(['y'])); return True
   except RuntimeError: return pf('t_proceed failed')
 
 def t_do_not_proceed():
   try: f(FakeInput(['n'])); return pf('t_do_not_proceed failed')
```

### Comparing `hak-0.0.88/hak/one/date/to_utc_timestamp.py` & `hak-0.0.9/hak/date/to_utc_timestamp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date
 from datetime import datetime as dt
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.print_and_return_false import f as pf
 from time import timezone
 
 f = lambda x: dt(x.year, x.month, x.day).timestamp() - timezone
 
 def t_0():
   x = date(1970,1,1)
   y = 0
```

### Comparing `hak-0.0.88/hak/one/dict/durations/load.py` & `hak-0.0.9/hak/load_durations_if_exists.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.one.file.pickle.load_if_exists import f as load_if_exists
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdir_if_exists
+from hak.file.pickle.load_if_exists import f as load_if_exists
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdir_if_exists
 from pickle import dump
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.print_and_return_false import f as pf
 
 f = lambda filename='durations.pickle': load_if_exists(filename) or {}
 
 temp_dir_path = './_load_durations_if_exists'
 temp_file_path = f'{temp_dir_path}/durations.pickle'
 data = {'a': 0, 'b': 1, 'c': 2}
```

### Comparing `hak-0.0.88/hak/one/dict/durations/save.py` & `hak-0.0.9/hak/save_durations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-from hak.one.file.pickle.load_if_exists import f as load_if_exists
-from hak.one.file.pickle.save import f as save
-from hak.one.string.print_and_return_false import f as pf
-from os import remove
+from hak.file.pickle.save import f as save
 from os.path import exists
-from copy import deepcopy
+from hak.file.pickle.load_if_exists import f as load_if_exists
+from os import remove
+from hak.string.print_and_return_false import f as pf
 
 f = lambda durations: save(durations, 'durations.pickle')
 
 dir_path = '.'
 file_path = f'{dir_path}/durations.pickle'
-
+data = {'a': 0, 'b': 1, 'c': {'x': True, 'y': False}}
 
 def up():
   if exists(file_path):
     backup = load_if_exists(file_path)
     remove(file_path)
     return backup
 
 dn = lambda backup: f(backup) if backup else remove(file_path)
 
 def t():
   backup = up()
-  x = {'a': 0, 'b': 1, 'c': {'x': True, 'y': False}}
-  y = deepcopy(x)
-  f(x)
+  y = data
+  f(data)
   z = load_if_exists(file_path)
   dn(backup)
   return y == z or pf([
     'Case where pickle does not exist failed.',
     f'y: {y}',
     f'z: {z}',
   ])
```

### Comparing `hak-0.0.88/hak/one/dict/proposed_dismantlement/show.py` & `hak-0.0.9/hak/dict/proposed_dismantlement/show.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from hak.one.string.hbar.make import f as hbar
-from hak.one.string.header.python_file.make import f as make_py_filename_header
-from hak.one.string.make_initial_content import f as make_initial_content
-from hak.one.string.make_function_text import f as make_function_text
-from hak.one.string.make_new_function_text import f as make_new_function_text
-from hak.one.string.make_content_without_function import f as make_content_wo_fn
-from hak.one.terminal import Terminal
+from hak.string.hbar.make import f as hbar
+from hak.string.header.python_file.make import f as make_py_filename_header
+from hak.string.make_initial_content import f as make_initial_content
+from hak.string.make_function_text import f as make_function_text
+from hak.string.make_new_function_text import f as make_new_function_text
+from hak.string.make_content_without_function import f as make_content_wo_func
+from hak.terminal import Terminal
 
 def f(_pi, silent=False, term=Terminal()):
   if silent: term.mode = 'test'
   term.clear()
   return term.print('\n'.join([
     hbar(),
     make_py_filename_header(_pi['_pi_filename']),
     make_initial_content(_pi['_pi_filename'], _pi['initial_content']),
     make_function_text(_pi['_pi_filename'], _pi['initial_function_text']),
     make_new_function_text(_pi['_pi_filename'], _pi['new_function_text']),
-    make_content_wo_fn(_pi['_pi_filename'], _pi['initial_other_text'])
+    make_content_wo_func(_pi['_pi_filename'], _pi['initial_other_text'])
   ]))
 
 t = lambda: f({
   '_pi_filename': 'foo.py',
   'initial_content': 'abc',
   'initial_function_text': 'def ghi(): return 0',
   'new_function_text': 'def ghi(): return 1',
```

### Comparing `hak-0.0.88/hak/one/dict/to_max_line_width_str.py` & `hak-0.0.9/hak/dict/to_max_line_width_str.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ignore_overlength_lines
-from hak.one.string.print_and_return_false import f as pf
-from hak.one.string.colour.bright.cyan import f as cy
-from hak.one.string.colour.bright.blue import f as bl
-from hak.one.string.colour.bright.magenta import f as mg
-from hak.one.string.char.last.find import f as find_last
+from hak.string.print_and_return_false import f as pf
+from hak.string.colour.bright.cyan import f as cy
+from hak.string.colour.bright.blue import f as bl
+from hak.string.colour.bright.magenta import f as mg
+from hak.string.char.last.find import f as find_last
 
 def t_short():
   x = {'a': 0, 'b': 1, 'c': 2, 'd': 3, 'e': 4, 'f': 5, 'g': 6, 'h': 7, 'i': 8}
   y = "{'a': 0, 'b': 1, 'c': 2, 'd': 3, 'e': 4, 'f': 5, 'g': 6, 'h': 7, 'i': 8}"
   z = f(x)
   return y == z or pf(['y != z', f'x: {x}', f'y: {y}', f'z: {z}'])
```

### Comparing `hak-0.0.88/hak/one/directory/compress_to_tar.py` & `hak-0.0.9/hak/directory/compress_to_tar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdirie
-from hak.one.file.save import f as save
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdirie
+from hak.file.save import f as save
 from subprocess import run
-from hak.one.file.tar.extract import f as extract_tar
-from hak.one.file.load import f as load
+from hak.file.tar.extract import f as extract_tar
+from hak.file.load import f as load
 
 _dir_name = './_test_directory_compress_to_tar'
 _source = f'{_dir_name}/source'
 _source_file_a_path = f'{_source}/a.txt'
 _source_file_a_content = "_source_file_a_path"
 _source_file_b_path = f'{_source}/b.txt'
 _source_file_b_content = "_source_file_b_path"
```

### Comparing `hak-0.0.88/hak/one/directory/empty.py` & `hak-0.0.9/hak/directory/empty.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from hak.one.directory.make import f as mkdir
-from hak.one.file.save import f as save
+from hak.directory.make import f as mkdir
+from hak.file.save import f as save
 from string import ascii_lowercase as az
-from hak.one.directory.remove import f as rmdir
+from hak.directory.remove import f as rmdir
 from os import listdir
-from hak.one.file.remove import f as remove
-from hak.one.string.print_and_return_false import f as pf
+from hak.file.remove import f as remove
+from hak.string.print_and_return_false import f as pf
 from os.path import isfile
 
-up = lambda x: [mkdir(x), *[save(f'{x}/{_}.txt', _) for _ in az]]
-dn = lambda x: rmdir(x)
+r = './temp'
+up = lambda: [mkdir(r), *[save(f'{r}/{_}.txt', _) for _ in az]]
+dn = lambda: rmdir(r)
 
-f = lambda x: [remove(f'{x}/{n}') for n in listdir(x) if isfile(f'{x}/{n}')]
-# f = lambda x: [remove(f'{x}/{n}') for n in listdir(x)]
+f = lambda x: [
+  remove(f'{r}/{filename}')
+  for filename
+  in listdir(x)
+  if isfile(f'{r}/{filename}')
+]
 
 def t():
-  x = './temp'
-  up(x)
-  α = len(listdir(x))
-  f(x)
-  ω = len(listdir(x))
+  up()
+  α = len(listdir(r))
+  f(r)
+  ω = len(listdir(r))
   result = all([α>ω, ω==0])
-  dn(x)
+  dn()
   return result or pf([f'α: {α}', f'ω: {ω}'])
```

### Comparing `hak-0.0.88/hak/one/directory/filepaths/packages/get.py` & `hak-0.0.9/hak/directory/remove.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,29 @@
-from os.path import isdir
-from os.path import isfile
+from os import listdir
+from os import mkdir
 from os import remove
+from os import rmdir
+from os.path import exists
+from os.path import isdir
 
-from hak.one.directory.filepaths.get import f as get_filepaths
-from hak.one.string.print_and_return_false import f as pf
-from hak.one.directory.make import f as mkdir
-from hak.one.directory.remove import f as remove_dir
-from hak.one.file.save import f as save
-
-def f(x):
-  _packages = set([])
-  directories = [_ for _ in get_filepaths(x, []) if isdir(_)]
-  for directory in directories:
-    python_files_in_directory = [
-      _
-      for _
-      in get_filepaths(directory, [])
-      if isfile(_) and _.endswith('.py')
-    ]
-    if python_files_in_directory: _packages.add(directory)
-  return _packages
+from hak.nop import f as nop
+from hak.file.save import f as save
 
-temp_dir_0 = './_get_packages'
-temp_dir_1 = f'{temp_dir_0}/_'
+def f(directory, filepaths=[]):
+  if not exists(directory): return
+  for item in listdir(directory):
+    _pi = directory+'/'+item
+    f(_pi, filepaths) if isdir(_pi) else remove(_pi)
+  rmdir(directory)
+
+temp_dir = './temp_directory_remove'
 temp_files_and_content = [
-  (f'{temp_dir_0}/foo.py', 'foo'),
-  (f'{temp_dir_0}/xyz.txt', 'xyz'),
-  (f'{temp_dir_1}/abc.txt', 'abc'),
-  (f'{temp_dir_1}/bar.py', 'bar'),
+  (f'{temp_dir}/foo.py', 'f = lambda: None\nt = lambda: f() is None'),
+  (f'{temp_dir}/xyz.txt', 'xyz'),
 ]
 
 def up():
-  for temp_dir in [temp_dir_0, temp_dir_1]: mkdir(temp_dir)
-  for (filename, content) in temp_files_and_content: save(filename, content)
+  (mkdir if not exists(temp_dir) else nop)(temp_dir)
+  [save(filename, content) for (filename, content) in temp_files_and_content]
+
+def t(): up(); f(temp_dir); return 0 == exists(temp_dir)
 
-def dn():
-  for (filename, _) in temp_files_and_content: remove(filename)
-  remove_dir(temp_dir_1)
-  remove_dir(temp_dir_0)
-
-def t():
-  up()
-  y = set([f'{temp_dir_1}'])
-  z = set(f(temp_dir_0))
-  dn()
-  return y == z or pf([f'y: {y}', f'z: {z}'])
```

### Comparing `hak-0.0.88/hak/one/directory/is_module.py` & `hak-0.0.9/hak/directory/is_module.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os.path import exists
 from os.path import isdir
-from hak.one.directory.make import f as mkdirine
-from hak.one.file.save import f as save
-from hak.one.directory.remove import f as rmdirie
+from hak.directory.make import f as mkdirine
+from hak.file.save import f as save
+from hak.directory.remove import f as rmdirie
 
 _dir = './_directory_is_module'
 
 _dir_expected_true = f'{_dir}/_expected_true'
 _dir_expected_false = f'{_dir}/_expected_false'
 
 def up():
```

### Comparing `hak-0.0.88/hak/one/duration.py` & `hak-0.0.9/hak/duration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ignore_overlength_lines
 from time import time
-from hak.one.number.duration_ms.to_bar import f as _duration_bar
-from hak.one.dict.durations.load import f as load_durations_if_exists
-from hak.one.dict.durations.save import f as save_durations
-from hak.one.dict.durations.update_one import f as update_duration
-from hak.one.number.int.width.to_text_colour import f as select_colour_from_width
+from hak.load_durations_if_exists import f as load_durations_if_exists
+from hak.update_duration import f as update_duration
+from hak.select_text_colour_from_width import f as select_colour_from_width
+from hak.save_durations import f as save_durations
+from hak.duration_bar import f as _duration_bar
 
 def f(t_0, name, now=time):
   δt_ms = (now()-t_0)*1000
   durations = load_durations_if_exists()
   durations = update_duration(durations, name, δt_ms)
   save_durations(durations)
   dbar, w = _duration_bar(δt_ms)
```

### Comparing `hak-0.0.88/hak/one/file/decrypt.py` & `hak-0.0.9/hak/file/decrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from hak.one.file.load import f as load
-from hak.one.file.remove import f as remove
+from hak.file.load import f as load
+from hak.file.remove import f as remove
 from subprocess import run
 
 _in_filepath = "_test_file_decrypt.txt.enc"
 _out_filepath = "_test_file_decrypt.txt"
 
 def f(in_filepath, out_filepath, password): run(
   args=[
```

### Comparing `hak-0.0.88/hak/one/file/encrypt.py` & `hak-0.0.9/hak/file/encrypt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from hak.one.file.save import f as save
-from hak.one.file.load import f as load
-from hak.one.file.remove import f as remove
-from hak.one.file.decrypt import f as decrypt
+from hak.file.save import f as save
+from hak.file.load import f as load
+from hak.file.remove import f as remove
+from hak.file.decrypt import f as decrypt
 from subprocess import run
 
 _content = "Dyson Sphere\n"
 _in_filename = "./_test_file_encrypt_in.txt"
 _enc_filename = "./_test_file_encrypt_in.txt.enc"
 _out_filename = "./_test_file_encrypt_out.txt"
 _password = "goldilocks"
```

### Comparing `hak-0.0.88/hak/one/file/load.py` & `hak-0.0.9/hak/file/load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os.path import exists
 from os import mkdir
-from hak.one.file.save import f as save
+from hak.file.save import f as save
 from os import remove
-from hak.one.directory.remove import f as remove_dir
+from hak.directory.remove import f as remove_dir
 
 def f(filename):
   with open(filename, 'r', encoding='utf8') as φ:
     return φ.read()
 
 temp_dir_0 = './_temp_file_load'
 temp_files_and_content = [(f'{temp_dir_0}/foo.py', 'foo')]
```

### Comparing `hak-0.0.88/hak/one/file/pickle/load_if_exists.py` & `hak-0.0.9/hak/file/pickle/load_if_exists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os.path import exists
 from pickle import load
 from pickle import dump
 
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdir_if_exists
-from hak.one.string.print_and_return_false import f as pf
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdir_if_exists
+from hak.string.print_and_return_false import f as pf
 
 def f(pickle_filename):
   if exists(pickle_filename):
     with open(pickle_filename, 'rb') as _file:
       return load(_file)
 
 temp_dir_path = './temp_pickle_load_if_exists'
```

### Comparing `hak-0.0.88/hak/one/file/pickle/save.py` & `hak-0.0.9/hak/file/pickle/save.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import mkdir
 from os.path import exists
 from pickle import dump
 
-from hak.one.directory.remove import f as rmdir_if_exists
-from hak.one.file.pickle.load_if_exists import f as load_if_exists
-from hak.one.file.remove import f as remove
-from hak.one.string.print_and_return_false import f as pf
+from hak.directory.remove import f as rmdir_if_exists
+from hak.file.pickle.load_if_exists import f as load_if_exists
+from hak.file.remove import f as remove
+from hak.string.print_and_return_false import f as pf
 
 def f(data, path):
   if '/' in path:
     dir_name = '/'.join(path.split('/')[:-1])
     existed = exists(dir_name)
     if not existed: mkdir(dir_name)
   with open(path, 'wb') as _file: dump(data, _file)
```

### Comparing `hak-0.0.88/hak/one/file/py/create.py` & `hak-0.0.9/hak/file/py/create.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdir
-from hak.one.file.load import f as load
-from hak.one.file.remove import f as remove
-from hak.one.file.save import f as save
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdir
+from hak.file.load import f as load
+from hak.file.remove import f as remove
+from hak.file.save import f as save
 
 f = lambda filename, data: save(filename, data)
 _dirname = './temp'
 _filename = f'{_dirname}/foo.py'
 _data = '\n'.join(["f = lambda: None", "t = lambda: False", ""])
 up = lambda: mkdirine(_dirname)
 dn = lambda: [remove(_filename), rmdir(_dirname)]
```

### Comparing `hak-0.0.88/hak/one/file/py/dismantle.py` & `hak-0.0.9/hak/file/py/dismantle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from hak.one.file.load import f as load
-from hak.one.string.separate_function_from_context import f as separate
-from hak.one.directory.make import f as mkdir
-from hak.one.directory.remove import f as rmdir
-from hak.one.string.split_fn_name_and_text import f as split_fn_name_and_text
-from hak.one.file.save import f as save
-from hak.one.string.fn_name.is_ignorable import f as function_is_ignorable
-from hak.one.string.prepend_import import f as prepend_import
-from hak.one.dict.proposed_dismantlement.show import f as show_proposed
-from hak.one.check_if_ok_to_proceed import f as check_if_ok_to_proceed
-from hak.one.function.write_to_file import f as write_function_to_file
-from hak.one.function.function import Function
+from hak.file.load import f as load
+from hak.string.separate_function_from_context import f as part_f_from_content
+from hak.directory.make import f as mkdir
+from hak.directory.remove import f as rmdir
+from hak.string.split_fn_name_and_text import f as split_function_name_and_text
+from hak.file.save import f as save
+from hak.string.fn_name.is_ignorable import f as function_is_ignorable
+from hak.string.prepend_import import f as prepend_import
+from hak.dict.proposed_dismantlement.show import f as show_proposed
+from hak.check_if_ok_to_proceed import f as check_if_ok_to_proceed
+from hak.function.write_to_file import f as write_function_to_file
+from hak.function.function import Function
 
 def f(_pi_filename, root='.', silent=True):
   initial_content = load(_pi_filename)
-  (initial_function_text, initial_other_text) = separate(initial_content)
+
+  (
+    initial_function_text,
+    initial_other_text
+  ) = part_f_from_content(initial_content)
 
   if not initial_function_text: return
 
-  f_name, f_body = split_fn_name_and_text(initial_function_text)
+  f_name, f_body = split_function_name_and_text(initial_function_text)
 
   if function_is_ignorable(f_name): return f_name
 
   new_content = prepend_import(f_name, initial_other_text)
   new_function_text = 'def f'+f_body
 
   show_proposed(
```

### Comparing `hak-0.0.88/hak/one/file/py/extract_fn.py` & `hak-0.0.9/hak/file/py/extract_fn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ignore_overlength_lines
-from hak.one.string.remove.empty_lines import f as remove_empty_lines
-from hak.one.string.colour.tgfr import f as tgfr
+from hak.string.remove.empty_lines import f as remove_empty_lines
+from hak.string.colour.tgfr import f as tgfr
 
 def f(content):
   first_def = content.find('def ')
   first_colon_following_first_def = content.find(':', first_def)
   second_def = content.find('def ', first_colon_following_first_def)
   _if_name_main = content.find("if __name__ == '__main__':")
   if first_def < 0: return ('', content)
```

### Comparing `hak-0.0.88/hak/one/file/save.py` & `hak-0.0.9/hak/file/save.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os.path import exists
 from os import remove
 from os import mkdir
 from os import rmdir
 
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.print_and_return_false import f as pf
 
-# from hak.none.nop import f as nop
+# from hak.nop import f as nop
 nop = lambda x=None: None # DELETE LINE
 
 def f(filepath, content):
   with open(filepath, 'w') as φ:
     φ.write(content)
     return content
 
@@ -20,15 +20,15 @@
 
 def dn():
   if exists(_filepath): remove(_filepath)
   rmdir(_root)
 
 def t():
   up()
-
+  
   x_content = 'apple'
   result = f(_filepath, x_content)
 
   if not exists(_filepath):
     dn()
     return pf(f'{_filepath} file was not created by file.write.run()')
```

### Comparing `hak-0.0.88/hak/one/file/save_lines.py` & `hak-0.0.9/hak/file/save_lines.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from os.path import exists
 from os import remove
 from os import mkdir
-from hak.none.nop import f as nopx
+from hak.nop import f as nopx
 from os import rmdir
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.print_and_return_false import f as pf
 
 def f(filepath, lines):
   with open(filepath, 'w') as _file: _file.writelines(lines)
   return lines
 
 _filename = './_/temp.txt'
 up = lambda: (mkdir if not exists('_') else nopx)('_')
```

### Comparing `hak-0.0.88/hak/one/file/secret/password/get.py` & `hak-0.0.9/hak/file/secret/password/get.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdirie
-from hak.one.file.save import f as save
-from hak.one.string.password.has_chars_from_3_sets import f as has_ch_from_3
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdirie
+from hak.file.save import f as save
+from hak.string.password.has_chars_from_3_sets import f as has_ch_from_3
 
 filename = 'password.secret'
 
 def f(root='.'):
   with open(f'{root}/{filename}', 'r') as φ: return φ.readlines()[0]
 
 _root = '../temp_secret_password'
```

### Comparing `hak-0.0.88/hak/one/file/secret/username/get.py` & `hak-0.0.9/hak/file/secret/username/get.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdirie
-from hak.one.file.save import f as save
-from hak.one.string.has_seven_digits import f as has_7_digits
-from hak.one.string.has_at_symbol import f as has_at_symbol
-from hak.one.string.has_lowercase import f as has_lowercase
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdirie
+from hak.file.save import f as save
+from hak.string.has_seven_digits import f as has_7_digits
+from hak.string.has_at_symbol import f as has_at_symbol
+from hak.string.has_lowercase import f as has_lowercase
 
 filename = 'username.secret'
 
 def f(root='.'):
   with open(f'{root}/{filename}', 'r') as φ: return φ.readlines()[0]
 
 _root = '../temp_secret_username'
```

### Comparing `hak-0.0.88/hak/one/file/tar/extract.py` & `hak-0.0.9/hak/file/tar/extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from subprocess import run
-from hak.one.directory.make import f as mkdirine
-from hak.one.file.load import f as load
-from hak.one.directory.remove import f as rmdirie
+from hak.directory.make import f as mkdirine
+from hak.file.load import f as load
+from hak.directory.remove import f as rmdirie
 
 data = (
   b'\x1f\x8b\x08\x00\x00\x00\x00\x00\x00\x03\xed\xd3\xe1\n\x820\x18\x85a/'
   b'\xc5+\xd0\xcd\xa6^\xce\x87\xd9\xa2\xa20\xb6\x05u\xf7)\x11T\x14\x8a\x85'
   b'\x11\xbd\xcf\x9f\x0f\xb6\xc16\x0e\'I%X\x1fd\xb1v\xb6\x0e\x8d;I\xdd\xec'
   b'\xf6\xcez/\xa1\x91P\xb9\xd47\x07W\xdb4\x1aO\xb5\xca2\xef\xa6.su;\xaf"m2'
   b'\xad\n\x95\x19\xdd\xae\xeb\xc2\xccL\x14\xe7o\xdc9\xd8\xc1\xb7\x9f\x8c\xe3h'
```

### Comparing `hak-0.0.88/hak/one/number/int/width/to_text_colour.py` & `hak-0.0.9/hak/select_text_colour_from_width.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.one.string.colour.bright.magenta import f as magenta
-from hak.one.string.colour.bright.blue import f as blue
-from hak.one.string.colour.bright.red import f as red
-from hak.one.string.colour.bright.cyan import f as cy
-from hak.one.string.colour.bright.green import f as green
+from hak.string.colour.bright.magenta import f as magenta
+from hak.string.colour.bright.blue import f as blue
+from hak.string.colour.bright.red import f as red
+from hak.string.colour.bright.cyan import f as cy
+from hak.string.colour.bright.green import f as green
 
 f = lambda w: {0: green, 1: cy, 2: blue, 3: magenta, 4: red}[w//5]
 
 t = lambda: all([
   *[green == f(_) for _ in range(5)],
   *[cy == f(_) for _ in range(5, 10)],
   *[blue == f(_) for _ in range(10, 15)],
```

### Comparing `hak-0.0.88/hak/one/schedule/make.py` & `hak-0.0.9/hak/schedule/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/one/string/camel_to_snake.py` & `hak-0.0.9/hak/string/camel_to_snake.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from hak.one.string.char.is_digit import f as is_digit
-from hak.one.string.char.is_upper import f as is_upper
+from hak.string.char.is_digit import f as is_digit
+from hak.string.char.is_upper import f as is_upper
 
 # camel_to_snake
 
 f = lambda ζ: (
   ('_' if is_digit(ζ[0]) else '')+ ζ[0].lower() + ''.join([
     f'_{ζ[θ].lower()}' if all([
       any([is_upper(ζ[θ]), is_digit(ζ[θ]), is_digit(ζ[θ-1])]),
```

### Comparing `hak-0.0.88/hak/one/string/chars/remove.py` & `hak-0.0.9/hak/string/chars/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/one/string/colour/rainbow.py` & `hak-0.0.9/hak/string/colour/rainbow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from hak.one.string.colour.dark.red import f as d_red
-from hak.one.string.colour.dark.green import f as d_green
-from hak.one.string.colour.dark.yellow import f as d_yellow
-from hak.one.string.colour.dark.blue import f as d_blue
-from hak.one.string.colour.dark.magenta import f as d_magenta
-from hak.one.string.colour.dark.cyan import f as d_cyan
-from hak.one.string.colour.dark.white import f as d_white
-from hak.one.string.colour.dark.default import f as d_default
-from hak.one.string.colour.bright.red import f as b_red
-from hak.one.string.colour.bright.yellow import f as b_yellow
-from hak.one.string.colour.bright.green import f as b_green
-from hak.one.string.colour.bright.cyan import f as b_cyan
-from hak.one.string.colour.bright.blue import f as b_blue
-from hak.one.string.colour.bright.magenta import f as b_mag
-from hak.one.string.colour.bright.white import f as b_white
+from hak.string.colour.dark.red import f as d_red
+from hak.string.colour.dark.green import f as d_green
+from hak.string.colour.dark.yellow import f as d_yellow
+from hak.string.colour.dark.blue import f as d_blue
+from hak.string.colour.dark.magenta import f as d_magenta
+from hak.string.colour.dark.cyan import f as d_cyan
+from hak.string.colour.dark.white import f as d_white
+from hak.string.colour.dark.default import f as d_default
+from hak.string.colour.bright.red import f as b_red
+from hak.string.colour.bright.yellow import f as b_yellow
+from hak.string.colour.bright.green import f as b_green
+from hak.string.colour.bright.cyan import f as b_cyan
+from hak.string.colour.bright.blue import f as b_blue
+from hak.string.colour.bright.magenta import f as b_mag
+from hak.string.colour.bright.white import f as b_white
 
 def f(μ):
   return '\n'.join([
     f'{(name+":"):<15} {fn(μ)}'
     for (name, fn)
     in [
       ('dark_red', d_red),
```

### Comparing `hak-0.0.88/hak/one/string/delete_character_safely.py` & `hak-0.0.9/hak/string/delete_character_safely.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/one/string/family_name/fake.py` & `hak-0.0.9/hak/string/family_name/fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,2992 +1,2855 @@
 from random import choice
-from hak.one.dict.frequencies.choose import f as choose
-from hak.one.string.family_name.is_a import f as is_a_family_name
+from hak.dict.frequencies.choose import f as choose
+from hak.string.family_name.is_a import f as is_a_family_name
 
 q3 = {
-  'Aa': {
-    'r': 8, 's': 4, 'b': 2, 'm': 2, 'n': 3, 'k': 1, 'g': 1, 'l': 4, 'v': 1, 
-    'd': 1
-  },
-  'aa': {
-    's': 39, 'c': 21, 'v': 3, 'g': 12, 'r': 61, 'd': 12, 'b': 12, 't': 15,
-    'f': 6, 'l': 14, 'n': 15, 'm': 6, 'p': 6, 'k': 15, '!': 19, 'i': 4, 'h': 2,
-    'e': 2, 'w': 2, 'u': 2, 'z': 2, 'y': 1
-  },
-  'Ab': {
-    'b': 21, 'r': 35, 'e': 37, 'n': 3, 'l': 8, 'd': 27, 's': 7, 'a': 20,
-    'u': 11, 'i': 9, 'p': 1, 't': 2, 'o': 11, 'k': 2
-  },
-  'ab': {
-    'r': 82, 't': 1, 'e': 208, 'c': 1, 'b': 59, 'o': 118, 'a': 207, '!': 40,
-    'i': 133, 'l': 65, 'n': 4, 'y': 22, 's': 12, 'h': 8, 'u': 30, 'j': 3,
-    'd': 1, 'k': 3, 'z': 2
-  },
-  'ac': {
-    'k': 557, 'e': 152, 'o': 136, 'h': 602, 'd': 15, 'i': 130, 'r': 35, 'y': 23,
-    'a': 102, '!': 50, 'q': 25, 's': 12, 'l': 26, 'c': 148, 'p': 6, 'm': 9,
-    'g': 4, 'f': 2, 'n': 12, 'z': 37, 'u': 29, 't': 6, 'b': 3, 'w': 1, 'v': 4
-  },
-  'Ac': {
-    'o': 11, 'e': 18, 'k': 23, 'u': 2, 'r': 6, 't': 2, 'h': 17, 'y': 1, 'q': 2,
-    'c': 10, 'i': 2, 'a': 2, 'f': 1, 'l': 1
-  },
-  'Ad': {
-    'a': 34, 'k': 6, 'd': 17, 'c': 2, 'l': 7, 'o': 12, 'r': 8, 'e': 30, 'g': 1,
-    'm': 2, 'w': 1, 's': 2, 'n': 2, 'i': 6, 'u': 3, 'j': 2, 'h': 2, 'z': 1,
-    'y': 1
-  },
-  'ad': {
-    'l': 76, 'e': 287, 'o': 215, 'a': 190, 'i': 162, 'y': 71, 'f': 13, '!': 264,
-    's': 35, 'd': 135, 'n': 22, 'g': 18, 'r': 39, 'w': 28, 'b': 18, 'm': 16,
-    'c': 4, 't': 37, 'u': 37, 'k': 8, 'h': 16, 'z': 8, 'j': 2, 'v': 5
-  },
-  'ae': {
-    'l': 35, 'f': 18, '!': 21, 'z': 13, 'n': 25, 'r': 44, 'g': 24, 's': 38,
-    'm': 10, 'c': 11, 'd': 14, 't': 38, 'p': 1, 'h': 14, 'k': 6, 'y': 3, 'e': 1,
-    'b': 8, 'o': 1, 'u': 3, 'v': 1, 'w': 2, 'a': 2
+  'Sm': {
+    'i': 45, 'a': 29, 'o': 24, 'y': 12, 'e': 25, 't': 1, 'u': 13, 'r': 1, 's': 1
   },
-  'Ae': {'s': 3, 'g': 1, 'r': 3, 'l': 1, 'm': 1, 'i': 1},
-  'Af': {
-    'a': 4, 'r': 1, 'f': 8, 't': 1, 'o': 2, 'z': 1, 's': 2, 'l': 1, 'u': 1
+  'mi': {
+    't': 126, 'r': 66, 'l': 116, 'd': 45, 'n': 264, 'c': 67, 's': 82, 'e': 82,
+    'j': 3, '!': 86, 'g': 24, 'a': 37, 'z': 3, 'u': 2, 'o': 11, 'k': 4, 'm': 2,
+    'h': 2, 'y': 4, 'i': 1, 'x': 1
   },
-  'af': {
-    'f': 197, 't': 48, 'e': 57, 's': 2, '!': 31, 'l': 23, 'o': 50, 'i': 39,
-    'r': 23, 'u': 19, 'a': 56, 'n': 3, 'k': 4, 'z': 1, 'd': 1, 'm': 1
+  'it': {
+    'h': 166, 'e': 237, 'c': 120, 't': 505, 'z': 316, 'a': 151, 'n': 23, 'f': 5,
+    'l': 33, '!': 117, 'o': 141, 'm': 40, 'u': 21, 'i': 68, 's': 102, 'w': 8,
+    'r': 43, 'y': 31, 'k': 29, 'b': 8, 'g': 4, 'v': 4, 'j': 2, 'p': 1
   },
-  'ag': {
-    'n': 127, 'o': 126, 'e': 332, 'h': 52, 'a': 249, 'u': 86, 'g': 121,
-    'l': 148, 's': 12, 'w': 6, '!': 43, 'y': 14, 'b': 7, 'i': 68, 'r': 43,
-    'd': 11, 'm': 11, 't': 8, 'p': 3, 'j': 1
+  'th': {
+    '!': 634, 'e': 410, 'y': 34, 'i': 87, 'o': 107, 'r': 38, 'u': 34, 'a': 199,
+    's': 13, 'c': 22, 'w': 27, 'm': 29, 'b': 11, 'l': 21, 'j': 5, 'n': 7,
+    'k': 6, 'v': 4, 'f': 5, 'h': 4, 't': 2, 'g': 6
   },
-  'Ag': {
-    'u': 35, 'e': 11, 'n': 9, 'o': 11, 'a': 6, 'i': 4, 'r': 15, 't': 1, 'b': 2,
-    'l': 3, 'y': 1, 'g': 3, 'c': 1, 'p': 1
+  'Jo': {
+    'h': 42, 'n': 25, 'r': 21, 's': 27, 'y': 10, 'i': 4, 'l': 19, 'b': 7,
+    'e': 12, 'u': 11, 'p': 2, 'w': 3, '!': 1, 'z': 3, 'a': 8, 'c': 7, 'o': 4,
+    'v': 6, 'f': 2, 'j': 1, 'd': 5, 'm': 3, 'k': 3, 't': 2, 'g': 1
   },
-  'ah': {
-    'a': 163, 'n': 70, 'o': 57, 'u': 23, '!': 103, 'l': 139, 'i': 46, 'e': 59,
-    'y': 7, 'r': 51, 'm': 36, 't': 5, 's': 7, 'p': 1, 'd': 4, 'b': 2, 'h': 1,
-    'f': 1, 'k': 2
+  'oh': {
+    'n': 80, 'e': 36, 'r': 56, 'l': 88, 'a': 78, 'u': 6, 'd': 4, 'o': 31,
+    '!': 31, 'm': 34, 's': 15, 'y': 1, 't': 1, 'i': 7, 'w': 4, 'b': 2, 'v': 1
   },
-  'Ah': {
-    'm': 5, 'r': 10, 'e': 3, 'n': 4, 'o': 3, 'l': 21, 'u': 3, 'a': 7, 's': 2,
-    'y': 2, 'i': 2, 'h': 1
+  'hn': {
+    's': 22, '!': 126, 'e': 182, 'k': 16, 'i': 42, 'a': 34, 'd': 2, 'o': 23,
+    'u': 5, 'h': 4, 'l': 4, 'y': 2, 'g': 1, 'c': 2, 'n': 1, 'q': 1, 'z': 1,
+    'b': 2, 'p': 1, 't': 1
   },
-  'Ai': {
-    'k': 6, 'n': 9, 'e': 2, 't': 8, 'c': 2, 's': 1, 'g': 1, 'r': 5, 'l': 9,
-    'o': 2, 'm': 2, 'v': 1, 'u': 3, 'd': 2, 'y': 1, 'h': 1, 'p': 3, 'a': 1
+  'ns': {
+    'o': 242, '!': 747, 't': 246, 'e': 183, 'l': 57, 'h': 43, 'f': 14, 'w': 19,
+    'k': 451, 'i': 77, 'b': 48, 's': 8, 'a': 46, 'm': 33, 'c': 80, 'd': 11,
+    'p': 12, 'u': 11, 'r': 6, 'v': 4, 'g': 1, 'z': 2, 'y': 2, 'n': 2
   },
-  'ai': {
-    'l': 154, 'g': 55, 'r': 165, 'n': 364, 's': 127, 'd': 48, 't': 103, 'e': 28,
-    '!': 80, 'm': 36, 'z': 23, 'b': 18, 'f': 8, 'v': 9, 'o': 19, 'k': 15,
-    'c': 20, 'a': 26, 'w': 2, 'p': 2, 'h': 1, 'x': 3, 'u': 1, 'y': 1
+  'so': {
+    'n': 1337, '!': 212, 'm': 52, 'e': 8, 'r': 57, 'l': 55, 's': 15, 'u': 31,
+    'c': 13, 'p': 6, 'y': 2, 'x': 1, 't': 15, 'h': 5, 'w': 31, 'b': 2, 'f': 6,
+    'o': 6, 'i': 5, 'g': 3, 'a': 2, 'z': 1, 'v': 10
   },
-  'Aj': {'a': 4, 'e': 1, 'o': 2},
-  'aj': {
-    'o': 19, 'a': 46, 'e': 32, 'k': 8, 'i': 18, 'd': 10, '!': 33, 'c': 8,
-    'u': 7, 's': 1, 't': 2, 'l': 3, 'w': 2, 'z': 1, 'n': 3, 'j': 1, 'm': 1,
-    'g': 1, 'h': 1
+  'on': {
+    '!': 3423, 'e': 746, 'z': 53, 'g': 307, 's': 255, 'a': 293, 't': 354,
+    'n': 209, 'd': 278, 'l': 17, 'r': 26, 'y': 33, 'w': 9, 'o': 106, 'c': 91,
+    'i': 305, 'k': 65, 'h': 22, 'v': 13, 'm': 6, 'f': 21, 'u': 12, 'b': 17,
+    'q': 4, 'j': 5, 'p': 1
   },
-  'Ak': {
-    'e': 12, 'i': 11, 'r': 4, 'b': 2, 'a': 10, 'h': 3, 'p': 1, 'm': 1, 'k': 1,
-    'u': 2, 's': 2, 'o': 2, 'l': 2, 'w': 1
+  'Wi': {
+    'l': 259, 's': 70, 'g': 36, 'n': 189, 't': 86, 'c': 45, 'm': 19, 'r': 20,
+    'e': 93, 'd': 34, 'b': 7, 'k': 12, 'x': 5, 'a': 8, 'f': 1, 'p': 5, 'z': 3,
+    'o': 1, 'u': 1, 'i': 1
   },
-  'ak': {
-    'e': 280, '!': 481, 'l': 32, 'a': 113, 's': 24, 'i': 103, 'k': 16, 'n': 5,
-    'o': 84, 'u': 30, 'm': 3, 'r': 7, 't': 1, 'f': 1, 'h': 13, 'd': 3, 'j': 2,
-    'y': 8, 'b': 1
+  'il': {
+    'l': 1559, 's': 89, 'e': 259, 't': 81, 'b': 106, 'v': 54, 'a': 165, 'k': 74,
+    'c': 53, 'm': 51, '!': 188, 'd': 138, 'g': 33, 'h': 37, 'p': 13, 'n': 11,
+    'y': 26, 'o': 95, 'i': 176, 'w': 8, 'f': 25, 'r': 8, 'u': 21, 'j': 4,
+    'z': 9, 'q': 1
   },
-  'al': {
-    'k': 111, 'l': 1054, 'e': 518, 'd': 301, 'm': 109, 't': 177, '!': 447,
-    's': 137, 'a': 442, 'o': 184, 'h': 24, 'i': 311, 'v': 99, 'y': 44, 'f': 34,
-    'g': 22, 'b': 80, 'c': 103, 'u': 56, 'p': 39, 'z': 39, 'r': 10, 'n': 13,
-    'w': 16, 'q': 3, 'j': 2
+  'll': {
+    'i': 1117, 'e': 1235, '!': 1626, 'y': 110, 'a': 965, 's': 116, 'o': 707,
+    'm': 136, 'u': 68, 'w': 30, 'r': 13, 'g': 15, 'n': 30, 'h': 28, 'c': 11,
   },
-  'Al': {
-    'l': 118, 'e': 63, 'v': 42, 's': 24, 'f': 20, 'b': 67, 'd': 34, 'i': 31,
-    't': 61, 'o': 15, 'a': 38, 'm': 40, 'c': 25, 'g': 11, 'p': 13, 'k': 6,
-    'r': 4, 'w': 8, 'u': 8, 'z': 3, 'y': 2, 'q': 4, 'n': 3, 'j': 1, 'h': 4
+  'li': {
+    'a': 233, 'p': 94, 'n': 1348, 'v': 76, 's': 293, 'o': 178, 'e': 255,
+    'f': 77, 'x': 10, 'g': 91, 'd': 34, 'c': 303, '!': 459, 'u': 21, 'l': 33,
+    'z': 36, 'k': 74, 't': 113, 'm': 85, 'b': 36, 'h': 19, 'r': 9, 'w': 8,
+    'i': 11, 'q': 2, 'j': 2
   },
-  'Am': {
-    'o': 32, 'e': 40, 'b': 29, 'a': 39, 'm': 10, 'u': 4, 'i': 25, 'y': 5,
-    's': 15, 'r': 5, 'w': 1, 'p': 4, 'd': 2, 't': 1, 'l': 1
+  'ia': {
+    'm': 54, '!': 534, 'z': 12, 'g': 26, 'n': 550, 's': 102, 'r': 125, 't': 49,
+    'l': 59, 'u': 12, 'k': 100, 'd': 22, 'f': 10, 'c': 48, 'v': 13, 'o': 8,
+    'h': 13, 'q': 2, 'i': 4, 'b': 4, 'p': 11, 'w': 1, 'j': 1, 'e': 1
   },
   'am': {
     's': 91, 'p': 295, 'i': 188, 'e': 241, '!': 460, 'o': 203, 'b': 237,
     'm': 190, 'a': 338, 'u': 39, 'l': 29, 'y': 21, 'r': 20, 'n': 13, 'k': 8,
-    'd': 10, 'c': 9, 'f': 8, 'w': 4, 'h': 4, 't': 2, 'z': 5, 'v': 1, 'g': 2,
-    'j': 2
   },
-  'An': {
-    'd': 104, 't': 79, 'a': 25, 'g': 82, 'n': 30, 's': 23, 'c': 15, 'z': 8,
-    'k': 9, 'w': 2, '!': 1, 'e': 13, 'f': 1, 'h': 2, 'o': 5, 'i': 11, 'l': 1,
-    'y': 1, 'r': 1
+  'ms': {
+    '!': 114, 't': 47, 'o': 29, 'e': 34, 'a': 8, 'l': 8, 'b': 10, 'd': 7,
   },
-  'an': {
-    'd': 1436, 's': 436, 'c': 402, '!': 3435, 't': 732, 'i': 477, 'e': 531,
-    'k': 253, 'l': 60, 'n': 782, 'a': 411, 'g': 474, 'o': 701, 'f': 59, 'u': 64,
-    'h': 70, 'z': 162, 'b': 57, 'm': 18, 'w': 42, 'j': 17, 'p': 23, 'y': 65,
-    'r': 19, 'v': 39, 'q': 10
+  'ne': {
+    's': 427, 'z': 74, 'r': 1147, 't': 222, 'd': 49, '!': 1257, 'y': 405,
+    'i': 47, 'a': 119, 'l': 366, 'e': 45, 'h': 28, 'n': 184, 'w': 22, 'g': 49,
+    'f': 21, 'j': 8, 'b': 57, 'p': 12, 'm': 83, 'c': 87, 'k': 97, 'u': 9,
+    'v': 21, 'o': 14, 'x': 5, 'q': 2
   },
-  'ao': {
-    '!': 82, 'n': 7, 'l': 25, 'r': 3, 'u': 5, 'k': 8, 'i': 6, 'o': 2, 'm': 3,
-    'a': 5, 's': 2, 'h': 1, 'p': 1, 'b': 2
+  'es': {
+    '!': 1688, 't': 470, 's': 533, 'e': 296, 'p': 53, 'u': 16, 'l': 79,
+    'c': 167, 'b': 37, 'o': 128, 'q': 9, 'h': 108, 'm': 47, 'i': 123, 'a': 91,
+    'j': 4, 'r': 10, 'd': 8, 'n': 59, 'k': 117, 'w': 14, 'g': 8, 'f': 6,
+    'z': 19, 'v': 5, 'y': 8
   },
-  'Ao': {'k': 1, 'a': 1, 'n': 1, '!': 1},
-  'ap': {
-    'm': 3, 'p': 172, '!': 37, 'i': 77, 'e': 109, 'l': 50, 'a': 109, 'o': 60,
-    't': 11, 'u': 25, 'h': 22, 's': 25, 'r': 28, 'k': 12, 'd': 2, 'n': 4,
-    'c': 2, 'f': 5, 'w': 1, 'g': 1, 'v': 1
+  'Br': {
+    'o': 311, 'y': 28, 'a': 402, 'e': 253, 'i': 247, 'u': 188, 'z': 10, 'w': 1,
+    'l': 1, 'r': 1, 'd': 1
   },
-  'Ap': {
-    'o': 12, 'p': 35, 'a': 8, 'e': 6, 'g': 1, 'r': 6, 'i': 2, 'u': 2, 'l': 5,
-    'f': 1, 't': 2, 's': 2, 'k': 3, 'y': 1
+  'ro': {
+    'w': 247, 'o': 144, 'l': 113, 'n': 479, '!': 665, 's': 389, 'c': 186,
+    'a': 51, 'e': 102, 'y': 62, 'u': 188, 'z': 56, 'v': 97, 't': 151, 'f': 72,
+    'g': 63, 'd': 113, 'p': 69, 'm': 198, 'i': 35, 'q': 4, 'r': 10, 'b': 54,
+    'h': 42, 'x': 11, 'k': 41, 'j': 12
   },
-  'aq': {'u': 51, 'v': 1, '!': 4, 'r': 1},
-  'Aq': {'u': 9},
-  'Ar': {
-    'n': 53, 'm': 56, 'r': 57, 'c': 49, 't': 38, 'i': 35, 'e': 42, 'a': 47,
-    's': 6, 'b': 18, 'd': 23, 'o': 23, 'g': 34, 'w': 1, 'v': 15, 'z': 8, 'p': 4,
-    'l': 10, 'y': 2, 'j': 3, 'q': 5, 'k': 9, 'u': 5, 'f': 2, 'h': 2, '!': 1
+  'ow': {
+    'n': 96, 'a': 87, 'e': 194, 'm': 13, 'l': 83, '!': 430, 's': 415, 'd': 60,
+    'r': 20, 'i': 155, 'b': 13, 'o': 8, 'y': 6, 'z': 4, 't': 10, 'k': 13,
+    'g': 4, 'h': 7, 'f': 1, 'c': 6, 'p': 1
   },
-  'ar': {
-    'r': 685, 't': 835, 'c': 251, 'k': 228, 'd': 1085, 'n': 296, 's': 298,
-    'p': 95, 'e': 459, 'z': 79, 'v': 91, 'l': 249, 'g': 183, 'b': 202, '!': 674,
-    'm': 170, 'a': 543, 'q': 23, 'i': 599, 'y': 107, 'o': 359, 'h': 26, 'u': 71,
-    'f': 45, 'x': 6, 'w': 35, 'j': 12
+  'wn': {
+    '!': 41, 's': 16, 'i': 9, 'e': 29, 'l': 6, 'f': 1, 'o': 1, 'b': 2, 'a': 4,
+    'd': 4, 'u': 2, 'r': 1, 'h': 3, 'w': 1, 't': 2, 'z': 1, 'y': 2
   },
-  'as': {
-    '!': 799, 'h': 227, 'o': 108, 'q': 29, 't': 402, 's': 493, 'e': 211,
-    'l': 52, 'm': 29, 'k': 154, 'w': 8, 'c': 195, 'i': 181, 'p': 56, 'a': 147,
-    'g': 8, 'b': 28, 'y': 14, 'u': 50, 'f': 4, 'z': 49, 'n': 25, 'd': 9, 'r': 2,
-    'v': 1
+  'Da': {
+    'v': 55, 'n': 118, 'y': 19, 'w': 15, 'l': 78, 'u': 53, 'i': 30, 'h': 31,
+    'r': 112, 'm': 53, 's': 30, 'b': 9, 'g': 32, 'c': 18, 'o': 3, 'd': 17,
+    't': 18, 'k': 8, 'q': 4, 'p': 9, 'z': 4, 'f': 7, 'e': 4, 'x': 1, 'j': 2
   },
-  'As': {
-    'h': 40, 'k': 16, 'b': 6, 't': 24, 'u': 1, 'c': 16, 'a': 14, 'e': 9, 'm': 5,
-    'p': 14, 's': 12, 'l': 7, 'i': 3, 'w': 1, 'q': 1, 'f': 1, 'r': 1, 'n': 2
+  'av': {
+    'i': 223, 'e': 373, 'a': 218, 'o': 78, 'y': 17, 'l': 30, 'n': 8, 's': 4,
   },
-  'At': {
-    'k': 7, 'w': 4, 'h': 16, 'c': 7, 'e': 5, 't': 23, 'l': 2, 'n': 1, 'i': 4,
-    'a': 6, 'o': 3, 'z': 2, 'm': 2
+  'vi': {
+    's': 87, 'd': 29, 'l': 181, 'n': 231, 'e': 75, 't': 91, 'g': 30, 'a': 52,
+    '!': 33, 'z': 9, 'c': 200, 'r': 17, 'h': 1, 'u': 3, 'v': 4, 'o': 23,
+    'k': 13, 'j': 1
   },
-  'at': {
-    's': 91, 't': 488, 'k': 33, 'e': 319, 'r': 87, 'h': 352, 'o': 241, 'f': 7,
-    'l': 55, 'c': 81, 'u': 48, 'z': 102, 'a': 187, 'm': 24, 'y': 23, 'i': 126,
-    '!': 158, 'n': 23, 'w': 8, 'd': 2, 'v': 1, 'g': 1
+  'is': {
+    '!': 857, 'h': 260, 'o': 217, 'e': 305, 't': 449, 'c': 195, 's': 283,
+    'n': 42, 'l': 77, 'p': 29, 'k': 108, 'b': 44, 'd': 14, 'w': 19, 'm': 41,
+    'v': 2, 'i': 107, 'a': 76, 'u': 13, 'g': 5, 'z': 25, 'y': 5, 'q': 2, 'r': 6,
+    'f': 4, 'j': 2
   },
-  'au': {
-    'g': 325, 'l': 240, 'n': 77, 'e': 120, 'f': 50, 's': 250, 'd': 123,
-    '!': 314, 't': 120, 'r': 119, 'x': 78, 'c': 72, 'm': 121, 'p': 36, 'b': 80,
-    'j': 1, 'v': 18, 'k': 18, 'z': 18, 'w': 7, 'a': 18, 'h': 9, 'i': 8, 'y': 2,
-    'o': 4, 'u': 1
+  'Mi': {
+    'l': 195, 't': 54, 'r': 48, 'd': 21, 'c': 101, 'n': 165, 'm': 8, 'x': 5,
+    'z': 16, 'g': 19, 'e': 39, 'k': 45, 'y': 22, 's': 66, 'j': 2, 'f': 2,
+    'u': 2, 'h': 23, 'a': 5, 'o': 7, 'v': 2, 'q': 2
   },
-  'Au': {
-    's': 26, 'g': 24, 't': 18, 'l': 14, 'c': 9, 'd': 13, 'b': 13, 'e': 5,
-    '!': 1, 'm': 9, 'r': 10, 'y': 4, 'x': 2, 'z': 3, 'v': 1, 'n': 5, 'i': 2,
-    'k': 4, 'j': 1, 'f': 3, 'w': 2, 'p': 2, 'a': 1
+  'le': {
+    'r': 1331, 'n': 513, 'z': 45, 'y': 1007, 'm': 186, 's': 596, 'x': 26,
+    '!': 1423, 't': 354, 'i': 150, 'o': 38, 'g': 69, 'a': 110, 'v': 49, 'd': 50,
+    'l': 37, 'j': 23, 'f': 39, 'e': 129, 'u': 32, 'b': 82, 'c': 98, 'h': 35,
+    'w': 72, 'k': 59, 'p': 32, 'q': 1
   },
-  'Av': {'i': 15, 'e': 35, 'a': 12, 'o': 4, 'r': 2, 'n': 1},
-  'av': {
-    'i': 223, 'e': 373, 'a': 218, 'o': 78, 'y': 17, 'l': 30, 'n': 8, 's': 4,
-    'r': 22, 'u': 5, '!': 4, 'j': 1, 'c': 2, 'z': 2, 'd': 3, 'k': 3, 'g': 1, 
-    't': 1
+  'er': {
+    '!': 8545, 's': 1089, 'n': 399, 'e': 424, 't': 869, 'a': 426, 'r': 660,
+    'g': 740, 'k': 187, 'c': 123, 'y': 169, 'o': 410, 'm': 467, 'w': 69,
+    'd': 187, 'v': 99, 'i': 499, 'f': 84, 'l': 385, 'b': 230, 'z': 56, 'h': 129,
+    'u': 55, 'p': 35, 'q': 7, 'j': 12, 'x': 1
   },
-  'Aw': {'a': 4, 'o': 1, 'e': 2, 'k': 2, 'b': 1, 't': 2, 'y': 1, '!': 1},
-  'aw': {
-    'f': 5, '!': 160, 'k': 21, 'r': 18, 's': 34, 'y': 8, 'a': 141, 't': 16,
-    'l': 47, 'e': 42, 'h': 14, 'c': 10, 'o': 10, 'n': 19, 'i': 27, 'v': 4,
-    'b': 9, 'g': 2, 'd': 16, 'w': 4, 'u': 2, 'm': 3
+  'ls': {
+    'o': 144, '!': 247, 'h': 30, 'e': 97, 't': 145, 'w': 9, 'k': 94, 'b': 31,
+    'c': 29, 'a': 31, 'z': 2, 's': 6, 'u': 2, 'i': 26, 'n': 2, 'l': 6, 'm': 14,
+    'p': 7, 'd': 6, 'f': 2, 'g': 5, 'r': 2, 'v': 1, 'y': 1
   },
-  'Ax': {'t': 5, 'f': 1, 'e': 6, 'l': 2, 's': 2, '!': 1, 'o': 1, 'm': 1},
-  'ax': {
-    'w': 1, 't': 11, '!': 27, 'e': 7, 'o': 3, 'l': 5, 'f': 2, 's': 4, 'i': 9,
-    'u': 1, 'm': 4, 'h': 1, 'b': 4, 'c': 2, 'a': 6
+  'Mo': {
+    'o': 50, 'r': 276, 'n': 287, 's': 90, 'l': 95, 'b': 8, 'y': 15, 'c': 20,
+    'h': 34, 't': 38, 'u': 55, 'f': 10, 'e': 30, 'j': 4, 'w': 17, 'a': 12,
+    'x': 4, 'd': 30, 'i': 13, 'z': 17, 'g': 16, '!': 1, 'm': 14, 'k': 6, 'q': 1,
+    'v': 3, 'p': 1
   },
-  'Ay': {
-    'a': 5, 'e': 5, 'r': 2, 'c': 2, 'o': 6, 'b': 1, 'l': 7, 'm': 2, 'u': 2,
-    's': 2, 'n': 1, 'd': 4, 'k': 1, 'y': 1, 't': 1, 'h': 1
+  'oo': {
+    'r': 83, 'k': 157, 'p': 53, 'd': 324, 'l': 108, 'n': 107, 'v': 7, 't': 88,
+    'm': 79, 'c': 13, '!': 44, 's': 64, 'h': 4, 'z': 8, 'f': 17, 'g': 17,
+    'e': 8, 'b': 6, 'y': 7, 'i': 3, 'w': 1
+  },
+  'or': {
+    'e': 577, '!': 365, 'r': 241, 'g': 154, 'd': 505, 't': 445, 'a': 259,
+    'y': 52, 'n': 386, 'm': 114, 's': 232, 'k': 87, 'i': 275, 'b': 67, 'l': 60,
+    'w': 20, 'p': 38, 'o': 161, 'c': 77, 'v': 28, 'h': 15, 'f': 114, 'z': 24,
+    'q': 8, 'u': 22, 'j': 4
+  },
+  're': {
+    '!': 861, 'e': 285, 'z': 108, 's': 442, 'n': 635, 'w': 77, 't': 283,
+    'r': 200, 'g': 109, 'l': 402, 'y': 184, 'v': 60, 'a': 203, 'd': 148,
+    'm': 112, 'i': 222, 'j': 21, 'c': 123, 'u': 61, 'b': 52, 'o': 18, 'h': 42,
+    'k': 71, 'f': 29, 'x': 6, 'p': 22, 'q': 5
+  },
+  'Ta': {
+    'y': 15, 't': 32, 'n': 80, 'l': 63, 'p': 26, 'b': 36, 'c': 24, 'v': 23,
+    'f': 12, 'g': 24, 'r': 89, 'm': 40, 'i': 16, 'k': 26, '!': 1, 's': 26,
   },
   'ay': {
     'l': 55, '!': 468, 'e': 104, 'n': 69, 't': 30, 's': 48, 'o': 55, 'd': 31,
     'm': 43, 'f': 9, 'w': 14, 'a': 103, 'b': 34, 'h': 21, 'r': 14, 'g': 5,
     'p': 3, 'c': 24, 'z': 5, 'v': 2, 'u': 5, 'k': 5, 'i': 3, 'y': 3
   },
-  'az': {
-    '!': 50, 'i': 82, 'a': 103, 'q': 5, 'z': 108, 'o': 49, 'e': 97, 'u': 16,
-    'l': 13, 'c': 4, 'd': 8, 'g': 4, 'm': 8, 'y': 7, 'k': 1, 'w': 1, 's': 3,
-    'n': 3, 'v': 1
+  'yl': {
+    'o': 38, 'e': 97, 'v': 12, 'i': 15, 'a': 43, 't': 2, 'l': 12, 's': 7,
+    '!': 16, 'w': 2, 'd': 2, 'y': 3, 'u': 2, 'k': 2, 'n': 2, 'm': 1
   },
-  'Az': {
-    'e': 5, 'u': 4, 'a': 5, 'i': 3, 'c': 1, 'b': 2, 'z': 7, 'h': 1, 'o': 4
+  'lo': {
+    'r': 145, '!': 638, 'v': 60, 'n': 270, 'w': 246, 'y': 24, 'c': 141, 'a': 17,
+    'm': 103, 'u': 96, 'o': 51, 'b': 14, 's': 200, 'g': 28, 'd': 25, 'i': 17,
+    't': 132, 'p': 32, 'e': 43, 'z': 11, 'q': 2, 'h': 22, 'f': 44, 'x': 4,
+    'k': 10, 'j': 1, 'l': 1
   },
-  'Ba': {
-    'k': 33, 'i': 66, 'r': 517, 'n': 107, 't': 100, 'l': 248, 's': 124, 'x': 7,
-    'u': 81, 'c': 81, 'e': 18, 'b': 50, 'g': 42, 'p': 5, 'd': 46, 'y': 46,
-    'h': 24, 'z': 24, 'v': 8, 'a': 9, 'm': 20, 'w': 9, '!': 1, 'f': 5, 'o': 1,
-    'q': 4, 'j': 7
+  'An': {
+    'd': 104, 't': 79, 'a': 25, 'g': 82, 'n': 30, 's': 23, 'c': 15, 'z': 8,
+    'k': 9, 'w': 2, '!': 1, 'e': 13, 'f': 1, 'h': 2, 'o': 5, 'i': 11, 'l': 1,
+    'y': 1, 'r': 1
   },
-  'ba': {
-    'r': 190, 'l': 103, 'n': 128, 'k': 32, '!': 128, 'u': 226, 'j': 7, 's': 55,
-    'y': 19, 'c': 246, 't': 48, 'p': 2, 'd': 18, 'z': 8, 'g': 13, 'i': 10,
-    'o': 4, 'm': 4, 'w': 3, 'h': 9, 'v': 3, 'b': 3, 'e': 4, 'a': 5
+  'nd': {
+    'e': 835, 'r': 267, 'o': 297, '!': 674, 'l': 128, 's': 120, 'a': 224,
+    't': 62, 'y': 53, 'i': 187, 'h': 23, 'q': 6, 'b': 31, 'm': 22, 'g': 9,
   },
-  'bb': {
-    '!': 35, 'a': 31, 'i': 59, 's': 35, 'o': 24, 'e': 104, 'y': 17, 'l': 26,
-    'r': 5, 'u': 1
+  'de': {
+    'r': 1033, 'z': 48, '!': 377, 's': 144, 'n': 500, 'l': 371, 'a': 59,
+    'i': 23, 'x': 5, 't': 38, 'b': 29, 'e': 35, 'v': 21, 'm': 81, 'u': 4,
+    'o': 17, 'k': 42, 'w': 23, 'j': 13, 'f': 9, 'g': 18, 'y': 25, 'c': 41,
+    'h': 16, 'p': 4, 'd': 1
   },
-  'bc': {'o': 1, 'z': 5, 'h': 1, 'k': 1},
-  'bd': {'u': 10, 'i': 4, 'y': 1, 'o': 7, 'e': 14, 'a': 5},
-  'Be': {
-    'l': 216, 'n': 241, 'r': 373, 'c': 70, 'a': 135, 's': 59, 't': 76, 'g': 22,
-    'e': 62, 'y': 22, 'v': 28, 'h': 42, 'd': 51, 'm': 15, 'j': 9, 'w': 4,
-    'i': 41, 'z': 9, 'q': 2, 'u': 23, 'b': 6, 'k': 9, 'f': 2, 'x': 1, 'o': 1,
-    'p': 1, '!': 1
+  'rs': {
+    'o': 268, '!': 641, 'h': 111, 'e': 148, 't': 234, 'p': 12, 'c': 88, 'y': 5,
+    'l': 32, 'w': 5, 'a': 51, 'b': 16, 'k': 115, 'i': 53, 'd': 14, 'u': 4,
+    'm': 28, 'g': 2, 's': 8, 'f': 6, 'z': 3, 'n': 7, 'j': 1, 'v': 2
   },
-  'be': {
-    'r': 1372, 'l': 230, 's': 42, 't': 52, '!': 142, 'd': 17, 'e': 78, 'c': 114,
-    'y': 39, 'a': 59, 'n': 141, 'i': 40, 'z': 7, 'v': 2, 'k': 25, 'b': 3,
-    'q': 1, 'h': 6, 'g': 2, 'm': 1, 'o': 5, 'u': 2, 'j': 1
+  'Th': {'o': 109, 'u': 37, 'a': 66, 'r': 40, 'i': 62, 'e': 68, 'w': 2, 'y': 6},
+  'ho': {
+    'm': 74, 'l': 226, 'p': 23, 'd': 19, 'r': 253, 'n': 128, 'u': 157, '!': 82,
+    'a': 15, 'e': 100, 'i': 10, 'o': 58, 'c': 25, 'f': 128, 'w': 82, 't': 34,
+    'y': 10, 'q': 1, 'b': 14, 'v': 27, 'j': 3, 's': 26, 'k': 7, 'g': 4, 'z': 1
   },
-  'bf': {'r': 1, 'l': 1},
-  'bg': {'o': 1, 'e': 2},
-  'bh': {'a': 14, 'r': 1, 'o': 5, 'u': 1, 'e': 1, '!': 1},
-  'Bh': {'a': 16, 'o': 1, 'u': 1},
-  'bi': {
-    'n': 182, 'o': 19, 's': 51, 't': 43, 'a': 66, 'e': 72, 'l': 63, 'c': 42,
-    'd': 17, '!': 26, 'k': 12, 'b': 4, 'r': 14, 'g': 20, 'z': 4, 'j': 2, 'm': 1,
-    'h': 2, 'f': 1, 'y': 1
+  'om': {
+    'a': 214, 'p': 60, 'e': 193, 'i': 106, 'b': 164, 'o': 58, '!': 265, 'l': 17,
+    's': 52, 'w': 2, 'm': 80, 'f': 5, 'q': 3, 'k': 16, 'r': 11, 'y': 8, 'c': 2,
+    'u': 13, 'g': 6, 'n': 4, 'h': 4, 't': 2, 'd': 4, 'j': 3, 'z': 4, 'v': 1
   },
-  'Bi': {
-    's': 66, 'r': 77, 'n': 48, 'l': 95, 'g': 36, 'd': 23, 'v': 8, 'c': 36,
-    't': 26, 'b': 17, 'a': 31, 'x': 3, 'e': 82, 'o': 6, 'z': 8, 'f': 3, 'h': 4,
-    'j': 2, 'p': 1, '!': 1, 'm': 1
+  'ma': {
+    's': 125, 'n': 2414, 'l': 69, 'c': 67, 'h': 13, 'r': 273, 'k': 62, 'y': 44,
+    'x': 2, 'd': 40, '!': 276, 't': 62, 'm': 5, 'i': 53, 'g': 37, 'z': 8,
   },
-  'bj': {'i': 1, 'e': 1, 'o': 1},
-  'Bj': {'o': 12, 'e': 6},
-  'bk': {'e': 11, 'o': 4, 'i': 4, 'a': 6},
-  'Bl': {'a': 218, 'e': 62, 'u': 39, 'o': 85, 'i': 35, 'y': 10},
-  'bl': {'e': 276, 'a': 47, 'o': 38, 'i': 44, 'u': 12, 'y': 9, '!': 9},
-  'bm': {'a': 11, 'e': 2, 'y': 1},
-  'bn': {'e': 31, 'a': 2, 'o': 1, 'y': 1, 'i': 3},
-  'bo': {
-    'r': 143, 't': 51, 'n': 89, 'i': 17, 's': 30, 'u': 80, '!': 98, 'd': 16,
-    'a': 9, 'e': 17, 'w': 40, 'g': 8, 'y': 16, 'z': 7, 'l': 77, 'x': 1, 'c': 7,
-    'm': 3, 'o': 14, 'v': 12, 'h': 3, 'k': 2, 'j': 1
+  'as': {
+    '!': 799, 'h': 227, 'o': 108, 'q': 29, 't': 402, 's': 493, 'e': 211,
+    'l': 52, 'm': 29, 'k': 154, 'w': 8, 'c': 195, 'i': 181, 'p': 56, 'a': 147,
   },
-  'Bo': {
-    'y': 50, 'w': 65, 'o': 51, 'n': 162, 'l': 114, 'u': 148, 'g': 54, 's': 82,
-    'r': 189, 'x': 7, 'b': 36, 'h': 53, 'c': 44, 'e': 82, 't': 61, 'z': 21,
-    'i': 30, 'a': 28, 'd': 55, 'v': 13, 'j': 4, 'm': 21, 'p': 2, 'q': 2, 'k': 8,
-    'f': 2, '!': 1
+  'Ja': {
+    'c': 61, 'm': 24, 'r': 63, 'n': 106, 's': 26, 'e': 8, 'y': 11, 'i': 6,
+    'f': 6, 'b': 13, 'q': 9, 'v': 11, 'w': 5, 'u': 16, 'h': 11, 'g': 16, 'l': 5,
+    'k': 19, 'z': 1, 'd': 3, 't': 1, 'x': 1, 'p': 3, 'a': 2, 'j': 1
   },
-  'bp': {'l': 1},
-  'br': {
-    'i': 158, 'e': 156, 'o': 179, 'a': 137, 'y': 23, 'u': 38, '!': 1, 'z': 3
+  'ac': {
+    'k': 557, 'e': 152, 'o': 136, 'h': 602, 'd': 15, 'i': 130, 'r': 35, 'y': 23,
+    'a': 102, '!': 50, 'q': 25, 's': 12, 'l': 26, 'c': 148, 'p': 6, 'm': 9,
+    'g': 4, 'f': 2, 'n': 12, 'z': 37, 'u': 29, 't': 6, 'b': 3, 'w': 1, 'v': 4
   },
-  'Br': {
-    'o': 311, 'y': 28, 'a': 402, 'e': 253, 'i': 247, 'u': 188, 'z': 10, 'w': 1,
-    'l': 1, 'r': 1, 'd': 1
+  'ck': {
+    's': 151, 'e': 760, '!': 1436, 'i': 314, 'l': 234, 'w': 28, 'm': 100,
+    'b': 25, 'n': 51, 'a': 103, 'h': 59, 't': 7, 'r': 36, 'f': 18, 'u': 18,
+    'o': 72, 'y': 28, 'd': 4, 'p': 2, 'k': 1, 'x': 3, 'g': 1, 'z': 1
   },
-  'bs': {
-    'o': 18, '!': 67, 't': 20, 'e': 7, 'h': 7, 'b': 1, 'c': 8, 'k': 11, 'm': 1,
-    'a': 5, 'w': 1, 'i': 1
+  'ks': {
+    'o': 54, '!': 206, 'd': 1, 't': 49, 'e': 26, 'h': 21, 'c': 6, 'l': 5,
+    'b': 4, 'w': 2, 's': 1, 'm': 5, 'a': 5, 'i': 9, 'y': 1, 'k': 2
   },
-  'bt': {'r': 1, '!': 3, 's': 1},
-  'bu': {
-    'r': 307, 'l': 16, 'c': 24, 's': 75, 'n': 11, 't': 17, 'h': 7, 'e': 9,
-    'q': 1, 'i': 2, 'd': 2, 'k': 1, '!': 7, 'f': 1, 'y': 1, 'a': 1, 'o': 1,
-    'm': 2, 'g': 2, 'b': 1
+  'Wh': {'i': 174, 'e': 45, 'a': 19, 'y': 9, 'o': 7, 't': 1},
+  'hi': {
+    't': 185, 'l': 207, 'n': 257, 's': 79, 'e': 146, 'p': 44, 'r': 92, 'b': 33,
+    'g': 24, 'v': 19, 'a': 103, 'f': 23, 'u': 8, 'c': 41, '!': 151, 'm': 98,
   },
-  'Bu': {
-    't': 73, 'r': 304, 's': 110, 'c': 111, 'l': 65, 'n': 55, 'f': 17, 'e': 50,
-    'm': 21, 'i': 12, 'x': 3, 'd': 42, 'g': 21, 'z': 19, 'o': 12, 'h': 10,
-    'k': 8, 'b': 16, 'p': 1, 'a': 3, 'y': 5, 'j': 5, 'q': 2, 'v': 2
+  'te': {
+    '!': 839, 'r': 1373, 'w': 24, 'v': 29, 'p': 44, 's': 177, 'e': 108, 'g': 33,
+    'n': 428, 'z': 22, 'h': 18, 'l': 370, 'i': 243, 'm': 58, 'a': 90, 'f': 43,
+    't': 46, 'd': 49, 'o': 13, 'b': 22, 'y': 30, 'c': 34, 'j': 8, 'k': 46,
+    'u': 18, 'q': 1, 'x': 2
   },
-  'Bv': {'e': 1},
-  'bv': {'r': 1, 'i': 1},
-  'bw': {'o': 1, 'e': 1},
-  'by': {
-    '!': 262, 'r': 1, 'l': 10, 'n': 4, 's': 5, 'f': 1, 'a': 3, 'o': 1, 'k': 1,
-    'c': 1, 'e': 1
+  'Ha': {
+    'r': 413, 'l': 155, 'y': 64, 'm': 146, 'w': 32, 'n': 208, 't': 53, 'h': 7,
+    'a': 27, 's': 98, 'i': 49, 'd': 39, 'g': 77, 'c': 41, 'u': 79, 'v': 36,
+    'z': 33, '!': 1, 'b': 32, 'k': 13, 'f': 19, 'j': 4, 'e': 23, 'p': 12,
+    'o': 1, 'x': 2, 'q': 2
   },
-  'By': {
-    'r': 18, 'e': 6, 'n': 9, 'a': 8, 'l': 5, 'b': 2, 'i': 1, 'f': 2, 'u': 2,
-    'h': 1, 'k': 2, 'w': 2, 'o': 4, 'm': 1, 't': 2, 's': 3, 'c': 1
+  'ar': {
+    'r': 685, 't': 835, 'c': 251, 'k': 228, 'd': 1085, 'n': 296, 's': 298,
+    'p': 95, 'e': 459, 'z': 79, 'v': 91, 'l': 249, 'g': 183, 'b': 202, '!': 674,
+    'm': 170, 'a': 543, 'q': 23, 'i': 599, 'y': 107, 'o': 359, 'h': 26, 'u': 71,
+    'f': 45, 'x': 6, 'w': 35, 'j': 12
   },
-  'bz': {'a': 1, 'i': 2, 'd': 1},
-  'Bz': {'h': 1},
-  'ca': {
-    'n': 138, 's': 75, 'r': 271, 'l': 134, 'd': 28, 'b': 12, '!': 219, 'i': 20,
-    'u': 22, 'm': 51, 'f': 16, 'h': 7, 'v': 21, 't': 47, 'y': 12, 'g': 16,
-    'w': 2, 'z': 6, 'a': 1, 'p': 13, 'k': 11, 'c': 9, 'j': 4, 'o': 5, 'e': 2
+  'rr': {
+    'i': 493, 'e': 446, 'y': 200, 'a': 336, 'o': 251, '!': 94, 'm': 4, 's': 6,
+    'u': 48, 'v': 1, 'l': 3, 'b': 2, 'g': 1, 't': 1, 'n': 1, 'h': 1, 'w': 1
   },
-  'Ca': {
-    'r': 474, 'm': 129, 's': 278, 'l': 199, 'n': 181, 'i': 28, 'b': 60, 't': 87,
-    'p': 121, 'u': 34, 'h': 13, 'v': 52, 'g': 12, 'd': 39, 'z': 11, 'e': 3,
-    'w': 8, 'o': 5, 'c': 22, 'f': 17, 'y': 15, 'j': 7, 'q': 1, 'a': 2, 'k': 3
+  'ri': {
+    's': 490, 'g': 255, 'c': 524, 'f': 51, 'e': 442, 'q': 21, 'd': 215,
+    'n': 766, 'm': 116, 't': 232, 'l': 158, 'o': 200, 'x': 15, 'a': 234,
+    'p': 48, 'v': 54, 'z': 61, 'b': 59, '!': 356, 'w': 6, 'j': 3, 'k': 41,
+    'u': 12, 'h': 10, 'i': 2, 'r': 2, 'y': 1
   },
-  'cb': {'r': 13, 'e': 6, 'u': 5, 'a': 4},
-  'cc': {
-    'o': 186, 'a': 205, 'l': 100, 'u': 63, 'r': 47, 'i': 209, 'h': 119, 'e': 12,
-    'k': 2
+  'Ma': {
+    'r': 622, 's': 183, 't': 247, 'y': 79, 'n': 347, 'c': 252, 'l': 225,
+    'x': 18, 'd': 99, 'h': 68, 'g': 128, 'j': 33, 'u': 67, 'b': 22, 'i': 80,
+    'p': 12, 'e': 23, '!': 1, 'a': 12, 'k': 33, 'z': 58, 'f': 10, 'o': 4,
+    'w': 6, 'v': 12, 'm': 17, 'q': 1
   },
-  'Cd': {'e': 1},
-  'cd': {'o': 30, 'a': 19, 'e': 15, 'u': 9, 'i': 5},
-  'ce': {
-    '!': 370, 'r': 81, 'n': 80, 'v': 15, 'l': 142, 'y': 43, 'd': 21, 'a': 26,
-    'p': 3, 'w': 13, 't': 29, 's': 32, 'f': 5, 'o': 2, 'u': 3, 'k': 82, 'g': 9,
-    'm': 8, 'b': 3, 'c': 3, 'e': 2, 'j': 1, 'h': 1, 'i': 7
+  'rt': {
+    'i': 203, 'e': 257, 's': 99, '!': 795, 'o': 219, 'h': 319, 'z': 93, 'm': 31,
+    'l': 69, 'y': 81, 'w': 18, 'n': 41, 'a': 85, 'u': 51, 'r': 33, 'c': 10,
   },
-  'Ce': {
-    'r': 88, 'c': 15, 'n': 22, 'j': 2, 'p': 8, 'b': 2, 'd': 11, 'a': 8, 'l': 27,
-    's': 13, 'v': 2, 'f': 3, 'z': 2, 'g': 3, 'm': 2, 't': 1, 'o': 2
+  'ti': {
+    'n': 482, 'z': 10, 'e': 167, 'l': 138, 's': 151, 'a': 65, 'c': 100, 't': 34,
+    'r': 22, 'v': 15, '!': 425, 'm': 32, 'd': 15, 'o': 28, 'g': 68, 'f': 10,
+    'h': 2, 'j': 4, 'u': 4, 'p': 10, 'b': 8, 'w': 2, 'x': 2, 'k': 14, 'y': 1
   },
-  'cf': {'a': 24, 'e': 9, 'i': 1, 'o': 1},
-  'cg': {
-    'e': 11, 'u': 29, 'o': 20, 'i': 28, 'r': 33, 'h': 8, 'a': 36, 'l': 28, 
-    'w': 2
+  'in': {
+    '!': 1906, 'e': 885, 's': 726, 'g': 2064, 'a': 359, 'n': 253, 'd': 310,
+    'o': 551, 'c': 156, 't': 245, 'l': 45, 'k': 305, 'b': 72, 'h': 61, 'f': 26,
+    'z': 66, 'i': 419, 'v': 14, 'q': 6, 'r': 24, 'm': 20, 'w': 20, 'y': 16,
+    'j': 2, 'u': 16, 'p': 3
   },
-  'Ch': {
-    'a': 343, 'r': 94, 'e': 172, 'u': 51, 'i': 164, 'o': 66, 'm': 7, 'y': 3,
-    'l': 4, 'h': 14, 'k': 1, 'w': 2, 'v': 1
+  'mp': {
+    's': 44, 'b': 4, 't': 26, '!': 113, 'h': 43, 'o': 42, 'l': 50, 'k': 16,
+    'i': 35, 'a': 65, 'e': 115, 'f': 23, 'u': 6, 'm': 5, 'n': 4, 'p': 8,
+    'r': 11, 'y': 4, 'c': 1
   },
-  'ch': {
-    'e': 1108, 'a': 539, 'o': 336, 'm': 202, '!': 1325, 'u': 196, 'n': 134,
-    'w': 147, 'r': 117, 'i': 506, 't': 174, 'c': 8, 's': 54, 'f': 24, 'k': 52,
-    'l': 228, 'h': 23, 'b': 33, 'v': 2, 'y': 19, 'p': 2, 'g': 3, 'z': 3, 'j': 1,
-    'd': 2
+  'ps': {
+    'o': 33, '!': 88, 'e': 21, 'c': 4, 't': 22, 'h': 14, 'k': 17, 'l': 2,
+    'w': 1, 'a': 4, 'z': 1, 'y': 2, 'i': 2, 'n': 1
+  },
+  'Ga': {
+    'r': 241, 't': 49, 'l': 216, 'i': 29, 'y': 25, 'm': 55, 'g': 21, 's': 63,
+    'b': 46, 'u': 66, 'n': 93, 'v': 25, 'f': 8, 'd': 27, 'o': 2, 'z': 14,
+    'e': 15, 'h': 8, 'j': 6, 'w': 11, 'x': 1, 'a': 4, 'p': 4, 'c': 10
+  },
+  'rc': {
+    'i': 76, 'e': 93, 'a': 46, 'h': 228, 'u': 26, 'o': 64, 'l': 12, 'y': 16,
+    'r': 8, '!': 8, 'k': 26, 'z': 32, 'q': 1, 'm': 1
   },
   'ci': {
     'a': 149, 's': 24, 'n': 124, 'o': 181, 'l': 59, 'e': 49, '!': 169, 'd': 11,
     'k': 31, 'v': 10, 'c': 42, 'r': 7, 't': 17, 'p': 8, 'u': 17, 'f': 8, 'm': 4,
     'g': 8, 'b': 6, 'z': 1, 'w': 1
   },
-  'Ci': {
-    's': 13, 'n': 21, 'm': 12, 'o': 9, 'f': 3, 'r': 22, 'p': 13, 'c': 30,
-    'e': 20, 'l': 13, 'a': 31, 't': 14, 'u': 7, 'd': 2, 'v': 7, 'b': 5, 'z': 1,
-    'h': 2, 'g': 1
+  'ez': {
+    '!': 378, 'a': 47, 'm': 1, 'e': 43, 'q': 2, 'i': 25, 'c': 2, 'u': 2,
+    'o': 12, 'z': 30, 'y': 2, 'n': 10, 'g': 3, 'r': 2, 'd': 1, 'l': 2, 's': 1,
+    'k': 1, 'w': 1
   },
-  'cj': {'u': 2},
-  'ck': {
-    's': 151, 'e': 760, '!': 1436, 'i': 314, 'l': 234, 'w': 28, 'm': 100,
-    'b': 25, 'n': 51, 'a': 103, 'h': 59, 't': 7, 'r': 36, 'f': 18, 'u': 18,
-    'o': 72, 'y': 28, 'd': 4, 'p': 2, 'k': 1, 'x': 3, 'g': 1, 'z': 1
+  'Ro': {
+    'b': 94, 'd': 103, 'g': 38, 's': 205, 'm': 79, 'w': 39, 'y': 19, 'j': 6,
+    't': 74, 'a': 26, 'l': 60, 'c': 62, 'u': 74, 'e': 68, 'p': 9, 'o': 26,
+    'n': 41, 'h': 40, 'q': 3, 'z': 23, 'r': 8, '!': 1, 'k': 7, 'f': 4, 'i': 6,
+    'x': 5, 'v': 10
+  },
+  'ob': {
+    'i': 83, 'e': 147, 's': 27, 'b': 58, 'l': 54, 'a': 63, 'o': 49, '!': 17,
+    'u': 16, 'y': 17, 'g': 1, 'd': 5, 'r': 40, 'c': 3, 'n': 3, 'k': 5, 'z': 2,
+    'h': 1, 'm': 2
+  },
+  'bi': {
+    'n': 182, 'o': 19, 's': 51, 't': 43, 'a': 66, 'e': 72, 'l': 63, 'c': 42,
+    'd': 17, '!': 26, 'k': 12, 'b': 4, 'r': 14, 'g': 20, 'z': 4, 'j': 2, 'm': 1,
+    'h': 2, 'f': 1, 'y': 1
   },
-  'cl': {'a': 103, 'u': 17, 'e': 101, 'o': 29, 'i': 30, '!': 3, 'y': 3},
   'Cl': {'a': 130, 'i': 47, 'e': 79, 'o': 59, 'y': 9, 'u': 24},
-  'Cm': {'i': 1},
-  'cm': {'i': 19, 'a': 30, 'u': 20, 'o': 6, 'e': 10},
-  'cn': {'e': 40, 'a': 25, 'u': 6, 'i': 17, 'y': 1, 'o': 2, '!': 1},
-  'Co': {
-    'l': 228, 'o': 70, 'x': 7, 'h': 17, 'n': 234, 'b': 32, 'p': 46, 'r': 283,
-    'c': 53, 'm': 77, 'f': 20, 't': 53, 'w': 34, 'v': 35, 's': 79, 'u': 111,
-    'k': 8, 'a': 27, 'd': 19, 'y': 12, 'e': 6, 'g': 19, 'z': 13, 'i': 8, '!': 1
+  'la': {
+    'r': 352, 'c': 182, 'n': 884, 's': 283, 'z': 62, 'i': 114, 'k': 111,
+    '!': 907, 'u': 124, 'y': 95, 'g': 102, 'h': 62, 'p': 41, 't': 160, 'l': 39,
+    'm': 158, 'd': 116, 'w': 60, 'b': 51, 'v': 69, 'f': 45, 'a': 21, 'x': 6,
+    'o': 10, 'e': 24, 'q': 4, 'j': 9
   },
-  'co': {
-    't': 91, 'y': 9, 'b': 30, 'r': 93, 'x': 20, 's': 41, 'n': 141, 'c': 57,
-    '!': 376, 'm': 101, 'l': 115, 'e': 17, 'u': 56, 'i': 15, 'o': 12, 'g': 7,
-    'w': 10, 'a': 15, 'f': 11, 'v': 25, 'p': 11, 'd': 3, 'z': 5, 'h': 1
+  'rk': {
+    '!': 128, 'e': 183, 'i': 85, 's': 46, 'l': 46, 'm': 17, 'p': 2, 'h': 28,
+    'w': 10, 'n': 9, 'o': 72, 'a': 53, 'u': 15, 'g': 1, 'b': 3, 'y': 5, 'd': 3,
+    'r': 5, 't': 2, 'q': 1, 'k': 2, 'v': 4, 'j': 1, 'c': 2
   },
-  'cp': {'h': 17, 'e': 5, 'a': 6, 'i': 1, 'r': 1},
-  'cq': {'u': 64, '!': 2},
-  'cr': {'a': 58, 'u': 15, 'o': 68, 'e': 53, 'i': 38, 'y': 1},
-  'Cr': {'u': 69, 'a': 132, 'o': 169, 'e': 103, 'i': 103, 'y': 10, 'n': 2},
-  'cs': {
-    '!': 10, 'o': 7, 'w': 5, 'h': 6, 'p': 5, 'i': 4, 's': 1, 'a': 3, 'f': 1,
-    'm': 1, 'e': 1, 'k': 5, 't': 1
+  'od': {
+    'r': 52, '!': 202, 's': 26, 'e': 185, 'g': 37, 'd': 47, 'w': 18, 'm': 13,
+    'y': 44, 'a': 92, 'f': 14, 'c': 3, 'l': 32, 'b': 18, 'i': 96, 'o': 48,
+    'h': 17, 'n': 23, 'k': 12, 'z': 10, 't': 14, 'u': 8, 'p': 3, 'v': 3
   },
-  'Cs': {'a': 1, 'u': 2, 'i': 1, 'e': 2},
-  'ct': {'o': 28, '!': 6, 'e': 13, 'a': 4, 'i': 10, 'l': 1, 'h': 5, 'u': 1},
-  'cu': {
-    'l': 43, 'm': 27, 't': 32, 's': 35, 'r': 36, 'n': 11, 'e': 15, 'a': 8,
-    'd': 8, 'f': 4, 'b': 5, 'p': 8, 'c': 9, 'y': 1, 'i': 8, 'o': 2, '!': 8,
-    'z': 7, 'k': 2, 'g': 1
+  'dr': {
+    'i': 201, 'e': 147, 'y': 26, 'a': 78, 'u': 32, 'o': 101, 'z': 4, 'g': 1,
+    'n': 1, 'l': 2, '!': 1, 's': 1
   },
-  'Cu': {
-    'n': 29, 'r': 82, 'm': 28, 'e': 13, 'l': 49, 't': 43, 's': 33, 'p': 10,
-    'o': 3, 'f': 8, 'd': 12, 'c': 18, 'a': 9, 'b': 14, 'y': 1, 'g': 1, 'i': 2,
-    'k': 1, 'z': 6, 'h': 1, 'v': 1, 'j': 1
+  'ig': {
+    'u': 74, 'h': 259, '!': 210, 'g': 141, 'a': 170, 'i': 41, 'e': 149, 'l': 99,
+    's': 25, 'p': 2, 'n': 99, 'd': 6, 'o': 63, 'r': 19, 'b': 9, 't': 7, 'm': 21,
+    'f': 5, 'w': 6, 'k': 2, 'y': 2
   },
-  'Cv': {'e': 1},
-  'cv': {'e': 6, 'a': 5, 'i': 5, 'o': 1},
-  'cw': {'i': 4, 'h': 7, 'a': 9, 'e': 3, 'r': 1},
-  'Cw': {'i': 5, 'a': 1},
-  'cy': {'!': 69, 'r': 1, 'o': 2, 'n': 2, 'p': 1, 'k': 2, 'u': 2, 't': 1},
-  'Cy': {
-    'r': 6, 'p': 7, 'b': 2, 'g': 3, 'n': 2, 'w': 1, 'l': 2, 'f': 1, 'c': 1
+  'gu': {
+    'e': 161, 's': 68, 'y': 11, 'i': 89, 'r': 29, 'm': 12, 'l': 16, 'a': 22,
+    'z': 2, 'n': 23, 'c': 16, 'f': 5, 'o': 2, 't': 5, 'd': 5, 'p': 3, 'h': 3,
+    'b': 2, 'g': 3, '!': 3
   },
-  'Cz': {'e': 12, 'a': 22, 'y': 4, 'u': 4, 'l': 1, 'o': 2, 'w': 1},
-  'cz': {
-    'y': 80, 'a': 41, 'm': 4, 'o': 7, '!': 142, 'n': 6, 'e': 40, 'k': 21,
-    'u': 5, 'b': 1, 'i': 1, 'w': 1
+  'ue': {
+    'z': 67, 'r': 297, 'l': 146, 'n': 130, 'v': 17, '!': 216, 'g': 24, 'e': 9,
+    's': 114, 't': 108, 'y': 11, 'h': 50, 'd': 28, 'b': 28, 'c': 34, 'i': 12,
   },
-  'da': {
-    'm': 69, 'n': 114, '!': 424, 'l': 143, 'r': 90, 'y': 56, 'i': 10, 'c': 22,
-    'd': 14, 'w': 12, 'v': 15, 'z': 8, 'k': 27, 's': 51, 'g': 20, 'u': 18,
-    'h': 51, 'b': 9, 'p': 6, 'f': 6, 'o': 3, 't': 21, 'j': 1, 'e': 3, 'q': 1
+  'Le': {
+    'w': 27, 'e': 38, 'o': 34, 's': 71, 'b': 44, 'a': 83, 'v': 96, '!': 1,
+    'h': 38, 'd': 42, 'm': 69, 'n': 97, 'g': 60, 'y': 20, 'c': 44, 'i': 111,
+    'u': 23, 'r': 22, 'f': 36, 't': 42, 'j': 5, 'p': 28, 'l': 11, 'z': 7,
+    'x': 2, 'q': 1, 'k': 7
   },
-  'Da': {
-    'v': 55, 'n': 118, 'y': 19, 'w': 15, 'l': 78, 'u': 53, 'i': 30, 'h': 31,
-    'r': 112, 'm': 53, 's': 30, 'b': 9, 'g': 32, 'c': 18, 'o': 3, 'd': 17,
-    't': 18, 'k': 8, 'q': 4, 'p': 9, 'z': 4, 'f': 7, 'e': 4, 'x': 1, 'j': 2
+  'ew': {
+    'i': 134, 'a': 94, 's': 135, 'e': 107, 'm': 10, 't': 6, '!': 110, 'c': 10,
+    'b': 24, 'k': 4, 'o': 27, 'h': 12, 'p': 2, 'l': 10, 'n': 6, 'r': 4, 'q': 1,
+    'y': 7, 'f': 1, 'v': 1, 'g': 3, 'd': 1, 'u': 1
   },
-  'db': {'e': 43, 'u': 16, 'o': 16, 'y': 8, 'l': 7, 'r': 5, 'a': 12, 'i': 2},
-  'dc': {'o': 7, 'l': 2, 'a': 5, 'h': 3, 'u': 1, 'r': 2},
-  'dd': {
-    '!': 37, 'l': 43, 'o': 50, 'e': 132, 'y': 40, 'a': 31, 'i': 105, 's': 4,
-    'u': 9, 'r': 8
+  'wi': {
+    's': 33, 'n': 166, 't': 86, 'f': 2, 'l': 49, 'g': 29, 'c': 207, 'e': 58,
+    'a': 25, 'd': 11, 'm': 5, 'h': 1, 'k': 7, 'r': 15, '!': 7, 'z': 1, 'p': 1
   },
-  'De': {
-    'a': 77, 'n': 126, 'l': 346, 'c': 91, 'j': 20, 'm': 165, 'w': 40, 'v': 98,
-    'x': 2, 'h': 26, 'r': 133, 'e': 30, 's': 154, 'b': 89, 'y': 10, 'u': 17,
-    'p': 67, 'g': 80, 'i': 36, 'f': 54, 't': 59, 'd': 21, 'k': 18, 'z': 10,
-    'o': 8, 'q': 2
+  'ee': {
+    '!': 437, 'n': 233, 'd': 94, 'm': 53, 'l': 127, 'v': 26, 's': 107, 'r': 125,
+    'k': 61, 't': 100, 'c': 40, 'h': 31, 'b': 38, 'f': 19, 'g': 32, 'p': 22,
+    'z': 11, 'a': 1, 'u': 4, 'w': 3, 'i': 1
   },
-  'de': {
-    'r': 1033, 'z': 48, '!': 377, 's': 144, 'n': 500, 'l': 371, 'a': 59,
-    'i': 23, 'x': 5, 't': 38, 'b': 29, 'e': 35, 'v': 21, 'm': 81, 'u': 4,
-    'o': 17, 'k': 42, 'w': 23, 'j': 13, 'f': 9, 'g': 18, 'y': 25, 'c': 41,
-    'h': 16, 'p': 4, 'd': 1
+  'Wa': {
+    'l': 210, 'r': 126, 't': 52, 's': 72, 'g': 36, 'd': 32, 'n': 57, 'i': 34,
+    'k': 20, 'y': 25, 'u': 11, 'h': 23, 'm': 11, 'c': 23, 'x': 3, 'f': 5,
+    'e': 6, 'w': 2, 'a': 6, 'j': 1, 'p': 3, 'v': 4, 'b': 2, 'z': 1
   },
-  'df': {'o': 27, 'r': 4, 'i': 15, 'a': 4, 'e': 8, 'l': 1, 'u': 3},
-  'dg': {
-    'e': 254, 'r': 12, 'i': 10, 'a': 7, 's': 2, 'w': 3, 'k': 4, 'd': 1, 'l': 8,
-    'o': 4, 'm': 5, 'p': 1, 'h': 3, 'u': 1, 'f': 2, 'c': 1, 'n': 1, '!': 1
+  'al': {
+    'k': 111, 'l': 1054, 'e': 518, 'd': 301, 'm': 109, 't': 177, '!': 447,
+    's': 137, 'a': 442, 'o': 184, 'h': 24, 'i': 311, 'v': 99, 'y': 44, 'f': 34,
+    'g': 22, 'b': 80, 'c': 103, 'u': 56, 'p': 39, 'z': 39, 'r': 10, 'n': 13,
+    'w': 16, 'q': 3, 'j': 2
   },
-  'dh': {
-    'a': 41, 'o': 27, 'e': 11, 'u': 16, 'i': 6, 'r': 3, 'y': 2, '!': 1, 'n': 1
+  'lk': {
+    'e': 146, 'i': 57, 'n': 9, '!': 68, 's': 13, 'm': 7, 'u': 7, 'o': 56,
+    'l': 5, 'a': 45, 'c': 1, 'w': 2, 'h': 2, 'b': 2, 'r': 1, 'k': 1, 'y': 1
   },
-  'Dh': {'i': 1, 'o': 2, 'e': 2, 'a': 4, 'r': 1},
-  'Di': {
-    'a': 20, 'x': 7, 'c': 60, 'l': 78, 'g': 34, 'e': 81, 'o': 13, 'n': 72,
-    'b': 30, 's': 62, 'p': 22, 'm': 56, 'z': 4, 'r': 24, 't': 32, 'v': 23,
-    'd': 15, 'f': 22, 'k': 7, 'i': 2, 'w': 1, 'h': 1, 'j': 1, 'u': 1
+  'ke': {
+    'r': 759, '!': 680, 's': 130, 'n': 323, 'e': 35, 't': 101, 'y': 170,
+    'w': 10, 'l': 272, 'f': 8, 'o': 3, 'a': 12, 'm': 50, 'd': 5, 'c': 3, 'b': 9,
+    'u': 2, 'i': 5, 'h': 6, 'p': 2, 'k': 2, 'g': 3, 'v': 7, 'z': 1
   },
-  'di': {
-    'n': 410, 'l': 50, 's': 93, 't': 27, 'c': 106, '!': 177, 'a': 72, 'v': 20,
-    'g': 38, 'e': 98, 'f': 16, 'm': 9, 'o': 40, 'x': 10, 'd': 6, 'r': 9,
-    'k': 12, 'z': 10, 'q': 8, 'b': 6, 'w': 2, 'p': 2, 'u': 1, 'h': 1
+  'Al': {
+    'l': 118, 'e': 63, 'v': 42, 's': 24, 'f': 20, 'b': 67, 'd': 34, 'i': 31,
+    't': 61, 'o': 15, 'a': 38, 'm': 40, 'c': 25, 'g': 11, 'p': 13, 'k': 6,
+    'r': 4, 'w': 8, 'u': 8, 'z': 3, 'y': 2, 'q': 4, 'n': 3, 'j': 1, 'h': 4
   },
-  'dj': {'o': 2, 'e': 2, 'i': 5, 'a': 1, 'u': 1, 'm': 1},
-  'Dj': {'u': 1},
-  'Dk': {'!': 1},
-  'dk': {'i': 21, 'e': 17, 'o': 3, 'n': 2, 'a': 8, 'l': 2, 'y': 1},
-  'dl': {'e': 299, 'i': 67, 'o': 49, 'a': 49, '!': 15, 'u': 9, 'y': 9},
-  'Dl': {'o': 2, 'u': 2, 'a': 1},
-  'dm': {'a': 107, 'o': 26, 'u': 8, 'i': 9, 'e': 13},
-  'Dm': {'i': 1},
-  'dn': {'e': 89, 'a': 17, 'i': 24, 'o': 11, 'y': 3, '!': 2, 'g': 1, 'u': 1},
-  'do': {
-    'n': 274, 'z': 11, '!': 419, 'v': 28, 'w': 59, 'l': 78, 'x': 3, 'm': 31,
-    'c': 29, 'r': 189, 'i': 9, 'u': 35, 's': 35, 'y': 8, 'o': 12, 'b': 3,
-    'p': 4, 'g': 2, 't': 11, 'e': 9, 'h': 4, 'f': 7, 'a': 1, 'k': 4
+  'en': {
+    '!': 2387, 'n': 411, 'd': 493, 'k': 145, 's': 573, 'r': 63, 'c': 164,
+    't': 570, 'e': 414, 'o': 185, 'a': 299, 'z': 173, 'p': 12, 'j': 12, 'w': 50,
+    'l': 35, 'b': 517, 'i': 234, 'g': 202, 'y': 40, 'f': 76, 'h': 160, 'm': 44,
+    'u': 27, 'q': 5, 'v': 6
   },
-  'Do': {
-    'u': 53, 'y': 9, 'm': 68, 'r': 115, 'd': 17, 't': 18, 'n': 114, 'w': 49,
-    'o': 22, 'b': 52, 's': 25, 'h': 13, 'l': 69, 'v': 8, 'z': 5, 'e': 26,
-    'c': 21, '!': 1, 'a': 4, 'g': 3, 'i': 10, 'x': 6, 'p': 9, 'k': 8, 'f': 1
+  'Yo': {
+    'u': 53, 'r': 15, 'd': 3, 's': 18, 'o': 2, 'c': 10, 'h': 5, 'n': 22, 'a': 2,
+    'w': 2, 'k': 8, 't': 3, 'p': 1, 'e': 3, 'x': 1, 'b': 1, 'z': 2, 'v': 3,
+    'm': 1, 'q': 1, '!': 1
   },
-  'dp': {'a': 6, 'h': 1, 'r': 1},
-  'dq': {'u': 8},
-  'Dr': {'a': 74, 'e': 67, 'i': 38, 'u': 30, 'y': 9, 'o': 51, 'z': 3, 'd': 1},
-  'dr': {
-    'i': 201, 'e': 147, 'y': 26, 'a': 78, 'u': 32, 'o': 101, 'z': 4, 'g': 1,
-    'n': 1, 'l': 2, '!': 1, 's': 1
+  'ou': {
+    'n': 156, 'g': 200, 's': 275, 'l': 186, 't': 182, 'c': 72, 'r': 323,
+    'd': 96, 'i': 36, 'z': 18, 'x': 30, 'p': 32, '!': 62, 'k': 28, 'a': 14,
+    'm': 18, 'f': 25, 'b': 24, 'q': 5, 'e': 25, 'v': 22, 'y': 12, 'w': 12,
+    'h': 7, 'j': 1, 'o': 2
   },
-  'ds': {
-    '!': 133, 'o': 58, 'e': 29, 'h': 9, 'a': 12, 't': 42, 'm': 9, 'w': 8,
-    'p': 3, 'l': 5, 'b': 9, 'k': 11, 'i': 7, 'd': 2, 'c': 9, 'f': 1, 'g': 1,
-    'u': 1, 'r': 2, 's': 1, 'v': 1
+  'un': {
+    'g': 131, 't': 123, 'n': 101, 'c': 57, 'o': 32, 'd': 314, 'e': 123, 'a': 75,
+    '!': 125, 'l': 21, 'b': 10, 'i': 82, 'h': 5, 'k': 95, 's': 92, 'y': 17,
+    'z': 43, 'r': 4, 'f': 9, 'p': 2, 'm': 8, 'w': 5, 'j': 2, 'q': 1, 'u': 4
   },
-  'Ds': {'o': 1, 'p': 1, 'a': 1},
-  'dt': {
-    '!': 282, 'r': 2, 'k': 12, 's': 4, 'b': 1, 'l': 2, 'o': 1, 'm': 5, 'a': 2,
-    'f': 1, 'h': 5, 'z': 1, 'e': 4, 'n': 1
+  'ng': {
+    '!': 1246, 't': 172, 'h': 126, 's': 181, 'r': 56, 'l': 151, 'u': 49,
+    'e': 859, 'f': 19, 'b': 39, 'o': 109, 'd': 12, 'a': 179, 'm': 26, 'w': 33,
   },
-  'du': {
-    'e': 17, 'f': 11, 'c': 23, 'm': 7, 'x': 3, 'z': 5, 'l': 24, 's': 30, 't': 6,
-    'g': 5, 'j': 3, 'r': 21, 'n': 16, 'k': 6, 'a': 10, 'p': 3, 'y': 3, 'i': 1,
-    '!': 10, 'd': 3, 'h': 1, 'o': 1
+  'He': {
+    'r': 226, 'n': 174, 'a': 85, 's': 43, 'b': 23, 'w': 15, 'l': 138, 'd': 37,
+    'm': 67, 'c': 27, 'i': 168, 'f': 24, 'y': 27, 't': 27, 'p': 19, 'u': 22,
+    'g': 31, '!': 1, 'e': 23, 'v': 10, 'h': 5, 'o': 1, 'j': 2, 'x': 1, 'k': 2,
+    'z': 1, 'q': 1
   },
-  'Du': {
-    'n': 108, 'r': 94, 'd': 26, 'k': 15, 'f': 30, 'b': 57, 'a': 4, 'p': 35,
-    'm': 34, 'g': 20, 'v': 8, 't': 27, 'c': 43, 'o': 3, 'l': 27, 'e': 33,
-    'q': 3, 'h': 9, 's': 32, '!': 1, 'w': 2, 'z': 1, 'x': 2, 'i': 5, 'y': 2
+  'rn': {
+    'a': 190, 'e': 374, 's': 91, 'o': 106, 't': 19, '!': 353, 'i': 137, 'd': 18,
+    'h': 26, 'w': 7, 'b': 47, 'u': 12, 'k': 5, 'l': 10, 'y': 12, 'm': 8, 'q': 3,
+    'r': 3, 'g': 6, 'f': 9, 'c': 3, 'z': 3, 'n': 4, 'p': 2
   },
-  'dv': {'e': 5, 'o': 4, 'i': 13, 'a': 6},
-  'Dv': {'o': 2},
-  'dw': {'a': 32, 'e': 38, 'i': 28, 'o': 9, 'y': 7},
-  'Dw': {'y': 2, 'i': 4, 'o': 4, 'e': 4, 'a': 3},
-  'dy': {
-    '!': 276, 'k': 17, 'a': 5, 'e': 4, 'c': 4, 'n': 4, 's': 7, 'u': 1, 'l': 1,
-    'g': 3, 'v': 2, 'm': 3, 'd': 1, 'b': 1, 'o': 1, 'f': 1
+  'na': {
+    'n': 227, 'l': 131, '!': 613, 'r': 239, 'd': 58, 's': 150, 'p': 30, 'g': 96,
+    'h': 58, 'm': 68, 'i': 31, 't': 104, 'y': 25, 'v': 26, 'u': 101, 'b': 43,
   },
-  'Dy': {
-    'e': 6, 'k': 9, 's': 5, 'c': 6, 'a': 4, '!': 1, 'm': 4, 'n': 2, 'g': 1,
-    'l': 4, 'b': 2, 'd': 3, 'r': 3
+  'an': {
+    'd': 1436, 's': 436, 'c': 402, '!': 3435, 't': 732, 'i': 477, 'e': 531,
+    'k': 253, 'l': 60, 'n': 782, 'a': 411, 'g': 474, 'o': 701, 'f': 59, 'u': 64,
+    'h': 70, 'z': 162, 'b': 57, 'm': 18, 'w': 42, 'j': 17, 'p': 23, 'y': 65,
+    'r': 19, 'v': 39, 'q': 10
   },
-  'Dz': {'i': 13, 'u': 4, 'l': 1, 'w': 1, 'a': 1},
-  'dz': {
-    'i': 45, 'e': 7, '!': 9, 'w': 3, 'y': 3, 'u': 2, 'a': 3, 'o': 1, 'm': 1,
-    'l': 1, 'h': 1, 'k': 2
+  'Ki': {
+    'n': 156, 'm': 48, 'r': 90, 'd': 10, 'l': 96, 's': 45, 't': 45, 'e': 60,
+    'p': 14, 'z': 7, 'b': 10, 'g': 4, 'f': 4, 'k': 4, 'v': 6, 'c': 6, 'j': 3,
+    'a': 3, 'o': 2, 'h': 2, 'y': 2, 'i': 1
   },
-  'Ea': {
-    't': 5, 's': 34, 'r': 32, 'v': 3, 'g': 15, 'd': 8, 'k': 7, 'm': 1, 'n': 3,
-    'l': 5, 'c': 3, 'p': 1, 'y': 1, 'b': 1, 'f': 1
+  'Wr': {'i': 17, 'a': 8, 'e': 8, 'o': 10, 'z': 2, 'y': 4, 'u': 2},
+  'gh': {
+    't': 234, 'e': 83, 'a': 139, 'n': 28, 'l': 23, '!': 360, 's': 8, 'b': 12,
+    'm': 13, 'o': 39, 'r': 17, 'u': 12, 'y': 7, 'f': 2, 'i': 32, 'd': 2, 'h': 1,
+    'v': 1, 'k': 1, 'g': 1
   },
-  'ea': {
-    'v': 72, 'n': 159, 'r': 352, 'l': 134, 't': 174, 's': 131, 'd': 171,
-    'c': 65, '!': 126, 'g': 72, 'u': 361, 'y': 7, 'm': 51, 'k': 54, 'h': 18,
-    'b': 27, 'f': 20, 'i': 6, 'z': 19, 'w': 6, 'p': 10, 'q': 3, 'a': 1, 'x': 1,
-    'j': 1, 'o': 1
+  'ht': {
+    '!': 208, 'e': 79, 'o': 40, 'y': 11, 'f': 3, 'n': 7, 'r': 7, 'a': 25,
+    'i': 18, 'l': 13, 's': 10, 'm': 9, 'b': 3, 'w': 2, 'c': 1, 'h': 9, 'z': 2
   },
-  'eb': {
-    'b': 33, 'e': 276, 's': 21, 'l': 44, 'r': 95, 'v': 1, 'a': 111, 'o': 83,
-    'u': 44, 'y': 18, '!': 38, 'n': 11, 'h': 6, 'k': 4, 'i': 35, 'm': 2, 'w': 1,
-    'd': 3, 'g': 1, 'c': 1
+  'Lo': {
+    'p': 27, 'n': 83, 'w': 38, 'v': 62, 'g': 26, 't': 30, 'z': 17, 'c': 60,
+    'r': 79, 'u': 82, 'o': 25, 'y': 12, 'f': 35, 'm': 33, '!': 1, 'e': 42,
+    'h': 22, 'd': 11, 'l': 11, 'i': 10, 's': 48, 'k': 13, 'b': 30, 'a': 10,
+    'x': 3, 'q': 1, 'j': 1
   },
-  'Eb': {
-    'e': 35, 'y': 1, 'n': 1, 'l': 4, 'r': 5, 'b': 8, 'i': 3, 'a': 5, 's': 1, 
-    'o': 1
+  'op': {
+    'e': 93, '!': 84, 'k': 16, 'p': 134, 'h': 21, 'l': 28, 's': 16, 'o': 55,
+    'm': 6, 'r': 7, 't': 5, 'f': 29, 'w': 3, 'a': 41, 'i': 44, 'c': 4, 'y': 3,
+    'g': 1, 'u': 10, 'n': 3, 'b': 1, 'z': 1
   },
-  'Ec': {'h': 18, 'k': 41, 'c': 2, 't': 2, 'o': 7, 'l': 1},
-  'ec': {
-    'k': 562, 'o': 73, 'e': 55, 't': 17, 'h': 269, 'a': 62, 'l': 17, 'i': 37,
-    'n': 4, 'q': 2, 'c': 44, '!': 81, 'r': 17, 'z': 31, 'u': 15, 's': 2, 'y': 4,
-    'v': 1, 'w': 1, 'm': 1
+  'pe': {
+    'z': 11, 'r': 382, 'n': 128, '!': 160, 'l': 167, 'a': 40, 'd': 12, 's': 43,
+    'e': 22, 'p': 2, 'i': 20, 't': 46, 'w': 3, 'c': 20, 'y': 24, 'o': 1, 'h': 3,
+    'v': 2, 'k': 11, 'j': 3, 'm': 4, 'g': 3
   },
-  'ed': {
-    '!': 137, 'y': 27, 'i': 124, 'e': 306, 'o': 125, 'g': 48, 'a': 127, 'm': 26,
-    'b': 16, 'r': 71, 'f': 11, 's': 24, 'd': 84, 'l': 83, 'h': 9, 'w': 13,
-    'u': 18, 'n': 19, 't': 38, 'z': 12, 'v': 3, 'k': 6, 'c': 4, 'p': 1, 'j': 2, 
-    'q': 1
+  'Hi': {
+    'l': 142, 'c': 31, 'n': 96, 'g': 49, 'r': 43, 't': 24, 'd': 10, 'a': 1,
+    'm': 17, 'b': 20, 'x': 4, 'p': 17, 'e': 22, 'v': 2, 's': 23, 'o': 1, 'z': 2,
+    'k': 2, 'j': 1
   },
-  'Ed': {
-    'w': 5, 'm': 18, 'd': 12, 'g': 20, 'e': 21, 'i': 9, 's': 4, 'n': 4, 'l': 9,
-    'b': 1, 'r': 4, 'u': 2, 'o': 1, 'v': 1, 'h': 1
+  'Sc': {
+    'o': 58, 'h': 1145, 'r': 36, 'a': 120, 'u': 20, 'i': 42, 'l': 2, 'e': 9,
+    'y': 1, 'z': 2, 's': 1
   },
-  'ee': {
-    '!': 437, 'n': 233, 'd': 94, 'm': 53, 'l': 127, 'v': 26, 's': 107, 'r': 125,
-    'k': 61, 't': 100, 'c': 40, 'h': 31, 'b': 38, 'f': 19, 'g': 32, 'p': 22,
-    'z': 11, 'a': 1, 'u': 4, 'w': 3, 'i': 1
+  'co': {
+    't': 91, 'y': 9, 'b': 30, 'r': 93, 'x': 20, 's': 41, 'n': 141, 'c': 57,
+    '!': 376, 'm': 101, 'l': 115, 'e': 17, 'u': 56, 'i': 15, 'o': 12, 'g': 7,
+    'w': 10, 'a': 15, 'f': 11, 'v': 25, 'p': 11, 'd': 3, 'z': 5, 'h': 1
   },
-  'Ee': {'l': 2, 'k': 1, 'd': 1, 'r': 1, '!': 1},
-  'ef': {
-    'f': 162, 'e': 84, 'i': 42, 'n': 6, 'l': 19, 'a': 37, 't': 25, '!': 32,
-    'o': 47, 's': 16, 'k': 10, 'u': 5, 'r': 26, 'c': 5, 'z': 2, 'y': 1
+  'ot': {
+    't': 550, 'o': 116, 'h': 193, 's': 36, 'e': 138, '!': 158, 'y': 6, 'l': 12,
+    'a': 75, 'n': 15, 'c': 11, 'z': 42, 'm': 8, 'w': 7, 'i': 35, 'r': 22,
+    'k': 10, 'v': 1, 'u': 10, 'f': 2, 'b': 2, 'd': 1
   },
-  'Ef': {'i': 1, 'f': 6, 'a': 1, 'u': 1, 'r': 2, 't': 2, 'l': 1},
-  'Eg': {
-    'a': 3, 'g': 18, 'b': 2, 'e': 12, 'u': 4, 'l': 10, 'n': 3, 'o': 2, 'i': 3,
-    'w': 1, 'v': 1
+  'tt': {
+    '!': 906, 'e': 836, 'h': 30, 'l': 127, 'o': 217, 's': 105, 'm': 51, 'y': 51,
+    'a': 230, 'i': 462, 'r': 48, 'n': 26, 'w': 8, 'c': 4, 'u': 18, 'f': 2,
+    'k': 13, 'z': 3, 'g': 6, 'b': 3, 'd': 1, 'j': 1
   },
-  'eg': {
-    'o': 90, 'a': 167, 'g': 77, 'e': 213, 'l': 66, 'u': 51, 'r': 105, 'i': 35,
-    'n': 25, 'h': 17, '!': 31, 'f': 2, 'w': 6, 's': 6, 'm': 16, 't': 3, 'y': 5,
-    'd': 2, 'b': 1
+  'Gr': {
+    'e': 200, 'a': 303, 'i': 169, 'o': 158, 'u': 85, 'y': 6, 'z': 9, 'b': 1,
+    'r': 1, 'h': 1, 'g': 1, 'd': 1
   },
-  'eh': {
-    'e': 55, 'm': 46, 'a': 107, 'l': 143, 'r': 118, 'u': 11, 'o': 49, 'n': 82,
-    't': 8, '!': 48, 'y': 5, 'i': 14, 'k': 2, 'b': 8, 'd': 3, 'g': 2, 'f': 3,
-    's': 6, 'j': 1
+  'Ad': {
+    'a': 34, 'k': 6, 'd': 17, 'c': 2, 'l': 7, 'o': 12, 'r': 8, 'e': 30, 'g': 1,
   },
-  'Eh': {'l': 11, 'r': 19, 'm': 5, 's': 1, 'n': 2, 'e': 1, 'o': 1, 'i': 3},
-  'ei': {
-    'd': 198, 'n': 566, 't': 194, 's': 338, 'l': 135, 'r': 100, 'e': 97,
-    'g': 133, 'b': 69, 'f': 50, 'c': 88, 'm': 141, 'a': 9, 'x': 6, 'j': 4,
-    'v': 6, 'k': 29, '!': 35, 'z': 9, 'p': 16, 'h': 15, 'w': 4, 'o': 4
+  'da': {
+    'm': 69, 'n': 114, '!': 424, 'l': 143, 'r': 90, 'y': 56, 'i': 10, 'c': 22,
+    'd': 14, 'w': 12, 'v': 15, 'z': 8, 'k': 27, 's': 51, 'g': 20, 'u': 18,
+    'h': 51, 'b': 9, 'p': 6, 'f': 6, 'o': 3, 't': 21, 'j': 1, 'e': 3, 'q': 1
   },
-  'Ei': {
-    's': 45, 'd': 9, 'c': 33, 'l': 11, 'n': 6, 'f': 2, 't': 4, 'm': 2, 'g': 4,
-    'k': 6, 'b': 3, 'r': 2, 'e': 1
+  'Ba': {
+    'k': 33, 'i': 66, 'r': 517, 'n': 107, 't': 100, 'l': 248, 's': 124, 'x': 7,
+    'u': 81, 'c': 81, 'e': 18, 'b': 50, 'g': 42, 'p': 5, 'd': 46, 'y': 46,
+    'h': 24, 'z': 24, 'v': 8, 'a': 9, 'm': 20, 'w': 9, '!': 1, 'f': 5, 'o': 1,
+    'q': 4, 'j': 7
   },
-  'Ej': {'i': 1},
-  'ej': {
-    'i': 3, 'e': 20, 'o': 45, 'a': 52, '!': 7, 'c': 9, 's': 4, 'u': 4, 'k': 10,
-    'n': 2, 'm': 3, 'j': 1, 'b': 1, 'l': 1, 't': 1, 'g': 1
+  'ak': {
+    'e': 280, '!': 481, 'l': 32, 'a': 113, 's': 24, 'i': 103, 'k': 16, 'n': 5,
+    'o': 84, 'u': 30, 'm': 3, 'r': 7, 't': 1, 'f': 1, 'h': 13, 'd': 3, 'j': 2,
+    'y': 8, 'b': 1
   },
-  'Ek': {
-    'l': 2, 's': 4, '!': 1, 'b': 1, 'k': 1, 'd': 1, 'h': 2, 'm': 2, 'i': 3,
-    'w': 1, 'e': 2, 'a': 1
+  'Go': {
+    'n': 56, 'm': 19, 'r': 89, 'o': 102, 'l': 146, 'u': 48, 'f': 11, 's': 50,
+    'd': 47, 'i': 10, 'e': 63, 'a': 8, 'b': 18, 'w': 15, 't': 42, 'v': 13,
+    'y': 10, 'g': 12, 'k': 1, 'z': 3, 'c': 13, '!': 1, 'h': 6, 'p': 3, 'j': 2
   },
-  'ek': {
-    's': 23, '!': 546, 'e': 120, 'l': 9, 'm': 7, 'i': 28, 'k': 5, 'n': 2,
-    'a': 43, 'h': 9, 'u': 13, 'o': 15, 'r': 6, 'b': 3, 'z': 1, 't': 2, 'w': 1,
-    'y': 1, 'f': 1
+  'nz': {
+    'a': 109, 'i': 93, 'u': 11, '!': 89, 'o': 70, 'e': 112, 'y': 8, 'w': 1,
+    'm': 9, 'l': 14, 'k': 2, 'h': 1, 's': 1, 'v': 1
   },
-  'El': {
-    'l': 90, 'd': 14, 'm': 11, 'k': 10, 'i': 31, 'a': 6, 'y': 1, 'r': 5,
-    's': 29, 'w': 8, 'e': 15, 'g': 9, 'b': 10, 't': 5, 'z': 5, 'v': 8, 'f': 8,
-    '!': 1, 'c': 2, 'h': 6, 'o': 2, 'u': 1, 'p': 1, 'n': 1, 'q': 1
+  'za': {
+    'l': 50, '!': 230, 'r': 150, 'n': 89, 'd': 20, 'k': 72, 's': 11, 'b': 14,
+    'g': 14, 'w': 5, 'j': 4, 'm': 8, 'p': 9, 't': 14, 'i': 7, 'o': 1, 'c': 9,
+    'f': 9, 'h': 6, 'q': 2, 'y': 4, 'v': 2, 'u': 1, 'z': 2, 'e': 1
+  },
+  'Ne': {
+    'l': 23, 'a': 29, 'w': 76, 'e': 30, 'f': 2, 'g': 15, 's': 35, 'u': 45,
+    't': 30, 'i': 59, 'v': 32, 'm': 19, 'c': 4, 'z': 3, 'r': 18, 'y': 9, 'h': 7,
+    'b': 11, 'd': 14, 'p': 4, 'n': 4, 'j': 3, 'k': 1, 'o': 1
   },
   'el': {
     's': 272, 'l': 2451, 'd': 435, 'e': 344, 'c': 59, 't': 195, '!': 1421,
     'g': 55, 'a': 345, 'p': 34, 'i': 304, 'm': 221, 'y': 86, 'r': 30, 'f': 67,
     'v': 52, 'o': 208, 'b': 106, 'u': 47, 'k': 93, 'h': 48, 'w': 15, 'n': 24,
     'z': 36, 'q': 4, 'j': 4
   },
-  'em': {
-    'a': 460, 'i': 121, 'p': 97, 'o': 135, 'e': 219, 'b': 83, 's': 40, 'u': 28,
-    'm': 128, '!': 123, 'k': 16, 'l': 19, 'y': 13, 'n': 6, 'w': 1, 'c': 7,
-    'r': 11, 'h': 3, 'z': 2, 'f': 2, 'j': 1
-  },
-  'Em': {
-    'e': 12, 'm': 18, 'a': 9, 'b': 18, 'o': 6, 'r': 3, 'i': 9, 'p': 7, 'l': 5,
-    's': 5, 'f': 2, '!': 1, 'c': 1, 'h': 1, 'g': 1, 'k': 1, 'z': 1, 'd': 2, 
-    'u': 1
-  },
-  'en': {
-    '!': 2387, 'n': 411, 'd': 493, 'k': 145, 's': 573, 'r': 63, 'c': 164,
-    't': 570, 'e': 414, 'o': 185, 'a': 299, 'z': 173, 'p': 12, 'j': 12, 'w': 50,
-    'l': 35, 'b': 517, 'i': 234, 'g': 202, 'y': 40, 'f': 76, 'h': 160, 'm': 44,
-    'u': 27, 'q': 5, 'v': 6
-  },
-  'En': {
-    'g': 77, 'r': 7, 'n': 12, 'o': 9, 'd': 24, 'l': 2, 'c': 9, 's': 15, 't': 16,
-    'y': 2, 'f': 3, 'z': 3, 'b': 1, 'm': 2, 'i': 3, 'e': 1, 'a': 2, 'w': 2, 
-    'k': 2
+  'Ca': {
+    'r': 474, 'm': 129, 's': 278, 'l': 199, 'n': 181, 'i': 28, 'b': 60, 't': 87,
+    'p': 121, 'u': 34, 'h': 13, 'v': 52, 'g': 12, 'd': 39, 'z': 11, 'e': 3,
+    'w': 8, 'o': 5, 'c': 22, 'f': 17, 'y': 15, 'j': 7, 'q': 1, 'a': 2, 'k': 3
   },
-  'Eo': {'f': 1, 'n': 1, 'v': 1},
-  'eo': {
-    'r': 24, 'n': 86, 'd': 10, 'p': 8, 'i': 2, 'l': 14, '!': 93, 'w': 2, 'u': 8,
-    's': 4, 'b': 2, 'm': 9, 'g': 5, 't': 8, 'c': 2, 'f': 5, 'z': 2, 'h': 4,
-    'v': 2, 'j': 1, 'k': 1, 'a': 1
+  'tc': {
+    'h': 318, 'a': 9, 'l': 7, 'o': 8, 'y': 1, 'z': 5, 'i': 3, 'r': 5, 'u': 1,
+    's': 1, 'e': 1, '!': 1
   },
-  'ep': {
-    'h': 40, 'p': 137, 'a': 52, 'e': 68, '!': 31, 'u': 11, 'c': 3, 'l': 25,
-    'r': 16, 'i': 32, 's': 15, 'o': 19, 'b': 2, 'n': 9, 'k': 23, 'w': 1,
-    't': 12, 'y': 3, 'f': 18, 'v': 1
+  'ch': {
+    'e': 1108, 'a': 539, 'o': 336, 'm': 202, '!': 1325, 'u': 196, 'n': 134,
+    'w': 147, 'r': 117, 'i': 506, 't': 174, 'c': 8, 's': 54, 'f': 24, 'k': 52,
   },
-  'Ep': {'p': 19, 's': 2, 'l': 4, 't': 1, 'h': 2, 'o': 1, 'e': 2, 'i': 1},
-  'eq': {'u': 28},
-  'Eq': {'u': 4},
-  'er': {
-    '!': 8545, 's': 1089, 'n': 399, 'e': 424, 't': 869, 'a': 426, 'r': 660,
-    'g': 740, 'k': 187, 'c': 123, 'y': 169, 'o': 410, 'm': 467, 'w': 69,
-    'd': 187, 'v': 99, 'i': 499, 'f': 84, 'l': 385, 'b': 230, 'z': 56, 'h': 129,
-    'u': 55, 'p': 35, 'q': 7, 'j': 12, 'x': 1
+  'he': {
+    'l': 334, 'z': 12, 's': 113, 'r': 935, 'n': 270, 'w': 40, 'e': 111, 'p': 29,
+    'a': 152, 'c': 32, 'f': 26, 'y': 75, 't': 116, '!': 199, 'u': 38, 'o': 15,
+    'v': 28, 'm': 51, 'i': 171, 'x': 1, 'd': 20, 'h': 12, 'g': 8, 'b': 12,
+    'k': 28, 'j': 1
   },
-  'Er': {
-    'i': 21, 'v': 5, 'w': 2, 'n': 13, 'd': 9, 's': 6, 'b': 10, 'l': 11, 't': 8,
-    'a': 6, 'h': 4, 'r': 4, 'x': 1, 'p': 4, 'k': 4, 'e': 6, 'c': 8, 'o': 5,
-    'm': 7, 'z': 1, 'g': 1, 'f': 1
+  'Pe': {
+    'r': 234, 't': 189, 'a': 57, 'n': 139, 'c': 42, 'o': 3, 'l': 86, 'p': 20,
+    'd': 40, 'm': 7, 'e': 29, 'y': 5, 'g': 10, 's': 43, 'i': 15, 'w': 3, 'h': 6,
+    'k': 6, 'f': 7, 'v': 9, 'b': 4, 'u': 1, 'z': 11, 'q': 2, 'x': 2
   },
-  'es': {
-    '!': 1688, 't': 470, 's': 533, 'e': 296, 'p': 53, 'u': 16, 'l': 79,
-    'c': 167, 'b': 37, 'o': 128, 'q': 9, 'h': 108, 'm': 47, 'i': 123, 'a': 91,
-    'j': 4, 'r': 10, 'd': 8, 'n': 59, 'k': 117, 'w': 14, 'g': 8, 'f': 6,
-    'z': 19, 'v': 5, 'y': 8
+  'be': {
+    'r': 1372, 'l': 230, 's': 42, 't': 52, '!': 142, 'd': 17, 'e': 78, 'c': 114,
+    'y': 39, 'a': 59, 'n': 141, 'i': 40, 'z': 7, 'v': 2, 'k': 25, 'b': 3,
+    'q': 1, 'h': 6, 'g': 2, 'm': 1, 'o': 5, 'u': 2, 'j': 1
   },
-  'Es': {
-    't': 58, 'p': 45, 'c': 50, 'q': 14, 'k': 17, 's': 24, 'h': 8, 'l': 4,
-    'a': 4, 'm': 6, 'g': 1, 'e': 2, 'w': 1, 'b': 3, 'f': 1, 'o': 1, 'n': 1
+  'ts': {
+    '!': 280, 'o': 83, 'c': 111, 't': 14, 'f': 3, 'e': 53, 'm': 17, 'h': 15,
+    'u': 41, 'i': 24, 'b': 7, 'w': 6, 'l': 9, 'k': 36, 's': 1, 'p': 1, 'y': 3,
+    'a': 11, 'd': 2, 'g': 2, 'z': 1
   },
-  'et': {
-    'e': 174, 't': 1287, 'c': 41, 'o': 111, '!': 370, 'i': 58, 'z': 172,
-    's': 103, 'a': 103, 'r': 150, 'h': 225, 'l': 41, 'm': 10, 'w': 6, 'f': 2,
-    'n': 3, 'j': 7, 'k': 16, 'u': 9, 'g': 5, 'y': 9, 'b': 3, 'd': 1, 'p': 2
+  'Tu': {
+    'r': 110, 'c': 19, 't': 20, 'b': 12, 'g': 7, 'd': 6, 'l': 19, 'n': 18,
+    '!': 1, 'p': 9, 'f': 9, 's': 9, 'm': 19, 'o': 6, 'e': 8, 'i': 4, 'a': 5,
+    'k': 3, 'x': 2, 'h': 1, 'z': 3, 'y': 1, 'u': 1, 'j': 1
   },
-  'Et': {
-    'h': 10, 't': 8, 'i': 2, 'z': 3, 'c': 4, 's': 1, 'l': 1, 'k': 1, 'u': 1,
-    'r': 1, 'o': 1
+  'ur': {
+    'n': 232, 'p': 22, 'r': 174, 't': 159, 'k': 99, 'g': 246, 'a': 190,
+    'e': 208, 's': 106, 'h': 6, 'c': 71, 'l': 87, '!': 178, 'm': 34, 'd': 82,
+    'i': 179, 'v': 16, 'b': 53, 'y': 100, 'q': 2, 'o': 73, 'f': 19, 'w': 13,
+    'u': 18, 'z': 21, 'j': 3
   },
-  'eu': {
-    '!': 41, 'm': 18, 'x': 20, 'r': 63, 'n': 27, 't': 44, 'f': 11, 'b': 21,
-    'e': 33, 'v': 11, 's': 51, 'd': 16, 'i': 10, 'l': 20, 'h': 6, 'c': 13,
-    'g': 8, 'z': 5, 'w': 7, 'k': 6, 'a': 10, 'p': 6, 'y': 2, 'j': 1
+  'Ph': {'i': 60, 'e': 19, 'a': 29, 'o': 16, 'u': 6, 'y': 3, 'l': 2, 'r': 1},
+  'ip': {
+    's': 35, '!': 50, 't': 11, 'p': 205, 'e': 43, 'l': 18, 'm': 4, 'k': 17,
   },
-  'Eu': {
-    'b': 3, 'd': 1, 'g': 3, 'r': 7, 's': 6, 'l': 2, 't': 3, 'e': 2, 'n': 2, 
-    'v': 1
+  'pb': {'e': 5, 'u': 1, 'a': 2, 'l': 1},
+  'Pa': {
+    'r': 228, 't': 103, 'l': 150, 'y': 31, 'g': 36, 'u': 51, 'd': 40, 'c': 57,
+    'i': 22, 'q': 3, 'x': 4, 'p': 58, 'z': 7, 'n': 130, 'k': 5, 's': 120,
+    'b': 7, 'e': 7, 'w': 17, 'o': 14, 'v': 45, 'h': 7, 'm': 8, 'f': 5, 'j': 3,
+    'a': 8, '!': 1
   },
   'Ev': {'a': 22, 'e': 52, 'i': 8, 'o': 4, 'j': 1},
-  'ev': {
-    'e': 325, 'i': 183, 'y': 7, 'a': 116, 'o': 43, 'l': 7, 'r': 14, '!': 11,
-    's': 7, 'c': 1, 'w': 2, 'n': 2, 'u': 1, 't': 1, 'k': 1, 'j': 1
-  },
-  'ew': {
-    'i': 134, 'a': 94, 's': 135, 'e': 107, 'm': 10, 't': 6, '!': 110, 'c': 10,
-    'b': 24, 'k': 4, 'o': 27, 'h': 12, 'p': 2, 'l': 10, 'n': 6, 'r': 4, 'q': 1,
-    'y': 7, 'f': 1, 'v': 1, 'g': 3, 'd': 1, 'u': 1
-  },
-  'Ew': {'i': 4, 'e': 7, 'a': 5, 'b': 1, 't': 1, 'y': 1, 'o': 1},
-  'ex': {
-    'a': 15, 't': 9, '!': 20, 'n': 2, 'l': 3, 'i': 10, 'e': 8, 'f': 1, 'r': 3,
-    's': 2, 'o': 1, 'h': 1, 'y': 2, 'w': 1, 'z': 1
-  },
-  'Ex': {
-    'u': 1, 'l': 3, 'n': 1, 'c': 1, 'f': 1, 'e': 2, 'o': 1, 'i': 1, 't': 2,
-    'a': 1, 'p': 1
-  },
-  'ey': {
-    '!': 2293, 'n': 36, 'e': 173, 'm': 23, 's': 21, 'c': 6, 'v': 3, 't': 12,
-    'w': 6, 'o': 10, 'a': 25, 'b': 7, 'r': 16, 'h': 9, 'l': 18, 'f': 8, 'd': 21,
-    'p': 2, 'i': 1, 'u': 1, 'k': 5, 'g': 1, 'z': 1
+  'va': {
+    'n': 219, 'r': 125, '!': 112, 'l': 126, 'g': 27, 's': 40, 'k': 13, 'z': 8,
+    't': 52, 'y': 12, 'c': 25, 'e': 3, 'd': 17, 'i': 23, 'j': 1, 'u': 9, 'o': 3,
+    'm': 2, 'a': 4, 'b': 1, 'v': 1, 'h': 2, 'p': 1
   },
-  'Ey': {
-    'r': 2, 'l': 3, 'e': 5, 'm': 1, 'n': 1, 't': 3, 's': 1, 'c': 1, 'u': 1
+  'Ed': {
+    'w': 5, 'm': 18, 'd': 12, 'g': 20, 'e': 21, 'i': 9, 's': 4, 'n': 4, 'l': 9,
+    'b': 1, 'r': 4, 'u': 2, 'o': 1, 'v': 1, 'h': 1
   },
-  'ez': {
-    '!': 378, 'a': 47, 'm': 1, 'e': 43, 'q': 2, 'i': 25, 'c': 2, 'u': 2,
-    'o': 12, 'z': 30, 'y': 2, 'n': 10, 'g': 3, 'r': 2, 'd': 1, 'l': 2, 's': 1,
-    'k': 1, 'w': 1
+  'dw': {'a': 32, 'e': 38, 'i': 28, 'o': 9, 'y': 7},
+  'wa': {
+    'r': 157, 'n': 118, 'y': 132, 'i': 40, 'k': 12, 'l': 156, 'b': 11, 'f': 1,
+    't': 53, '!': 77, 'd': 18, 'x': 2, 's': 22, 'c': 13, 'm': 11, 'g': 18,
+    'p': 2, 'a': 3, 'j': 2, 'h': 7, 'o': 1, 'u': 1, 'v': 1, 'e': 2, 'z': 1
   },
-  'Ez': {'e': 6, 'z': 3, 'a': 1, 'p': 2, 'd': 1},
-  'Fa': {
-    'r': 128, 'u': 62, 'i': 49, 'g': 25, 'y': 10, 'l': 88, 'n': 48, 'j': 2,
-    'b': 28, 'h': 21, 'w': 8, 'v': 25, 'z': 11, 's': 29, 'c': 14, 'd': 12,
-    'm': 10, 'a': 2, 't': 16, 'e': 5, 'k': 3, 'f': 2, 'x': 1
+  'rd': {
+    's': 50, '!': 908, 'a': 112, 'o': 170, 'n': 21, 'y': 33, 'i': 246, 'e': 226,
+    'u': 38, 'w': 14, 'm': 16, 't': 75, 'h': 4, 'l': 27, 'c': 1, 'r': 10,
+    'q': 1, 'b': 2, 'g': 9, 'z': 3, 'v': 1, 'd': 1
   },
-  'fa': {
-    'r': 55, 'd': 5, 'l': 40, 'f': 2, 'n': 74, 'c': 8, 't': 14, 'v': 9, 'y': 7,
-    'z': 2, '!': 24, 'u': 11, 'x': 3, 'e': 2, 'k': 1, 'm': 3, 'i': 14, 's': 6,
-    'w': 1, 'g': 7, 'h': 11, 'b': 5, 'a': 1
+  'ds': {
+    '!': 133, 'o': 58, 'e': 29, 'h': 9, 'a': 12, 't': 42, 'm': 9, 'w': 8,
+    'p': 3, 'l': 5, 'b': 9, 'k': 11, 'i': 7, 'd': 2, 'c': 9, 'f': 1, 'g': 1,
+    'u': 1, 'r': 2, 's': 1, 'v': 1
   },
-  'fb': {'a': 1, 'o': 2},
-  'fc': {'o': 4, 'h': 2, 'a': 1, 'i': 1},
-  'fd': {'e': 2},
-  'fe': {
-    '!': 76, 'r': 321, 'y': 30, 't': 17, 'i': 13, 'e': 33, 'n': 70, 'b': 5,
-    'l': 210, 'v': 6, 'f': 3, 's': 6, 'o': 4, 'w': 2, 'a': 5, 'u': 2, 'c': 3,
-    'k': 3, 'g': 2, 'd': 3, 'm': 3, 'h': 2
+  'Co': {
+    'l': 228, 'o': 70, 'x': 7, 'h': 17, 'n': 234, 'b': 32, 'p': 46, 'r': 283,
+    'c': 53, 'm': 77, 'f': 20, 't': 53, 'w': 34, 'v': 35, 's': 79, 'u': 111,
+    'k': 8, 'a': 27, 'd': 19, 'y': 12, 'e': 6, 'g': 19, 'z': 13, 'i': 8, '!': 1
   },
-  'Fe': {
-    'r': 164, 'l': 94, 'n': 58, 'e': 24, 'a': 33, 't': 22, 'd': 36, 'c': 11,
-    'i': 40, 'w': 3, 'y': 5, 's': 18, 'h': 14, 'b': 7, 'u': 10, 'g': 11, 'k': 2,
-    'o': 2, 'm': 5, 'j': 1, 'v': 2, 'q': 1, 'f': 1
+  'ol': {
+    'l': 574, 'e': 294, 'd': 327, 'm': 77, 's': 121, 't': 171, 'f': 94,
+    'o': 203, 'i': 363, 'p': 43, 'a': 387, 'c': 31, 'k': 55, 'b': 49, 'v': 21,
+    '!': 117, 'n': 22, 'w': 8, 'g': 18, 'z': 68, 'u': 28, 'q': 3, 'r': 2,
+    'y': 23, 'h': 12, 'j': 3
   },
-  'ff': {
-    'i': 95, 'm': 19, 'e': 288, '!': 452, 'o': 60, 'y': 11, 'r': 44, 'n': 20,
-    'l': 53, 'c': 2, 'a': 43, 'u': 7, 't': 13, 's': 17, 'k': 4, 'p': 2, 'h': 2, 
-    'z': 1
+  'St': {
+    'e': 401, 'o': 290, 'a': 458, 'r': 347, 'u': 145, 'i': 167, 'j': 8, 'c': 6,
+    'p': 5, 'y': 11, 'g': 5, 'l': 5, 'h': 3, 'm': 4, 't': 1, 'w': 2, 'f': 4,
+    'd': 2, 's': 1, 'v': 3
   },
-  'fg': {'a': 1, 'r': 4, 'o': 1, 'u': 1, 'e': 1},
-  'fh': {'i': 3, 'a': 2, 'o': 2, 'e': 1},
-  'fi': {
-    'n': 94, 't': 21, 'e': 235, 's': 12, 'l': 28, '!': 29, 'r': 4, 'g': 8,
-    'o': 8, 'c': 12, 'b': 2, 'd': 5, 'a': 12, 'u': 1, 'h': 1, 'q': 1, 'k': 1,
-    'p': 1, 'f': 1
+  'Sa': {
+    'n': 297, 'l': 220, 'u': 63, 'w': 26, 'v': 59, 'm': 93, 'r': 130, 'd': 34,
+    'e': 21, 'p': 17, 'y': 28, 't': 38, 'a': 19, 'g': 33, 'x': 10, 's': 23,
+    'b': 59, 'c': 32, 'i': 34, 'f': 20, 'o': 2, 'k': 29, 'h': 16, '!': 1,
+    'j': 5, 'z': 1
   },
-  'Fi': {
-    's': 43, 'e': 40, 't': 41, 'g': 32, 'n': 99, 'o': 23, 'f': 3, 'k': 2,
-    'x': 3, 'l': 78, 'd': 9, 'c': 26, 'r': 19, 'a': 9, 'z': 1, 'q': 1, 'm': 2,
-    'v': 2, 'u': 3, 'j': 2, 'p': 1, 'w': 1
+  'nc': {
+    'h': 189, 'e': 240, 'a': 90, 'i': 141, 'o': 90, '!': 11, 'l': 19, 'y': 21,
+    'u': 13, 'k': 65, 'r': 14, 't': 3, 'z': 18, 's': 2, 'n': 1
   },
-  'Fj': {'e': 3},
-  'fj': {'o': 1},
-  'fk': {'o': 6, 'i': 4, 'a': 11, 'e': 7, 'n': 1},
-  'fl': {'e': 96, 'i': 30, 'a': 18, 'o': 14, 'u': 12, '!': 5, 'y': 2},
-  'Fl': {'o': 72, 'e': 84, 'y': 7, 'a': 76, 'i': 36, 'u': 27},
-  'fm': {'a': 35, 'e': 3},
-  'fn': {'e': 33, 'a': 4, 'i': 1},
-  'fo': {
-    'r': 345, 'o': 17, 'n': 41, 'y': 6, 'u': 13, '!': 32, 'l': 20, 'x': 3,
-    's': 11, 'e': 4, 'h': 1, 'g': 1, 't': 1, 'i': 2, 'a': 1
+  'og': {
+    'e': 78, 'a': 75, 'g': 69, 'u': 34, 't': 6, '!': 28, 'l': 46, 's': 15,
+    'd': 15, 'n': 24, 'b': 4, 'h': 21, 'o': 26, 'm': 3, 'r': 12, 'i': 22,
+    'y': 4, 'w': 1
   },
-  'Fo': {
-    's': 33, 'r': 167, 'x': 8, 'w': 11, 'l': 44, 'n': 49, 'u': 42, 'o': 12,
-    'g': 20, 'y': 3, 't': 6, 'd': 9, 'b': 2, 'm': 1, 'c': 4, 'e': 9, 'a': 2,
-    'i': 4, 'p': 2, 'k': 2, 'h': 2
+  'ge': {
+    'r': 1307, '!': 482, 's': 101, 'e': 23, 'n': 280, 'l': 279, 't': 78,
+    'o': 30, 'w': 6, 'h': 5, 'p': 2, 'm': 48, 'z': 3, 'v': 6, 'a': 27, 'y': 20,
+    'd': 8, 'b': 13, 'f': 5, 'c': 4, 'i': 3, 'g': 1, 'u': 3
   },
-  'fp': {'a': 2},
-  'fq': {'u': 1},
-  'Fr': {'e': 183, 'a': 200, 'o': 61, 'y': 17, 'i': 140, 'u': 26},
-  'fr': {'e': 62, 'i': 38, 'o': 28, 'a': 54, 'u': 1, 'y': 4},
-  'fs': {
-    'o': 15, 't': 21, 'i': 2, '!': 13, 'k': 19, 'n': 2, 'c': 3, 'u': 1, 'e': 9,
-    'r': 1, 'h': 3, 'a': 2, 'b': 1
+  'Re': {
+    'e': 39, 'y': 28, 'i': 187, 'd': 84, 'a': 71, 'g': 38, 'c': 36, 'n': 102,
+    'u': 23, 'm': 49, 's': 42, 'x': 7, 'b': 25, 'v': 32, 'p': 26, 'h': 35,
   },
-  'ft': {
-    '!': 97, 'o': 19, 'i': 9, 'u': 1, 'w': 1, 's': 8, 'e': 17, 'h': 5, 'y': 3,
-    'z': 3, 'r': 1, 'm': 2, 'l': 2, 'a': 4, 'g': 1
+  'ed': {
+    '!': 137, 'y': 27, 'i': 124, 'e': 306, 'o': 125, 'g': 48, 'a': 127, 'm': 26,
+    'b': 16, 'r': 71, 'f': 11, 's': 24, 'd': 84, 'l': 83, 'h': 9, 'w': 13,
   },
-  'Fu': {
-    'l': 51, 'e': 22, 'n': 27, 'g': 15, 'r': 68, 'c': 5, 'q': 2, 's': 24,
-    'h': 8, 't': 6, 'd': 5, 'j': 11, '!': 1, 'k': 8, 'o': 1, 'm': 2, 'a': 1, 
-    'p': 1
+  'ok': {
+    '!': 100, 's': 44, 'e': 84, 'i': 25, 'o': 33, 'a': 55, 'm': 6, 'l': 10,
+    'k': 12, 'u': 18, 'h': 7, 'r': 4, 'y': 2, 'f': 2, 'w': 3, 'b': 2, 't': 1
   },
-  'fu': {
-    's': 31, 'e': 10, 't': 8, 'm': 1, 'r': 11, 'c': 1, 'l': 5, 'n': 4, 'h': 2,
-    'k': 1, 'a': 1, 'z': 1
+  'rg': {
+    'a': 120, 'u': 54, 'e': 445, '!': 521, 'r': 32, 'o': 53, 'm': 11, 'i': 77,
   },
-  'Fv': {'e': 1},
-  'fv': {'i': 1, 'e': 1},
-  'fw': {'e': 1, 'a': 1},
-  'fy': {'!': 17},
-  'Fy': {'e': 1, 'f': 2, 'o': 1, 'k': 3, 'a': 1, 'l': 3, 'd': 1},
-  'fz': {'i': 4, 'a': 1, '!': 1, 'g': 1},
   'ga': {
     'n': 329, 's': 86, 'd': 23, '!': 221, 'y': 11, 't': 56, 'l': 108, 'r': 254,
     'h': 9, 'm': 33, 'a': 22, 'u': 11, 'w': 15, 'c': 14, 'o': 6, 'v': 5,
     'i': 12, 'e': 4, 'z': 6, 'b': 9, 'k': 4, 'j': 2, 'f': 7, 'g': 3
   },
-  'Ga': {
-    'r': 241, 't': 49, 'l': 216, 'i': 29, 'y': 25, 'm': 55, 'g': 21, 's': 63,
-    'b': 46, 'u': 66, 'n': 93, 'v': 25, 'f': 8, 'd': 27, 'o': 2, 'z': 14,
-    'e': 15, 'h': 8, 'j': 6, 'w': 11, 'x': 1, 'a': 4, 'p': 4, 'c': 10
-  },
-  'gb': {
-    'l': 6, 'y': 8, 'e': 26, 'u': 7, 'o': 10, 'a': 7, 'i': 7, 'r': 2, 'h': 1
-  },
-  'Gb': {'u': 1},
-  'gc': {'h': 2, 'o': 9, 'k': 1, 'a': 2, 'l': 1},
-  'gd': {'e': 9, 'o': 19, 'a': 21, 'i': 2, '!': 2, 'y': 1, 's': 1},
-  'Gd': {'o': 1, 'u': 1},
-  'Ge': {
-    'o': 24, 'n': 86, 'e': 15, 'i': 32, 'r': 159, 'a': 21, 't': 31, 'y': 4,
-    'l': 41, 'h': 26, 'b': 12, 'd': 12, 's': 20, 'm': 15, 'p': 4, 'u': 3,
-    'g': 1, 'f': 6, 'v': 5, 'k': 1, 'c': 4, 'z': 1, 'w': 2
-  },
-  'ge': {
-    'r': 1307, '!': 482, 's': 101, 'e': 23, 'n': 280, 'l': 279, 't': 78,
-    'o': 30, 'w': 6, 'h': 5, 'p': 2, 'm': 48, 'z': 3, 'v': 6, 'a': 27, 'y': 20,
-    'd': 8, 'b': 13, 'f': 5, 'c': 4, 'i': 3, 'g': 1, 'u': 3
-  },
-  'Gf': {'e': 1, 'r': 1},
-  'gf': {'o': 9, 'i': 12, 'a': 2, 'e': 7, 'r': 3},
-  'gg': {
-    'i': 114, 's': 48, '!': 77, 'e': 167, 'o': 13, 'l': 22, 'a': 47, 'r': 2,
-    'h': 3, 'm': 2, 'n': 1, 'u': 3, 'b': 1, 'y': 5
-  },
-  'Gh': {'o': 8, 'e': 14, 'i': 8, 'a': 13, 'r': 2},
-  'gh': {
-    't': 234, 'e': 83, 'a': 139, 'n': 28, 'l': 23, '!': 360, 's': 8, 'b': 12,
-    'm': 13, 'o': 39, 'r': 17, 'u': 12, 'y': 7, 'f': 2, 'i': 32, 'd': 2, 'h': 1,
-    'v': 1, 'k': 1, 'g': 1
+  'Be': {
+    'l': 216, 'n': 241, 'r': 373, 'c': 70, 'a': 135, 's': 59, 't': 76, 'g': 22,
+    'e': 62, 'y': 22, 'v': 28, 'h': 42, 'd': 51, 'm': 15, 'j': 9, 'w': 4,
+    'i': 41, 'z': 9, 'q': 2, 'u': 23, 'b': 6, 'k': 9, 'f': 2, 'x': 1, 'o': 1,
+    'p': 1, '!': 1
   },
-  'Gi': {
-    'b': 25, 'l': 153, 'v': 7, 'p': 5, 'f': 7, 'r': 45, 'o': 26, 's': 14,
-    'n': 39, 'd': 10, 'e': 43, 'g': 12, 't': 20, 'a': 76, 'u': 12, 'm': 8,
-    'z': 4, 'c': 4, 'h': 1
+  'Mu': {
+    'r': 100, 'n': 102, 'l': 98, 'e': 19, 's': 92, 'i': 7, 'h': 14, 'd': 10,
+    'm': 13, 't': 24, 'c': 26, 'f': 4, 'k': 3, 'j': 2, '!': 1, 'z': 9, 'g': 9,
+    'o': 1, 'y': 3, 'w': 1, 'p': 1
   },
-  'gi': {
-    'n': 162, 'l': 57, 's': 34, 'e': 63, 'o': 64, 'a': 55, 'b': 8, 'r': 11,
-    '!': 42, 't': 13, 'u': 7, 'v': 7, 'f': 1, 'd': 5, 'c': 6, 'm': 7, 'y': 1,
-    'k': 1, 'z': 1, 'h': 1
+  'rp': {
+    'h': 18, 'e': 49, '!': 26, 'i': 36, 'o': 23, 'u': 4, 'l': 10, 'a': 15,
+    's': 12, 't': 1, 'r': 5, 'y': 2, 'f': 2, 'n': 1, 'm': 1, 'k': 3
   },
-  'gj': {'e': 1},
-  'Gj': {'e': 6, 'o': 2},
-  'gk': {'i': 5, 'h': 5, 'a': 1, '!': 3, 'n': 1},
-  'gl': {
-    'a': 54, 'e': 343, 'i': 190, 'y': 6, 'o': 35, 'u': 16, '!': 12, 'm': 1,
-    't': 1, 's': 1
+  'ph': {
+    'y': 14, 'e': 71, '!': 37, 'r': 14, 'i': 29, 'a': 55, 's': 8, 'u': 7,
+    'o': 23, 'l': 1, 'f': 1, 'c': 1, 'p': 1, 't': 1
   },
-  'Gl': {'o': 44, 'e': 34, 'a': 104, 'y': 3, 'i': 23, 'u': 13},
-  'gm': {'a': 72, 'o': 12, 'i': 7, 'u': 2, 'e': 6, '!': 1, 'y': 2},
-  'Gm': {'e': 1},
-  'gn': {'e': 103, 'o': 80, 'u': 5, 'y': 5, 'a': 83, 'i': 39, '!': 4, 's': 2},
-  'Gn': {'e': 3, 'i': 1, 'a': 5, 'o': 1},
-  'go': {
-    'm': 7, 'r': 56, '!': 182, 's': 48, 'w': 20, 'n': 79, 'v': 9, 'o': 41,
-    'z': 10, 'u': 17, 'i': 6, 'l': 41, 't': 20, 'p': 3, 'y': 7, 'e': 5, 'd': 13,
-    'a': 5, 'f': 5, 'j': 1, 'c': 6, 'b': 4, 'h': 1
+  'hy': {
+    '!': 91, 't': 3, 'n': 10, 'm': 9, 's': 4, 'g': 1, 'd': 2, 'a': 8, 'b': 3,
+    'r': 2, 'f': 3, 'w': 1, 'e': 2, 'u': 1, 'o': 2, 'l': 1, 'k': 1
   },
-  'Go': {
-    'n': 56, 'm': 19, 'r': 89, 'o': 102, 'l': 146, 'u': 48, 'f': 11, 's': 50,
-    'd': 47, 'i': 10, 'e': 63, 'a': 8, 'b': 18, 'w': 15, 't': 42, 'v': 13,
-    'y': 10, 'g': 12, 'k': 1, 'z': 3, 'c': 13, '!': 1, 'h': 6, 'p': 3, 'j': 2
+  'ai': {
+    'l': 154, 'g': 55, 'r': 165, 'n': 364, 's': 127, 'd': 48, 't': 103, 'e': 28,
+    '!': 80, 'm': 36, 'z': 23, 'b': 18, 'f': 8, 'v': 9, 'o': 19, 'k': 15,
+    'c': 20, 'a': 26, 'w': 2, 'p': 2, 'h': 1, 'x': 3, 'u': 1, 'y': 1
   },
-  'gp': {'e': 2, 'u': 2, 'h': 1, 'i': 1, 'r': 1, 'a': 2},
-  'gq': {'u': 6},
-  'gr': {'a': 136, 'o': 90, 'e': 135, 'i': 42, 'u': 12, 'z': 1, 'y': 3, 't': 1},
-  'Gr': {
-    'e': 200, 'a': 303, 'i': 169, 'o': 158, 'u': 85, 'y': 6, 'z': 9, 'b': 1,
-    'r': 1, 'h': 1, 'g': 1, 'd': 1
+  'ey': {
+    '!': 2293, 'n': 36, 'e': 173, 'm': 23, 's': 21, 'c': 6, 'v': 3, 't': 12,
+    'w': 6, 'o': 10, 'a': 25, 'b': 7, 'r': 16, 'h': 9, 'l': 18, 'f': 8, 'd': 21,
+    'p': 2, 'i': 1, 'u': 1, 'k': 5, 'g': 1, 'z': 1
   },
-  'gs': {
-    '!': 139, 't': 67, 'w': 6, 'd': 7, 'b': 16, 'l': 6, 'o': 15, 'h': 8,
-    'e': 15, 'a': 14, 'm': 6, 'f': 4, 'j': 1, 'c': 2, 'i': 1, 'p': 1, 'y': 1
+  'Ri': {
+    'v': 41, 'c': 100, 'l': 12, 'o': 15, 'd': 49, 'g': 50, 't': 39, 'n': 80,
+    'z': 17, 'p': 23, 'f': 12, 'e': 87, 'm': 15, 's': 56, 'b': 18, 'k': 3,
+    'x': 2, 'a': 5, 'i': 5, 'h': 5, 'u': 1, 'j': 2, 'q': 1
   },
-  'Gs': {'c': 2, 'e': 1, 't': 1},
-  'gt': {
-    'o': 168, '!': 11, 's': 2, 'i': 3, 'a': 5, 'r': 1, 'e': 4, 'm': 3, 'h': 2, 
-    'l': 2
+  'iv': {
+    'e': 195, 'a': 108, 'i': 89, 'o': 21, 'n': 5, 'r': 4, 's': 4, 'y': 4,
+    'k': 4, 'h': 1, '!': 5, 'l': 6, 'c': 1
   },
-  'gu': {
-    'e': 161, 's': 68, 'y': 11, 'i': 89, 'r': 29, 'm': 12, 'l': 16, 'a': 22,
-    'z': 2, 'n': 23, 'c': 16, 'f': 5, 'o': 2, 't': 5, 'd': 5, 'p': 3, 'h': 3,
-    'b': 2, 'g': 3, '!': 3
+  've': {
+    'r': 627, 'n': 239, 'z': 18, 'y': 64, 's': 109, '!': 167, 'd': 28, 'l': 205,
+    't': 59, 'i': 13, 'j': 6, 'a': 23, 'c': 28, 'e': 19, 'v': 2, 'g': 4, 'u': 6,
+    'm': 5, 'q': 1, 'o': 2, 'h': 4, 'k': 4, 'b': 3
   },
-  'Gu': {
-    't': 59, 'z': 20, 'e': 68, 'y': 16, 'n': 47, 's': 35, 'i': 110, 'a': 43,
-    'r': 36, 'l': 50, 'f': 4, 'p': 4, 'm': 18, 'd': 16, 'g': 13, 'o': 2, '!': 1,
-    'h': 1, 'c': 8, 'b': 9
+  'ra': {
+    '!': 740, 'y': 121, 'h': 84, 'w': 74, 'l': 156, 'n': 923, 'd': 204, 'z': 96,
+    'v': 131, 'i': 139, 'm': 216, 't': 255, 'k': 97, 's': 286, 'f': 89,
+    'c': 190, 'u': 155, 'b': 134, 'p': 60, 'g': 145, 'e': 32, 'j': 23, 'x': 5,
+    'r': 92, 'a': 19, 'o': 14, 'q': 2
   },
-  'Gv': {'e': 1},
-  'gv': {'y': 1, 'a': 2, 'o': 3, 'i': 6},
-  'gw': {'e': 15, 'a': 13, 'o': 19, 'i': 13, 'u': 1, 'y': 1},
-  'Gw': {'i': 6, 'a': 4, 'y': 3, 'o': 1, 'e': 1},
-  'gx': {'a': 4},
-  'gy': {'!': 33, 'a': 2, 'e': 3, 'l': 1, 'i': 5, 'u': 1, 's': 1},
-  'Gy': {'l': 3, 'g': 1, 's': 1, 'a': 2, 'u': 1},
-  'gz': {'e': 1},
-  'Gz': {'y': 1},
-  'Ha': {
-    'r': 413, 'l': 155, 'y': 64, 'm': 146, 'w': 32, 'n': 208, 't': 53, 'h': 7,
-    'a': 27, 's': 98, 'i': 49, 'd': 39, 'g': 77, 'c': 41, 'u': 79, 'v': 36,
-    'z': 33, '!': 1, 'b': 32, 'k': 13, 'f': 19, 'j': 4, 'e': 23, 'p': 12,
-    'o': 1, 'x': 2, 'q': 2
+  'ic': {
+    'h': 859, 'e': 176, 'k': 1148, 'i': 58, 't': 19, 'o': 198, '!': 188,
+    'a': 154, 'c': 83, 's': 7, 'u': 28, 'z': 120, 'l': 13, 'q': 1, 'y': 1,
+    'd': 1, 'r': 2, 'n': 1
   },
   'ha': {
     'r': 550, 'm': 397, 'l': 270, 'w': 92, 'v': 41, 'p': 62, 'n': 512, 's': 52,
     'f': 43, 'e': 32, '!': 145, 'c': 53, 'u': 175, 't': 80, 'y': 36, 'h': 16,
     'd': 71, 'o': 10, 'i': 68, 'x': 2, 'b': 43, 'a': 22, 'g': 44, 'k': 70,
     'z': 14, 'j': 5
   },
-  'hb': {'u': 10, 'y': 5, 'e': 32, 'o': 11, 'a': 34, 'r': 3, 'i': 5},
-  'hc': {'o': 17, 'r': 7, 'u': 2, 'a': 4, 'h': 1, 'l': 2, 'e': 1},
-  'hd': {'e': 8, 'r': 2, '!': 1, 'i': 4, 'o': 3, 'a': 4},
-  'he': {
-    'l': 334, 'z': 12, 's': 113, 'r': 935, 'n': 270, 'w': 40, 'e': 111, 'p': 29,
-    'a': 152, 'c': 32, 'f': 26, 'y': 75, 't': 116, '!': 199, 'u': 38, 'o': 15,
-    'v': 28, 'm': 51, 'i': 171, 'x': 1, 'd': 20, 'h': 12, 'g': 8, 'b': 12,
-    'k': 28, 'j': 1
-  },
-  'He': {
-    'r': 226, 'n': 174, 'a': 85, 's': 43, 'b': 23, 'w': 15, 'l': 138, 'd': 37,
-    'm': 67, 'c': 27, 'i': 168, 'f': 24, 'y': 27, 't': 27, 'p': 19, 'u': 22,
-    'g': 31, '!': 1, 'e': 23, 'v': 10, 'h': 5, 'o': 1, 'j': 2, 'x': 1, 'k': 2,
-    'z': 1, 'q': 1
+  'ox': {
+    '!': 39, 'l': 4, 'w': 6, 'e': 14, 'x': 2, 'i': 4, 'o': 7, 's': 4, 't': 8,
+    'h': 3, 'a': 2, 'b': 4, 'm': 1, 'u': 1, 'n': 1, 'f': 1
   },
-  'hf': {'o': 13, 'i': 23, 'u': 2, 'e': 7},
-  'hg': {'a': 3, 'e': 6, 'i': 1, 'o': 1, 'h': 1},
-  'hh': {'o': 15, 'e': 9, 'a': 14, 'i': 2, 'u': 4},
-  'Hi': {
-    'l': 142, 'c': 31, 'n': 96, 'g': 49, 'r': 43, 't': 24, 'd': 10, 'a': 1,
-    'm': 17, 'b': 20, 'x': 4, 'p': 17, 'e': 22, 'v': 2, 's': 23, 'o': 1, 'z': 2,
-    'k': 2, 'j': 1
+  'Ho': {
+    'w': 48, 'l': 265, 'f': 49, 'p': 34, 'r': 127, 'd': 39, 'u': 78, 'g': 40,
+    'o': 44, 'b': 27, 's': 63, '!': 1, 'y': 16, 'n': 65, 'a': 14, 'm': 33,
+    'k': 10, 'c': 35, 't': 24, 'e': 59, 'v': 28, 'h': 24, 'i': 13, 'x': 4,
+    'j': 3, 'q': 1, 'z': 2
   },
-  'hi': {
-    't': 185, 'l': 207, 'n': 257, 's': 79, 'e': 146, 'p': 44, 'r': 92, 'b': 33,
-    'g': 24, 'v': 19, 'a': 103, 'f': 23, 'u': 8, 'c': 41, '!': 151, 'm': 98,
-    'd': 31, 'o': 78, 'h': 8, 'i': 3, 'k': 26, 'y': 6, 'z': 9, 'q': 1, 'x': 1, 
-    'j': 2
+  'To': {
+    'r': 103, 'd': 17, 'w': 33, 'l': 55, 'm': 77, 'n': 42, 'b': 25, 'v': 6,
+    't': 20, 's': 18, 'o': 34, 'u': 40, 'y': 8, '!': 1, 'p': 39, 'k': 13,
+    'c': 10, 'z': 4, 'e': 14, 'f': 8, 'a': 7, 'x': 1, 'h': 5, 'g': 5, 'j': 1,
+    'i': 1, 'q': 1
   },
-  'hj': {'e': 6, 'i': 1, '!': 2},
-  'Hj': {'o': 1, 'e': 3, 'a': 1},
-  'hk': {'i': 8, 'o': 21, 'e': 41, 'r': 1, 'a': 4, 'h': 1, '!': 1},
-  'Hl': {'a': 8, 'u': 1, 'e': 1, 'y': 1},
-  'hl': {
-    'i': 107, 'e': 275, '!': 175, 'o': 30, 'u': 12, 'm': 33, 'g': 4, 'b': 12,
-    'a': 63, 's': 26, 'k': 13, 'q': 3, 'y': 12, 'f': 11, 'w': 2, 't': 2,
-    'h': 10, 'l': 1, 'n': 1, 'r': 2, 'd': 1
+  'et': {
+    'e': 174, 't': 1287, 'c': 41, 'o': 111, '!': 370, 'i': 58, 'z': 172,
+    's': 103, 'a': 103, 'r': 150, 'h': 225, 'l': 41, 'm': 10, 'w': 6, 'f': 2,
+    'n': 3, 'j': 7, 'k': 16, 'u': 9, 'g': 5, 'y': 9, 'b': 3, 'd': 1, 'p': 2
   },
-  'hm': {
-    'i': 63, 'o': 18, 'a': 215, 'e': 77, '!': 51, 's': 2, 'u': 12, 'k': 5,
-    'b': 1, 'y': 2
+  'Ra': {
+    'm': 120, 'y': 46, 'n': 91, 't': 65, 's': 63, 'i': 57, 'g': 31, 'd': 76,
+    'l': 13, 'p': 37, 'w': 19, 'u': 43, 'f': 25, 'z': 12, 'c': 40, 'e': 13,
+    'b': 47, 'h': 20, 'o': 2, 'k': 16, 'a': 6, 'v': 28, 'r': 10, 'j': 13,
+    '!': 1, 'x': 2, 'q': 2
   },
-  'Hn': {'a': 2, 'y': 1, 'o': 1},
-  'hn': {
-    's': 22, '!': 126, 'e': 182, 'k': 16, 'i': 42, 'a': 34, 'd': 2, 'o': 23,
-    'u': 5, 'h': 4, 'l': 4, 'y': 2, 'g': 1, 'c': 2, 'n': 1, 'q': 1, 'z': 1,
-    'b': 2, 'p': 1, 't': 1
+  'ir': {
+    'e': 216, '!': 115, 'k': 93, 'b': 13, 'a': 165, 'r': 40, 'd': 46, 'l': 23,
+    's': 64, 'o': 137, 'i': 74, 'c': 48, 't': 52, 'm': 22, 'n': 28, 'g': 23,
+    'w': 4, 'f': 5, 'h': 5, 'v': 8, 'u': 8, 'z': 4, 'y': 12, 'p': 6, 'j': 3
   },
-  'ho': {
-    'm': 74, 'l': 226, 'p': 23, 'd': 19, 'r': 253, 'n': 128, 'u': 157, '!': 82,
-    'a': 15, 'e': 100, 'i': 10, 'o': 58, 'c': 25, 'f': 128, 'w': 82, 't': 34,
-    'y': 10, 'q': 1, 'b': 14, 'v': 27, 'j': 3, 's': 26, 'k': 7, 'g': 4, 'z': 1
+  'me': {
+    's': 137, 'z': 14, 'r': 684, 'n': 233, '!': 179, 'y': 139, 'l': 202, 'w': 5,
+    'i': 90, 'd': 37, 'o': 14, 't': 72, 'a': 26, 'e': 23, 'c': 12, 'k': 18,
+    'u': 6, 'j': 5, 'h': 9, 'g': 4, 'b': 3, 'm': 3, 'f': 1
   },
-  'Ho': {
-    'w': 48, 'l': 265, 'f': 49, 'p': 34, 'r': 127, 'd': 39, 'u': 78, 'g': 40,
-    'o': 44, 'b': 27, 's': 63, '!': 1, 'y': 16, 'n': 65, 'a': 14, 'm': 33,
-    'k': 10, 'c': 35, 't': 24, 'e': 59, 'v': 28, 'h': 24, 'i': 13, 'x': 4,
-    'j': 3, 'q': 1, 'z': 2
+  'at': {
+    's': 91, 't': 488, 'k': 33, 'e': 319, 'r': 87, 'h': 352, 'o': 241, 'f': 7,
+    'l': 55, 'c': 81, 'u': 48, 'z': 102, 'a': 187, 'm': 24, 'y': 23, 'i': 126,
+    '!': 158, 'n': 23, 'w': 8, 'd': 2, 'v': 1, 'g': 1
   },
-  'hp': {'e': 1, 'a': 3, 'u': 1, 'o': 2},
-  'hr': {
-    'i': 168, 'a': 71, 'o': 85, 'e': 132, '!': 67, 'l': 17, 'm': 26, 'u': 21,
-    'k': 9, 'y': 19, 'h': 6, 'b': 6, 's': 16, 'z': 3, 'n': 8, 't': 7, 'g': 1,
-    'w': 2, 'd': 2, 'f': 1
+  'Ke': {
+    'l': 79, 'n': 95, 'i': 43, 'm': 45, 'r': 88, 'y': 14, 's': 32, 'e': 60,
+    'a': 59, 'c': 4, 't': 43, 'h': 11, 'p': 14, 'o': 13, 'f': 2, 'g': 6, 'd': 6,
+    'v': 9, 'b': 7, 'z': 3, 'k': 4, '!': 1, 'w': 4, 'u': 3, 'x': 1
   },
-  'Hr': {
-    'u': 2, 'b': 2, 'e': 2, 'i': 6, 'o': 5, 'a': 5, 'd': 1, 'y': 3, 'n': 1, 
-    'c': 1
+  'ly': {
+    '!': 384, 'n': 30, 't': 7, 'e': 25, 'd': 3, 'b': 2, 'l': 3, 'a': 20,
+    'm': 14, 'k': 3, 'f': 2, 'o': 9, 's': 7, 'w': 5, 'c': 3, 'g': 1, 'z': 3,
+    'u': 2, 'q': 1, 'h': 1
   },
-  'hs': {
-    '!': 49, 'o': 10, 't': 17, 'm': 4, 'l': 3, 'c': 4, 'e': 21, 'n': 1, 'i': 5,
-    'a': 2, 'h': 2, 'w': 1, 'p': 2, 'b': 1
+  'Pr': {
   },
-  'Hs': {'u': 3, 'i': 6, 'y': 1},
-  'ht': {
-    '!': 208, 'e': 79, 'o': 40, 'y': 11, 'f': 3, 'n': 7, 'r': 7, 'a': 25,
-    'i': 18, 'l': 13, 's': 10, 'm': 9, 'b': 3, 'w': 2, 'c': 1, 'h': 9, 'z': 2
+  'ce': {
+    '!': 370, 'r': 81, 'n': 80, 'v': 15, 'l': 142, 'y': 43, 'd': 21, 'a': 26,
+    'p': 3, 'w': 13, 't': 29, 's': 32, 'f': 5, 'o': 2, 'u': 3, 'k': 82, 'g': 9,
+    'm': 8, 'b': 3, 'c': 3, 'e': 2, 'j': 1, 'h': 1, 'i': 7
   },
-  'Ht': {'w': 1},
-  'Hu': {
-    'g': 38, 'n': 59, 'd': 35, 'b': 30, 'f': 22, 'm': 45, 't': 37, 'r': 51,
-    'l': 46, 'e': 36, 'y': 10, 'a': 5, 's': 60, 'c': 17, '!': 1, 'p': 11,
-    'i': 16, 'o': 3, 'h': 7, 'x': 6, 'k': 2, 'w': 1, 'v': 2, 'z': 1, 'u': 1, 
-    'j': 1
+  'nn': {
+    'e': 579, '!': 476, 'i': 338, 'o': 127, 'a': 213, 'y': 39, 's': 17, 'u': 24,
+    't': 2, 'd': 3, 'h': 4, 'l': 4, 'r': 1, 'b': 1, 'f': 1, 'z': 1, 'c': 1,
+    'g': 1, 'k': 1
   },
-  'hu': {
-    'l': 74, 'r': 110, 'e': 44, 'n': 49, '!': 20, 'm': 63, 'g': 13, 's': 41,
-    'b': 23, 'p': 16, 't': 41, 'c': 21, 'a': 13, 'h': 10, 'y': 8, 'f': 15,
-    'k': 18, 'd': 8, 'i': 15, 'u': 3, 'o': 4, 'j': 1
+  'Wo': {
+    'o': 116, 'l': 105, 'n': 13, 'r': 63, 'm': 11, 'f': 1, 'z': 5, 'j': 24,
+    't': 3, 'e': 16, 'h': 17, 'u': 4, 'b': 4, 'g': 2, 'd': 3, 'w': 1, 'i': 2,
+    'y': 5, 's': 3, 'k': 1
   },
-  'Hv': {'i': 1},
-  'hv': {'i': 5, 'e': 4, 'a': 1},
-  'Hw': {'a': 1, 'e': 1},
-  'hw': {'a': 83, 'o': 12, 'e': 70, 'i': 29, 'u': 2, 'r': 1},
-  'hy': {
-    '!': 91, 't': 3, 'n': 10, 'm': 9, 's': 4, 'g': 1, 'd': 2, 'a': 8, 'b': 3,
-    'r': 2, 'f': 3, 'w': 1, 'e': 2, 'u': 1, 'o': 2, 'l': 1, 'k': 1
+  'os': {
+    's': 322, 't': 271, '!': 487, 'e': 246, 'l': 36, 'h': 104, 'b': 31,
+    'a': 113, 'k': 193, 'w': 12, 'i': 127, 'o': 67, 'c': 93, 'g': 6, 'm': 27,
+    'n': 23, 'q': 8, 'p': 16, 'r': 4, 'z': 28, 'd': 11, 'f': 4, 'v': 2, 'u': 9,
+    'j': 1, 'y': 4
   },
-  'Hy': {
-    'd': 5, 'a': 4, 'm': 8, 'n': 8, 'l': 10, 's': 10, 'e': 3, 'p': 3, '!': 1,
-    'r': 2, 'u': 1, 'c': 2, 'b': 2, 'o': 1, 'z': 1, 't': 3, 'k': 1
+  'ss': {
+    '!': 421, 'e': 592, 'o': 223, 'a': 195, 'l': 83, 'i': 228, 'm': 80, 'u': 14,
+    'y': 17, 'n': 34, 'c': 3, 'b': 14, 'f': 6, 'w': 13, 'h': 9, 'k': 5, 'g': 2,
+    't': 2, 'p': 2, 'r': 1
   },
-  'hz': {'i': 1, 'e': 1, '!': 1},
-  'Ia': {
-    'c': 12, 'n': 12, 'd': 1, 'r': 4, 'l': 1, 'f': 1, 'm': 2, 'v': 1, 't': 1
+  'em': {
+    'a': 460, 'i': 121, 'p': 97, 'o': 135, 'e': 219, 'b': 83, 's': 40, 'u': 28,
+    'm': 128, '!': 123, 'k': 16, 'l': 19, 'y': 13, 'n': 6, 'w': 1, 'c': 7,
+    'r': 11, 'h': 3, 'z': 2, 'f': 2, 'j': 1
   },
-  'ia': {
-    'm': 54, '!': 534, 'z': 12, 'g': 26, 'n': 550, 's': 102, 'r': 125, 't': 49,
-    'l': 59, 'u': 12, 'k': 100, 'd': 22, 'f': 10, 'c': 48, 'v': 13, 'o': 8,
-    'h': 13, 'q': 2, 'i': 4, 'b': 4, 'p': 11, 'w': 1, 'j': 1, 'e': 1
+  'Je': {
+    'n': 51, 'f': 23, 'w': 7, 'r': 39, 'a': 28, 't': 8, 's': 30, 'm': 8, 'p': 8,
+    'l': 18, 'o': 3, 'h': 3, 'z': 5, 'd': 6, 'x': 1, 'u': 2, 'c': 4, 'g': 1,
+    'e': 1, 'v': 2, 'b': 2, 'k': 2
   },
-  'Ib': {
-    'a': 7, 'r': 3, 's': 1, 'e': 3, 'u': 1, 'o': 1, 'l': 1, 'b': 2, 'd': 1
+  'nk': {
+    'i': 67, 'l': 83, 's': 59, '!': 168, 'e': 282, 'f': 5, 'm': 7, 'o': 106,
+    'n': 7, 'h': 16, 'a': 73, 'b': 2, 'r': 16, 'w': 6, 'u': 9, 'v': 1, 't': 1,
+    'k': 1, 'x': 1, 'y': 1
   },
-  'ib': {
-    's': 6, 'b': 98, 'e': 133, 'o': 36, 'l': 52, 'a': 70, 'n': 6, '!': 24,
-    'u': 16, 'i': 25, 'r': 15, 'd': 1, 'y': 5, 'm': 4, 'f': 1, 'w': 1, 'k': 1,
-    'g': 1, 't': 1
+  'ki': {
+    'n': 457, '!': 1404, 'd': 4, 'r': 23, 'p': 3, 'l': 41, 'e': 91, 's': 58,
+    'b': 12, 'f': 3, 'm': 15, 't': 13, 'y': 3, 'v': 3, 'c': 9, 'j': 1, 'h': 3,
+    'u': 2, 'o': 3, 'z': 1, 'k': 2, 'w': 2, 'a': 11, 'g': 1
   },
-  'ic': {
-    'h': 859, 'e': 176, 'k': 1148, 'i': 58, 't': 19, 'o': 198, '!': 188,
-    'a': 154, 'c': 83, 's': 7, 'u': 28, 'z': 120, 'l': 13, 'q': 1, 'y': 1,
-    'd': 1, 'r': 2, 'n': 1
+  'ry': {
+    '!': 708, 'a': 24, 'e': 24, 'o': 8, 's': 36, 'm': 20, 'd': 13, 'h': 2,
+    'c': 12, 'b': 9, 'k': 4, 'n': 18, 'x': 1, 'l': 13, 'v': 1, 'w': 1, 'r': 1,
+    't': 6, 'j': 1, 'g': 6, 'z': 3, 'p': 1, 'i': 1, 'f': 1, 'u': 1
   },
-  'Ic': {'k': 2, 'e': 3, 'h': 3, 'a': 2},
-  'Id': {'e': 6, 'd': 1, 'a': 1, 'o': 1, 'l': 2, 'r': 3, 'i': 1},
-  'id': {
-    't': 30, '!': 90, 's': 15, 'e': 287, 'g': 152, 'd': 96, 'w': 9, 'a': 91,
-    'y': 10, 'r': 21, 'l': 54, 'm': 22, 'o': 71, 'h': 11, 'n': 12, 'k': 4,
-    'i': 62, 'b': 9, 'c': 3, 'u': 7, 'p': 2, 'v': 2, 'j': 2, 'z': 1
+  'Po': {
+    'w': 21, 'r': 78, 't': 45, 'p': 48, 'o': 20, 'l': 143, 'n': 41, 'e': 22,
+    's': 53, 'i': 28, 'u': 37, 'g': 6, 'm': 32, 'h': 6, 'y': 9, 'f': 4, 'c': 18,
+    'a': 7, 'k': 10, 'z': 8, 'd': 23, 'b': 3, 'q': 2, 'v': 2, '!': 1, 'x': 1
   },
-  'ie': {
-    'l': 538, 'r': 893, 'n': 218, '!': 598, 'v': 36, 'd': 157, 's': 283,
-    'g': 91, 't': 151, 'u': 25, 'h': 32, 'w': 94, 'f': 62, 'b': 109, 'i': 1,
-    'm': 75, 'p': 19, 'c': 95, 'z': 18, 'j': 12, 'k': 38, 'y': 1, 'a': 11, 
-    'x': 2
+  'we': {
+    'l': 255, 'n': 72, 'r': 152, '!': 52, 'e': 53, 'y': 16, 's': 20, 'a': 31,
+    'i': 61, 't': 31, 'h': 6, 'd': 20, 'g': 16, 'c': 8, 'b': 6, 'k': 6, 'm': 3,
+    'z': 2, 'p': 2, 'j': 1, 'f': 1
   },
-  'Ie': {'z': 1, 's': 1, 'n': 3},
-  'if': {
-    'f': 171, 't': 14, 'e': 68, 'o': 31, 'i': 20, 'u': 7, '!': 20, 'l': 12,
-    'r': 11, 'a': 18, 's': 8, 'k': 4, 'n': 1, 'm': 2, 'g': 1, 'y': 1
+  'Hu': {
+    'g': 38, 'n': 59, 'd': 35, 'b': 30, 'f': 22, 'm': 45, 't': 37, 'r': 51,
+    'l': 46, 'e': 36, 'y': 10, 'a': 5, 's': 60, 'c': 17, '!': 1, 'p': 11,
   },
-  'If': {'i': 2, 'f': 3, 'v': 1, 'e': 1, 'a': 1},
-  'Ig': {
-    'l': 5, 'n': 5, 'o': 3, 'b': 2, 'a': 1, 'e': 1, 'w': 1, 't': 1, 'u': 2
+  'ug': {
+    'h': 483, 'l': 47, 'o': 13, 'g': 60, 'a': 67, 'e': 71, 'u': 26, '!': 19,
   },
-  'ig': {
-    'u': 74, 'h': 259, '!': 210, 'g': 141, 'a': 170, 'i': 41, 'e': 149, 'l': 99,
-    's': 25, 'p': 2, 'n': 99, 'd': 6, 'o': 63, 'r': 19, 'b': 9, 't': 7, 'm': 21,
-    'f': 5, 'w': 6, 'k': 2, 'y': 2
+  'Fl': {'o': 72, 'e': 84, 'y': 7, 'a': 76, 'i': 36, 'u': 27},
+  'sh': {
+    'i': 204, 'e': 207, 'a': 227, 'o': 78, '!': 312, 'l': 22, 'b': 31, 't': 7,
+    'c': 3, 'f': 8, 'w': 14, 'm': 41, 'n': 27, 'u': 27, 'r': 4, 'k': 10, 'j': 1,
+    'y': 5, 'd': 4, 'p': 3
   },
-  'ih': {
-    'a': 60, '!': 4, 'i': 6, 'y': 1, 'e': 22, 'o': 10, 'm': 3, 'l': 13, 'u': 7,
-    'n': 3, 't': 1, 'k': 1, 'r': 1
+  'gt': {
   },
-  'Ih': {'l': 2, 'r': 2, 'd': 1, 'a': 1, 'n': 2, 'm': 1, 'e': 2},
-  'ii': {
-    '!': 13, 'n': 2, 's': 3, 'o': 1, 'g': 1, 'k': 1, 'h': 3, 'm': 1, 'u': 1,
-    'b': 1, 'p': 3, 'r': 1, 'v': 1, 'l': 1
+  'to': {
+    'n': 1084, '!': 614, 's': 86, 'k': 14, 'y': 11, 'u': 45, 'r': 222, 'p': 30,
+    'v': 14, 'w': 59, 'c': 64, 'd': 14, 'x': 2, 'o': 21, 'l': 123, 'j': 3,
+    'm': 46, 'i': 9, 't': 27, 'f': 33, 'g': 14, 'e': 34, 'b': 13, 'h': 9,
+    'a': 3, 'z': 5
   },
-  'Ii': {'a': 1, 'd': 1, 'n': 1},
-  'Ij': {'a': 2},
-  'ij': {'e': 7, 'o': 14, 'a': 24, '!': 2, 'u': 1, 'i': 3},
-  'ik': {
-    'e': 113, '!': 294, 'o': 56, 's': 18, 'h': 6, 'i': 27, 'u': 16, 'l': 15,
-    'k': 16, 'a': 39, 'r': 2, 'm': 2, 't': 2, 'n': 1, 'y': 2
+  'Bu': {
+    't': 73, 'r': 304, 's': 110, 'c': 111, 'l': 65, 'n': 55, 'f': 17, 'e': 50,
+    'm': 21, 'i': 12, 'x': 3, 'd': 42, 'g': 21, 'z': 19, 'o': 12, 'h': 10,
+    'k': 8, 'b': 16, 'p': 1, 'a': 3, 'y': 5, 'j': 5, 'q': 2, 'v': 2
   },
-  'Ik': {'e': 9, 'n': 1, 'a': 1, 'u': 1, 'z': 1, 'k': 1},
-  'Il': {'e': 2, 'i': 3, 'l': 17, 'd': 1, 'a': 7, 's': 1, 't': 1, 'g': 1},
-  'il': {
-    'l': 1559, 's': 89, 'e': 259, 't': 81, 'b': 106, 'v': 54, 'a': 165, 'k': 74,
-    'c': 53, 'm': 51, '!': 188, 'd': 138, 'g': 33, 'h': 37, 'p': 13, 'n': 11,
-    'y': 26, 'o': 95, 'i': 176, 'w': 8, 'f': 25, 'r': 8, 'u': 21, 'j': 4,
-    'z': 9, 'q': 1
+  'ut': {
+    'l': 26, 'i': 63, 't': 215, 'c': 62, '!': 113, 'h': 169, 'z': 81, 'n': 20,
+    's': 47, 'u': 14, 'm': 17, 'r': 39, 'o': 69, 'e': 131, 'y': 15, 'w': 7,
+    'p': 2, 'k': 21, 'a': 55, 'f': 3, 'g': 4, 'j': 3, 'b': 2, 'v': 1
   },
-  'Im': {
-    'h': 3, 'e': 3, '!': 1, 'l': 2, 'a': 7, 'm': 8, 'b': 14, 'p': 5, 'o': 2,
-    'r': 1, 'd': 1, 'i': 1, 'u': 1, 'f': 1, 'g': 1
+  'tl': {'e': 343, 'i': 67, 'o': 32, 'a': 52, 'u': 5, 'y': 12, '!': 15, 'l': 1},
+  'Si': {
+    'm': 115, 'l': 95, 'n': 79, 'z': 4, 'e': 90, 's': 34, 'k': 14, 'g': 31,
+    'b': 19, 'p': 18, 'd': 40, 't': 35, 'r': 40, 'f': 7, 'c': 28, 'u': 3,
+    'x': 6, 'a': 10, 'v': 27, 'q': 1, 'o': 5, 'w': 5, '!': 1
   },
   'im': {
     'm': 112, 'p': 47, 's': 36, '!': 116, 'e': 198, 'o': 131, 'b': 78, 'a': 174,
     'u': 26, 'i': 83, 'k': 18, 'c': 9, 'z': 3, 'l': 22, 'r': 5, 'h': 2, 't': 2,
     'w': 1, 'n': 5, 'f': 1
   },
-  'in': {
-    '!': 1906, 'e': 885, 's': 726, 'g': 2064, 'a': 359, 'n': 253, 'd': 310,
-    'o': 551, 'c': 156, 't': 245, 'l': 45, 'k': 305, 'b': 72, 'h': 61, 'f': 26,
-    'z': 66, 'i': 419, 'v': 14, 'q': 6, 'r': 24, 'm': 20, 'w': 20, 'y': 16,
-    'j': 2, 'u': 16, 'p': 3
-  },
-  'In': {
-    'g': 43, 'm': 2, 'f': 6, 'i': 3, 'n': 9, 'o': 6, 'c': 10, 'a': 8, 's': 13,
-    'e': 4, 'k': 4, 'd': 8, '!': 1, 'l': 2, 'z': 5, 'v': 1, 'y': 1, 't': 10,
-    'h': 1, 'b': 1
-  },
-  'Io': {
-    'r': 1, 'n': 2, 'v': 1, 'e': 1, 't': 1, 'l': 1, 'd': 1, 'a': 1, 'z': 2,
-    'p': 1, 's': 1
-  },
-  'io': {
-    't': 68, 's': 43, '!': 596, 'n': 255, 'r': 85, 'l': 96, 'j': 2, 'u': 35,
-    'v': 14, 'f': 3, 'i': 2, 'k': 7, 'd': 7, 'p': 12, 'c': 7, 'w': 4, 'g': 4,
-    'b': 2, 'm': 6, 'x': 2, 'a': 2, 'e': 1, 'z': 2
-  },
-  'Ip': {'p': 1, 'o': 1, 's': 2, '!': 1},
-  'ip': {
-    's': 35, '!': 50, 't': 11, 'p': 205, 'e': 43, 'l': 18, 'm': 4, 'k': 17,
-    'h': 11, 'i': 30, 'a': 21, 'r': 9, 'f': 9, 'o': 26, 'w': 3, 'n': 1, 'u': 2, 
-    'c': 1
+  'mm': {
+    'o': 78, 'i': 78, 'e': 336, 's': 6, '!': 59, 'a': 79, 'u': 3, 'y': 7,
+    'r': 4, 'l': 6
   },
-  'Iq': {'b': 1},
-  'iq': {'u': 45, 'i': 1, '!': 4},
-  'ir': {
-    'e': 216, '!': 115, 'k': 93, 'b': 13, 'a': 165, 'r': 40, 'd': 46, 'l': 23,
-    's': 64, 'o': 137, 'i': 74, 'c': 48, 't': 52, 'm': 22, 'n': 28, 'g': 23,
-    'w': 4, 'f': 5, 'h': 5, 'v': 8, 'u': 8, 'z': 4, 'y': 12, 'p': 6, 'j': 3
+  'mo': {
+    'n': 430, 's': 32, 'r': 222, 'u': 32, 't': 76, '!': 121, 'o': 12, 'c': 7,
+    'i': 2, 'd': 13, 'l': 44, 'a': 6, 'y': 11, 'e': 9, 'w': 11, 'g': 4, 'k': 4,
+    'h': 4, 'm': 2, 'f': 2, 'p': 3, 'v': 5, 'z': 4, 'x': 1
   },
-  'Ir': {
-    'w': 1, 'v': 4, 'i': 14, 'b': 1, 'e': 8, 'o': 3, 'a': 3, 'l': 2, 'u': 1,
-    'm': 1, 's': 1, 'z': 1, 'r': 1
+  'Fo': {
+    's': 33, 'r': 167, 'x': 8, 'w': 11, 'l': 44, 'n': 49, 'u': 42, 'o': 12,
+    'g': 20, 'y': 3, 't': 6, 'd': 9, 'b': 2, 'm': 1, 'c': 4, 'e': 9, 'a': 2,
+    'i': 4, 'p': 2, 'k': 2, 'h': 2
   },
-  'is': {
-    '!': 857, 'h': 260, 'o': 217, 'e': 305, 't': 449, 'c': 195, 's': 283,
-    'n': 42, 'l': 77, 'p': 29, 'k': 108, 'b': 44, 'd': 14, 'w': 19, 'm': 41,
-    'v': 2, 'i': 107, 'a': 76, 'u': 13, 'g': 5, 'z': 25, 'y': 5, 'q': 2, 'r': 6,
-    'f': 4, 'j': 2
+  'st': {
+    'e': 898, '!': 431, 'r': 304, 'i': 255, 'o': 400, 'a': 372, 'l': 84,
+    'm': 24, 'b': 12, 'y': 27, 'n': 19, 'f': 4, 'u': 30, 'p': 3, 'c': 3,
+    'w': 11, 'g': 3, 'h': 14, 'k': 7, 'v': 2, 's': 1, 'z': 1
   },
-  'Is': {
-    'a': 28, 'o': 4, 'b': 5, 'r': 5, 'h': 13, 'e': 14, 'l': 10, 'm': 3, 's': 4,
-    't': 2, 'k': 1, 'n': 1, 'i': 8, 'c': 1, 'g': 3
+  'ya': {
+    'n': 104, 'l': 31, 't': 13, '!': 81, 'r': 53, 's': 28, 'm': 32, 'k': 15,
+    'w': 3, 'c': 9, 'h': 7, 'g': 6, 'z': 2, 'd': 6, 'y': 1, 'b': 4, 'v': 2,
+    'i': 2, 'o': 3, 'p': 1, 'e': 1, 'u': 1
   },
-  'it': {
-    'h': 166, 'e': 237, 'c': 120, 't': 505, 'z': 316, 'a': 151, 'n': 23, 'f': 5,
-    'l': 33, '!': 117, 'o': 141, 'm': 40, 'u': 21, 'i': 68, 's': 102, 'w': 8,
-    'r': 43, 'y': 31, 'k': 29, 'b': 8, 'g': 4, 'v': 4, 'j': 2, 'p': 1
+  'nt': {
+    '!': 389, 'e': 432, 'g': 8, 'i': 266, 'o': 304, 'h': 96, 'r': 99, 'y': 37,
+    'u': 52, 'l': 44, 'a': 196, 's': 54, 'z': 122, 't': 9, 'w': 10, 'n': 18,
+    'f': 7, 'b': 2, 'v': 4, 'j': 4, 'c': 4, 'k': 10, 'p': 2, 'd': 2, 'm': 6
   },
-  'It': {
-    'o': 1, 'a': 3, 'h': 1, 's': 1, 'u': 3, 'z': 1, 'r': 1, 'k': 1, 't': 1, 
-    'n': 1
+  'ex': {
+    'a': 15, 't': 9, '!': 20, 'n': 2, 'l': 3, 'i': 10, 'e': 8, 'f': 1, 'r': 3,
+    's': 2, 'o': 1, 'h': 1, 'y': 2, 'w': 1, 'z': 1
   },
-  'Iu': {'l': 4, 'r': 1, 'c': 1},
-  'iu': {
-    's': 72, '!': 12, 'l': 18, 'n': 3, 'r': 6, 'd': 6, 'c': 5, 'f': 5, 'z': 4,
-    't': 6, 'k': 11, 'm': 7, 'b': 3, 'e': 3
+  'xa': {
+    'n': 9, 'd': 2, 's': 3, 'u': 1, 'm': 1, 'c': 2, 'l': 1, 'y': 8, '!': 4,
+    'k': 2, 'r': 1
   },
-  'Iv': {'e': 13, 'y': 1, 'o': 2, 'i': 2, 'a': 8, 'r': 1},
-  'iv': {
-    'e': 195, 'a': 108, 'i': 89, 'o': 21, 'n': 5, 'r': 4, 's': 4, 'y': 4,
-    'k': 4, 'h': 1, '!': 5, 'l': 6, 'c': 1
+  'Ru': {
+    's': 86, 'i': 8, 't': 40, 'c': 15, 'b': 51, 'f': 24, 'd': 55, 'n': 31,
+    'p': 20, 'g': 17, 'e': 37, 'l': 15, 'm': 38, 'v': 4, 'h': 15, 'a': 6,
+    'z': 7, 'y': 6, 'u': 2, 'o': 8, 'x': 1, 'k': 2, 'w': 2, 'r': 2, 'j': 1
   },
-  'Iw': {'a': 13},
-  'iw': {'e': 12, 'i': 8, 'a': 15, 'o': 4, '!': 3, 'r': 1, 'c': 2, 's': 2},
-  'ix': {
-    'o': 11, '!': 61, 's': 8, 'l': 3, 'e': 9, 'b': 1, 'i': 7, 't': 8, 'n': 3,
-    'k': 1, 'a': 5, 'd': 1
+  'us': {
+    's': 233, 'o': 59, 't': 209, 'h': 153, 'e': 285, '!': 539, 'k': 106,
+    'b': 18, 'c': 125, 'a': 72, 'i': 78, 'g': 4, 'l': 28, 'q': 4, 'm': 21,
+    'n': 17, 'u': 14, 'w': 5, 'z': 34, 'd': 6, 'y': 1, 'f': 1, 'r': 1
   },
-  'iy': {'a': 37, 'o': 6, 'u': 1, 'e': 3},
-  'Iy': {'e': 2, 'o': 1},
-  'iz': {
-    '!': 60, 'e': 59, 'a': 67, 'z': 79, 'o': 25, 'u': 16, 'i': 31, 'c': 4,
-    'r': 1, 'm': 4, 'b': 1, 'n': 4, 'v': 1, 'k': 2, 'w': 2, 'l': 1, 'd': 1, 
-    's': 1
+  'se': {
+    'l': 361, '!': 613, 'n': 628, 'y': 170, 'p': 12, 's': 26, 'r': 429, 'm': 50,
+    't': 132, 'c': 25, 'a': 28, 'u': 13, 'b': 26, 'x': 2, 'e': 29, 'h': 9,
+    'k': 64, 'v': 7, 'g': 13, 'f': 10, 'd': 11, 'i': 17, 'w': 13, 'z': 2,
+    'q': 1, 'o': 3
   },
-  'Iz': {'z': 3, 'a': 7, 'q': 1, 'u': 1, 's': 1},
-  'Ja': {
-    'c': 61, 'm': 24, 'r': 63, 'n': 106, 's': 26, 'e': 8, 'y': 11, 'i': 6,
-    'f': 6, 'b': 13, 'q': 9, 'v': 11, 'w': 5, 'u': 16, 'h': 11, 'g': 16, 'l': 5,
-    'k': 19, 'z': 1, 'd': 3, 't': 1, 'x': 1, 'p': 3, 'a': 2, 'j': 1
+  'if': {
+    'f': 171, 't': 14, 'e': 68, 'o': 31, 'i': 20, 'u': 7, '!': 20, 'l': 12,
+    'r': 11, 'a': 18, 's': 8, 'k': 4, 'n': 1, 'm': 2, 'g': 1, 'y': 1
   },
-  'ja': {
-    's': 16, 'm': 7, 'n': 38, 'r': 43, '!': 54, 'd': 4, 'l': 14, 'w': 3,
-    'c': 13, 'k': 7, 'e': 1, 'h': 7, 't': 3, 'a': 1, 'u': 1, 'y': 5, 'b': 1,
-    'j': 2, 'g': 3, 'i': 2, 'p': 1
+  'ff': {
+    'i': 95, 'm': 19, 'e': 288, '!': 452, 'o': 60, 'y': 11, 'r': 44, 'n': 20,
   },
-  'jb': {'k': 1},
-  'jc': {'i': 9, 'z': 8, 'h': 2, 'a': 1, '!': 1, 'e': 3},
-  'jd': {'u': 2, 'a': 8, 'e': 2},
-  'Je': {
-    'n': 51, 'f': 23, 'w': 7, 'r': 39, 'a': 28, 't': 8, 's': 30, 'm': 8, 'p': 8,
-    'l': 18, 'o': 3, 'h': 3, 'z': 5, 'd': 6, 'x': 1, 'u': 2, 'c': 4, 'g': 1,
-    'e': 1, 'v': 2, 'b': 2, 'k': 2
+  'fi': {
+    'n': 94, 't': 21, 'e': 235, 's': 12, 'l': 28, '!': 29, 'r': 4, 'g': 8,
+    'o': 8, 'c': 12, 'b': 2, 'd': 5, 'a': 12, 'u': 1, 'h': 1, 'q': 1, 'k': 1,
+    'p': 1, 'f': 1
   },
-  'je': {
-    's': 15, 'd': 6, 'r': 35, 'u': 2, 'w': 12, 'a': 9, 'k': 8, 'n': 20, 'e': 4,
-    'l': 19, '!': 15, 't': 4, 'i': 5, 'c': 2, 'm': 3, 'v': 2, 'p': 1, 'b': 1
+  'Di': {
+    'a': 20, 'x': 7, 'c': 60, 'l': 78, 'g': 34, 'e': 81, 'o': 13, 'n': 72,
+    'b': 30, 's': 62, 'p': 22, 'm': 56, 'z': 4, 'r': 24, 't': 32, 'v': 23,
+    'd': 15, 'f': 22, 'k': 7, 'i': 2, 'w': 1, 'h': 1, 'j': 1, 'u': 1
   },
-  'jg': {'r': 1, 'e': 1},
-  'Jh': {'o': 2, 'i': 1, 'a': 1},
-  'jh': {'o': 2},
-  'ji': {
-    'l': 5, 'a': 17, 'c': 7, 'v': 2, 'm': 8, 'i': 1, 'g': 1, 'w': 1, 't': 2,
-    '!': 9, 'o': 1, 'h': 1, 'd': 3, 'k': 2, 's': 2, 'r': 3, 'e': 3, 'n': 2
+  'az': {
+    '!': 50, 'i': 82, 'a': 103, 'q': 5, 'z': 108, 'o': 49, 'e': 97, 'u': 16,
+    'l': 13, 'c': 4, 'd': 8, 'g': 4, 'm': 8, 'y': 7, 'k': 1, 'w': 1, 's': 3,
+    'n': 3, 'v': 1
   },
-  'Ji': {
-    'm': 14, 'l': 5, 'n': 12, 'r': 8, 'a': 2, 'g': 1, 't': 1, 'v': 1, 'p': 1, 
-    '!': 1
+  'ye': {
+    's': 32, 'r': 334, 'n': 34, '!': 84, 't': 26, 'a': 28, 'u': 4, 'd': 9,
+    'k': 2, 'l': 12, 'h': 2, 'g': 1, 'm': 7, 'e': 2, 'z': 1, 'w': 1
   },
-  'jj': {'a': 2},
-  'jk': {'o': 10, 'a': 9, 'u': 1, '!': 1},
-  'jl': {'a': 1, 'y': 1, 'o': 1, '!': 1, 'i': 1},
-  'jm': {'a': 3, 'u': 1, 'e': 1, 'o': 1},
-  'Jn': {'!': 1},
-  'jn': {'a': 6, 'i': 4, 'o': 4, 'y': 2, 'e': 1},
-  'Jo': {
-    'h': 42, 'n': 25, 'r': 21, 's': 27, 'y': 10, 'i': 4, 'l': 19, 'b': 7,
-    'e': 12, 'u': 11, 'p': 2, 'w': 3, '!': 1, 'z': 3, 'a': 8, 'c': 7, 'o': 4,
-    'v': 6, 'f': 2, 'j': 1, 'd': 5, 'm': 3, 'k': 3, 't': 2, 'g': 1
+  'My': {
+    'e': 5, 'l': 4, 'r': 15, 'a': 3, 'h': 3, 'n': 5, 's': 6, 'u': 1, 'k': 3,
+    'o': 1, 'i': 1, 't': 1, 'c': 1
   },
-  'jo': {
-    'r': 25, '!': 51, 's': 19, 'h': 12, 'y': 7, 'i': 2, 'n': 13, 'g': 1, 'e': 1,
-    'l': 9, 'w': 1, 'b': 1, 'd': 1, 'u': 6, 'k': 3, 'q': 1, 'o': 2, 'v': 1, 
-    'c': 2
+  'lt': {
+    'o': 116, 'e': 149, '!': 220, 'z': 100, 'r': 45, 'a': 36, 'm': 28, 'y': 24,
+    'n': 13, 'i': 36, 's': 43, 'h': 38, 'g': 4, 'b': 10, 'q': 1, 'k': 3, 'u': 6,
+    'f': 1, 'j': 4, 'v': 2, 'c': 1, 't': 2, 'w': 1
   },
-  'js': {'k': 1, 'e': 1, 'i': 1, 'a': 1, 'n': 1},
-  'jt': {'o': 2, 'c': 1, 'k': 2, 'a': 8, '!': 1, 'e': 1},
-  'Ju': {
-    'a': 8, 's': 20, 'd': 11, 'n': 36, 'l': 22, 'r': 37, 'm': 5, 'h': 4,
-    'e': 12, 'c': 2, 't': 2, 'p': 2, 'b': 11, 'k': 2, '!': 1, 'i': 2, 'g': 2,
-    'v': 3, 'u': 1, 'z': 1, 'f': 1
+  'ah': {
+    'a': 163, 'n': 70, 'o': 57, 'u': 23, '!': 103, 'l': 139, 'i': 46, 'e': 59,
+    'y': 7, 'r': 51, 'm': 36, 't': 5, 's': 7, 'p': 1, 'd': 4, 'b': 2, 'h': 1,
+    'f': 1, 'k': 2
   },
-  'ju': {
-    'n': 6, 'a': 1, '!': 3, 'l': 6, 'r': 4, 'e': 4, 's': 2, 'c': 3, 't': 1, 
-    'd': 1
+  'Su': {
+    'l': 47, 't': 35, 'm': 60, 'a': 5, 'g': 22, 'n': 39, 'r': 46, 'b': 15,
+    'z': 1, '!': 1, 'h': 4, 'd': 26, 's': 25, 'i': 9, 'p': 11, 'e': 14, 'y': 3,
+    'c': 15, 'f': 3, 'o': 6, 'k': 8, 'w': 1, 'v': 1
   },
-  'jw': {'a': 2},
-  'jy': {'!': 1},
-  'jz': {'!': 1, 'a': 1, 'i': 1},
-  'Ka': {
-    'n': 84, 'u': 39, 't': 56, 'i': 24, 'p': 46, 'y': 13, 'h': 28, 'm': 70,
-    'r': 131, 's': 88, 'v': 10, 'o': 2, 'c': 23, 'e': 17, 'l': 124, 'g': 10,
-    'd': 19, 'w': 19, 'b': 17, 'z': 22, 'f': 5, 'k': 10, 'a': 13, 'j': 2, '!': 1
+  'ul': {
+    'l': 366, 't': 167, '!': 56, 'k': 53, 'd': 60, 'e': 127, 'v': 17, 's': 66,
+    'z': 11, 'i': 159, 'p': 10, 'b': 27, 'm': 18, 'c': 21, 'o': 76, 'a': 146,
+    'h': 14, 'x': 3, 'f': 16, 'u': 15, 'g': 13, 'w': 10, 'y': 9, 'n': 11,
+    'r': 8, 'j': 1, 'q': 1
   },
-  'ka': {
-    'y': 12, 'g': 8, 'r': 96, '!': 361, 'm': 85, 'b': 15, 's': 68, 'h': 9,
-    'n': 56, 'w': 16, 'i': 17, 'c': 13, 'd': 11, 'l': 50, 'k': 7, 't': 14,
-    'f': 8, 'u': 15, 'z': 1, 'a': 6, 'o': 3, 'v': 5, 'p': 4, 'j': 5, 'e': 2
+  'We': {
+    's': 115, 'l': 68, 'b': 9, 'a': 49, 'i': 167, 'e': 28, 'r': 57, 't': 26,
+    'n': 77, 'd': 28, 'g': 16, 'x': 2, 'y': 17, 'c': 10, 'h': 26, 'v': 1,
+    'm': 7, 'p': 1, 'k': 2, 'f': 1, 'u': 1, 'w': 1
   },
-  'kb': {
-    'u': 6, 'a': 7, 'e': 13, 'r': 3, 's': 1, 'y': 1, 'i': 5, 'o': 4, 'l': 1
+  'Ow': {'e': 5, 'i': 1, 's': 2, 'n': 4, 'u': 1, 'c': 2, 'o': 2, '!': 1},
+  'yn': {
+    'o': 32, 'e': 125, 'c': 3, 'n': 16, 'a': 36, 'u': 5, 'h': 5, 't': 12,
+    '!': 68, 'i': 15, 'd': 20, 'k': 5, 's': 55, 'g': 9, 'v': 1
   },
-  'kc': {'o': 3, 'e': 1},
-  'kd': {'a': 4, 'o': 2, 'u': 1, 'i': 1, 'e': 2, 'y': 1},
-  'Ke': {
-    'l': 79, 'n': 95, 'i': 43, 'm': 45, 'r': 88, 'y': 14, 's': 32, 'e': 60,
-    'a': 59, 'c': 4, 't': 43, 'h': 11, 'p': 14, 'o': 13, 'f': 2, 'g': 6, 'd': 6,
-    'v': 9, 'b': 7, 'z': 3, 'k': 4, '!': 1, 'w': 4, 'u': 3, 'x': 1
+  'no': {
+    'l': 76, '!': 1118, 'z': 18, 'n': 136, 'r': 102, 'w': 119, 'x': 3, 'v': 72,
+    't': 66, 's': 109, 'u': 54, 'i': 15, 'j': 3, 'd': 15, 'h': 14, 'y': 18,
+    'o': 15, 'c': 49, 'f': 33, 'p': 19, 'g': 10, 'e': 19, 'm': 17, 'b': 11,
+    'a': 4, 'k': 7
   },
-  'ke': {
-    'r': 759, '!': 680, 's': 130, 'n': 323, 'e': 35, 't': 101, 'y': 170,
-    'w': 10, 'l': 272, 'f': 8, 'o': 3, 'a': 12, 'm': 50, 'd': 5, 'c': 3, 'b': 9,
-    'u': 2, 'i': 5, 'h': 6, 'p': 2, 'k': 2, 'g': 3, 'v': 7, 'z': 1
+  'ld': {
+    's': 59, '!': 531, 'w': 10, 'e': 256, 'o': 95, 'r': 69, 'b': 9, 'm': 15,
+    'i': 94, 'a': 74, 'h': 14, 'u': 17, 't': 51, 'f': 11, 'y': 11, 'n': 12,
+    'g': 3, 'v': 3, 'k': 6, 'p': 1, 'c': 1
   },
-  'kf': {'o': 16, 'i': 9, 'e': 2},
-  'kg': {'r': 1, 'o': 1},
-  'Kh': {'a': 33, 'o': 14, 'i': 3, 'e': 5, 'u': 4, 'n': 1, 'l': 1},
-  'kh': {
-    'a': 76, 'o': 44, 'u': 9, 'e': 11, '!': 4, 'i': 12, 't': 4, 'm': 2, 'l': 1,
-    'r': 1, 's': 1
+  'Fi': {
+    's': 43, 'e': 40, 't': 41, 'g': 32, 'n': 99, 'o': 23, 'f': 3, 'k': 2,
+    'x': 3, 'l': 78, 'd': 9, 'c': 26, 'r': 19, 'a': 9, 'z': 1, 'q': 1, 'm': 2,
+    'v': 2, 'u': 3, 'j': 2, 'p': 1, 'w': 1
   },
-  'Ki': {
-    'n': 156, 'm': 48, 'r': 90, 'd': 10, 'l': 96, 's': 45, 't': 45, 'e': 60,
-    'p': 14, 'z': 7, 'b': 10, 'g': 4, 'f': 4, 'k': 4, 'v': 6, 'c': 6, 'j': 3,
-    'a': 3, 'o': 2, 'h': 2, 'y': 2, 'i': 1
+  'El': {
+    'l': 90, 'd': 14, 'm': 11, 'k': 10, 'i': 31, 'a': 6, 'y': 1, 'r': 5,
+    's': 29, 'w': 8, 'e': 15, 'g': 9, 'b': 10, 't': 5, 'z': 5, 'v': 8, 'f': 8,
+    '!': 1, 'c': 2, 'h': 6, 'o': 2, 'u': 1, 'p': 1, 'n': 1, 'q': 1
   },
-  'ki': {
-    'n': 457, '!': 1404, 'd': 4, 'r': 23, 'p': 3, 'l': 41, 'e': 91, 's': 58,
-    'b': 12, 'f': 3, 'm': 15, 't': 13, 'y': 3, 'v': 3, 'c': 9, 'j': 1, 'h': 3,
-    'u': 2, 'o': 3, 'z': 1, 'k': 2, 'w': 2, 'a': 11, 'g': 1
+  'Gi': {
+    'b': 25, 'l': 153, 'v': 7, 'p': 5, 'f': 7, 'r': 45, 'o': 26, 's': 14,
+    'n': 39, 'd': 10, 'e': 43, 'g': 12, 't': 20, 'a': 76, 'u': 12, 'm': 8,
+    'z': 4, 'c': 4, 'h': 1
   },
-  'Kj': {'o': 2, 'e': 7, 'a': 1},
-  'kj': {'y': 1, 'e': 1, 'i': 2},
-  'kk': {'e': 34, 'i': 11, 'a': 11, 'o': 7, 'h': 1, 'u': 1},
-  'Kl': {'e': 104, 'i': 74, 'u': 35, 'o': 44, 'a': 65, 'y': 3, 'j': 1},
-  'kl': {'i': 59, 'a': 38, 'e': 310, 'u': 13, 'y': 7, 'o': 18, '!': 10, 'v': 1},
-  'km': {'a': 118, 'o': 14, 'e': 17, 'u': 1, 'i': 3},
-  'Km': {'e': 3, 'i': 3, 'a': 2},
-  'Kn': {'i': 47, 'o': 59, 'a': 38, 'u': 16, 'e': 34, 'k': 1, 'y': 1},
-  'kn': {'i': 7, 'e': 69, 'a': 11, 'o': 8, '!': 1},
-  'Ko': {
-    'c': 34, 'e': 66, 'h': 32, 'w': 23, 'l': 83, 'o': 29, 'p': 51, 'z': 34,
-    'v': 27, 'n': 63, 'r': 93, 's': 96, 'b': 27, '!': 1, 'g': 8, 'u': 27,
-    't': 51, 'm': 22, 'f': 13, 'k': 10, 'i': 5, 'j': 1, 'd': 7, 'y': 3
+  'ib': {
+    's': 6, 'b': 98, 'e': 133, 'o': 36, 'l': 52, 'a': 70, 'n': 6, '!': 24,
+    'u': 16, 'i': 25, 'r': 15, 'd': 1, 'y': 5, 'm': 4, 'f': 1, 'w': 1, 'k': 1,
+    'g': 1, 't': 1
   },
-  'ko': {
-    'u': 11, 'w': 227, 'y': 3, 'f': 27, 'l': 45, 'r': 46, '!': 257, 'x': 1,
-    'k': 6, 'p': 27, 'o': 8, 'v': 73, 't': 14, 's': 69, 'g': 7, 'b': 5, 'e': 3,
-    'n': 27, 'd': 5, 'm': 8, 'c': 10, 'j': 2, 'a': 2, 'h': 4, 'i': 1, 'z': 1
+  'bs': {
+    'o': 18, '!': 67, 't': 20, 'e': 7, 'h': 7, 'b': 1, 'c': 8, 'k': 11, 'm': 1,
+    'a': 5, 'w': 1, 'i': 1
   },
-  'kp': {'a': 3, 'o': 1, 'e': 1},
-  'kq': {'u': 1},
-  'Kr': {
-    'a': 132, 'u': 73, 'e': 101, 'i': 75, 'o': 80, 'z': 14, 'y': 16, 's': 1, 
-    'n': 1
+  'Mc': {
+    'd': 62, 'c': 420, 'k': 139, 'g': 190, 'b': 25, 'l': 65, 'i': 36, 'm': 73,
+    'n': 71, 'f': 32, 'p': 24, 'a': 56, 'e': 63, 'q': 31, 'w': 21, 'r': 21,
+    'h': 14, 'v': 11, 's': 18, 'j': 2, 't': 13, 'z': 1, 'o': 4, '!': 1, 'u': 1
   },
-  'kr': {'e': 25, 'i': 22, 'u': 7, 'a': 30, 'z': 4, 'o': 18, 'y': 2, '!': 2},
-  'Ks': {'i': 1, 'h': 1, 'z': 1},
-  'ks': {
-    'o': 54, '!': 206, 'd': 1, 't': 49, 'e': 26, 'h': 21, 'c': 6, 'l': 5,
-    'b': 4, 'w': 2, 's': 1, 'm': 5, 'a': 5, 'i': 9, 'y': 1, 'k': 2
+  'cd': {'o': 30, 'a': 19, 'e': 15, 'u': 9, 'i': 5},
+  'do': {
+    'n': 274, 'z': 11, '!': 419, 'v': 28, 'w': 59, 'l': 78, 'x': 3, 'm': 31,
+    'c': 29, 'r': 189, 'i': 9, 'u': 35, 's': 35, 'y': 8, 'o': 12, 'b': 3,
+    'p': 4, 'g': 2, 't': 11, 'e': 9, 'h': 4, 'f': 7, 'a': 1, 'k': 4
   },
-  'kt': {'o': 7, 'a': 3, 'e': 3, '!': 2, 'n': 1, 'i': 1, 'h': 1, 's': 1},
-  'Ku': {
-    'h': 29, 'r': 59, 'y': 5, 'n': 47, 'm': 12, 'e': 27, 't': 24, 'j': 7,
-    '!': 1, 's': 36, 'c': 31, 'g': 2, 'l': 41, 'b': 46, 'o': 2, 'z': 15, 'i': 7,
-    'k': 16, 'a': 8, 'p': 17, 'd': 14, 'f': 6, 'w': 3
+  'Cr': {'u': 69, 'a': 132, 'o': 169, 'e': 103, 'i': 103, 'y': 10, 'n': 2},
+  'ru': {
+    'z': 36, 'c': 81, 'i': 34, 'j': 5, 'm': 177, 'e': 88, 'f': 19, 'n': 136,
+    'g': 39, 'b': 48, 's': 134, 'o': 5, 't': 59, 'r': 2, 'd': 71, 'a': 9,
   },
-  'ku': {
-    's': 54, 'p': 8, 'm': 20, 'l': 26, 'b': 11, 'c': 7, 'd': 3, 'h': 5, '!': 11,
-    'r': 12, 't': 14, 'k': 2, 'i': 2, 'n': 13, 'e': 3, 'f': 1, 'a': 4, 'o': 1, 
-    'y': 1
+  'uz': {
+    '!': 28, 'm': 12, 'a': 33, 'c': 2, 'u': 4, 'z': 79, 'o': 7, 'i': 35, 't': 1,
+    'b': 4, 'y': 6, 'e': 27, 'l': 1, 'q': 1, 'n': 4, 'h': 1, 's': 1
   },
-  'Kv': {'a': 3, 'i': 1, 'z': 1, 'o': 1, 'e': 3},
-  'kv': {'e': 3, 'l': 1, 'i': 2},
-  'Kw': {'a': 10, 'o': 3, 'i': 6, 'e': 1},
-  'kw': {'e': 14, 'o': 14, 'i': 10, 'a': 19, 'r': 1, 'u': 2},
-  'kx': {'!': 2, 't': 1, 'l': 1},
-  'ky': {'!': 375, 'l': 1, 'e': 5, 'a': 6, 'n': 3, 'b': 1, 'm': 1, 't': 1},
-  'Ky': {
-    'l': 5, 's': 3, 't': 2, 'z': 2, 'g': 1, 'e': 2, 'k': 1, 'u': 1, 'n': 3,
-    'm': 1, '!': 1, 'h': 1, 'p': 2
+  'Or': {
+    't': 34, 'r': 12, 'o': 18, 'n': 12, 'l': 18, 'e': 29, 'd': 20, 'c': 4,
+    'a': 15, 'm': 12, 's': 12, 'g': 7, 'v': 2, 'i': 20, 'b': 5, 'z': 5, 'w': 3,
+    'u': 1, 'y': 1, 'k': 3, 'f': 3, 'p': 3, 'j': 1, '!': 1, 'h': 1
   },
-  'kz': {'a': 1, 'e': 1, 'd': 1},
-  'La': {
-    'n': 287, 'w': 48, 'r': 132, 'm': 167, 'k': 13, 't': 79, 'c': 79, 'd': 37,
-    'y': 23, 'i': 33, 's': 95, 'u': 138, 'v': 72, 'p': 68, 'f': 73, 'b': 81,
-    'h': 21, 'l': 29, 'j': 7, 'z': 38, 'g': 64, 'o': 3, 'x': 4, '!': 1, 'a': 8,
-    'q': 2, 'e': 4
+  'iz': {
+    '!': 60, 'e': 59, 'a': 67, 'z': 79, 'o': 25, 'u': 16, 'i': 31, 'c': 4,
   },
-  'la': {
-    'r': 352, 'c': 182, 'n': 884, 's': 283, 'z': 62, 'i': 114, 'k': 111,
-    '!': 907, 'u': 124, 'y': 95, 'g': 102, 'h': 62, 'p': 41, 't': 160, 'l': 39,
-    'm': 158, 'd': 116, 'w': 60, 'b': 51, 'v': 69, 'f': 45, 'a': 21, 'x': 6,
-    'o': 10, 'e': 24, 'q': 4, 'j': 9
+  'Fr': {'e': 183, 'a': 200, 'o': 61, 'y': 17, 'i': 140, 'u': 26},
+  'eb': {
+    'b': 33, 'e': 276, 's': 21, 'l': 44, 'r': 95, 'v': 1, 'a': 111, 'o': 83,
+    'u': 44, 'y': 18, '!': 38, 'n': 11, 'h': 6, 'k': 4, 'i': 35, 'm': 2, 'w': 1,
+    'd': 3, 'g': 1, 'c': 1
   },
-  'lb': {
-    'e': 195, 'r': 73, 'o': 55, 'u': 35, 'y': 22, '!': 13, 'a': 86, 'i': 23,
-    'l': 5, 'f': 1, 'n': 1
+  'bb': {
+    '!': 35, 'a': 31, 'i': 59, 's': 35, 'o': 24, 'e': 104, 'y': 17, 'l': 26,
+    'r': 5, 'u': 1
   },
-  'lc': {
-    'h': 85, 'o': 81, 'e': 20, 'i': 22, 'a': 45, 'z': 18, 'r': 11, 'u': 12,
-    'k': 9, 'l': 2, '!': 4, 'y': 3
+  'ev': {
+    'e': 325, 'i': 183, 'y': 7, 'a': 116, 'o': 43, 'l': 7, 'r': 14, '!': 11,
+    's': 7, 'c': 1, 'w': 2, 'n': 2, 'u': 1, 't': 1, 'k': 1, 'j': 1
   },
-  'ld': {
-    's': 59, '!': 531, 'w': 10, 'e': 256, 'o': 95, 'r': 69, 'b': 9, 'm': 15,
-    'i': 94, 'a': 74, 'h': 14, 'u': 17, 't': 51, 'f': 11, 'y': 11, 'n': 12,
-    'g': 3, 'v': 3, 'k': 6, 'p': 1, 'c': 1
+  'uc': {
+    'k': 270, 'a': 48, 'h': 303, 'e': 51, '!': 12, 'i': 50, 'o': 15, 'y': 4,
+    'c': 152, 'l': 5, 'u': 6, 'z': 19, 'm': 1, 'r': 2, 'w': 1, 'n': 1, 'v': 1,
+    't': 1, 'g': 1
   },
-  'le': {
-    'r': 1331, 'n': 513, 'z': 45, 'y': 1007, 'm': 186, 's': 596, 'x': 26,
-    '!': 1423, 't': 354, 'i': 150, 'o': 38, 'g': 69, 'a': 110, 'v': 49, 'd': 50,
-    'l': 37, 'j': 23, 'f': 39, 'e': 129, 'u': 32, 'b': 82, 'c': 98, 'h': 35,
-    'w': 72, 'k': 59, 'p': 32, 'q': 1
+  'aw': {
+    'f': 5, '!': 160, 'k': 21, 'r': 18, 's': 34, 'y': 8, 'a': 141, 't': 16,
+    'l': 47, 'e': 42, 'h': 14, 'c': 10, 'o': 10, 'n': 19, 'i': 27, 'v': 4,
+    'b': 9, 'g': 2, 'd': 16, 'w': 4, 'u': 2, 'm': 3
   },
-  'Le': {
-    'w': 27, 'e': 38, 'o': 34, 's': 71, 'b': 44, 'a': 83, 'v': 96, '!': 1,
-    'h': 38, 'd': 42, 'm': 69, 'n': 97, 'g': 60, 'y': 20, 'c': 44, 'i': 111,
-    'u': 23, 'r': 22, 'f': 36, 't': 42, 'j': 5, 'p': 28, 'l': 11, 'z': 7,
-    'x': 2, 'q': 1, 'k': 7
+  'wf': {'o': 4, 'i': 1, '!': 1, 'e': 1},
+  'fo': {
+    'r': 345, 'o': 17, 'n': 41, 'y': 6, 'u': 13, '!': 32, 'l': 20, 'x': 3,
+    's': 11, 'e': 4, 'h': 1, 'g': 1, 't': 1, 'i': 2, 'a': 1
   },
-  'lf': {
-    'e': 50, '!': 42, 'o': 57, 'f': 9, 'a': 26, 'r': 23, 's': 14, 'i': 44,
-    'g': 4, 'l': 8, 'h': 1, 'm': 2, 'u': 3, 'y': 2, 't': 1
+  'nr': {'y': 9, 'o': 34, 'a': 21, 'i': 57, 'u': 9, 'e': 19, 'r': 4, 'h': 1},
+  'Bo': {
+    'y': 50, 'w': 65, 'o': 51, 'n': 162, 'l': 114, 'u': 148, 'g': 54, 's': 82,
+    'r': 189, 'x': 7, 'b': 36, 'h': 53, 'c': 44, 'e': 82, 't': 61, 'z': 21,
+    'i': 30, 'a': 28, 'd': 55, 'v': 13, 'j': 4, 'm': 21, 'p': 2, 'q': 2, 'k': 8,
+    'f': 2, '!': 1
   },
-  'lg': {
-    'a': 46, 'o': 19, 'u': 10, 'e': 54, 'r': 30, 'h': 5, 'i': 14, 'l': 2,
-    'n': 1, '!': 3, 'v': 1, 'y': 1
+  'oy': {
+    'd': 22, '!': 137, 'l': 28, 'a': 53, 'e': 69, 'c': 6, 'n': 31, 'o': 16,
+    't': 14, 'k': 6, 's': 19, 'b': 2, 'i': 3, 'u': 1, 'h': 1, 'm': 2
   },
-  'Lh': {'e': 1, 'u': 1, 'o': 1},
-  'lh': {'o': 67, 'e': 28, 'i': 15, 'a': 60, 'u': 12, 'y': 1, 'j': 1},
-  'li': {
-    'a': 233, 'p': 94, 'n': 1348, 'v': 76, 's': 293, 'o': 178, 'e': 255,
-    'f': 77, 'x': 10, 'g': 91, 'd': 34, 'c': 303, '!': 459, 'u': 21, 'l': 33,
-    'z': 36, 'k': 74, 't': 113, 'm': 85, 'b': 36, 'h': 19, 'r': 9, 'w': 8,
-    'i': 11, 'q': 2, 'j': 2
+  'yd': {
+    '!': 20, 'e': 58, 'o': 15, 'n': 5, 's': 2, 'a': 23, 'r': 4, 'b': 1, 'i': 8,
+    't': 5, 'l': 6, 'z': 2, 'g': 1, 'm': 2, 'u': 4, 'd': 1
   },
-  'Li': {
-    't': 60, 'n': 198, 'v': 34, 'l': 32, 'g': 30, 'm': 31, '!': 1, 'p': 56,
-    'b': 25, 'u': 5, 'r': 5, 's': 47, 'e': 73, 'd': 18, 'a': 10, 'z': 12,
-    'c': 48, 'k': 7, 'o': 9, 'j': 1, 'q': 2, 'f': 12, 'w': 1, 'i': 1
+  'dy': {
+    '!': 276, 'k': 17, 'a': 5, 'e': 4, 'c': 4, 'n': 4, 's': 7, 'u': 1, 'l': 1,
+    'g': 3, 'v': 2, 'm': 3, 'd': 1, 'b': 1, 'o': 1, 'f': 1
   },
-  'lj': {'e': 8, 'u': 2, 'a': 6, '!': 1, 'o': 2},
-  'Lj': {'u': 1},
-  'lk': {
-    'e': 146, 'i': 57, 'n': 9, '!': 68, 's': 13, 'm': 7, 'u': 7, 'o': 56,
-    'l': 5, 'a': 45, 'c': 1, 'w': 2, 'h': 2, 'b': 2, 'r': 1, 'k': 1, 'y': 1
+  'ix': {
+    'o': 11, '!': 61, 's': 8, 'l': 3, 'e': 9, 'b': 1, 'i': 7, 't': 8, 'n': 3,
+    'k': 1, 'a': 5, 'd': 1
   },
-  'll': {
-    'i': 1117, 'e': 1235, '!': 1626, 'y': 110, 'a': 965, 's': 116, 'o': 707,
-    'm': 136, 'u': 68, 'w': 30, 'r': 13, 'g': 15, 'n': 30, 'h': 28, 'c': 11,
-    'z': 1, 'b': 39, 'd': 5, 'f': 10, 'p': 7, 'v': 2, 't': 2, 'q': 1, 'j': 1, 
-    'k': 1
+  'xo': {'n': 22, 'm': 2, 'p': 1, 't': 1, 'l': 1, '!': 1},
+  'Sh': {
+    'a': 265, 'e': 249, 'o': 125, 'i': 179, 'u': 99, 'r': 36, 'y': 5, 'k': 1,
+    'm': 1, 'v': 1, 'w': 1, 'b': 1
   },
-  'Ll': {'o': 5, 'e': 5, 'a': 11, 'y': 1},
   'lm': {
     'e': 132, 'o': 81, 'a': 339, 's': 22, '!': 59, 'i': 35, 'q': 6, 'b': 7,
     'g': 3, 'u': 15, 'y': 6, 'l': 5, 'k': 2, 'r': 1, 'c': 1
   },
-  'ln': {
-    '!': 8, 'e': 50, 'a': 16, 'i': 31, 'u': 4, 'y': 3, 'h': 1, 'o': 7, 'n': 1
+  'Bl': {'a': 218, 'e': 62, 'u': 39, 'o': 85, 'i': 35, 'y': 10},
+  'ni': {
+    'e': 237, 'g': 113, 'n': 305, 's': 217, 'd': 17, 'z': 21, 'l': 28, 't': 62,
+    'p': 21, 'c': 287, '!': 596, 'o': 88, 'a': 121, 'h': 7, 'x': 19, 'k': 107,
+    'q': 5, 'f': 36, 'm': 18, 'v': 12, 'u': 19, 'b': 12, 'r': 10, 'w': 3, 'y': 2
   },
-  'Lo': {
-    'p': 27, 'n': 83, 'w': 38, 'v': 62, 'g': 26, 't': 30, 'z': 17, 'c': 60,
-    'r': 79, 'u': 82, 'o': 25, 'y': 12, 'f': 35, 'm': 33, '!': 1, 'e': 42,
-    'h': 22, 'd': 11, 'l': 11, 'i': 10, 's': 48, 'k': 13, 'b': 30, 'a': 10,
-    'x': 3, 'q': 1, 'j': 1
+  'ie': {
+    'l': 538, 'r': 893, 'n': 218, '!': 598, 'v': 36, 'd': 157, 's': 283,
+    'g': 91, 't': 151, 'u': 25, 'h': 32, 'w': 94, 'f': 62, 'b': 109, 'i': 1,
   },
-  'lo': {
-    'r': 145, '!': 638, 'v': 60, 'n': 270, 'w': 246, 'y': 24, 'c': 141, 'a': 17,
-    'm': 103, 'u': 96, 'o': 51, 'b': 14, 's': 200, 'g': 28, 'd': 25, 'i': 17,
-    't': 132, 'p': 32, 'e': 43, 'z': 11, 'q': 2, 'h': 22, 'f': 44, 'x': 4,
-    'k': 10, 'j': 1, 'l': 1
+  'Ni': {
+    'c': 103, 'x': 5, 'e': 82, 'l': 12, 'n': 14, 's': 34, 'g': 16, 'p': 7,
+    'm': 13, 'v': 8, 't': 19, 'd': 4, 'b': 7, 'k': 13, 'z': 4, 'w': 1, 'h': 3,
+    'a': 3, '!': 1, 'u': 1, 'f': 3, 'i': 2, 'r': 4, 'q': 1
   },
-  'lp': {
-    's': 4, 'h': 44, 'a': 23, 'e': 26, '!': 17, 'i': 22, 'o': 13, 'r': 5,
-    'l': 2, 'm': 1, 'u': 2, 'p': 2, 'f': 1
+  'Kn': {'i': 47, 'o': 59, 'a': 38, 'u': 16, 'e': 34, 'k': 1, 'y': 1},
+  'Fe': {
+    'r': 164, 'l': 94, 'n': 58, 'e': 24, 'a': 33, 't': 22, 'd': 36, 'c': 11,
+    'i': 40, 'w': 3, 'y': 5, 's': 18, 'h': 14, 'b': 7, 'u': 10, 'g': 11, 'k': 2,
+    'o': 2, 'm': 5, 'j': 1, 'v': 2, 'q': 1, 'f': 1
   },
-  'lq': {'u': 22},
-  'lr': {'o': 30, 'e': 15, 'i': 21, 'y': 3, 'a': 13, 'u': 2, 'k': 1, '!': 1},
-  'ls': {
-    'o': 144, '!': 247, 'h': 30, 'e': 97, 't': 145, 'w': 9, 'k': 94, 'b': 31,
-    'c': 29, 'a': 31, 'z': 2, 's': 6, 'u': 2, 'i': 26, 'n': 2, 'l': 6, 'm': 14,
-    'p': 7, 'd': 6, 'f': 2, 'g': 5, 'r': 2, 'v': 1, 'y': 1
+  'wk': {'i': 11, '!': 5, 's': 4, 'e': 9, 'a': 10, 'w': 1, 'o': 2},
+  'Du': {
+    'n': 108, 'r': 94, 'd': 26, 'k': 15, 'f': 30, 'b': 57, 'a': 4, 'p': 35,
+    'm': 34, 'g': 20, 'v': 8, 't': 27, 'c': 43, 'o': 3, 'l': 27, 'e': 33,
+    'q': 3, 'h': 9, 's': 32, '!': 1, 'w': 2, 'z': 1, 'x': 2, 'i': 5, 'y': 2
   },
-  'lt': {
-    'o': 116, 'e': 149, '!': 220, 'z': 100, 'r': 45, 'a': 36, 'm': 28, 'y': 24,
-    'n': 13, 'i': 36, 's': 43, 'h': 38, 'g': 4, 'b': 10, 'q': 1, 'k': 3, 'u': 6,
-    'f': 1, 'j': 4, 'v': 2, 'c': 1, 't': 2, 'w': 1
+  'ud': {
+    's': 10, 'l': 25, '!': 94, 'o': 34, 'i': 78, 'd': 61, 'e': 177, 'r': 32,
+    'w': 8, 'g': 20, 'k': 7, 'y': 24, 'a': 67, 'n': 20, 't': 11, 'h': 8, 'j': 3,
+    'u': 4, 'z': 19, 'f': 1, 'm': 10, 'b': 4, 'v': 3
   },
-  'Lu': {
-    'c': 79, 'n': 56, 't': 35, 'g': 9, 's': 21, 'j': 2, 'd': 29, 'k': 27,
-    'm': 23, '!': 1, 'o': 5, 'i': 10, 'e': 45, 'p': 21, 'u': 1, 'x': 5, 'b': 23,
-    'f': 7, 'z': 10, 'r': 10, 'q': 3, 'h': 7, 'y': 2, 'l': 7, 'a': 9, 'v': 5
+  'Sp': {
   },
-  'lu': {
-    'r': 15, 'm': 98, 'e': 39, 'c': 52, 'p': 17, 'n': 99, 'g': 21, 's': 81,
-    'k': 18, 'h': 6, 'f': 6, 'd': 11, 'b': 12, 't': 31, 'z': 15, 'i': 10,
-    '!': 14, 'l': 3, 'o': 2, 'v': 5, 'a': 10, 'y': 3, 'x': 2, 'w': 1, 'q': 2, 
-    'j': 1
+  'dn': {'e': 89, 'a': 17, 'i': 24, 'o': 11, 'y': 3, '!': 2, 'g': 1, 'u': 1},
+  'ep': {
+    'h': 40, 'p': 137, 'a': 52, 'e': 68, '!': 31, 'u': 11, 'c': 3, 'l': 25,
+    'r': 16, 'i': 32, 's': 15, 'o': 19, 'b': 2, 'n': 9, 'k': 23, 'w': 1,
+    't': 12, 'y': 3, 'f': 18, 'v': 1
   },
-  'lv': {'a': 85, 'e': 135, 'i': 70, 'o': 17, 'y': 6, 'r': 1, 'u': 1, 's': 1},
-  'Lw': {'e': 1},
-  'lw': {'o': 23, 'e': 24, 'a': 35, 'i': 21, 'h': 1, 'r': 3, 'y': 2, 's': 1},
-  'lx': {'!': 3},
-  'ly': {
-    '!': 384, 'n': 30, 't': 7, 'e': 25, 'd': 3, 'b': 2, 'l': 3, 'a': 20,
-    'm': 14, 'k': 3, 'f': 2, 'o': 9, 's': 7, 'w': 5, 'c': 3, 'g': 1, 'z': 3,
-    'u': 2, 'q': 1, 'h': 1
+  'Pi': {
+    'e': 89, 't': 52, 'c': 96, 'k': 8, 'n': 110, 'p': 17, 'm': 6, 'l': 61,
+    'a': 19, 'g': 22, 'r': 26, 'z': 22, 's': 30, 'f': 1, 'o': 10, 'x': 2,
+    'd': 3, 'q': 2, 'w': 2, 'h': 3, 'v': 2, 'j': 1, 'u': 2, '!': 1, 'i': 1
   },
-  'Ly': {
-    'n': 26, 'o': 2, 'l': 2, '!': 1, 't': 7, 'm': 5, 'k': 8, 'd': 9, 'b': 6,
-    'a': 4, 'f': 1, 'v': 1, 's': 10, 'e': 5, 'c': 2
+  'ws': {
+    '!': 40, 'o': 21, 't': 7, 'e': 20, 'k': 491, 'l': 2, 'b': 2, 'h': 4, 'm': 1,
+    'u': 1, 'a': 2
   },
-  'lz': {
-    '!': 55, 'e': 50, 'a': 17, 'm': 7, 'i': 11, 'o': 8, 'y': 2, 'w': 4, 'g': 1,
-    'h': 4, 'b': 3, 'l': 5, 'u': 2, 'r': 1, 'n': 2
+  'Ar': {
+    'n': 53, 'm': 56, 'r': 57, 'c': 49, 't': 38, 'i': 35, 'e': 42, 'a': 47,
+    's': 6, 'b': 18, 'd': 23, 'o': 23, 'g': 34, 'w': 1, 'v': 15, 'z': 8, 'p': 4,
+    'l': 10, 'y': 2, 'j': 3, 'q': 5, 'k': 9, 'u': 5, 'f': 2, 'h': 2, '!': 1
   },
-  'Ma': {
-    'r': 622, 's': 183, 't': 247, 'y': 79, 'n': 347, 'c': 252, 'l': 225,
-    'x': 18, 'd': 99, 'h': 68, 'g': 128, 'j': 33, 'u': 67, 'b': 22, 'i': 80,
-    'p': 12, 'e': 23, '!': 1, 'a': 12, 'k': 33, 'z': 58, 'f': 10, 'o': 4,
-    'w': 6, 'v': 12, 'm': 17, 'q': 1
+  'ag': {
+    'n': 127, 'o': 126, 'e': 332, 'h': 52, 'a': 249, 'u': 86, 'g': 121,
+    'l': 148, 's': 12, 'w': 6, '!': 43, 'y': 14, 'b': 7, 'i': 68, 'r': 43,
+    'd': 11, 'm': 11, 't': 8, 'p': 3, 'j': 1
   },
-  'ma': {
-    's': 125, 'n': 2414, 'l': 69, 'c': 67, 'h': 13, 'r': 273, 'k': 62, 'y': 44,
-    'x': 2, 'd': 40, '!': 276, 't': 62, 'm': 5, 'i': 53, 'g': 37, 'z': 8,
-    'e': 8, 'w': 3, 'u': 23, 'v': 6, 'b': 4, 'o': 5, 'a': 5, 'j': 5, 'p': 1, 
-    'q': 1
+  'gn': {'e': 103, 'o': 80, 'u': 5, 'y': 5, 'a': 83, 'i': 39, '!': 4, 's': 2},
+  'tk': {
+    'i': 30, 'e': 43, 'o': 65, 'a': 25, 'y': 2, 'n': 1, 'u': 8, 'r': 1, 'l': 1},
+  'Ol': {
+    's': 11, 'i': 47, 'e': 28, 'd': 19, 'v': 6, 'm': 9, 'n': 3, 'g': 3, 'a': 16,
+    'l': 18, 'o': 5, 't': 8, 'b': 2, 'c': 3, 'p': 2, 'k': 2, 'u': 3, 'r': 1,
+    'q': 1, 'y': 1, 'w': 1, 'h': 1, 'f': 1
   },
-  'mb': {
-    'e': 219, '!': 43, 's': 13, 'l': 89, 'a': 118, 'r': 118, 'y': 15, 'o': 70,
-    'i': 39, 'u': 45, 'd': 2, 'h': 3, 'k': 3, 't': 1, 'c': 1
+  'ca': {
+    'n': 138, 's': 75, 'r': 271, 'l': 134, 'd': 28, 'b': 12, '!': 219, 'i': 20,
+    'u': 22, 'm': 51, 'f': 16, 'h': 7, 'v': 21, 't': 47, 'y': 12, 'g': 16,
+    'w': 2, 'z': 6, 'a': 1, 'p': 13, 'k': 11, 'c': 9, 'j': 4, 'o': 5, 'e': 2
   },
-  'Mb': {'o': 1, 'a': 1},
-  'Mc': {
-    'd': 62, 'c': 420, 'k': 139, 'g': 190, 'b': 25, 'l': 65, 'i': 36, 'm': 73,
-    'n': 71, 'f': 32, 'p': 24, 'a': 56, 'e': 63, 'q': 31, 'w': 21, 'r': 21,
-    'h': 14, 'v': 11, 's': 18, 'j': 2, 't': 13, 'z': 1, 'o': 4, '!': 1, 'u': 1
+  'Sn': {'y': 2, 'o': 25, 'i': 11, 'e': 29, 'a': 13, 'u': 2},
+  'ny': {
+    'd': 4, '!': 184, 'o': 14, 'e': 21, 'a': 33, 's': 3, 'p': 1, 'w': 1, 'k': 2,
+    'g': 1, 'u': 1, 'c': 1, 'n': 1, 'm': 1, 'l': 1, 'i': 5, 'z': 1, 'r': 1
   },
-  'mc': {'o': 4, 'z': 7, 'h': 14, 'k': 1, 'a': 2, '!': 1, 'i': 2},
-  'md': {'e': 8, 'a': 8, 'i': 4, 'n': 2},
-  'me': {
-    's': 137, 'z': 14, 'r': 684, 'n': 233, '!': 179, 'y': 139, 'l': 202, 'w': 5,
-    'i': 90, 'd': 37, 'o': 14, 't': 72, 'a': 26, 'e': 23, 'c': 12, 'k': 18,
-    'u': 6, 'j': 5, 'h': 9, 'g': 4, 'b': 3, 'm': 3, 'f': 1
+  'Cu': {
+    'n': 29, 'r': 82, 'm': 28, 'e': 13, 'l': 49, 't': 43, 's': 33, 'p': 10,
+    'o': 3, 'f': 8, 'd': 12, 'c': 18, 'a': 9, 'b': 14, 'y': 1, 'g': 1, 'i': 2,
+    'k': 1, 'z': 6, 'h': 1, 'v': 1, 'j': 1
   },
-  'Me': {
-    'y': 18, 'n': 150, 'd': 70, 'l': 147, 'r': 160, 'j': 4, 'a': 50, 'e': 29,
-    'z': 13, 't': 64, 's': 78, 'i': 61, 'f': 3, 'c': 20, 'h': 34, 'u': 14,
-    'b': 2, 'w': 5, 'g': 24, 'm': 10, 'o': 2, 'k': 4, '!': 1, 'x': 1, 'v': 2
+  'ad': {
+    'l': 76, 'e': 287, 'o': 215, 'a': 190, 'i': 162, 'y': 71, 'f': 13, '!': 264,
+    's': 35, 'd': 135, 'n': 22, 'g': 18, 'r': 39, 'w': 28, 'b': 18, 'm': 16,
+    'c': 4, 't': 37, 'u': 37, 'k': 8, 'h': 16, 'z': 8, 'j': 2, 'v': 5
   },
-  'mf': {'i': 10, 'o': 10, 'e': 7, 'l': 1, 'f': 1, 'r': 1, 'a': 1},
-  'mg': {'a': 15, 'r': 6, 'o': 5, 'e': 2, '!': 1},
-  'Mg': {'u': 1},
-  'Mh': {'o': 1},
-  'mh': {'o': 12, 'e': 3, 'a': 8, 'i': 1},
-  'Mi': {
-    'l': 195, 't': 54, 'r': 48, 'd': 21, 'c': 101, 'n': 165, 'm': 8, 'x': 5,
-    'z': 16, 'g': 19, 'e': 39, 'k': 45, 'y': 22, 's': 66, 'j': 2, 'f': 2,
-    'u': 2, 'h': 23, 'a': 5, 'o': 7, 'v': 2, 'q': 2
+  'dl': {'e': 299, 'i': 67, 'o': 49, 'a': 49, '!': 15, 'u': 9, 'y': 9},
+  'La': {
+    'n': 287, 'w': 48, 'r': 132, 'm': 167, 'k': 13, 't': 79, 'c': 79, 'd': 37,
+    'y': 23, 'i': 33, 's': 95, 'u': 138, 'v': 72, 'p': 68, 'f': 73, 'b': 81,
+    'h': 21, 'l': 29, 'j': 7, 'z': 38, 'g': 64, 'o': 3, 'x': 4, '!': 1, 'a': 8,
+    'q': 2, 'e': 4
   },
-  'mi': {
-    't': 126, 'r': 66, 'l': 116, 'd': 45, 'n': 264, 'c': 67, 's': 82, 'e': 82,
-    'j': 3, '!': 86, 'g': 24, 'a': 37, 'z': 3, 'u': 2, 'o': 11, 'k': 4, 'm': 2,
-    'h': 2, 'y': 4, 'i': 1, 'x': 1
+  'ui': {
+    'z': 26, 'l': 130, 'n': 143, 'r': 55, 't': 76, 'c': 16, 'd': 28, 's': 132,
+    'v': 7, 'g': 16, 'a': 18, '!': 44, 'e': 25, 'm': 8, 'b': 5, 'j': 7, 'o': 4,
+    'p': 3, 'k': 7, 'h': 4, 'f': 2, 'u': 1
   },
-  'mj': {'a': 3, 'i': 1, 'u': 1, 'h': 1},
-  'mk': {'e': 27, 'i': 12, 'o': 16, 'u': 8, 'a': 12},
-  'Ml': {'e': 3, 'i': 1, 'y': 1, 'o': 1},
-  'ml': {'i': 41, 'e': 76, 'a': 12, 'y': 6, 'o': 3, 'u': 1, '!': 5, 's': 1},
-  'mm': {
-    'o': 78, 'i': 78, 'e': 336, 's': 6, '!': 59, 'a': 79, 'u': 3, 'y': 7,
-    'r': 4, 'l': 6
+  'rm': {
+    's': 23, 'e': 155, 'o': 91, 'a': 496, 'i': 85, 'u': 18, '!': 25, 'b': 8,
+    'l': 7, 'w': 4, 'y': 3, 'f': 1, 't': 1, 'k': 1, 'h': 1
   },
-  'mn': {'e': 12, 'a': 8, 'i': 7, 'o': 2, 'y': 2, 'u': 1, '!': 3},
-  'mo': {
-    'n': 430, 's': 32, 'r': 222, 'u': 32, 't': 76, '!': 121, 'o': 12, 'c': 7,
-    'i': 2, 'd': 13, 'l': 44, 'a': 6, 'y': 11, 'e': 9, 'w': 11, 'g': 4, 'k': 4,
-    'h': 4, 'm': 2, 'f': 2, 'p': 3, 'v': 5, 'z': 4, 'x': 1
+  'tr': {
+    'o': 360, 'i': 215, 'a': 282, 'e': 240, 'y': 46, 'u': 78, 'z': 10, 'b': 1,
+    'n': 2, 's': 2, 'm': 1, '!': 2
   },
-  'Mo': {
-    'o': 50, 'r': 276, 'n': 287, 's': 90, 'l': 95, 'b': 8, 'y': 15, 'c': 20,
-    'h': 34, 't': 38, 'u': 55, 'f': 10, 'e': 30, 'j': 4, 'w': 17, 'a': 12,
-    'x': 4, 'd': 30, 'i': 13, 'z': 17, 'g': 16, '!': 1, 'm': 14, 'k': 6, 'q': 1,
-    'v': 3, 'p': 1
+  'ea': {
+    'v': 72, 'n': 159, 'r': 352, 'l': 134, 't': 174, 's': 131, 'd': 171,
+    'c': 65, '!': 126, 'g': 72, 'u': 361, 'y': 7, 'm': 51, 'k': 54, 'h': 18,
+    'b': 27, 'f': 20, 'i': 6, 'z': 19, 'w': 6, 'p': 10, 'q': 3, 'a': 1, 'x': 1,
+    'j': 1, 'o': 1
   },
-  'mp': {
-    's': 44, 'b': 4, 't': 26, '!': 113, 'h': 43, 'o': 42, 'l': 50, 'k': 16,
-    'i': 35, 'a': 65, 'e': 115, 'f': 23, 'u': 6, 'm': 5, 'n': 4, 'p': 8,
-    'r': 11, 'y': 4, 'c': 1
+  'wr': {'e': 10, 'i': 24, 'y': 11, 'a': 6, 'o': 8, 'z': 1},
+  'io': {
+    't': 68, 's': 43, '!': 596, 'n': 255, 'r': 85, 'l': 96, 'j': 2, 'u': 35,
+    'v': 14, 'f': 3, 'i': 2, 'k': 7, 'd': 7, 'p': 12, 'c': 7, 'w': 4, 'g': 4,
+    'b': 2, 'm': 6, 'x': 2, 'a': 2, 'e': 1, 'z': 2
   },
-  'mq': {'u': 9},
-  'Mr': {'a': 5, 'o': 9, 'u': 2, 'n': 1, 'v': 1, 'k': 1},
-  'mr': {'i': 26, 'o': 16, 'a': 10, 'e': 13, 'h': 1, 'y': 3, '!': 1, 'u': 1},
-  'ms': {
-    '!': 114, 't': 47, 'o': 29, 'e': 34, 'a': 8, 'l': 8, 'b': 10, 'd': 7,
-    'h': 12, 'k': 27, 'i': 15, 'w': 3, 'p': 4, 'c': 5, 'f': 1, 'y': 3, 'n': 1, 
-    'u': 1
+  'Ch': {
+    'a': 343, 'r': 94, 'e': 172, 'u': 51, 'i': 164, 'o': 66, 'm': 7, 'y': 3,
+    'l': 4, 'h': 14, 'k': 1, 'w': 2, 'v': 1
   },
-  'Mt': {'!': 1, 'h': 1},
-  'mt': {'i': 2, 'e': 4, 'h': 3, 'z': 1, 'o': 2},
-  'Mu': {
-    'r': 100, 'n': 102, 'l': 98, 'e': 19, 's': 92, 'i': 7, 'h': 14, 'd': 10,
-    'm': 13, 't': 24, 'c': 26, 'f': 4, 'k': 3, 'j': 2, '!': 1, 'z': 9, 'g': 9,
-    'o': 1, 'y': 3, 'w': 1, 'p': 1
+  'Au': {
+    's': 26, 'g': 24, 't': 18, 'l': 14, 'c': 9, 'd': 13, 'b': 13, 'e': 5,
+    '!': 1, 'm': 9, 'r': 10, 'y': 4, 'x': 2, 'z': 3, 'v': 1, 'n': 5, 'i': 2,
+    'k': 4, 'j': 1, 'f': 3, 'w': 2, 'p': 2, 'a': 1
   },
-  'mu': {
-    's': 45, 'e': 9, 'l': 25, 'd': 15, 'r': 48, 'n': 40, 'k': 5, 't': 37,
-    'c': 15, 'z': 2, 'i': 2, 'h': 1, 'a': 1, '!': 3, 'f': 1, 'g': 1
+  'kl': {'i': 59, 'a': 38, 'e': 310, 'u': 13, 'y': 7, 'o': 18, '!': 10, 'v': 1},
+  'Gu': {
+    't': 59, 'z': 20, 'e': 68, 'y': 16, 'n': 47, 's': 35, 'i': 110, 'a': 43,
+    'r': 36, 'l': 50, 'f': 4, 'p': 4, 'm': 18, 'd': 16, 'g': 13, 'o': 2, '!': 1,
+    'h': 1, 'c': 8, 'b': 9
   },
-  'mv': {'o': 1, 'i': 1, 'a': 1},
-  'Mw': {'a': 2},
-  'mw': {'e': 7, 'a': 7, 'o': 3, 'i': 1, 'r': 1},
-  'my': {
-    '!': 45, 't': 2, 'e': 25, 'r': 7, 'a': 3, 'x': 1, 's': 2, 'l': 3, 'o': 2,
-    'n': 2, 'k': 2
+  'Ry': {
+    'a': 5, 'd': 12, 'e': 5, 'm': 5, 'l': 11, 'b': 14, 'c': 4, 's': 5, 'n': 9,
+    'k': 8, 'g': 4, 'u': 2, 'z': 1, 't': 2, 'o': 1, 'h': 2
   },
-  'My': {
-    'e': 5, 'l': 4, 'r': 15, 'a': 3, 'h': 3, 'n': 5, 's': 6, 'u': 1, 'k': 3,
-    'o': 1, 'i': 1, 't': 1, 'c': 1
+  'hm': {
+    'i': 63, 'o': 18, 'a': 215, 'e': 77, '!': 51, 's': 2, 'u': 12, 'k': 5,
+    'b': 1, 'y': 2
   },
-  'mz': {'e': 4, 'o': 1, 'a': 6, '!': 2, 'i': 3},
-  'na': {
-    'n': 227, 'l': 131, '!': 613, 'r': 239, 'd': 58, 's': 150, 'p': 30, 'g': 96,
-    'h': 58, 'm': 68, 'i': 31, 't': 104, 'y': 25, 'v': 26, 'u': 101, 'b': 43,
-    'w': 28, 'k': 66, 'c': 91, 'x': 5, 'o': 6, 'f': 12, 'a': 12, 'j': 4, 'e': 5,
-    'z': 15
+  'id': {
+    't': 30, '!': 90, 's': 15, 'e': 287, 'g': 152, 'd': 96, 'w': 9, 'a': 91,
+    'y': 10, 'r': 21, 'l': 54, 'm': 22, 'o': 71, 'h': 11, 'n': 12, 'k': 4,
+    'i': 62, 'b': 9, 'c': 3, 'u': 7, 'p': 2, 'v': 2, 'j': 2, 'z': 1
   },
-  'Na': {
-    's': 39, 'v': 34, 'n': 30, 'd': 17, 'p': 20, 'q': 2, 'y': 7, 'g': 26,
-    'j': 6, 'b': 17, 't': 35, 'l': 14, 'r': 43, 'k': 24, 'i': 16, 'z': 14,
-    'u': 16, 'c': 18, '!': 1, 'm': 15, 'w': 5, 'a': 3, 'f': 7, 'e': 8, 'h': 9, 
-    'o': 3
+  'dt': {
+    '!': 282, 'r': 2, 'k': 12, 's': 4, 'b': 1, 'l': 2, 'o': 1, 'm': 5, 'a': 2,
+    'f': 1, 'h': 5, 'z': 1, 'e': 4, 'n': 1
   },
-  'nb': {
-    'a': 161, 'e': 316, 'o': 55, 'u': 96, 'l': 15, 'y': 16, 'r': 58, 'i': 10
+  'Va': {
+    's': 52, 'r': 79, 'u': 20, 'l': 141, 'z': 5, 'n': 527, 'i': 16, 'c': 22,
+    'd': 7, 't': 9, 'v': 4, 'q': 4, 'w': 1, 'h': 3, 'y': 4, 'g': 9, 'k': 4,
+    'j': 3, '!': 1, 'm': 1, 'f': 2, 'e': 2
   },
-  'nc': {
-    'h': 189, 'e': 240, 'a': 90, 'i': 141, 'o': 90, '!': 11, 'l': 19, 'y': 21,
-    'u': 13, 'k': 65, 'r': 14, 't': 3, 'z': 18, 's': 2, 'n': 1
+  'sq': {'u': 69},
+  'qu': {
+    'e': 209, 'i': 198, 'a': 53, 'h': 3, 'r': 1, 'o': 7, 'z': 1, 'y': 2, 't': 1
   },
-  'Nc': {'n': 1},
-  'nd': {
-    'e': 835, 'r': 267, 'o': 297, '!': 674, 'l': 128, 's': 120, 'a': 224,
-    't': 62, 'y': 53, 'i': 187, 'h': 23, 'q': 6, 'b': 31, 'm': 22, 'g': 9,
-    'n': 5, 'u': 36, 'w': 7, 'f': 12, 'v': 7, 'z': 19, 'j': 1, 'c': 2, 'k': 5, 
-    'p': 1
+  'ap': {
+    'm': 3, 'p': 172, '!': 37, 'i': 77, 'e': 109, 'l': 50, 'a': 109, 'o': 60,
+    't': 11, 'u': 25, 'h': 22, 's': 25, 'r': 28, 'k': 12, 'd': 2, 'n': 4,
+    'c': 2, 'f': 5, 'w': 1, 'g': 1, 'v': 1
   },
-  'Ne': {
-    'l': 23, 'a': 29, 'w': 76, 'e': 30, 'f': 2, 'g': 15, 's': 35, 'u': 45,
-    't': 30, 'i': 59, 'v': 32, 'm': 19, 'c': 4, 'z': 3, 'r': 18, 'y': 9, 'h': 7,
-    'b': 11, 'd': 14, 'p': 4, 'n': 4, 'j': 3, 'k': 1, 'o': 1
+  'pm': {'a': 19, 'o': 2, 'e': 3},
+  'tg': {'o': 2, 'e': 34, 'a': 4, 'r': 9, 'i': 1, '!': 1},
+  'go': {
+    'm': 7, 'r': 56, '!': 182, 's': 48, 'w': 20, 'n': 79, 'v': 9, 'o': 41,
+    'z': 10, 'u': 17, 'i': 6, 'l': 41, 't': 20, 'p': 3, 'y': 7, 'e': 5, 'd': 13,
+    'a': 5, 'f': 5, 'j': 1, 'c': 6, 'b': 4, 'h': 1
   },
-  'ne': {
-    's': 427, 'z': 74, 'r': 1147, 't': 222, 'd': 49, '!': 1257, 'y': 405,
-    'i': 47, 'a': 119, 'l': 366, 'e': 45, 'h': 28, 'n': 184, 'w': 22, 'g': 49,
-    'f': 21, 'j': 8, 'b': 57, 'p': 12, 'm': 83, 'c': 87, 'k': 97, 'u': 9,
-    'v': 21, 'o': 14, 'x': 5, 'q': 2
+  'Me': {
+    'y': 18, 'n': 150, 'd': 70, 'l': 147, 'r': 160, 'j': 4, 'a': 50, 'e': 29,
+    'z': 13, 't': 64, 's': 78, 'i': 61, 'f': 3, 'c': 20, 'h': 34, 'u': 14,
+    'b': 2, 'w': 5, 'g': 24, 'm': 10, 'o': 2, 'k': 4, '!': 1, 'x': 1, 'v': 2
   },
-  'nf': {
-    'o': 45, 'i': 48, 'r': 24, 'e': 56, 'a': 15, 'u': 10, 'l': 6, 't': 5,
-    'f': 1, '!': 2
+  'Bi': {
+    's': 66, 'r': 77, 'n': 48, 'l': 95, 'g': 36, 'd': 23, 'v': 8, 'c': 36,
+    't': 26, 'b': 17, 'a': 31, 'x': 3, 'e': 82, 'o': 6, 'z': 8, 'f': 3, 'h': 4,
+    'j': 2, 'p': 1, '!': 1, 'm': 1
   },
-  'ng': {
-    '!': 1246, 't': 172, 'h': 126, 's': 181, 'r': 56, 'l': 151, 'u': 49,
-    'e': 859, 'f': 19, 'b': 39, 'o': 109, 'd': 12, 'a': 179, 'm': 26, 'w': 33,
-    'i': 87, 'q': 5, 'n': 9, 'g': 11, 'y': 6, 'c': 13, 'k': 9, 'p': 2, 'v': 9, 
-    'x': 4
+  'cc': {
   },
+  'lv': {'a': 85, 'e': 135, 'i': 70, 'o': 17, 'y': 6, 'r': 1, 'u': 1, 's': 1},
+  'rz': {
+    'a': 52, '!': 44, 'o': 16, 'i': 24, 'y': 49, 'e': 67, 'b': 6, 'u': 8,
+    'w': 4, 'f': 1, 'm': 2, 'k': 1, 'c': 1, 'l': 3, 't': 1
+  },
+  'rv': {'e': 76, 'a': 53, 'i': 120, 'o': 17, 'r': 1, 'y': 4, 'l': 1},
+  'Li': {
+    't': 60, 'n': 198, 'v': 34, 'l': 32, 'g': 30, 'm': 31, '!': 1, 'p': 56,
+    'b': 25, 'u': 5, 'r': 5, 's': 47, 'e': 73, 'd': 18, 'a': 10, 'z': 12,
+    'c': 48, 'k': 7, 'o': 9, 'j': 1, 'q': 2, 'f': 12, 'w': 1, 'i': 1
+  },
+  'ta': {
+    'n': 364, '!': 550, 'k': 50, 'f': 30, 'r': 162, 'i': 65, 'c': 50, 'p': 15,
+    'l': 167, 't': 29, 'h': 22, 'm': 60, 'd': 135, 'g': 68, 's': 100, 'u': 31,
+    'z': 6, 'w': 16, 'b': 30, 'a': 7, 'y': 27, 'v': 27, 'o': 6, 'j': 6, 'q': 4,
+    'e': 11, 'x': 1
+  },
+  'nl': {'e': 90, 'a': 37, 'o': 28, 'i': 34, 'y': 9, 'u': 8, '!': 3},
   'Ng': {'u': 6, '!': 1, 'o': 3, 'h': 2, 'y': 1, 'v': 1, 'i': 1},
-  'nh': {
-    'a': 163, '!': 19, 'o': 111, 'i': 10, 'u': 14, 'e': 45, 'y': 1, 's': 1
+  'uy': {
+    'e': 27, '!': 21, 'n': 13, 't': 5, 'k': 3, 'l': 8, 'b': 1, 'd': 3, 's': 11,
+    'p': 3, 'a': 14, 'r': 3, 'm': 2, 'o': 7, 'v': 1, 'c': 2, 'g': 1, 'z': 1
   },
-  'Nh': {'e': 2, 'a': 2},
-  'Ni': {
-    'c': 103, 'x': 5, 'e': 82, 'l': 12, 'n': 14, 's': 34, 'g': 16, 'p': 7,
-    'm': 13, 'v': 8, 't': 19, 'd': 4, 'b': 7, 'k': 13, 'z': 4, 'w': 1, 'h': 3,
-    'a': 3, '!': 1, 'u': 1, 'f': 3, 'i': 2, 'r': 4, 'q': 1
+  'Ge': {
+    'o': 24, 'n': 86, 'e': 15, 'i': 32, 'r': 159, 'a': 21, 't': 31, 'y': 4,
+    'l': 41, 'h': 26, 'b': 12, 'd': 12, 's': 20, 'm': 15, 'p': 4, 'u': 3,
+    'g': 1, 'f': 6, 'v': 5, 'k': 1, 'c': 4, 'z': 1, 'w': 2
   },
-  'ni': {
-    'e': 237, 'g': 113, 'n': 305, 's': 217, 'd': 17, 'z': 21, 'l': 28, 't': 62,
-    'p': 21, 'c': 287, '!': 596, 'o': 88, 'a': 121, 'h': 7, 'x': 19, 'k': 107,
-    'q': 5, 'f': 36, 'm': 18, 'v': 12, 'u': 19, 'b': 12, 'r': 10, 'w': 3, 'y': 2
+  'eo': {
+    'r': 24, 'n': 86, 'd': 10, 'p': 8, 'i': 2, 'l': 14, '!': 93, 'w': 2, 'u': 8,
+    's': 4, 'b': 2, 'm': 9, 'g': 5, 't': 8, 'c': 2, 'f': 5, 'z': 2, 'h': 4,
+    'v': 2, 'j': 1, 'k': 1, 'a': 1
   },
-  'nj': {'a': 13, 'o': 9, 'i': 5, 'u': 3, 'e': 8},
-  'Nj': {'o': 1, 'i': 1, 'a': 1},
-  'nk': {
-    'i': 67, 'l': 83, 's': 59, '!': 168, 'e': 282, 'f': 5, 'm': 7, 'o': 106,
-    'n': 7, 'h': 16, 'a': 73, 'b': 2, 'r': 16, 'w': 6, 'u': 9, 'v': 1, 't': 1,
-    'k': 1, 'x': 1, 'y': 1
+  'ei': {
+    'd': 198, 'n': 566, 't': 194, 's': 338, 'l': 135, 'r': 100, 'e': 97,
+    'g': 133, 'b': 69, 'f': 50, 'c': 88, 'm': 141, 'a': 9, 'x': 6, 'j': 4,
+    'v': 6, 'k': 29, '!': 35, 'z': 9, 'p': 16, 'h': 15, 'w': 4, 'o': 4
   },
-  'Nk': {'u': 1, 'o': 1},
-  'nl': {'e': 90, 'a': 37, 'o': 28, 'i': 34, 'y': 9, 'u': 8, '!': 3},
-  'nm': {'a': 59, 'e': 18, 'i': 12, 'o': 9, 'u': 3, 'y': 7},
-  'nn': {
-    'e': 579, '!': 476, 'i': 338, 'o': 127, 'a': 213, 'y': 39, 's': 17, 'u': 24,
-    't': 2, 'd': 3, 'h': 4, 'l': 4, 'r': 1, 'b': 1, 'f': 1, 'z': 1, 'c': 1,
-    'g': 1, 'k': 1
+  'Fu': {
+    'l': 51, 'e': 22, 'n': 27, 'g': 15, 'r': 68, 'c': 5, 'q': 2, 's': 24,
   },
-  'no': {
-    'l': 76, '!': 1118, 'z': 18, 'n': 136, 'r': 102, 'w': 119, 'x': 3, 'v': 72,
-    't': 66, 's': 109, 'u': 54, 'i': 15, 'j': 3, 'd': 15, 'h': 14, 'y': 18,
-    'o': 15, 'c': 49, 'f': 33, 'p': 19, 'g': 10, 'e': 19, 'm': 17, 'b': 11,
-    'a': 4, 'k': 7
+  'Ly': {
+    'n': 26, 'o': 2, 'l': 2, '!': 1, 't': 7, 'm': 5, 'k': 8, 'd': 9, 'b': 6,
+    'a': 4, 'f': 1, 'v': 1, 's': 10, 'e': 5, 'c': 2
   },
-  'No': {
-    'r': 138, 'b': 14, 'l': 35, 'e': 11, 'v': 36, 'w': 20, 'y': 7, 'o': 15,
-    'a': 5, 't': 30, 'c': 12, 'k': 4, 'g': 14, 'd': 7, 'u': 8, 's': 15, 'f': 5,
-    '!': 1, 'p': 3, 'h': 3, 'n': 10, 'm': 3, 'z': 3, 'x': 1, 'j': 1, 'i': 3
+  'De': {
+    'a': 77, 'n': 126, 'l': 346, 'c': 91, 'j': 20, 'm': 165, 'w': 40, 'v': 98,
+    'x': 2, 'h': 26, 'r': 133, 'e': 30, 's': 154, 'b': 89, 'y': 10, 'u': 17,
+    'p': 67, 'g': 80, 'i': 36, 'f': 54, 't': 59, 'd': 21, 'k': 18, 'z': 10,
+    'o': 8, 'q': 2
   },
-  'np': {
-    'o': 7, 'e': 5, 'h': 10, 'i': 3, 'a': 12, 'u': 1, 'l': 1, 'r': 2, 's': 1,
-    't': 1, 'f': 1
+  'lb': {
+    'e': 195, 'r': 73, 'o': 55, 'u': 35, 'y': 22, '!': 13, 'a': 86, 'i': 23,
+    'l': 5, 'f': 1, 'n': 1
   },
-  'Nq': {'u': 1},
-  'nq': {'u': 30},
-  'nr': {'y': 9, 'o': 34, 'a': 21, 'i': 57, 'u': 9, 'e': 19, 'r': 4, 'h': 1},
-  'ns': {
-    'o': 242, '!': 747, 't': 246, 'e': 183, 'l': 57, 'h': 43, 'f': 14, 'w': 19,
-    'k': 451, 'i': 77, 'b': 48, 's': 8, 'a': 46, 'm': 33, 'c': 80, 'd': 11,
-    'p': 12, 'u': 11, 'r': 6, 'v': 4, 'g': 1, 'z': 2, 'y': 2, 'n': 2
+  'lc': {
+    'h': 85, 'o': 81, 'e': 20, 'i': 22, 'a': 45, 'z': 18, 'r': 11, 'u': 12,
+    'k': 9, 'l': 2, '!': 4, 'y': 3
   },
-  'nt': {
-    '!': 389, 'e': 432, 'g': 8, 'i': 266, 'o': 304, 'h': 96, 'r': 99, 'y': 37,
-    'u': 52, 'l': 44, 'a': 196, 's': 54, 'z': 122, 't': 9, 'w': 10, 'n': 18,
-    'f': 7, 'b': 2, 'v': 4, 'j': 4, 'c': 4, 'k': 10, 'p': 2, 'd': 2, 'm': 6
+  'zi': {
+    'e': 77, 'l': 20, 'a': 51, 'o': 75, '!': 139, 'n': 115, 'z': 3, 'g': 20,
+    'c': 27, 'k': 21, 'm': 9, 's': 10, 't': 4, 'u': 5, 'q': 1, 'v': 1, 'r': 3,
+    'i': 1, 'w': 1, 'd': 2
   },
-  'nu': {
-    'e': 20, 's': 31, 'm': 24, 't': 34, 'l': 9, 'd': 8, 'a': 8, 'n': 13,
-    'c': 19, 'p': 7, 'r': 7, 'g': 3, 'z': 9, 'k': 6, 'o': 1, '!': 10, 'i': 4,
-    'f': 1, 'h': 1
+  'oz': {
+    'a': 65, '!': 31, 'c': 2, 'i': 39, 'l': 9, 'e': 42, 'n': 14, 'o': 29,
   },
-  'Nu': {
-    'n': 26, 'm': 4, 'g': 3, 't': 10, 'l': 5, 's': 10, 'r': 6, 'c': 11, 'z': 5,
-    'o': 1, 'a': 2, 'u': 1, 'b': 1, 'q': 1, 'f': 1, 'x': 1, 'h': 2, 'v': 1,
-    'd': 2, 'e': 4
+  'wm': {'a': 20, 'e': 4, 'o': 1, '!': 1, 'y': 1},
+  'di': {
+    'n': 410, 'l': 50, 's': 93, 't': 27, 'c': 106, '!': 177, 'a': 72, 'v': 20,
+    'g': 38, 'e': 98, 'f': 16, 'm': 9, 'o': 40, 'x': 10, 'd': 6, 'r': 9,
+    'k': 12, 'z': 10, 'q': 8, 'b': 6, 'w': 2, 'p': 2, 'u': 1, 'h': 1
   },
-  'nv': {'i': 34, 'e': 22, 'a': 9, 'l': 3, 'o': 6, 'r': 1, 'u': 1},
-  'nw': {
-    'a': 55, 'o': 21, 'e': 30, 'i': 17, 'r': 5, 'y': 8, '!': 1, 'h': 1, 'u': 1
+  'wl': {
+    'e': 66, 'a': 15, 'i': 30, 's': 6, 't': 1, 'k': 1, 'o': 6, '!': 8, 'b': 1,
+    'd': 1, 'u': 4, 'y': 1
   },
-  'Nw': {'a': 6},
-  'ny': {
-    'd': 4, '!': 184, 'o': 14, 'e': 21, 'a': 33, 's': 3, 'p': 1, 'w': 1, 'k': 2,
-    'g': 1, 'u': 1, 'c': 1, 'n': 1, 'm': 1, 'l': 1, 'i': 5, 'z': 1, 'r': 1
+  'of': {
+    'f': 344, 't': 53, 'i': 18, 'o': 13, 'm': 8, 'e': 25, '!': 31, 'r': 11,
+    'a': 16, 'g': 3, 'n': 2, 's': 26, 'l': 11, 'q': 1, 'w': 2, 'k': 3, 'z': 1,
+    'h': 3, 'b': 2, 'u': 2
   },
-  'Ny': {
-    'e': 2, 's': 4, 'b': 2, 'g': 4, 'm': 1, 'q': 1, 'l': 5, 'c': 2, 'h': 3,
-    'r': 1, 'd': 3, 'p': 1, '!': 1, 'u': 1, 'k': 1, 'a': 1
+  'fm': {'a': 35, 'e': 3},
+  'rl': {
+    's': 26, 'e': 268, 'a': 115, 'o': 83, 'i': 219, 't': 6, '!': 49, 'y': 77,
+    'm': 3, 'b': 7, 'u': 11, 'd': 3, 'l': 3, 'g': 2, 'w': 1
   },
-  'nz': {
-    'a': 109, 'i': 93, 'u': 11, '!': 89, 'o': 70, 'e': 112, 'y': 8, 'w': 1,
-    'm': 9, 'l': 14, 'k': 2, 'h': 1, 's': 1, 'v': 1
+  'Do': {
+    'u': 53, 'y': 9, 'm': 68, 'r': 115, 'd': 17, 't': 18, 'n': 114, 'w': 49,
+    'o': 22, 'b': 52, 's': 25, 'h': 13, 'l': 69, 'v': 8, 'z': 5, 'e': 26,
+    'c': 21, '!': 1, 'a': 4, 'g': 3, 'i': 10, 'x': 6, 'p': 9, 'k': 8, 'f': 1
   },
-  'oa': {
-    '!': 43, 'n': 39, 'c': 16, 't': 54, 'd': 47, 'r': 32, 'g': 13, 'k': 21,
-    'h': 5, 'f': 3, 'z': 1, 'x': 1, 's': 11, 'i': 2, 'l': 15, 'q': 1, 'p': 3,
-    'm': 3, 'y': 2, 'o': 1
+  'gl': {
+    'a': 54, 'e': 343, 'i': 190, 'y': 6, 'o': 35, 'u': 16, '!': 12, 'm': 1,
+    't': 1, 's': 1
   },
-  'Oa': {'k': 10, 't': 9, 's': 1, 'r': 3, 'c': 1, 'j': 1, 'x': 1},
-  'ob': {
-    'i': 83, 'e': 147, 's': 27, 'b': 58, 'l': 54, 'a': 63, 'o': 49, '!': 17,
-    'u': 16, 'y': 17, 'g': 1, 'd': 5, 'r': 40, 'c': 3, 'n': 3, 'k': 5, 'z': 2,
-    'h': 1, 'm': 2
+  'By': {
+    'r': 18, 'e': 6, 'n': 9, 'a': 8, 'l': 5, 'b': 2, 'i': 1, 'f': 2, 'u': 2,
+    'h': 1, 'k': 2, 'w': 2, 'o': 4, 'm': 1, 't': 2, 's': 3, 'c': 1
+  },
+  'yr': {
+    'd': 3, 'e': 44, 'n': 8, 'i': 11, '!': 6, 'o': 21, 'u': 5, 'r': 2, 'a': 23,
+    'g': 1, 'k': 2, 'l': 3, 's': 4, 't': 1, 'm': 1, 'c': 1
+  },
+  'pk': {'i': 26, 'e': 41, 'a': 23, 'o': 17, 'y': 1},
+  'Te': {
+    'r': 88, 'a': 32, 'm': 21, 'e': 23, 'n': 59, 'l': 34, 'j': 6, 's': 37,
+    't': 19, 'd': 11, 'w': 10, 'i': 19, 'f': 4, 'p': 12, 'b': 8, 'x': 6, 'v': 6,
+  },
+  'So': {
+    't': 20, 'l': 113, 's': 19, 'r': 63, 'u': 61, 'w': 18, 'm': 37, 'a': 5,
+    'n': 50, 'i': 6, 'p': 13, 'k': 13, '!': 1, 'h': 8, 'b': 39, 'c': 11,
+    'd': 24, 'z': 3, 'o': 14, 'v': 10, 'j': 5, 'g': 3, 'f': 9, 'e': 7, 'x': 1,
+    'q': 1, 'y': 2
+  },
+  'gs': {
+    '!': 139, 't': 67, 'w': 6, 'd': 7, 'b': 16, 'l': 6, 'o': 15, 'h': 8,
+    'e': 15, 'a': 14, 'm': 6, 'f': 4, 'j': 1, 'c': 2, 'i': 1, 'p': 1, 'y': 1
+  },
+  'Ji': {
   },
   'Ob': {
     'r': 16, 'e': 44, 'a': 11, 'o': 3, 'y': 2, 's': 2, 'i': 6, 'l': 7, 'h': 2,
     'b': 1, 'n': 1
   },
-  'oc': {
-    'k': 565, 'h': 223, 't': 4, 'u': 13, 'e': 35, 'c': 75, 'a': 38, 'o': 33,
-    'q': 4, '!': 12, 's': 7, 'z': 16, 'i': 31, 'r': 4, 'y': 3, 'l': 2, 'n': 1
+  'br': {
+    'i': 158, 'e': 156, 'o': 179, 'a': 137, 'y': 23, 'u': 38, '!': 1, 'z': 3},
+  'eg': {
+    'o': 90, 'a': 167, 'g': 77, 'e': 213, 'l': 66, 'u': 51, 'r': 105, 'i': 35,
+    'n': 25, 'h': 17, '!': 31, 'f': 2, 'w': 6, 's': 6, 'm': 16, 't': 3, 'y': 5,
+    'd': 2, 'b': 1
   },
-  'Oc': {
-    'o': 6, 'h': 16, 'a': 12, 'e': 5, 'c': 4, 'k': 9, 'l': 1, 'r': 1, 't': 1,
-    'z': 1, 'u': 1
+  'Lu': {
+    'c': 79, 'n': 56, 't': 35, 'g': 9, 's': 21, 'j': 2, 'd': 29, 'k': 27,
+    'm': 23, '!': 1, 'o': 5, 'i': 10, 'e': 45, 'p': 21, 'u': 1, 'x': 5, 'b': 23,
+    'f': 7, 'z': 10, 'r': 10, 'q': 3, 'h': 7, 'y': 2, 'l': 7, 'a': 9, 'v': 5
   },
-  'Od': {
-    'o': 20, 'e': 20, 'u': 2, 'a': 5, 'l': 1, 'd': 3, 'r': 1, 'w': 1, 'h': 2,
-    'n': 1, 'g': 2, 'i': 5, 'm': 1
+  'iq': {'u': 45, 'i': 1, '!': 4},
+  'mb': {
+    'e': 219, '!': 43, 's': 13, 'l': 89, 'a': 118, 'r': 118, 'y': 15, 'o': 70,
+    'i': 39, 'u': 45, 'd': 2, 'h': 3, 'k': 3, 't': 1, 'c': 1
   },
-  'od': {
-    'r': 52, '!': 202, 's': 26, 'e': 185, 'g': 37, 'd': 47, 'w': 18, 'm': 13,
-    'y': 44, 'a': 92, 'f': 14, 'c': 3, 'l': 32, 'b': 18, 'i': 96, 'o': 48,
-    'h': 17, 'n': 23, 'k': 12, 'z': 10, 't': 14, 'u': 8, 'p': 3, 'v': 3
+  'Rh': {'o': 24, 'e': 18, 'y': 9, 'i': 7, 'a': 3, 'u': 6},
+  'ec': {
+    'k': 562, 'o': 73, 'e': 55, 't': 17, 'h': 269, 'a': 62, 'l': 17, 'i': 37,
+    'n': 4, 'q': 2, 'c': 44, '!': 81, 'r': 17, 'z': 31, 'u': 15, 's': 2, 'y': 4,
+    'v': 1, 'w': 1, 'm': 1
   },
-  'oe': {
-    '!': 125, 'd': 35, 'l': 97, 'm': 24, 'n': 103, 'h': 70, 't': 65, 'b': 26,
-    'r': 103, 'u': 8, 's': 93, 'f': 32, 'g': 25, 'y': 8, 'k': 21, 'p': 52,
-    'w': 11, 'c': 34, 'v': 12, 'z': 2, 'i': 2
+  'au': {
+    'g': 325, 'l': 240, 'n': 77, 'e': 120, 'f': 50, 's': 250, 'd': 123,
+    '!': 314, 't': 120, 'r': 119, 'x': 78, 'c': 72, 'm': 121, 'p': 36, 'b': 80,
+    'j': 1, 'v': 18, 'k': 18, 'z': 18, 'w': 7, 'a': 18, 'h': 9, 'i': 8, 'y': 2,
+    'o': 4, 'u': 1
   },
-  'Oe': {
-    's': 8, 'h': 10, 'r': 3, 'l': 6, 't': 3, 'c': 1, 'd': 2, 'n': 1, 'f': 1
+  'No': {
+    'r': 138, 'b': 14, 'l': 35, 'e': 11, 'v': 36, 'w': 20, 'y': 7, 'o': 15,
+    'a': 5, 't': 30, 'c': 12, 'k': 4, 'g': 14, 'd': 7, 'u': 8, 's': 15, 'f': 5,
+    '!': 1, 'p': 3, 'h': 3, 'n': 10, 'm': 3, 'z': 3, 'x': 1, 'j': 1, 'i': 3
   },
-  'Of': {'f': 16, 'a': 2, 't': 1, 'l': 3, 's': 1, 'e': 1},
-  'of': {
-    'f': 344, 't': 53, 'i': 18, 'o': 13, 'm': 8, 'e': 25, '!': 31, 'r': 11,
-    'a': 16, 'g': 3, 'n': 2, 's': 26, 'l': 11, 'q': 1, 'w': 2, 'k': 3, 'z': 1,
-    'h': 3, 'b': 2, 'u': 2
+  'ov': {
+    'e': 250, 'a': 129, 'i': 252, 'o': 27, 's': 29, 'y': 1, 'l': 5, 'v': 1,
+    '!': 31, 'd': 4, 'r': 1, 'n': 3, 'm': 1, 'g': 1, 'k': 1, 'f': 1
   },
-  'Og': {
-    'd': 1, 'l': 6, 'r': 4, 'b': 3, 'i': 6, 'g': 1, 'o': 1, 'a': 14, 'u': 5,
-    'w': 2, 'e': 4, 'z': 1, 's': 1
+  'hu': {
+    'l': 74, 'r': 110, 'e': 44, 'n': 49, '!': 20, 'm': 63, 'g': 13, 's': 41,
+    'b': 23, 'p': 16, 't': 41, 'c': 21, 'a': 13, 'h': 10, 'y': 8, 'f': 15,
+    'k': 18, 'd': 8, 'i': 15, 'u': 3, 'o': 4, 'j': 1
   },
-  'og': {
-    'e': 78, 'a': 75, 'g': 69, 'u': 34, 't': 6, '!': 28, 'l': 46, 's': 15,
-    'd': 15, 'n': 24, 'b': 4, 'h': 21, 'o': 26, 'm': 3, 'r': 12, 'i': 22,
-    'y': 4, 'w': 1
+  'tz': {
+    '!': 572, 'g': 11, 'p': 2, 'e': 206, 'l': 48, 's': 14, 'm': 43, 'f': 5,
+    'w': 4, 'h': 6, 'o': 11, 'c': 1, 'i': 37, 'y': 3, 'k': 45, 'b': 15, 'a': 9,
+    'n': 12, 'r': 4, 'u': 1
   },
-  'Oh': {
-    'a': 16, '!': 1, 'l': 18, 'm': 9, 'e': 4, 'o': 3, 't': 1, 'r': 5, 's': 1,
-    'n': 2, 'y': 1
+  'zm': {'a': 78, 'e': 6, 'i': 13, 'o': 2, 'u': 2, 'd': 1},
+  'yo': {
+    'n': 42, '!': 35, 'r': 16, 'u': 13, 't': 12, 's': 13, 'c': 5, 'l': 7,
+    'a': 3, 'e': 1, 'm': 2, 'v': 2, 'k': 2, 'z': 1, 'o': 2, 'd': 2, 'w': 2
   },
-  'oh': {
-    'n': 80, 'e': 36, 'r': 56, 'l': 88, 'a': 78, 'u': 6, 'd': 4, 'o': 31,
-    '!': 31, 'm': 34, 's': 15, 'y': 1, 't': 1, 'i': 7, 'w': 4, 'b': 2, 'v': 1
+  'lf': {
+    'e': 50, '!': 42, 'o': 57, 'f': 9, 'a': 26, 'r': 23, 's': 14, 'i': 44,
+    'g': 4, 'l': 8, 'h': 1, 'm': 2, 'u': 3, 'y': 2, 't': 1
   },
-  'Oi': {'l': 2, 's': 1, 'e': 2, 'n': 2},
-  'oi': {
-    'n': 64, 's': 107, '!': 16, 't': 28, 'r': 16, 'e': 11, 'x': 2, 'g': 9,
-    'l': 23, 'c': 11, 'a': 22, 'v': 2, 'z': 1, 'd': 11, 'k': 7, 'b': 3, 'o': 2,
-    'u': 1, 'w': 2, 'f': 1, 'm': 1
+  'fe': {
+    '!': 76, 'r': 321, 'y': 30, 't': 17, 'i': 13, 'e': 33, 'n': 70, 'b': 5,
+    'l': 210, 'v': 6, 'f': 3, 's': 6, 'o': 4, 'w': 2, 'a': 5, 'u': 2, 'c': 3,
+    'k': 3, 'g': 2, 'd': 3, 'm': 3, 'h': 2
   },
-  'oj': {
-    'a': 18, 'o': 10, 'i': 7, 'c': 6, 't': 12, 'n': 11, 'k': 3, 'e': 10, '!': 2,
-    'z': 2, 'u': 1, 'd': 2, 'm': 1
+  'rb': {
+    'e': 187, 'y': 37, 'r': 29, 'i': 65, 'o': 99, 'a': 129, 'u': 52, 'l': 9,
+    's': 8, '!': 18, 'm': 1, 'k': 1
   },
-  'Oj': {'e': 1, 'a': 5, 'i': 2},
-  'ok': {
-    '!': 100, 's': 44, 'e': 84, 'i': 25, 'o': 33, 'a': 55, 'm': 6, 'l': 10,
-    'k': 12, 'u': 18, 'h': 7, 'r': 4, 'y': 2, 'f': 2, 'w': 3, 'b': 2, 't': 1
+  'um': {
+    'm': 107, 'p': 92, '!': 299, 'b': 131, 'a': 124, 'n': 6, 'f': 10, 'g': 16,
+    'e': 83, 'o': 28, 'l': 27, 'w': 6, 's': 28, 'r': 9, 't': 2, 'h': 5, 'u': 6,
+    'i': 41, 'k': 5, 'z': 1, 'v': 1, 'd': 1, 'y': 1
   },
-  'Ok': {
-    'e': 13, 'a': 9, 'u': 13, '!': 1, 'o': 12, 'i': 9, 't': 1, 'r': 2, 's': 1,
-    'k': 1, 'w': 1
+  'ub': {
+    'b': 56, 'e': 151, 'i': 99, 'o': 30, 'a': 88, 'y': 14, '!': 39, 'l': 36,
   },
-  'ol': {
-    'l': 574, 'e': 294, 'd': 327, 'm': 77, 's': 121, 't': 171, 'f': 94,
-    'o': 203, 'i': 363, 'p': 43, 'a': 387, 'c': 31, 'k': 55, 'b': 49, 'v': 21,
-    '!': 117, 'n': 22, 'w': 8, 'g': 18, 'z': 68, 'u': 28, 'q': 3, 'r': 2,
-    'y': 23, 'h': 12, 'j': 3
+  'ba': {
+    'r': 190, 'l': 103, 'n': 128, 'k': 32, '!': 128, 'u': 226, 'j': 7, 's': 55,
+    'y': 19, 'c': 246, 't': 48, 'p': 2, 'd': 18, 'z': 8, 'g': 13, 'i': 10,
+    'o': 4, 'm': 4, 'w': 3, 'h': 9, 'v': 3, 'b': 3, 'e': 4, 'a': 5
   },
-  'Ol': {
-    's': 11, 'i': 47, 'e': 28, 'd': 19, 'v': 6, 'm': 9, 'n': 3, 'g': 3, 'a': 16,
-    'l': 18, 'o': 5, 't': 8, 'b': 2, 'c': 3, 'p': 2, 'k': 2, 'u': 3, 'r': 1,
-    'q': 1, 'y': 1, 'w': 1, 'h': 1, 'f': 1
+  'cg': {
   },
-  'om': {
-    'a': 214, 'p': 60, 'e': 193, 'i': 106, 'b': 164, 'o': 58, '!': 265, 'l': 17,
-    's': 52, 'w': 2, 'm': 80, 'f': 5, 'q': 3, 'k': 16, 'r': 11, 'y': 8, 'c': 2,
-    'u': 13, 'g': 6, 'n': 4, 'h': 4, 't': 2, 'd': 4, 'j': 3, 'z': 4, 'v': 1
+  'Fa': {
+    'r': 128, 'u': 62, 'i': 49, 'g': 25, 'y': 10, 'l': 88, 'n': 48, 'j': 2,
+    'b': 28, 'h': 21, 'w': 8, 'v': 25, 'z': 11, 's': 29, 'c': 14, 'd': 12,
+    'm': 10, 'a': 2, 't': 16, 'e': 5, 'k': 3, 'f': 2, 'x': 1
   },
-  'Om': {
-    'a': 7, 'e': 5, 'o': 4, 'u': 3, 't': 1, 'l': 3, 'd': 1, 's': 1, 'm': 1, 
-    'i': 1
+  'lg': {
+    'a': 46, 'o': 19, 'u': 10, 'e': 54, 'r': 30, 'h': 5, 'i': 14, 'l': 2,
+    'n': 1, '!': 3, 'v': 1, 'y': 1
   },
-  'on': {
-    '!': 3423, 'e': 746, 'z': 53, 'g': 307, 's': 255, 'a': 293, 't': 354,
-    'n': 209, 'd': 278, 'l': 17, 'r': 26, 'y': 33, 'w': 9, 'o': 106, 'c': 91,
-    'i': 305, 'k': 65, 'h': 22, 'v': 13, 'm': 6, 'f': 21, 'u': 12, 'b': 17,
-    'q': 4, 'j': 5, 'p': 1
+  'Ag': {
+    'u': 35, 'e': 11, 'n': 9, 'o': 11, 'a': 6, 'i': 4, 'r': 15, 't': 1, 'b': 2,
+    'l': 3, 'y': 1, 'g': 3, 'c': 1, 'p': 1
   },
-  'On': {
-    'e': 8, 't': 3, 'g': 1, 'o': 6, 'k': 3, 'i': 7, 'a': 3, 's': 5, 'c': 1,
-    'l': 1, '!': 1, 'd': 8, 'n': 1, 'u': 2, 'y': 2, 'w': 1
+  'Ve': {
+    'g': 8, 'l': 54, 'n': 83, 'r': 144, 's': 25, 't': 11, 'a': 14, 'i': 15,
+    'd': 3, 'c': 8, 'z': 2, 'y': 4, 'v': 3, 'e': 8, 'j': 2, 'h': 2, 'k': 1,
+    'm': 1, 'b': 1, '!': 1
   },
-  'oo': {
-    'r': 83, 'k': 157, 'p': 53, 'd': 324, 'l': 108, 'n': 107, 'v': 7, 't': 88,
-    'm': 79, 'c': 13, '!': 44, 's': 64, 'h': 4, 'z': 8, 'f': 17, 'g': 17,
-    'e': 8, 'b': 6, 'y': 7, 'i': 3, 'w': 1
+  'Gl': {'o': 44, 'e': 34, 'a': 104, 'y': 3, 'i': 23, 'u': 13},
+  'dg': {
+    'e': 254, 'r': 12, 'i': 10, 'a': 7, 's': 2, 'w': 3, 'k': 4, 'd': 1, 'l': 8,
+    'o': 4, 'm': 5, 'p': 1, 'h': 3, 'u': 1, 'f': 2, 'c': 1, 'n': 1, '!': 1
   },
-  'Oo': {'t': 2, 'm': 1, 'l': 1, 's': 1},
-  'op': {
-    'e': 93, '!': 84, 'k': 16, 'p': 134, 'h': 21, 'l': 28, 's': 16, 'o': 55,
-    'm': 6, 'r': 7, 't': 5, 'f': 29, 'w': 3, 'a': 41, 'i': 44, 'c': 4, 'y': 3,
-    'g': 1, 'u': 10, 'n': 3, 'b': 1, 'z': 1
+  'wt': {'o': 8, 'h': 16, 'e': 6, 'y': 1, 'i': 1, 'r': 2, 's': 1},
+  'dd': {
+    '!': 37, 'l': 43, 'o': 50, 'e': 132, 'y': 40, 'a': 31, 'i': 105, 's': 4,
+    'u': 9, 'r': 8
   },
-  'Op': {
-    'p': 11, 'i': 6, 'l': 2, 'e': 6, 'f': 1, 'd': 2, 'h': 3, 'a': 7, 's': 2,
-    'u': 2, 'o': 2, 'r': 1, 'y': 1, 't': 1
+  'gg': {
+    'i': 114, 's': 48, '!': 77, 'e': 167, 'o': 13, 'l': 22, 'a': 47, 'r': 2,
+    'h': 3, 'm': 2, 'n': 1, 'u': 3, 'b': 1, 'y': 5
   },
-  'oq': {'u': 22},
-  'Oq': {'u': 4},
-  'or': {
-    'e': 577, '!': 365, 'r': 241, 'g': 154, 'd': 505, 't': 445, 'a': 259,
-    'y': 52, 'n': 386, 'm': 114, 's': 232, 'k': 87, 'i': 275, 'b': 67, 'l': 60,
-    'w': 20, 'p': 38, 'o': 161, 'c': 77, 'v': 28, 'h': 15, 'f': 114, 'z': 24,
-    'q': 8, 'u': 22, 'j': 4
+  'gi': {
+    'n': 162, 'l': 57, 's': 34, 'e': 63, 'o': 64, 'a': 55, 'b': 8, 'r': 11,
+    '!': 42, 't': 13, 'u': 7, 'v': 7, 'f': 1, 'd': 5, 'c': 6, 'm': 7, 'y': 1,
+    'k': 1, 'z': 1, 'h': 1
   },
-  'Or': {
-    't': 34, 'r': 12, 'o': 18, 'n': 12, 'l': 18, 'e': 29, 'd': 20, 'c': 4,
-    'a': 15, 'm': 12, 's': 12, 'g': 7, 'v': 2, 'i': 20, 'b': 5, 'z': 5, 'w': 3,
-    'u': 1, 'y': 1, 'k': 3, 'f': 3, 'p': 3, 'j': 1, '!': 1, 'h': 1
+  'In': {
+    'g': 43, 'm': 2, 'f': 6, 'i': 3, 'n': 9, 'o': 6, 'c': 10, 'a': 8, 's': 13,
+    'e': 4, 'k': 4, 'd': 8, '!': 1, 'l': 2, 'z': 5, 'v': 1, 'y': 1, 't': 10,
+    'h': 1, 'b': 1
+  },
+  'gr': {'a': 136, 'o': 90, 'e': 135, 'i': 42, 'u': 12, 'z': 1, 'y': 3, 't': 1},
+  'pt': {
+    'o': 35, 'i': 14, 'e': 13, '!': 13, 'a': 9, 'm': 3, 'u': 3, 'r': 3, 'h': 3,
+    'g': 1, 'y': 1, 'l': 1
+  },
+  'Sw': {'a': 108, 'e': 85, 'i': 70, 'o': 18, 'y': 3},
+  'dm': {'a': 107, 'o': 26, 'u': 8, 'i': 9, 'e': 13},
+  'Ya': {
+    't': 4, 'n': 53, 'r': 28, 'z': 4, 'm': 24, 'g': 10, 'l': 2, 'p': 3, 'o': 1,
+    'e': 3, 'w': 3, 'u': 5, 'h': 5, 'd': 3, 's': 11, 'c': 12, 'b': 2, 'f': 6,
+    'k': 7, '!': 1, 'x': 1, 'i': 2, 'v': 1
   },
+  'Er': {
+    'i': 21, 'v': 5, 'w': 2, 'n': 13, 'd': 9, 's': 6, 'b': 10, 'l': 11, 't': 8,
+    'a': 6, 'h': 4, 'r': 4, 'x': 1, 'p': 4, 'k': 4, 'e': 6, 'c': 8, 'o': 5,
+    'm': 7, 'z': 1, 'g': 1, 'f': 1
+  },
+  'dk': {'i': 21, 'e': 17, 'o': 3, 'n': 2, 'a': 8, 'l': 2, 'y': 1},
+  'Qu': {'i': 115, 'e': 43, 'a': 71, 'o': 2, 'r': 2, 'n': 1},
+  'ax': {
+    'w': 1, 't': 11, '!': 27, 'e': 7, 'o': 3, 'l': 5, 'f': 2, 's': 4, 'i': 9,
+    'u': 1, 'm': 4, 'h': 1, 'b': 4, 'c': 2, 'a': 6
+  },
+  'xw': {'e': 5, 'o': 3, 'i': 1},
   'Os': {
     'b': 12, 'o': 11, 't': 57, 'w': 2, 'g': 1, 'u': 5, 'h': 11, 'm': 11, 'c': 4,
     'p': 2, 'l': 7, 'i': 7, 'e': 9, 's': 6, 'a': 7, 'd': 2, 'k': 1, 'z': 1,
     'v': 1, 'n': 1
   },
-  'os': {
-    's': 322, 't': 271, '!': 487, 'e': 246, 'l': 36, 'h': 104, 'b': 31,
-    'a': 113, 'k': 193, 'w': 12, 'i': 127, 'o': 67, 'c': 93, 'g': 6, 'm': 27,
-    'n': 23, 'q': 8, 'p': 16, 'r': 4, 'z': 28, 'd': 11, 'f': 4, 'v': 2, 'u': 9,
-    'j': 1, 'y': 4
+  'sb': {
   },
-  'Ot': {
-    't': 32, 'e': 4, 'o': 4, 'i': 3, 'a': 6, 'w': 1, 'h': 4, 's': 3, 'u': 3,
-    'r': 1, 'l': 1
+  'bo': {
+    'r': 143, 't': 51, 'n': 89, 'i': 17, 's': 30, 'u': 80, '!': 98, 'd': 16,
+    'a': 9, 'e': 17, 'w': 40, 'g': 8, 'y': 16, 'z': 7, 'l': 77, 'x': 1, 'c': 7,
+    'm': 3, 'o': 14, 'v': 12, 'h': 3, 'k': 2, 'j': 1
   },
-  'ot': {
-    't': 550, 'o': 116, 'h': 193, 's': 36, 'e': 138, '!': 158, 'y': 6, 'l': 12,
-    'a': 75, 'n': 15, 'c': 11, 'z': 42, 'm': 8, 'w': 7, 'i': 35, 'r': 22,
-    'k': 10, 'v': 1, 'u': 10, 'f': 2, 'b': 2, 'd': 1
+  'Es': {
+    't': 58, 'p': 45, 'c': 50, 'q': 14, 'k': 17, 's': 24, 'h': 8, 'l': 4,
+    'a': 4, 'm': 6, 'g': 1, 'e': 2, 'w': 1, 'b': 3, 'f': 1, 'o': 1, 'n': 1
   },
-  'Ou': {
-    'e': 4, 't': 13, 's': 2, 'b': 1, 'z': 1, 'r': 7, 'i': 4, 'l': 2, 'k': 1,
-    'm': 1, '!': 1, 'n': 2, 'd': 3, 'c': 2, 'y': 1
+  'Ty': {
+    'l': 5, 's': 9, 'r': 12, 'n': 7, 'e': 3, 'u': 1, 'g': 2, 'o': 2, 'm': 5,
+    'b': 2, 'c': 2, 'a': 1, 't': 1, '!': 1, 'p': 1, 'k': 1, 'd': 2
   },
-  'ou': {
-    'n': 156, 'g': 200, 's': 275, 'l': 186, 't': 182, 'c': 72, 'r': 323,
-    'd': 96, 'i': 36, 'z': 18, 'x': 30, 'p': 32, '!': 62, 'k': 28, 'a': 14,
-    'm': 18, 'f': 25, 'b': 24, 'q': 5, 'e': 25, 'v': 22, 'y': 12, 'w': 12,
-    'h': 7, 'j': 1, 'o': 2
+  'zg': {'e': 7, 'i': 2, 'a': 9, 'u': 2, 'r': 1, 'h': 1, 'o': 4},
+  'Nu': {
+    'n': 26, 'm': 4, 'g': 3, 't': 10, 'l': 5, 's': 10, 'r': 6, 'c': 11, 'z': 5,
+    'o': 1, 'a': 2, 'u': 1, 'b': 1, 'q': 1, 'f': 1, 'x': 1, 'h': 2, 'v': 1,
+    'd': 2, 'e': 4
   },
-  'ov': {
-    'e': 250, 'a': 129, 'i': 252, 'o': 27, 's': 29, 'y': 1, 'l': 5, 'v': 1,
-    '!': 31, 'd': 4, 'r': 1, 'n': 3, 'm': 1, 'g': 1, 'k': 1, 'f': 1
+  'hw': {'a': 83, 'o': 12, 'e': 70, 'i': 29, 'u': 2, 'r': 1},
+  'cb': {'r': 13, 'e': 6, 'u': 5, 'a': 4},
+  'hr': {
+    'i': 168, 'a': 71, 'o': 85, 'e': 132, '!': 67, 'l': 17, 'm': 26, 'u': 21,
+    'k': 9, 'y': 19, 'h': 6, 'b': 6, 's': 16, 'z': 3, 'n': 8, 't': 7, 'g': 1,
+    'w': 2, 'd': 2, 'f': 1
   },
-  'Ov': {'e': 50, 'a': 6, 'i': 6, 's': 1, 'd': 1},
-  'Ow': {'e': 5, 'i': 1, 's': 2, 'n': 4, 'u': 1, 'c': 2, 'o': 2, '!': 1},
-  'ow': {
-    'n': 96, 'a': 87, 'e': 194, 'm': 13, 'l': 83, '!': 430, 's': 415, 'd': 60,
-    'r': 20, 'i': 155, 'b': 13, 'o': 8, 'y': 6, 'z': 4, 't': 10, 'k': 13,
-    'g': 4, 'h': 7, 'f': 1, 'c': 6, 'p': 1
+  'Kl': {'e': 104, 'i': 74, 'u': 35, 'o': 44, 'a': 65, 'y': 3, 'j': 1},
+  'cl': {'a': 103, 'u': 17, 'e': 101, 'o': 29, 'i': 30, '!': 3, 'y': 3},
+  'hl': {
+    'i': 107, 'e': 275, '!': 175, 'o': 30, 'u': 12, 'm': 33, 'g': 4, 'b': 12,
+    'a': 63, 's': 26, 'k': 13, 'q': 3, 'y': 12, 'f': 11, 'w': 2, 't': 2,
+    'h': 10, 'l': 1, 'n': 1, 'r': 2, 'd': 1
   },
-  'ox': {
-    '!': 39, 'l': 4, 'w': 6, 'e': 14, 'x': 2, 'i': 4, 'o': 7, 's': 4, 't': 8,
-    'h': 3, 'a': 2, 'b': 4, 'm': 1, 'u': 1, 'n': 1, 'f': 1
+  'Zi': {
+    'm': 19, 'e': 56, 'n': 29, 't': 8, 'r': 9, 'g': 5, 'c': 11, 'o': 4, 'p': 8,
+    'l': 12, 'f': 1, 'k': 2, 'z': 2, 'v': 1, 's': 4, 'd': 3, 'a': 5, 'b': 3,
+    'y': 1, 'h': 1
   },
-  'Ox': {'f': 1, 'l': 1, 'e': 2, 'n': 2, 'b': 2, 'm': 1, 't': 1},
-  'oy': {
-    'd': 22, '!': 137, 'l': 28, 'a': 53, 'e': 69, 'c': 6, 'n': 31, 'o': 16,
-    't': 14, 'k': 6, 's': 19, 'b': 2, 'i': 3, 'u': 1, 'h': 1, 'm': 2
+  'tm': {'a': 206, 'o': 18, 'i': 11, 'e': 27, 'u': 3, 'y': 3},
+  'oc': {
+    'k': 565, 'h': 223, 't': 4, 'u': 13, 'e': 35, 'c': 75, 'a': 38, 'o': 33,
+    'q': 4, '!': 12, 's': 7, 'z': 16, 'i': 31, 'r': 4, 'y': 3, 'l': 2, 'n': 1
   },
-  'Oy': {'l': 1, 'o': 1, 'e': 4, 'a': 3, 's': 2, 'u': 1},
-  'oz': {
-    'a': 65, '!': 31, 'c': 2, 'i': 39, 'l': 9, 'e': 42, 'n': 14, 'o': 29,
-    'd': 8, 'w': 3, 'z': 57, 'm': 6, 'y': 6, 'b': 2, 'u': 6, 'g': 4, 's': 1, 
-    'h': 1
+  'Dr': {'a': 74, 'e': 67, 'i': 38, 'u': 30, 'y': 9, 'o': 51, 'z': 3, 'd': 1},
+  'ef': {
+    'f': 162, 'e': 84, 'i': 42, 'n': 6, 'l': 19, 'a': 37, 't': 25, '!': 32,
+    'o': 47, 's': 16, 'k': 10, 'u': 5, 'r': 26, 'c': 5, 'z': 2, 'y': 1
   },
-  'Oz': {
-    'u': 1, 'm': 2, 'a': 6, 'i': 2, 'b': 2, 'l': 1, 'o': 3, 'g': 1, 'e': 2,
-    'z': 1, '!': 1
+  'Ab': {
+    'b': 21, 'r': 35, 'e': 37, 'n': 3, 'l': 8, 'd': 27, 's': 7, 'a': 20,
+    'u': 11, 'i': 9, 'p': 1, 't': 2, 'o': 11, 'k': 2
   },
   'pa': {
     'r': 110, 't': 40, 'u': 33, 'n': 109, 'g': 26, 'i': 19, '!': 86, 's': 42,
     'l': 42, 'z': 7, 'e': 5, 'd': 27, 'h': 10, 'c': 41, 'o': 12, 'p': 4, 'f': 1,
     'k': 11, 'm': 2, 'y': 8, 'a': 3, 'w': 5, 'v': 4, 'j': 3
   },
-  'Pa': {
-    'r': 228, 't': 103, 'l': 150, 'y': 31, 'g': 36, 'u': 51, 'd': 40, 'c': 57,
-    'i': 22, 'q': 3, 'x': 4, 'p': 58, 'z': 7, 'n': 130, 'k': 5, 's': 120,
-    'b': 7, 'e': 7, 'w': 17, 'o': 14, 'v': 45, 'h': 7, 'm': 8, 'f': 5, 'j': 3,
-    'a': 8, '!': 1
+  'uf': {
+    'f': 179, 'm': 2, 'o': 15, '!': 33, 'r': 4, 't': 9, 'e': 24, 'i': 10,
+    'a': 13, 'k': 3, 'u': 3, 'n': 4, 's': 5, 'l': 2, 'h': 1, 'd': 1, 'c': 1,
+    'z': 1, 'v': 1, 'b': 1
   },
-  'pb': {'e': 5, 'u': 1, 'a': 2, 'l': 1},
-  'pc': {'h': 7, 'i': 3, 'z': 3, 'a': 2},
-  'pd': {'i': 2, 'e': 5, 'y': 2, 'a': 1},
-  'Pe': {
-    'r': 234, 't': 189, 'a': 57, 'n': 139, 'c': 42, 'o': 3, 'l': 86, 'p': 20,
-    'd': 40, 'm': 7, 'e': 29, 'y': 5, 'g': 10, 's': 43, 'i': 15, 'w': 3, 'h': 6,
-    'k': 6, 'f': 7, 'v': 9, 'b': 4, 'u': 1, 'z': 11, 'q': 2, 'x': 2
+  'yt': {
+    'o': 28, '!': 10, 'l': 5, 'h': 17, 'e': 29, 'a': 8, 't': 3, 's': 3, 'c': 4,
+    'u': 2, 'z': 1, 'i': 1, 'k': 1, 'r': 1, 'y': 1
   },
-  'pe': {
-    'z': 11, 'r': 382, 'n': 128, '!': 160, 'l': 167, 'a': 40, 'd': 12, 's': 43,
-    'e': 22, 'p': 2, 'i': 20, 't': 46, 'w': 3, 'c': 20, 'y': 24, 'o': 1, 'h': 3,
-    'v': 2, 'k': 11, 'j': 3, 'm': 4, 'g': 3
+  'Ll': {'o': 5, 'e': 5, 'a': 11, 'y': 1},
+  'oa': {
+    '!': 43, 'n': 39, 'c': 16, 't': 54, 'd': 47, 'r': 32, 'g': 13, 'k': 21,
+    'h': 5, 'f': 3, 'z': 1, 'x': 1, 's': 11, 'i': 2, 'l': 15, 'q': 1, 'p': 3,
+    'm': 3, 'y': 2, 'o': 1
   },
-  'pf': {'!': 47, 'o': 1, 'i': 3, 'e': 33, 'f': 2, 'a': 3, 'l': 9, 'n': 1},
-  'Pf': {'e': 13, 'a': 14, 'i': 6, 'l': 15, 'o': 5, 'u': 3, 'r': 2, 'n': 1},
-  'pg': {'a': 1, 'o': 2},
-  'Ph': {'i': 60, 'e': 19, 'a': 29, 'o': 16, 'u': 6, 'y': 3, 'l': 2, 'r': 1},
-  'ph': {
-    'y': 14, 'e': 71, '!': 37, 'r': 14, 'i': 29, 'a': 55, 's': 8, 'u': 7,
-    'o': 23, 'l': 1, 'f': 1, 'c': 1, 'p': 1, 't': 1
+  'Tr': {
   },
-  'Pi': {
-    'e': 89, 't': 52, 'c': 96, 'k': 8, 'n': 110, 'p': 17, 'm': 6, 'l': 61,
-    'a': 19, 'g': 22, 'r': 26, 'z': 22, 's': 30, 'f': 1, 'o': 10, 'x': 2,
-    'd': 3, 'q': 2, 'w': 2, 'h': 3, 'v': 2, 'j': 1, 'u': 2, '!': 1, 'i': 1
+  'Un': {
+    'd': 10, 'g': 12, 'r': 5, 'k': 2, 'z': 2, 's': 4, 't': 9, 'n': 3, 'o': 1,
+    'i': 4, 'c': 3, 'a': 2, 'l': 1, 'v': 2
   },
-  'pi': {
-    'n': 201, 'e': 79, 'v': 5, 'a': 35, 'r': 22, 'c': 39, 'o': 23, 'l': 29,
-    't': 38, 'k': 12, '!': 39, 's': 20, 'g': 9, 'd': 8, 'z': 6, 'j': 1, 'i': 1,
-    'w': 1, 'h': 3, 'p': 2, 'b': 1, 'f': 1
+  'rw': {'o': 32, 'i': 54, 'e': 31, 'h': 1, 'a': 33, 'y': 2},
+  'wo': {
+    'o': 111, 'r': 137, 'l': 25, 'p': 3, 'n': 15, 'm': 3, 'k': 1, 'f': 2,
+    'b': 1, 'z': 2, 'g': 3, 's': 4, 'u': 4, 'y': 2, 'h': 4, 'a': 2, '!': 6,
+    'w': 2, 'c': 2, 'e': 2, 'd': 3
+  },
+  'lp': {
+    's': 4, 'h': 44, 'a': 23, 'e': 26, '!': 17, 'i': 22, 'o': 13, 'r': 5,
+    'l': 2, 'm': 1, 'u': 2, 'p': 2, 'f': 1
+  },
+  'Na': {
+    's': 39, 'v': 34, 'n': 30, 'd': 17, 'p': 20, 'q': 2, 'y': 7, 'g': 26,
+    'j': 6, 'b': 17, 't': 35, 'l': 14, 'r': 43, 'k': 24, 'i': 16, 'z': 14,
+  },
+  'At': {
+    'k': 7, 'w': 4, 'h': 16, 'c': 7, 'e': 5, 't': 23, 'l': 2, 'n': 1, 'i': 4,
+    'a': 6, 'o': 3, 'z': 2, 'm': 2
+  },
+  'rq': {'u': 52},
+  'np': {
+    'o': 7, 'e': 5, 'h': 10, 'i': 3, 'a': 12, 'u': 1, 'l': 1, 'r': 2, 's': 1,
+    't': 1, 'f': 1
   },
-  'Pj': {'e': 1},
-  'pk': {'i': 26, 'e': 41, 'a': 23, 'o': 17, 'y': 1},
-  'pl': {'e': 185, 'a': 37, 'i': 53, 'o': 9, 'u': 6, 'k': 1, '!': 4},
-  'Pl': {'u': 32, 'a': 103, 'e': 42, 'o': 35, 'y': 8, 'i': 10},
-  'pm': {'a': 19, 'o': 2, 'e': 3},
-  'pn': {'e': 21, 'i': 7, 'o': 2, 'a': 1, 'u': 1},
-  'Pn': {'i': 1},
   'po': {
     'r': 53, 's': 22, 'o': 18, 'n': 54, '!': 57, 'i': 7, 'd': 6, 'l': 78,
     't': 19, 'v': 10, 'c': 5, 'h': 5, 'b': 2, 'z': 7, 'u': 32, 'f': 3, 'w': 6,
     'e': 5, 'm': 3, 'p': 4, 'k': 2, 'y': 2, 'g': 1
   },
-  'Po': {
-    'w': 21, 'r': 78, 't': 45, 'p': 48, 'o': 20, 'l': 143, 'n': 41, 'e': 22,
-    's': 53, 'i': 28, 'u': 37, 'g': 6, 'm': 32, 'h': 6, 'y': 9, 'f': 4, 'c': 18,
-    'a': 7, 'k': 10, 'z': 8, 'd': 23, 'b': 3, 'q': 2, 'v': 2, '!': 1, 'x': 1
+  'Ay': {
+    'a': 5, 'e': 5, 'r': 2, 'c': 2, 'o': 6, 'b': 1, 'l': 7, 'm': 2, 'u': 2,
+    's': 2, 'n': 1, 'd': 4, 'k': 1, 'y': 1, 't': 1, 'h': 1
   },
-  'pp': {
-    'a': 61, '!': 142, 'e': 298, 's': 37, 'l': 69, 'i': 84, 'o': 50, 'y': 14,
-    'n': 7, 'm': 2, 'r': 3, 'u': 6, 'h': 4, 'k': 5, 'd': 1
+  'wy': {
+    'e': 13, 'm': 3, 'n': 13, 'k': 5, '!': 9, 'g': 1, 'l': 2, 'f': 1, 'h': 1,
+    'r': 1, 't': 1, 's': 1, 'c': 2, 'a': 1, 'i': 1
   },
-  'Pr': {
-    'i': 118, 'a': 70, 'u': 43, 'e': 149, 'o': 134, 'y': 10, 'z': 12, 'c': 2, 
-    'v': 1
+  'zq': {'u': 10},
+  'Ac': {
+    'o': 11, 'e': 18, 'k': 23, 'u': 2, 'r': 6, 't': 2, 'h': 17, 'y': 1, 'q': 2,
+    'c': 10, 'i': 2, 'a': 2, 'f': 1, 'l': 1
   },
-  'pr': {'i': 62, 'e': 56, 'a': 57, 'u': 12, 'o': 32, 'y': 5, 'z': 2, 'v': 1},
-  'Ps': {'o': 1, 'e': 1, 'u': 2, 'i': 1},
-  'ps': {
-    'o': 33, '!': 88, 'e': 21, 'c': 4, 't': 22, 'h': 14, 'k': 17, 'l': 2,
-    'w': 1, 'a': 4, 'z': 1, 'y': 2, 'i': 2, 'n': 1
+  'sp': {
+    'i': 52, 'a': 57, 'o': 24, '!': 6, 'e': 97, 'r': 11, 'y': 3, 'u': 2, 'h': 2,
+    'l': 6, 'b': 1, 'f': 2, 'd': 1, 'k': 1
   },
-  'Pt': {'a': 4, 'o': 1},
-  'pt': {
-    'o': 35, 'i': 14, 'e': 13, '!': 13, 'a': 9, 'm': 3, 'u': 3, 'r': 3, 'h': 3,
-    'g': 1, 'y': 1, 'l': 1
+  'pi': {
+    'n': 201, 'e': 79, 'v': 5, 'a': 35, 'r': 22, 'c': 39, 'o': 23, 'l': 29,
+    't': 38, 'k': 12, '!': 39, 's': 20, 'g': 9, 'd': 8, 'z': 6, 'j': 1, 'i': 1,
+    'w': 1, 'h': 3, 'p': 2, 'b': 1, 'f': 1
   },
-  'Pu': {
-    'g': 10, 'c': 18, 'r': 51, 't': 17, 'l': 55, 'e': 13, 'm': 9, 's': 12,
-    'i': 4, 'n': 13, 'f': 7, 'a': 1, 'z': 5, 'j': 4, '!': 1, 'p': 4, 'd': 4,
-    'o': 2, 'h': 5, 'y': 1, 'u': 1, 'b': 1
+  'oe': {
+    '!': 125, 'd': 35, 'l': 97, 'm': 24, 'n': 103, 'h': 70, 't': 65, 'b': 26,
+    'r': 103, 'u': 8, 's': 93, 'f': 32, 'g': 25, 'y': 8, 'k': 21, 'p': 52,
+    'w': 11, 'c': 34, 'v': 12, 'z': 2, 'i': 2
   },
-  'pu': {
-    'r': 19, 'l': 18, 'i': 2, 't': 9, 'z': 7, 'a': 7, 's': 15, 'y': 3, 'e': 5,
-    '!': 4, 'c': 4, 'h': 1, 'n': 5, 'g': 1, 'd': 1, 'p': 1
+  'Oc': {
+    'o': 6, 'h': 16, 'a': 12, 'e': 5, 'c': 4, 'k': 9, 'l': 1, 'r': 1, 't': 1,
+    'z': 1, 'u': 1
   },
-  'pv': {'l': 1, 'a': 1},
-  'pw': {'o': 4, 'e': 3, 'a': 2},
-  'py': {'!': 30, 'r': 3, 'd': 1, 'u': 1, 'i': 1, 'c': 1},
-  'Py': {
-    'l': 5, 'e': 4, 'a': 2, 'n': 2, 'r': 3, 'b': 2, 'p': 1, 'k': 1, 'u': 1,
-    't': 4, 'o': 2, 's': 2, 'c': 2, '!': 1, 'w': 1, 'f': 2
+  'Sk': {
+    'i': 36, 'a': 35, 'e': 29, 'o': 41, 'l': 2, 'y': 5, 'u': 12, 'r': 13,
+    'j': 1, 'w': 3, 'n': 1
   },
-  'pz': {'e': 1},
-  'Qa': {'z': 1, 'd': 2, 's': 1, 'r': 1},
-  'qb': {'a': 1},
-  'qd': {'a': 1},
-  'qi': {'!': 1},
-  'Qi': {'a': 1, 'u': 1, 'n': 1},
-  'qr': {'i': 1},
-  'qu': {
-    'e': 209, 'i': 198, 'a': 53, 'h': 3, 'r': 1, 'o': 7, 'z': 1, 'y': 2, 't': 1
+  'by': {
+    '!': 262, 'r': 1, 'l': 10, 'n': 4, 's': 5, 'f': 1, 'a': 3, 'o': 1, 'k': 1,
+    'c': 1, 'e': 1
   },
-  'Qu': {'i': 115, 'e': 43, 'a': 71, 'o': 2, 'r': 2, 'n': 1},
-  'qv': {'i': 1},
-  'ra': {
-    '!': 740, 'y': 121, 'h': 84, 'w': 74, 'l': 156, 'n': 923, 'd': 204, 'z': 96,
-    'v': 131, 'i': 139, 'm': 216, 't': 255, 'k': 97, 's': 286, 'f': 89,
-    'c': 190, 'u': 155, 'b': 134, 'p': 60, 'g': 145, 'e': 32, 'j': 23, 'x': 5,
-    'r': 92, 'a': 19, 'o': 14, 'q': 2
+  'df': {'o': 27, 'r': 4, 'i': 15, 'a': 4, 'e': 8, 'l': 1, 'u': 3},
+  'On': {
+    'e': 8, 't': 3, 'g': 1, 'o': 6, 'k': 3, 'i': 7, 'a': 3, 's': 5, 'c': 1,
+    'l': 1, '!': 1, 'd': 8, 'n': 1, 'u': 2, 'y': 2, 'w': 1
   },
-  'Ra': {
-    'm': 120, 'y': 46, 'n': 91, 't': 65, 's': 63, 'i': 57, 'g': 31, 'd': 76,
-    'l': 13, 'p': 37, 'w': 19, 'u': 43, 'f': 25, 'z': 12, 'c': 40, 'e': 13,
-    'b': 47, 'h': 20, 'o': 2, 'k': 16, 'a': 6, 'v': 28, 'r': 10, 'j': 13,
-    '!': 1, 'x': 2, 'q': 2
+  'Kr': {
   },
-  'rb': {
-    'e': 187, 'y': 37, 'r': 29, 'i': 65, 'o': 99, 'a': 129, 'u': 52, 'l': 9,
-    's': 8, '!': 18, 'm': 1, 'k': 1
+  'af': {
+    'f': 197, 't': 48, 'e': 57, 's': 2, '!': 31, 'l': 23, 'o': 50, 'i': 39,
+    'r': 23, 'u': 19, 'a': 56, 'n': 3, 'k': 4, 'z': 1, 'd': 1, 'm': 1
   },
-  'rc': {
-    'i': 76, 'e': 93, 'a': 46, 'h': 228, 'u': 26, 'o': 64, 'l': 12, 'y': 16,
-    'r': 8, '!': 8, 'k': 26, 'z': 32, 'q': 1, 'm': 1
+  'sc': {
   },
-  'rd': {
-    's': 50, '!': 908, 'a': 112, 'o': 170, 'n': 21, 'y': 33, 'i': 246, 'e': 226,
-    'u': 38, 'w': 14, 'm': 16, 't': 75, 'h': 4, 'l': 27, 'c': 1, 'r': 10,
-    'q': 1, 'b': 2, 'g': 9, 'z': 3, 'v': 1, 'd': 1
+  'sl': {'e': 321, 'i': 68, 'o': 40, 'a': 70, 'y': 16, 'u': 8, '!': 7},
+  'Dy': {
+    'e': 6, 'k': 9, 's': 5, 'c': 6, 'a': 4, '!': 1, 'm': 4, 'n': 2, 'g': 1,
+    'l': 4, 'b': 2, 'd': 3, 'r': 3
   },
-  're': {
-    '!': 861, 'e': 285, 'z': 108, 's': 442, 'n': 635, 'w': 77, 't': 283,
-    'r': 200, 'g': 109, 'l': 402, 'y': 184, 'v': 60, 'a': 203, 'd': 148,
-    'm': 112, 'i': 222, 'j': 21, 'c': 123, 'u': 61, 'b': 52, 'o': 18, 'h': 42,
-    'k': 71, 'f': 29, 'x': 6, 'p': 22, 'q': 5
+  'Wy': {
+    'a': 4, 'n': 12, 'm': 4, 'l': 8, 'c': 4, 'r': 5, 's': 6, 'b': 3, 'g': 4,
+    'd': 6, 'e': 3, 'k': 5, 't': 2, 'z': 2, 'o': 1
   },
-  'Re': {
-    'e': 39, 'y': 28, 'i': 187, 'd': 84, 'a': 71, 'g': 38, 'c': 36, 'n': 102,
-    'u': 23, 'm': 49, 's': 42, 'x': 7, 'b': 25, 'v': 32, 'p': 26, 'h': 35,
-    'z': 10, 't': 26, 'l': 17, '!': 1, 'w': 6, 'f': 7, 'q': 3, 'o': 5, 'k': 6, 
-    'r': 2
+  'xt': {'e': 13, 'o': 26, 'a': 3, '!': 3, 'h': 1, 'i': 1, 'r': 1, 'm': 1},
+  'eh': {
+    'e': 55, 'm': 46, 'a': 107, 'l': 143, 'r': 118, 'u': 11, 'o': 49, 'n': 82,
+    't': 8, '!': 48, 'y': 5, 'i': 14, 'k': 2, 'b': 8, 'd': 3, 'g': 2, 'f': 3,
+    's': 6, 'j': 1
   },
-  'rf': {
-    'o': 29, 'i': 38, 'l': 8, 'a': 15, 'e': 45, '!': 93, 'f': 31, 'm': 4,
-    'u': 6, 'h': 1, 'k': 1, 's': 1, 'y': 1, 'r': 1, 't': 1
+  'Vi': {
+    'n': 45, 'l': 118, 'g': 28, 'c': 40, 'd': 22, 't': 44, 'e': 44, 'o': 8,
+    'r': 36, 'a': 17, 's': 33, 'v': 18, 'z': 10, 'b': 3, 'p': 2, 'm': 1, 'x': 3,
+    'k': 3, 'j': 2
   },
-  'rg': {
-    'a': 120, 'u': 54, 'e': 445, '!': 521, 'r': 32, 'o': 53, 'm': 11, 'i': 77,
-    's': 13, 'n': 7, 'l': 9, 'q': 1, 'g': 2, 'h': 33, 'f': 4, 'd': 4, 'y': 7, 
-    'b': 1
+  'lh': {'o': 67, 'e': 28, 'i': 15, 'a': 60, 'u': 12, 'y': 1, 'j': 1},
+  'Ea': {
+    't': 5, 's': 34, 'r': 32, 'v': 3, 'g': 15, 'd': 8, 'k': 7, 'm': 1, 'n': 3,
+    'l': 5, 'c': 3, 'p': 1, 'y': 1, 'b': 1, 'f': 1
   },
-  'rh': {'a': 70, 'i': 10, 'e': 34, 'o': 73, 'u': 9, 'y': 2, '!': 1},
-  'Rh': {'o': 24, 'e': 18, 'y': 9, 'i': 7, 'a': 3, 'u': 6},
-  'ri': {
-    's': 490, 'g': 255, 'c': 524, 'f': 51, 'e': 442, 'q': 21, 'd': 215,
-    'n': 766, 'm': 116, 't': 232, 'l': 158, 'o': 200, 'x': 15, 'a': 234,
-    'p': 48, 'v': 54, 'z': 61, 'b': 59, '!': 356, 'w': 6, 'j': 3, 'k': 41,
-    'u': 12, 'h': 10, 'i': 2, 'r': 2, 'y': 1
+  'bl': {'e': 276, 'a': 47, 'o': 38, 'i': 44, 'u': 12, 'y': 9, '!': 9},
+  'Av': {'i': 15, 'e': 35, 'a': 12, 'o': 4, 'r': 2, 'n': 1},
+  'kw': {'e': 14, 'o': 14, 'i': 10, 'a': 19, 'r': 1, 'u': 2},
+  'oj': {
+    'a': 18, 'o': 10, 'i': 7, 'c': 6, 't': 12, 'n': 11, 'k': 3, 'e': 10, '!': 2,
+    'z': 2, 'u': 1, 'd': 2, 'm': 1
   },
-  'Ri': {
-    'v': 41, 'c': 100, 'l': 12, 'o': 15, 'd': 49, 'g': 50, 't': 39, 'n': 80,
-    'z': 17, 'p': 23, 'f': 12, 'e': 87, 'm': 15, 's': 56, 'b': 18, 'k': 3,
-    'x': 2, 'a': 5, 'i': 5, 'h': 5, 'u': 1, 'j': 2, 'q': 1
+  'ja': {
+    's': 16, 'm': 7, 'n': 38, 'r': 43, '!': 54, 'd': 4, 'l': 14, 'w': 3,
+    'c': 13, 'k': 7, 'e': 1, 'h': 7, 't': 3, 'a': 1, 'u': 1, 'y': 5, 'b': 1,
+    'j': 2, 'g': 3, 'i': 2, 'p': 1
   },
-  'rj': {'a': 12, 'o': 8, 'u': 3, 'e': 10, 'i': 5},
-  'rk': {
-    '!': 128, 'e': 183, 'i': 85, 's': 46, 'l': 46, 'm': 17, 'p': 2, 'h': 28,
-    'w': 10, 'n': 9, 'o': 72, 'a': 53, 'u': 15, 'g': 1, 'b': 3, 'y': 5, 'd': 3,
-    'r': 5, 't': 2, 'q': 1, 'k': 2, 'v': 4, 'j': 1, 'c': 2
+  'Se': {
+    'r': 112, 'x': 3, 'l': 95, 'a': 95, 'y': 20, 'w': 9, 'g': 35, 'i': 75,
+    'p': 21, 'e': 54, 's': 21, 't': 35, 'v': 31, 'n': 72, 'b': 26, 'd': 29,
   },
-  'rl': {
-    's': 26, 'e': 268, 'a': 115, 'o': 83, 'i': 219, 't': 6, '!': 49, 'y': 77,
-    'm': 3, 'b': 7, 'u': 11, 'd': 3, 'l': 3, 'g': 2, 'w': 1
+  'km': {'a': 118, 'o': 14, 'e': 17, 'u': 1, 'i': 3},
+  'En': {
+    'g': 77, 'r': 7, 'n': 12, 'o': 9, 'd': 24, 'l': 2, 'c': 9, 's': 15, 't': 16,
   },
-  'Rm': {'!': 1},
-  'rm': {
-    's': 23, 'e': 155, 'o': 91, 'a': 496, 'i': 85, 'u': 18, '!': 25, 'b': 8,
-    'l': 7, 'w': 4, 'y': 3, 'f': 1, 't': 1, 'k': 1, 'h': 1
+  'lu': {
+    'r': 15, 'm': 98, 'e': 39, 'c': 52, 'p': 17, 'n': 99, 'g': 21, 's': 81,
+    'k': 18, 'h': 6, 'f': 6, 'd': 11, 'b': 12, 't': 31, 'z': 15, 'i': 10,
   },
-  'rn': {
-    'a': 190, 'e': 374, 's': 91, 'o': 106, 't': 19, '!': 353, 'i': 137, 'd': 18,
-    'h': 26, 'w': 7, 'b': 47, 'u': 12, 'k': 5, 'l': 10, 'y': 12, 'm': 8, 'q': 3,
-    'r': 3, 'g': 6, 'f': 9, 'c': 3, 'z': 3, 'n': 4, 'p': 2
+  'nw': {
+    'a': 55, 'o': 21, 'e': 30, 'i': 17, 'r': 5, 'y': 8, '!': 1, 'h': 1, 'u': 1
   },
-  'Ro': {
-    'b': 94, 'd': 103, 'g': 38, 's': 205, 'm': 79, 'w': 39, 'y': 19, 'j': 6,
-    't': 74, 'a': 26, 'l': 60, 'c': 62, 'u': 74, 'e': 68, 'p': 9, 'o': 26,
-    'n': 41, 'h': 40, 'q': 3, 'z': 23, 'r': 8, '!': 1, 'k': 7, 'f': 4, 'i': 6,
-    'x': 5, 'v': 10
+  'uj': {'i': 15, 'a': 23, 'o': 8, 'n': 1, 'l': 1, 'c': 1, '!': 1, 'e': 1},
+  'ji': {
+    'l': 5, 'a': 17, 'c': 7, 'v': 2, 'm': 8, 'i': 1, 'g': 1, 'w': 1, 't': 2,
+    '!': 9, 'o': 1, 'h': 1, 'd': 3, 'k': 2, 's': 2, 'r': 3, 'e': 3, 'n': 2
   },
-  'ro': {
-    'w': 247, 'o': 144, 'l': 113, 'n': 479, '!': 665, 's': 389, 'c': 186,
-    'a': 51, 'e': 102, 'y': 62, 'u': 188, 'z': 56, 'v': 97, 't': 151, 'f': 72,
-    'g': 63, 'd': 113, 'p': 69, 'm': 198, 'i': 35, 'q': 4, 'r': 10, 'b': 54,
-    'h': 42, 'x': 11, 'k': 41, 'j': 12
+  'Sl': {'o': 51, 'a': 66, 'e': 30, 'u': 15, 'y': 4, 'i': 37},
+  'Ju': {
+    'a': 8, 's': 20, 'd': 11, 'n': 36, 'l': 22, 'r': 37, 'm': 5, 'h': 4,
+    'e': 12, 'c': 2, 't': 2, 'p': 2, 'b': 11, 'k': 2, '!': 1, 'i': 2, 'g': 2,
+    'v': 3, 'u': 1, 'z': 1, 'f': 1
   },
-  'rp': {
-    'h': 18, 'e': 49, '!': 26, 'i': 36, 'o': 23, 'u': 4, 'l': 10, 'a': 15,
-    's': 12, 't': 1, 'r': 5, 'y': 2, 'f': 2, 'n': 1, 'm': 1, 'k': 3
+  'ua': {
+    'r': 94, 'n': 63, 'l': 38, 'j': 1, '!': 75, 'y': 15, 'x': 1, 'd': 21,
+    'c': 5, 'z': 5, 't': 14, 'm': 8, 'i': 18, 's': 14, 'v': 2, 'g': 10, 'h': 2,
+    'k': 3, 'w': 1, 'p': 2, 'a': 2, 'e': 1, 'f': 2
   },
-  'rq': {'u': 52},
-  'rr': {
-    'i': 493, 'e': 446, 'y': 200, 'a': 336, 'o': 251, '!': 94, 'm': 4, 's': 6,
-    'u': 48, 'v': 1, 'l': 3, 'b': 2, 'g': 1, 't': 1, 'n': 1, 'h': 1, 'w': 1
+  'rh': {'a': 70, 'i': 10, 'e': 34, 'o': 73, 'u': 9, 'y': 2, '!': 1},
+  'Pu': {
+    'g': 10, 'c': 18, 'r': 51, 't': 17, 'l': 55, 'e': 13, 'm': 9, 's': 12,
+    'i': 4, 'n': 13, 'f': 7, 'a': 1, 'z': 5, 'j': 4, '!': 1, 'p': 4, 'd': 4,
+    'o': 2, 'h': 5, 'y': 1, 'u': 1, 'b': 1
   },
-  'rs': {
-    'o': 268, '!': 641, 'h': 111, 'e': 148, 't': 234, 'p': 12, 'c': 88, 'y': 5,
-    'l': 32, 'w': 5, 'a': 51, 'b': 16, 'k': 115, 'i': 53, 'd': 14, 'u': 4,
-    'm': 28, 'g': 2, 's': 8, 'f': 6, 'z': 3, 'n': 7, 'j': 1, 'v': 2
+  'pp': {
+    'a': 61, '!': 142, 'e': 298, 's': 37, 'l': 69, 'i': 84, 'o': 50, 'y': 14,
+    'n': 7, 'm': 2, 'r': 3, 'u': 6, 'h': 4, 'k': 5, 'd': 1
   },
-  'rt': {
-    'i': 203, 'e': 257, 's': 99, '!': 795, 'o': 219, 'h': 319, 'z': 93, 'm': 31,
-    'l': 69, 'y': 81, 'w': 18, 'n': 41, 'a': 85, 'u': 51, 'r': 33, 'c': 10,
-    'f': 5, 't': 19, 'g': 9, 'k': 10, 'j': 3, 'p': 1, 'd': 1, 'v': 2, 'b': 1, 
-    'q': 1
+  'ek': {
+    's': 23, '!': 546, 'e': 120, 'l': 9, 'm': 7, 'i': 28, 'k': 5, 'n': 2,
+    'a': 43, 'h': 9, 'u': 13, 'o': 15, 'r': 6, 'b': 3, 'z': 1, 't': 2, 'w': 1,
+    'y': 1, 'f': 1
   },
-  'Ru': {
-    's': 86, 'i': 8, 't': 40, 'c': 15, 'b': 51, 'f': 24, 'd': 55, 'n': 31,
-    'p': 20, 'g': 17, 'e': 37, 'l': 15, 'm': 38, 'v': 4, 'h': 15, 'a': 6,
-    'z': 7, 'y': 6, 'u': 2, 'o': 8, 'x': 1, 'k': 2, 'w': 2, 'r': 2, 'j': 1
+  'tf': {'i': 15, 'a': 3, 'o': 14, 'r': 3, 'e': 6, 'l': 3, 'y': 1, 'u': 1},
+  'As': {
+    'h': 40, 'k': 16, 'b': 6, 't': 24, 'u': 1, 'c': 16, 'a': 14, 'e': 9, 'm': 5,
+    'p': 14, 's': 12, 'l': 7, 'i': 3, 'w': 1, 'q': 1, 'f': 1, 'r': 1, 'n': 2
   },
-  'ru': {
-    'z': 36, 'c': 81, 'i': 34, 'j': 5, 'm': 177, 'e': 88, 'f': 19, 'n': 136,
-    'g': 39, 'b': 48, 's': 134, 'o': 5, 't': 59, 'r': 2, 'd': 71, 'a': 9,
-    'h': 8, 'l': 44, 'p': 52, 'v': 8, '!': 6, 'k': 10, 'y': 13, 'w': 2, 'x': 4, 
-    'u': 2
+  'kb': {'u': 6, 'a': 7, 'e': 13, 'r': 3, 's': 1, 'y': 1, 'i': 5, 'o': 4, 'l': 1
   },
-  'rv': {'e': 76, 'a': 53, 'i': 120, 'o': 17, 'r': 1, 'y': 4, 'l': 1},
-  'Rv': {'i': 1},
-  'rw': {'o': 32, 'i': 54, 'e': 31, 'h': 1, 'a': 33, 'y': 2},
-  'rx': {'!': 5, 'l': 1, 'e': 1, 's': 1},
-  'ry': {
-    '!': 708, 'a': 24, 'e': 24, 'o': 8, 's': 36, 'm': 20, 'd': 13, 'h': 2,
-    'c': 12, 'b': 9, 'k': 4, 'n': 18, 'x': 1, 'l': 13, 'v': 1, 'w': 1, 'r': 1,
-    't': 6, 'j': 1, 'g': 6, 'z': 3, 'p': 1, 'i': 1, 'f': 1, 'u': 1
+  'bu': {
+    'r': 307, 'l': 16, 'c': 24, 's': 75, 'n': 11, 't': 17, 'h': 7, 'e': 9,
+    'q': 1, 'i': 2, 'd': 2, 'k': 1, '!': 7, 'f': 1, 'y': 1, 'a': 1, 'o': 1,
+    'm': 2, 'g': 2, 'b': 1
   },
-  'Ry': {
-    'a': 5, 'd': 12, 'e': 5, 'm': 5, 'l': 11, 'b': 14, 'c': 4, 's': 5, 'n': 9,
-    'k': 8, 'g': 4, 'u': 2, 'z': 1, 't': 2, 'o': 1, 'h': 2
+  'Ko': {
+    'c': 34, 'e': 66, 'h': 32, 'w': 23, 'l': 83, 'o': 29, 'p': 51, 'z': 34,
+    'v': 27, 'n': 63, 'r': 93, 's': 96, 'b': 27, '!': 1, 'g': 8, 'u': 27,
+    't': 51, 'm': 22, 'f': 13, 'k': 10, 'i': 5, 'j': 1, 'd': 7, 'y': 3
   },
-  'rz': {
-    'a': 52, '!': 44, 'o': 16, 'i': 24, 'y': 49, 'e': 67, 'b': 6, 'u': 8,
-    'w': 4, 'f': 1, 'm': 2, 'k': 1, 'c': 1, 'l': 3, 't': 1
+  'cu': {
+    'l': 43, 'm': 27, 't': 32, 's': 35, 'r': 36, 'n': 11, 'e': 15, 'a': 8,
+    'd': 8, 'f': 4, 'b': 5, 'p': 8, 'c': 9, 'y': 1, 'i': 8, 'o': 2, '!': 8,
+    'z': 7, 'k': 2, 'g': 1
   },
-  'Rz': {'e': 4, 'a': 1, 'u': 1},
-  'Sa': {
-    'n': 297, 'l': 220, 'u': 63, 'w': 26, 'v': 59, 'm': 93, 'r': 130, 'd': 34,
-    'e': 21, 'p': 17, 'y': 28, 't': 38, 'a': 19, 'g': 33, 'x': 10, 's': 23,
-    'b': 59, 'c': 32, 'i': 34, 'f': 20, 'o': 2, 'k': 29, 'h': 16, '!': 1,
-    'j': 5, 'z': 1
+  'ej': {
+    'i': 3, 'e': 20, 'o': 45, 'a': 52, '!': 7, 'c': 9, 's': 4, 'u': 4, 'k': 10,
+    'n': 2, 'm': 3, 'j': 1, 'b': 1, 'l': 1, 't': 1, 'g': 1
   },
-  'sa': {
-    'r': 121, '!': 181, 'l': 78, 'y': 25, 'd': 28, 's': 21, 'a': 12, 'n': 195,
-    'i': 26, 'u': 19, 'k': 50, 'p': 7, 't': 24, 'w': 21, 'c': 43, 'v': 14,
-    'b': 15, 'm': 48, 'g': 22, 'o': 4, 'z': 4, 'h': 7, 'f': 4, 'e': 3, 'x': 1, 
-    'q': 2
+  'Ka': {
+    'n': 84, 'u': 39, 't': 56, 'i': 24, 'p': 46, 'y': 13, 'h': 28, 'm': 70,
+    'r': 131, 's': 88, 'v': 10, 'o': 2, 'c': 23, 'e': 17, 'l': 124, 'g': 10,
+    'd': 19, 'w': 19, 'b': 17, 'z': 22, 'f': 5, 'k': 10, 'a': 13, 'j': 2, '!': 1
   },
-  'Sb': {'e': 1, 'a': 2, 'o': 1},
-  'sb': {
-    'o': 25, 'y': 65, 'i': 14, 'u': 51, 'e': 124, 'a': 37, 'r': 28, 'm': 1, 
-    'n': 1
+  'yc': {
   },
-  'sc': {
-    'h': 757, 'o': 216, 'a': 120, 'u': 25, 'e': 24, 'i': 72, 'l': 6, 'y': 1, 
-    'r': 6
+  'kn': {'i': 7, 'e': 69, 'a': 11, 'o': 8, '!': 1},
+  'cm': {'i': 19, 'a': 30, 'u': 20, 'o': 6, 'e': 10},
+  'ys': {
+    '!': 53, 'o': 35, 't': 24, 'e': 42, 'a': 11, 'i': 16, 's': 7, 'd': 4,
+    'l': 10, 'h': 10, 'm': 4, 'k': 9, 'c': 4, 'z': 12, 'r': 1, 'u': 2, 'y': 1,
+    'n': 1, 'w': 1, 'q': 1, 'b': 1
   },
-  'Sc': {
-    'o': 58, 'h': 1145, 'r': 36, 'a': 120, 'u': 20, 'i': 42, 'l': 2, 'e': 9,
-    'y': 1, 'z': 2, 's': 1
+  'ty': {
+    'r': 7, '!': 276, 'l': 6, 'm': 2, 'j': 1, 's': 5, 'n': 13, 'k': 5, 'e': 5,
+    'o': 1, 'a': 7, 'c': 2, 'b': 1, 'd': 1, 'i': 1
   },
-  'sd': {'a': 38, 'o': 28, 'e': 32, 'i': 5, 'y': 1},
-  'Sd': {'o': 1},
-  'se': {
-    'l': 361, '!': 613, 'n': 628, 'y': 170, 'p': 12, 's': 26, 'r': 429, 'm': 50,
-    't': 132, 'c': 25, 'a': 28, 'u': 13, 'b': 26, 'x': 2, 'e': 29, 'h': 9,
-    'k': 64, 'v': 7, 'g': 13, 'f': 10, 'd': 11, 'i': 17, 'w': 13, 'z': 2,
-    'q': 1, 'o': 3
+  'tn': {'e': 156, 'a': 16, 'u': 2, 'y': 5, 'o': 7, 'i': 25, '!': 1},
+  'tu': {
+    '!': 19, 'a': 9, 'm': 30, 'b': 21, 'r': 82, 's': 52, 'n': 30, 'c': 38,
+    'l': 33, 'd': 21, 't': 18, 'k': 6, 'g': 4, 'p': 9, 'i': 5, 'h': 4, 'f': 6,
+    'e': 19, 'o': 7, 'z': 2, 'v': 1, 'y': 2, 'q': 1
   },
-  'Se': {
-    'r': 112, 'x': 3, 'l': 95, 'a': 95, 'y': 20, 'w': 9, 'g': 35, 'i': 75,
-    'p': 21, 'e': 54, 's': 21, 't': 35, 'v': 31, 'n': 72, 'b': 26, 'd': 29,
-    'm': 40, 'c': 24, 'q': 3, 'o': 1, 'k': 7, 'h': 7, 'f': 6, 'u': 10, '!': 1, 
-    'j': 1
+  'Ti': {
+    'l': 35, 'p': 22, 'd': 7, 'm': 48, 'n': 56, 't': 18, 'r': 13, 's': 22,
+    'b': 17, 'j': 4, 'e': 35, 'c': 13, 'f': 7, 'g': 13, 'a': 3, 'u': 1, 'o': 3,
+    'z': 2, 'k': 1, 'x': 2, 'w': 1, 'v': 2
   },
-  'sf': {'i': 13, 'o': 31, 'a': 2, 'e': 12, 'j': 1},
-  'Sf': {'o': 1, 'e': 3, 'a': 1},
-  'sg': {'o': 4, 'r': 19, 'e': 9, 'u': 6, 'a': 7, 'i': 3, 'l': 1},
-  'Sg': {'r': 3, 'a': 2, 'u': 1},
-  'Sh': {
-    'a': 265, 'e': 249, 'o': 125, 'i': 179, 'u': 99, 'r': 36, 'y': 5, 'k': 1,
-    'm': 1, 'v': 1, 'w': 1, 'b': 1
+  'nf': {
+    'o': 45, 'i': 48, 'r': 24, 'e': 56, 'a': 15, 'u': 10, 'l': 6, 't': 5,
+    'f': 1, '!': 2
   },
-  'sh': {
-    'i': 204, 'e': 207, 'a': 227, 'o': 78, '!': 312, 'l': 22, 'b': 31, 't': 7,
-    'c': 3, 'f': 8, 'w': 14, 'm': 41, 'n': 27, 'u': 27, 'r': 4, 'k': 10, 'j': 1,
-    'y': 5, 'd': 4, 'p': 3
+  'ab': {
+    'r': 82, 't': 1, 'e': 208, 'c': 1, 'b': 59, 'o': 118, 'a': 207, '!': 40,
+    'i': 133, 'l': 65, 'n': 4, 'y': 22, 's': 12, 'h': 8, 'u': 30, 'j': 3,
+    'd': 1, 'k': 3, 'z': 2
   },
-  'si': {
-    'd': 25, '!': 167, 't': 35, 'l': 61, 'n': 325, 'e': 115, 'o': 55, 'm': 29,
-    'c': 84, 'a': 84, 's': 34, 'g': 32, 'u': 10, 'k': 34, 'r': 11, 'f': 8,
-    'v': 2, 'z': 5, 'p': 2, 'b': 4, 'q': 1, 'x': 2, 'y': 1
+  'Ce': {
+    'r': 88, 'c': 15, 'n': 22, 'j': 2, 'p': 8, 'b': 2, 'd': 11, 'a': 8, 'l': 27,
+    's': 13, 'v': 2, 'f': 3, 'z': 2, 'g': 3, 'm': 2, 't': 1, 'o': 2
   },
-  'Si': {
-    'm': 115, 'l': 95, 'n': 79, 'z': 4, 'e': 90, 's': 34, 'k': 14, 'g': 31,
-    'b': 19, 'p': 18, 'd': 40, 't': 35, 'r': 40, 'f': 7, 'c': 28, 'u': 3,
-    'x': 6, 'a': 10, 'v': 27, 'q': 1, 'o': 5, 'w': 5, '!': 1
+  'Za': {
+    'm': 30, 'v': 13, 'p': 20, 'r': 44, 'c': 26, 'y': 4, 'h': 20, 'n': 41,
+    'k': 10, 'j': 4, 'b': 21, 'l': 17, 'g': 12, 'w': 5, 's': 4, 'z': 4, 'u': 6,
+    'i': 10, 'd': 12, 'f': 5, 't': 3, 'e': 1, 'x': 1
   },
-  'sj': {'a': 4, 'e': 1, 'o': 4},
-  'Sj': {'o': 8, 'a': 1, 'u': 1, 'e': 1},
-  'sk': {
-    'i': 1223, '!': 27, 'e': 207, 'r': 8, 'o': 116, 'y': 332, 'a': 106, 'u': 6,
-    'w': 2, 'n': 1, 'l': 3, 'v': 1, 't': 1
+  'cn': {'e': 40, 'a': 25, 'u': 6, 'i': 17, 'y': 1, 'o': 2, '!': 1},
+  'cf': {'a': 24, 'e': 9, 'i': 1, 'o': 1},
+  'fa': {
+    'r': 55, 'd': 5, 'l': 40, 'f': 2, 'n': 74, 'c': 8, 't': 14, 'v': 9, 'y': 7,
+    'z': 2, '!': 24, 'u': 11, 'x': 3, 'e': 2, 'k': 1, 'm': 3, 'i': 14, 's': 6,
+    'w': 1, 'g': 7, 'h': 11, 'b': 5, 'a': 1
   },
-  'Sk': {
-    'i': 36, 'a': 35, 'e': 29, 'o': 41, 'l': 2, 'y': 5, 'u': 12, 'r': 13,
-    'j': 1, 'w': 3, 'n': 1
+  'sa': {
+    'r': 121, '!': 181, 'l': 78, 'y': 25, 'd': 28, 's': 21, 'a': 12, 'n': 195,
+    'i': 26, 'u': 19, 'k': 50, 'p': 7, 't': 24, 'w': 21, 'c': 43, 'v': 14,
   },
-  'sl': {'e': 321, 'i': 68, 'o': 40, 'a': 70, 'y': 16, 'u': 8, '!': 7},
-  'Sl': {'o': 51, 'a': 66, 'e': 30, 'u': 15, 'y': 4, 'i': 37},
-  'Sm': {
-    'i': 45, 'a': 29, 'o': 24, 'y': 12, 'e': 25, 't': 1, 'u': 13, 'r': 1, 's': 1
+  'Sy': {
+    'k': 3, 'l': 14, 'd': 6, 'm': 11, 'n': 8, 'e': 3, 'v': 3, '!': 1, 'r': 8,
+    't': 2, 'p': 6, 'b': 2, 's': 2, 'a': 2, 'o': 1, 'c': 1, 'z': 1
   },
-  'sm': {'u': 20, 'i': 53, 'a': 240, '!': 2, 'o': 34, 'e': 45, 'y': 1},
-  'sn': {'e': 131, 'i': 35, 'a': 31, 'u': 2, 'o': 15, '!': 4, 'y': 6},
-  'Sn': {'y': 2, 'o': 25, 'i': 11, 'e': 29, 'a': 13, 'u': 2},
-  'so': {
-    'n': 1337, '!': 212, 'm': 52, 'e': 8, 'r': 57, 'l': 55, 's': 15, 'u': 31,
-    'c': 13, 'p': 6, 'y': 2, 'x': 1, 't': 15, 'h': 5, 'w': 31, 'b': 2, 'f': 6,
-    'o': 6, 'i': 5, 'g': 3, 'a': 2, 'z': 1, 'v': 10
+  'yk': {
+    'e': 37, 'i': 8, 's': 4, '!': 79, 'o': 16, 'a': 11, 'l': 2, 'h': 3, 'k': 2,
+    'r': 1, 't': 1
   },
-  'So': {
-    't': 20, 'l': 113, 's': 19, 'r': 63, 'u': 61, 'w': 18, 'm': 37, 'a': 5,
-    'n': 50, 'i': 6, 'p': 13, 'k': 13, '!': 1, 'h': 8, 'b': 39, 'c': 11,
-    'd': 24, 'z': 3, 'o': 14, 'v': 10, 'j': 5, 'g': 3, 'f': 9, 'e': 7, 'x': 1,
-    'q': 1, 'y': 2
+  'nj': {'a': 13, 'o': 9, 'i': 5, 'u': 3, 'e': 8},
+  'ka': {
+    'y': 12, 'g': 8, 'r': 96, '!': 361, 'm': 85, 'b': 15, 's': 68, 'h': 9,
+    'n': 56, 'w': 16, 'i': 17, 'c': 13, 'd': 11, 'l': 50, 'k': 7, 't': 14,
+    'f': 8, 'u': 15, 'z': 1, 'a': 6, 'o': 3, 'v': 5, 'p': 4, 'j': 5, 'e': 2
   },
-  'Sp': {
-    'e': 115, 'a': 111, 'r': 95, 'i': 113, 'u': 18, 'o': 42, 'l': 9, 'y': 4, 
-    'h': 1
+  'Ew': {'i': 4, 'e': 7, 'a': 5, 'b': 1, 't': 1, 'y': 1, 'o': 1},
+  'vy': {'!': 36, 'e': 2, 'n': 1, 'a': 1, 'd': 1},
+  'uk': {
+    'e': 58, '!': 63, 'i': 21, 'u': 18, 'a': 46, 'o': 29, 'n': 3, 'l': 7,
+    'h': 10, 's': 4, 'w': 1, 'm': 1, 'k': 5, 'c': 1, 'r': 3
   },
-  'sp': {
-    'i': 52, 'a': 57, 'o': 24, '!': 6, 'e': 97, 'r': 11, 'y': 3, 'u': 2, 'h': 2,
-    'l': 6, 'b': 1, 'f': 2, 'd': 1, 'k': 1
+  'Od': {
+    'o': 20, 'e': 20, 'u': 2, 'a': 5, 'l': 1, 'd': 3, 'r': 1, 'w': 1, 'h': 2,
+    'n': 1, 'g': 2, 'i': 5, 'm': 1
   },
-  'Sq': {'u': 15},
-  'sq': {'u': 69},
-  'sr': {'a': 10, 'o': 10, 'e': 6, 'y': 1, 'u': 10, 'i': 5, '!': 2},
-  'Sr': {'o': 5, 'i': 3, 's': 2, 'n': 1, 'e': 2, 'a': 2, 'y': 1},
-  'ss': {
-    '!': 421, 'e': 592, 'o': 223, 'a': 195, 'l': 83, 'i': 228, 'm': 80, 'u': 14,
-    'y': 17, 'n': 34, 'c': 3, 'b': 14, 'f': 6, 'w': 13, 'h': 9, 'k': 5, 'g': 2,
-    't': 2, 'p': 2, 'r': 1
+  'ae': {
+    'l': 35, 'f': 18, '!': 21, 'z': 13, 'n': 25, 'r': 44, 'g': 24, 's': 38,
+    'm': 10, 'c': 11, 'd': 14, 't': 38, 'p': 1, 'h': 14, 'k': 6, 'y': 3, 'e': 1,
+    'b': 8, 'o': 1, 'u': 3, 'v': 1, 'w': 2, 'a': 2
   },
-  'St': {
-    'e': 401, 'o': 290, 'a': 458, 'r': 347, 'u': 145, 'i': 167, 'j': 8, 'c': 6,
-    'p': 5, 'y': 11, 'g': 5, 'l': 5, 'h': 3, 'm': 4, 't': 1, 'w': 2, 'f': 4,
-    'd': 2, 's': 1, 'v': 3
+  'fy': {'!': 17},
+  'zp': {'a': 4, 'e': 1},
+  'zu': {
+    'e': 9, 'r': 20, 'n': 8, 'k': 7, '!': 5, 't': 11, 'm': 14, 'l': 14, 'c': 7,
+    'b': 11, 'a': 4, 'o': 2, 's': 5, 'f': 1, 'w': 1, 'g': 1, 'p': 1
   },
-  'st': {
-    'e': 898, '!': 431, 'r': 304, 'i': 255, 'o': 400, 'a': 372, 'l': 84,
-    'm': 24, 'b': 12, 'y': 27, 'n': 19, 'f': 4, 'u': 30, 'p': 3, 'c': 3,
-    'w': 11, 'g': 3, 'h': 14, 'k': 7, 'v': 2, 's': 1, 'z': 1
+  'cp': {'h': 17, 'e': 5, 'a': 6, 'i': 1, 'r': 1},
+  'ym': {
+    'o': 39, 'a': 69, 'p': 4, 'e': 35, 'i': 10, 'u': 7, 'c': 2, 'k': 3, '!': 6,
+    's': 4, 'm': 2, 'y': 1
   },
-  'Su': {
-    'l': 47, 't': 35, 'm': 60, 'a': 5, 'g': 22, 'n': 39, 'r': 46, 'b': 15,
-    'z': 1, '!': 1, 'h': 4, 'd': 26, 's': 25, 'i': 9, 'p': 11, 'e': 14, 'y': 3,
-    'c': 15, 'f': 3, 'o': 6, 'k': 8, 'w': 1, 'v': 1
+  'ft': {
+    '!': 97, 'o': 19, 'i': 9, 'u': 1, 'w': 1, 's': 8, 'e': 17, 'h': 5, 'y': 3,
+    'z': 3, 'r': 1, 'm': 2, 'l': 2, 'a': 4, 'g': 1
   },
-  'su': {
-    's': 8, '!': 23, 'l': 17, 'p': 4, 'n': 12, 'm': 26, 'r': 27, 'c': 10,
-    'd': 9, 'e': 15, 'i': 10, 'j': 1, 't': 11, 'o': 4, 'a': 6, 'u': 1, 'z': 2,
-    'b': 7, 'k': 7, 'f': 2, 'h': 5, 'y': 1, 'g': 1
+  'Em': {
+    'e': 12, 'm': 18, 'a': 9, 'b': 18, 'o': 6, 'r': 3, 'i': 9, 'p': 7, 'l': 5,
   },
-  'sv': {'e': 6, 'o': 4, 'a': 4, 'i': 6},
-  'Sv': {'o': 3, 'e': 15, 'a': 5, 'r': 1, 'i': 1},
-  'Sw': {'a': 108, 'e': 85, 'i': 70, 'o': 18, 'y': 3},
-  'sw': {'o': 68, 'e': 36, 'a': 20, 'i': 16, 'h': 1, 'u': 1},
-  'Sy': {
-    'k': 3, 'l': 14, 'd': 6, 'm': 11, 'n': 8, 'e': 3, 'v': 3, '!': 1, 'r': 8,
-    't': 2, 'p': 6, 'b': 2, 's': 2, 'a': 2, 'o': 1, 'c': 1, 'z': 1
+  'Ir': {
+    'w': 1, 'v': 4, 'i': 14, 'b': 1, 'e': 8, 'o': 3, 'a': 3, 'l': 2, 'u': 1,
+    'm': 1, 's': 1, 'z': 1, 'r': 1
   },
-  'sy': {
-    't': 2, '!': 50, 'e': 1, 'u': 1, 'c': 2, 'a': 7, 'n': 2, 'o': 1, 'l': 2, 
-    'g': 1
+  'cr': {'a': 58, 'u': 15, 'o': 68, 'e': 53, 'i': 38, 'y': 1},
+  'sm': {'u': 20, 'i': 53, 'a': 240, '!': 2, 'o': 34, 'e': 45, 'y': 1},
+  'mu': {
+    's': 45, 'e': 9, 'l': 25, 'd': 15, 'r': 48, 'n': 40, 'k': 5, 't': 37,
+    'c': 15, 'z': 2, 'i': 2, 'h': 1, 'a': 1, '!': 3, 'f': 1, 'g': 1
   },
-  'sz': {
-    'e': 41, '!': 57, 'y': 21, 'a': 20, 'k': 14, 'l': 4, 'u': 5, 'o': 2, 'c': 7,
-    't': 2, 'i': 2, 'b': 1, 'm': 1, 'w': 1
+  'je': {
+    's': 15, 'd': 6, 'r': 35, 'u': 2, 'w': 12, 'a': 9, 'k': 8, 'n': 20, 'e': 4,
+    'l': 19, '!': 15, 't': 4, 'i': 5, 'c': 2, 'm': 3, 'v': 2, 'p': 1, 'b': 1
   },
-  'Sz': {
-    'y': 14, 'a': 18, 'e': 14, 'c': 10, 'o': 8, 'i': 3, 'w': 6, 'u': 11, 'm': 2,
-    'n': 1, 'l': 1, 'p': 1, 'k': 1
+  'su': {
+    's': 8, '!': 23, 'l': 17, 'p': 4, 'n': 12, 'm': 26, 'r': 27, 'c': 10,
+    'd': 9, 'e': 15, 'i': 10, 'j': 1, 't': 11, 'o': 4, 'a': 6, 'u': 1, 'z': 2,
+    'b': 7, 'k': 7, 'f': 2, 'h': 5, 'y': 1, 'g': 1
   },
-  'ta': {
-    'n': 364, '!': 550, 'k': 50, 'f': 30, 'r': 162, 'i': 65, 'c': 50, 'p': 15,
-    'l': 167, 't': 29, 'h': 22, 'm': 60, 'd': 135, 'g': 68, 's': 100, 'u': 31,
-    'z': 6, 'w': 16, 'b': 30, 'a': 7, 'y': 27, 'v': 27, 'o': 6, 'j': 6, 'q': 4,
-    'e': 11, 'x': 1
+  'Hy': {
+    'd': 5, 'a': 4, 'm': 8, 'n': 8, 'l': 10, 's': 10, 'e': 3, 'p': 3, '!': 1,
+    'r': 2, 'u': 1, 'c': 2, 'b': 2, 'o': 1, 'z': 1, 't': 3, 'k': 1
   },
-  'Ta': {
-    'y': 15, 't': 32, 'n': 80, 'l': 63, 'p': 26, 'b': 36, 'c': 24, 'v': 23,
-    'f': 12, 'g': 24, 'r': 89, 'm': 40, 'i': 16, 'k': 26, '!': 1, 's': 26,
-    'd': 17, 'u': 26, 'o': 3, 'w': 4, 'h': 5, 'a': 3, 'e': 3, 'z': 3, 'j': 4, 
-    'q': 1
+  'yf': {'i': 9, 'o': 11, 'e': 7, 'f': 1, 'r': 2, 'u': 2, 'a': 2},
+  'aa': {
+    's': 39, 'c': 21, 'v': 3, 'g': 12, 'r': 61, 'd': 12, 'b': 12, 't': 15,
+    'f': 6, 'l': 14, 'n': 15, 'm': 6, 'p': 6, 'k': 15, '!': 19, 'i': 4, 'h': 2,
+    'e': 2, 'w': 2, 'u': 2, 'z': 2, 'y': 1
   },
-  'tb': {'r': 12, 'e': 16, 'y': 4, 'u': 3, 'o': 2, 'a': 5, 'i': 4, 'l': 1},
-  'Tc': {'h': 1},
-  'tc': {
-    'h': 318, 'a': 9, 'l': 7, 'o': 8, 'y': 1, 'z': 5, 'i': 3, 'r': 5, 'u': 1,
-    's': 1, 'e': 1, '!': 1
+  'ct': {'o': 28, '!': 6, 'e': 13, 'a': 4, 'i': 10, 'l': 1, 'h': 5, 'u': 1},
+  'nu': {
+    'e': 20, 's': 31, 'm': 24, 't': 34, 'l': 9, 'd': 8, 'a': 8, 'n': 13,
+    'c': 19, 'p': 7, 'r': 7, 'g': 3, 'z': 9, 'k': 6, 'o': 1, '!': 10, 'i': 4,
+    'f': 1, 'h': 1
   },
-  'td': {'o': 5, 'e': 4, '!': 1},
-  'te': {
-    '!': 839, 'r': 1373, 'w': 24, 'v': 29, 'p': 44, 's': 177, 'e': 108, 'g': 33,
-    'n': 428, 'z': 22, 'h': 18, 'l': 370, 'i': 243, 'm': 58, 'a': 90, 'f': 43,
-    't': 46, 'd': 49, 'o': 13, 'b': 22, 'y': 30, 'c': 34, 'j': 8, 'k': 46,
-    'u': 18, 'q': 1, 'x': 2
+  'Ib': {'a': 7, 'r': 3, 's': 1, 'e': 3, 'u': 1, 'o': 1, 'l': 1, 'b': 2, 'd': 1
   },
-  'Te': {
-    'r': 88, 'a': 32, 'm': 21, 'e': 23, 'n': 59, 'l': 34, 'j': 6, 's': 37,
-    't': 19, 'd': 11, 'w': 10, 'i': 19, 'f': 4, 'p': 12, 'b': 8, 'x': 6, 'v': 6,
-    'g': 8, 'z': 2, 'k': 5, 'h': 3, '!': 1, 'c': 6, 'u': 3, 'o': 3, 'y': 1, 
-    'q': 1
+  'pr': {'i': 62, 'e': 56, 'a': 57, 'u': 12, 'o': 32, 'y': 5, 'z': 2, 'v': 1},
+  'kh': {
+    'a': 76, 'o': 44, 'u': 9, 'e': 11, '!': 4, 'i': 12, 't': 4, 'm': 2, 'l': 1,
+    'r': 1, 's': 1
   },
-  'tf': {'i': 15, 'a': 3, 'o': 14, 'r': 3, 'e': 6, 'l': 3, 'y': 1, 'u': 1},
-  'tg': {'o': 2, 'e': 34, 'a': 4, 'r': 9, 'i': 1, '!': 1},
-  'th': {
-    '!': 634, 'e': 410, 'y': 34, 'i': 87, 'o': 107, 'r': 38, 'u': 34, 'a': 199,
-    's': 13, 'c': 22, 'w': 27, 'm': 29, 'b': 11, 'l': 21, 'j': 5, 'n': 7,
-    'k': 6, 'v': 4, 'f': 5, 'h': 4, 't': 2, 'g': 6
+  'cy': {'!': 69, 'r': 1, 'o': 2, 'n': 2, 'p': 1, 'k': 2, 'u': 2, 't': 1},
+  'Ak': {
+    'e': 12, 'i': 11, 'r': 4, 'b': 2, 'a': 10, 'h': 3, 'p': 1, 'm': 1, 'k': 1,
+    'u': 2, 's': 2, 'o': 2, 'l': 2, 'w': 1
   },
-  'Th': {'o': 109, 'u': 37, 'a': 66, 'r': 40, 'i': 62, 'e': 68, 'w': 2, 'y': 6},
-  'Ti': {
-    'l': 35, 'p': 22, 'd': 7, 'm': 48, 'n': 56, 't': 18, 'r': 13, 's': 22,
-    'b': 17, 'j': 4, 'e': 35, 'c': 13, 'f': 7, 'g': 13, 'a': 3, 'u': 1, 'o': 3,
-    'z': 2, 'k': 1, 'x': 2, 'w': 1, 'v': 2
+  'zc': {'o': 7, 'l': 1, 'u': 1, 'a': 7, 'z': 17, 'h': 1},
+  'rf': {
+    'o': 29, 'i': 38, 'l': 8, 'a': 15, 'e': 45, '!': 93, 'f': 31, 'm': 4,
+    'u': 6, 'h': 1, 'k': 1, 's': 1, 'y': 1, 'r': 1, 't': 1
   },
-  'ti': {
-    'n': 482, 'z': 10, 'e': 167, 'l': 138, 's': 151, 'a': 65, 'c': 100, 't': 34,
-    'r': 22, 'v': 15, '!': 425, 'm': 32, 'd': 15, 'o': 28, 'g': 68, 'f': 10,
-    'h': 2, 'j': 4, 'u': 4, 'p': 10, 'b': 8, 'w': 2, 'x': 2, 'k': 14, 'y': 1
+  'fr': {'e': 62, 'i': 38, 'o': 28, 'a': 54, 'u': 1, 'y': 4},
+  'bt': {'r': 1, '!': 3, 's': 1},
+  'kp': {'a': 3, 'o': 1, 'e': 1},
+  'nb': {
+    'a': 161, 'e': 316, 'o': 55, 'u': 96, 'l': 15, 'y': 16, 'r': 58, 'i': 10
   },
-  'Tj': {'a': 3, 'e': 2},
-  'tj': {'o': 5, 'e': 21, 'a': 3, 'u': 3},
-  'Tk': {'a': 3},
-  'tk': {
-    'i': 30, 'e': 43, 'o': 65, 'a': 25, 'y': 2, 'n': 1, 'u': 8, 'r': 1, 'l': 1
+  'ik': {
+    'e': 113, '!': 294, 'o': 56, 's': 18, 'h': 6, 'i': 27, 'u': 16, 'l': 15,
+    'k': 16, 'a': 39, 'r': 2, 'm': 2, 't': 2, 'n': 1, 'y': 2
   },
-  'tl': {'e': 343, 'i': 67, 'o': 32, 'a': 52, 'u': 5, 'y': 12, '!': 15, 'l': 1},
-  'Tl': {'u': 2, 'l': 1, 'a': 3},
-  'tm': {'a': 206, 'o': 18, 'i': 11, 'e': 27, 'u': 3, 'y': 3},
-  'tn': {'e': 156, 'a': 16, 'u': 2, 'y': 5, 'o': 7, 'i': 25, '!': 1},
-  'to': {
-    'n': 1084, '!': 614, 's': 86, 'k': 14, 'y': 11, 'u': 45, 'r': 222, 'p': 30,
-    'v': 14, 'w': 59, 'c': 64, 'd': 14, 'x': 2, 'o': 21, 'l': 123, 'j': 3,
-    'm': 46, 'i': 9, 't': 27, 'f': 33, 'g': 14, 'e': 34, 'b': 13, 'h': 9,
-    'a': 3, 'z': 5
+  'Pl': {'u': 32, 'a': 103, 'e': 42, 'o': 35, 'y': 8, 'i': 10},
+  'Zu': {
+    'n': 7, 'b': 11, 'm': 14, 'c': 16, 'k': 8, 'r': 16, 'l': 8, 'e': 7, 'p': 5,
   },
-  'To': {
-    'r': 103, 'd': 17, 'w': 33, 'l': 55, 'm': 77, 'n': 42, 'b': 25, 'v': 6,
-    't': 20, 's': 18, 'o': 34, 'u': 40, 'y': 8, '!': 1, 'p': 39, 'k': 13,
-    'c': 10, 'z': 4, 'e': 14, 'f': 8, 'a': 7, 'x': 1, 'h': 5, 'g': 5, 'j': 1,
-    'i': 1, 'q': 1
+  'db': {'e': 43, 'u': 16, 'o': 16, 'y': 8, 'l': 7, 'r': 5, 'a': 12, 'i': 2},
+  'oi': {
+    'n': 64, 's': 107, '!': 16, 't': 28, 'r': 16, 'e': 11, 'x': 2, 'g': 9,
+    'l': 23, 'c': 11, 'a': 22, 'v': 2, 'z': 1, 'd': 11, 'k': 7, 'b': 3, 'o': 2,
+    'u': 1, 'w': 2, 'f': 1, 'm': 1
   },
-  'tp': {'i': 4, 'h': 5, 'e': 4, 'a': 2, 'f': 1},
-  'tq': {'u': 2},
-  'Tr': {
-    'a': 137, 'e': 153, 'u': 99, 'i': 126, 'o': 120, 'y': 12, 'n': 2, 'b': 1, 
-    'z': 1
+  'Iv': {'e': 13, 'y': 1, 'o': 2, 'i': 2, 'a': 8, 'r': 1},
+  'sk': {
+    'i': 1223, '!': 27, 'e': 207, 'r': 8, 'o': 116, 'y': 332, 'a': 106, 'u': 6,
+    'w': 2, 'n': 1, 'l': 3, 'v': 1, 't': 1
   },
-  'tr': {
-    'o': 360, 'i': 215, 'a': 282, 'e': 240, 'y': 46, 'u': 78, 'z': 10, 'b': 1,
-    'n': 2, 's': 2, 'm': 1, '!': 2
+  'lr': {'o': 30, 'e': 15, 'i': 21, 'y': 3, 'a': 13, 'u': 2, 'k': 1, '!': 1},
+  'tw': {'r': 5, 'o': 20, 'e': 26, 'a': 10, 'i': 33, 'y': 1},
+  'Ci': {
+    's': 13, 'n': 21, 'm': 12, 'o': 9, 'f': 3, 'r': 22, 'p': 13, 'c': 30,
+    'e': 20, 'l': 13, 'a': 31, 't': 14, 'u': 7, 'd': 2, 'v': 7, 'b': 5, 'z': 1,
+    'h': 2, 'g': 1
   },
-  'ts': {
-    '!': 280, 'o': 83, 'c': 111, 't': 14, 'f': 3, 'e': 53, 'm': 17, 'h': 15,
-    'u': 41, 'i': 24, 'b': 7, 'w': 6, 'l': 9, 'k': 36, 's': 1, 'p': 1, 'y': 3,
-    'a': 11, 'd': 2, 'g': 2, 'z': 1
+  'sn': {'e': 131, 'i': 35, 'a': 31, 'u': 2, 'o': 15, '!': 4, 'y': 6},
+  'Am': {
+    'o': 32, 'e': 40, 'b': 29, 'a': 39, 'm': 10, 'u': 4, 'i': 25, 'y': 5,
+    's': 15, 'r': 5, 'w': 1, 'p': 4, 'd': 2, 't': 1, 'l': 1
   },
-  'Ts': {'o': 3, 'a': 8, 'e': 4, 'c': 9, 'u': 16, 'i': 5, 'h': 1},
-  'tt': {
-    '!': 906, 'e': 836, 'h': 30, 'l': 127, 'o': 217, 's': 105, 'm': 51, 'y': 51,
-    'a': 230, 'i': 462, 'r': 48, 'n': 26, 'w': 8, 'c': 4, 'u': 18, 'f': 2,
-    'k': 13, 'z': 3, 'g': 6, 'b': 3, 'd': 1, 'j': 1
+  'Ku': {
+    'h': 29, 'r': 59, 'y': 5, 'n': 47, 'm': 12, 'e': 27, 't': 24, 'j': 7,
+    '!': 1, 's': 36, 'c': 31, 'g': 2, 'l': 41, 'b': 46, 'o': 2, 'z': 15, 'i': 7,
+    'k': 16, 'a': 8, 'p': 17, 'd': 14, 'f': 6, 'w': 3
   },
-  'tu': {
-    '!': 19, 'a': 9, 'm': 30, 'b': 21, 'r': 82, 's': 52, 'n': 30, 'c': 38,
-    'l': 33, 'd': 21, 't': 18, 'k': 6, 'g': 4, 'p': 9, 'i': 5, 'h': 4, 'f': 6,
-    'e': 19, 'o': 7, 'z': 2, 'v': 1, 'y': 2, 'q': 1
+  'uh': {
+    'n': 27, 'a': 35, 'l': 48, 'r': 27, '!': 14, 'o': 7, 'm': 11, 'e': 8,
+    't': 8, 'u': 3, 's': 5, 'y': 4, 'i': 2, 'f': 1, 'd': 1
   },
-  'Tu': {
-    'r': 110, 'c': 19, 't': 20, 'b': 12, 'g': 7, 'd': 6, 'l': 19, 'n': 18,
-    '!': 1, 'p': 9, 'f': 9, 's': 9, 'm': 19, 'o': 6, 'e': 8, 'i': 4, 'a': 5,
-    'k': 3, 'x': 2, 'h': 1, 'z': 3, 'y': 1, 'u': 1, 'j': 1
+  'wd': {
+    'e': 36, 'y': 8, '!': 5, 'l': 3, 'h': 1, 'o': 5, 'r': 3, 'i': 9, 'u': 1,
+    'z': 1, 'a': 4, 's': 1
   },
-  'Tv': {'e': 1},
-  'tv': {'i': 8, 'a': 3, 'e': 6, 'r': 1, '!': 1, 'o': 2},
-  'Tw': {'o': 8, 'i': 23, 'e': 15, 'y': 3, 'a': 3},
-  'tw': {'r': 5, 'o': 20, 'e': 26, 'a': 10, 'i': 33, 'y': 1},
-  'Ty': {
-    'l': 5, 's': 9, 'r': 12, 'n': 7, 'e': 3, 'u': 1, 'g': 2, 'o': 2, 'm': 5,
-    'b': 2, 'c': 2, 'a': 1, 't': 1, '!': 1, 'p': 1, 'k': 1, 'd': 2
+  'sw': {'o': 68, 'e': 36, 'a': 20, 'i': 16, 'h': 1, 'u': 1},
+  'ml': {'i': 41, 'e': 76, 'a': 12, 'y': 6, 'o': 3, 'u': 1, '!': 5, 's': 1},
+  'pl': {'e': 185, 'a': 37, 'i': 53, 'o': 9, 'u': 6, 'k': 1, '!': 4},
+  'cq': {'u': 64, '!': 2},
+  'Vo': {
+    'g': 22, 's': 17, '!': 1, 'l': 56, 'i': 13, 'o': 7, 'y': 3, 'e': 14, 'w': 3,
+    'n': 48, 't': 10, 'r': 24, 'u': 2, 'h': 1, 'k': 1, 'd': 3, 'j': 3, 'c': 6,
+    'v': 2, 'p': 1
   },
-  'ty': {
-    'r': 7, '!': 276, 'l': 6, 'm': 2, 'j': 1, 's': 5, 'n': 13, 'k': 5, 'e': 5,
-    'o': 1, 'a': 7, 'c': 2, 'b': 1, 'd': 1, 'i': 1
+  'nh': {'a': 163, '!': 19, 'o': 111, 'i': 10, 'u': 14, 'e': 45, 'y': 1, 's': 1
   },
-  'tz': {
-    '!': 572, 'g': 11, 'p': 2, 'e': 206, 'l': 48, 's': 14, 'm': 43, 'f': 5,
-    'w': 4, 'h': 6, 'o': 11, 'c': 1, 'i': 37, 'y': 3, 'k': 45, 'b': 15, 'a': 9,
-    'n': 12, 'r': 4, 'u': 1
+  'nm': {'a': 59, 'e': 18, 'i': 12, 'o': 9, 'u': 3, 'y': 7},
+  'Dw': {'y': 2, 'i': 4, 'o': 4, 'e': 4, 'a': 3},
+  'ze': {
+    'm': 14, 'l': 203, '!': 93, 'r': 227, 'n': 118, 'v': 3, 'e': 18, 'w': 62,
+    'a': 10, 'y': 21, 't': 13, 'c': 10, 'o': 4, 'k': 56, 'z': 4, 'j': 5, 'i': 2,
+    'p': 10, 'b': 8, 's': 22, 'g': 2, 'd': 1
   },
-  'Tz': {'e': 2},
-  'ua': {
-    'r': 94, 'n': 63, 'l': 38, 'j': 1, '!': 75, 'y': 15, 'x': 1, 'd': 21,
-    'c': 5, 'z': 5, 't': 14, 'm': 8, 'i': 18, 's': 14, 'v': 2, 'g': 10, 'h': 2,
-    'k': 3, 'w': 1, 'p': 2, 'a': 2, 'e': 1, 'f': 2
+  'up': {
+    'r': 20, 's': 12, 'u': 6, 'o': 12, 'p': 55, 'i': 30, '!': 71, 'e': 51,
+    't': 21, 'l': 14, 'a': 35, 'h': 6, 'k': 12, 'f': 6, 'b': 1, 'n': 2, 'c': 3,
+    'm': 1, 'y': 2
   },
-  'ub': {
-    'b': 56, 'e': 151, 'i': 99, 'o': 30, 'a': 88, 'y': 14, '!': 39, 'l': 36,
-    'r': 32, 'u': 12, 'm': 4, 'n': 7, 's': 12, 'k': 4, 'h': 2, 'v': 1, 'd': 1, 
-    'c': 1
+  'fs': {
+    'o': 15, 't': 21, 'i': 2, '!': 13, 'k': 19, 'n': 2, 'c': 3, 'u': 1, 'e': 9,
+    'r': 1, 'h': 3, 'a': 2, 'b': 1
   },
-  'Ub': {'e': 3, 'a': 2, 'o': 1, 'l': 1, 'r': 1, 'i': 1},
-  'Uc': {'h': 5, 'c': 4, '!': 1},
-  'uc': {
-    'k': 270, 'a': 48, 'h': 303, 'e': 51, '!': 12, 'i': 50, 'o': 15, 'y': 4,
-    'c': 152, 'l': 5, 'u': 6, 'z': 19, 'm': 1, 'r': 2, 'w': 1, 'n': 1, 'v': 1,
-    't': 1, 'g': 1
+  'aj': {
+    'o': 19, 'a': 46, 'e': 32, 'k': 8, 'i': 18, 'd': 10, '!': 33, 'c': 8,
+    'u': 7, 's': 1, 't': 2, 'l': 3, 'w': 2, 'z': 1, 'n': 3, 'j': 1, 'm': 1,
+    'g': 1, 'h': 1
   },
-  'Ud': {'e': 2, 'y': 1, 'o': 2, 'd': 1, 'l': 1, 'a': 1, 'i': 2},
-  'ud': {
-    's': 10, 'l': 25, '!': 94, 'o': 34, 'i': 78, 'd': 61, 'e': 177, 'r': 32,
-    'w': 8, 'g': 20, 'k': 7, 'y': 24, 'a': 67, 'n': 20, 't': 11, 'h': 8, 'j': 3,
-    'u': 4, 'z': 19, 'f': 1, 'm': 10, 'b': 4, 'v': 3
+  'jo': {
+    'r': 25, '!': 51, 's': 19, 'h': 12, 'y': 7, 'i': 2, 'n': 13, 'g': 1, 'e': 1,
   },
-  'Ue': {
-    'c': 2, 'h': 1, 'm': 1, 'd': 1, 'n': 1, 'l': 1, 'r': 1, 'k': 1, 'b': 1
+  'Aa': {
   },
-  'ue': {
-    'z': 67, 'r': 297, 'l': 146, 'n': 130, 'v': 17, '!': 216, 'g': 24, 'e': 9,
-    's': 114, 't': 108, 'y': 11, 'h': 50, 'd': 28, 'b': 28, 'c': 34, 'i': 12,
-    'x': 1, 'f': 5, 'm': 21, 'a': 7, 'u': 2, 'j': 1, 'k': 4, 'p': 4, 'o': 1, 
-    'w': 2
+  'Ot': {
+    't': 32, 'e': 4, 'o': 4, 'i': 3, 'a': 6, 'w': 1, 'h': 4, 's': 3, 'u': 3,
+    'r': 1, 'l': 1
   },
-  'uf': {
-    'f': 179, 'm': 2, 'o': 15, '!': 33, 'r': 4, 't': 9, 'e': 24, 'i': 10,
-    'a': 13, 'k': 3, 'u': 3, 'n': 4, 's': 5, 'l': 2, 'h': 1, 'd': 1, 'c': 1,
-    'z': 1, 'v': 1, 'b': 1
+  'si': {
+    'd': 25, '!': 167, 't': 35, 'l': 61, 'n': 325, 'e': 115, 'o': 55, 'm': 29,
+    'c': 84, 'a': 84, 's': 34, 'g': 32, 'u': 10, 'k': 34, 'r': 11, 'f': 8,
+    'v': 2, 'z': 5, 'p': 2, 'b': 4, 'q': 1, 'x': 2, 'y': 1
   },
-  'Uf': {'f': 2},
-  'Ug': {'a': 4, 'l': 3, 'o': 1},
-  'ug': {
-    'h': 483, 'l': 47, 'o': 13, 'g': 60, 'a': 67, 'e': 71, 'u': 26, '!': 19,
-    'b': 3, 's': 6, 'r': 8, 'i': 21, 'w': 1, 'n': 9, 'm': 6, 'd': 3, 't': 3, 
-    'f': 1
+  'Ky': {
+    'l': 5, 's': 3, 't': 2, 'z': 2, 'g': 1, 'e': 2, 'k': 1, 'u': 1, 'n': 3,
+    'm': 1, '!': 1, 'h': 1, 'p': 2
   },
-  'Uh': {'l': 9, 'r': 6, 'm': 1, 'y': 1, 'e': 1, 'a': 1, 'd': 1},
-  'uh': {
-    'n': 27, 'a': 35, 'l': 48, 'r': 27, '!': 14, 'o': 7, 'm': 11, 'e': 8,
-    't': 8, 'u': 3, 's': 5, 'y': 4, 'i': 2, 'f': 1, 'd': 1
+  'yw': {'o': 12, 'a': 12, 'e': 6, 'i': 8, 'h': 1},
+  'Ep': {'p': 19, 's': 2, 'l': 4, 't': 1, 'h': 2, 'o': 1, 'e': 2, 'i': 1},
+  'Ye': {
+    'a': 32, 'e': 3, 'h': 3, 'p': 4, 'u': 2, 'n': 12, 't': 6, 'l': 14, 'r': 22,
+    'o': 3, '!': 1, 'd': 3, 's': 4, 'c': 1, 'i': 3, 'b': 1, 'm': 2, 'w': 1,
+    'z': 1, 'k': 1, 'g': 1
   },
-  'Ui': {'t': 1, 'm': 1, 'h': 1},
-  'ui': {
-    'z': 26, 'l': 130, 'n': 143, 'r': 55, 't': 76, 'c': 16, 'd': 28, 's': 132,
-    'v': 7, 'g': 16, 'a': 18, '!': 44, 'e': 25, 'm': 8, 'b': 5, 'j': 7, 'o': 4,
-    'p': 3, 'k': 7, 'h': 4, 'f': 2, 'u': 1
+  'Ov': {'e': 50, 'a': 6, 'i': 6, 's': 1, 'd': 1},
+  'mn': {'e': 12, 'a': 8, 'i': 7, 'o': 2, 'y': 2, 'u': 1, '!': 3},
+  'cw': {'i': 4, 'h': 7, 'a': 9, 'e': 3, 'r': 1},
+  'sf': {'i': 13, 'o': 31, 'a': 2, 'e': 12, 'j': 1},
+  'Eu': {
   },
-  'Uj': {'a': 1},
-  'uj': {'i': 15, 'a': 23, 'o': 8, 'n': 1, 'l': 1, 'c': 1, '!': 1, 'e': 1},
-  'uk': {
-    'e': 58, '!': 63, 'i': 21, 'u': 18, 'a': 46, 'o': 29, 'n': 3, 'l': 7,
-    'h': 10, 's': 4, 'w': 1, 'm': 1, 'k': 5, 'c': 1, 'r': 3
+  'Eg': {
+    'a': 3, 'g': 18, 'b': 2, 'e': 12, 'u': 4, 'l': 10, 'n': 3, 'o': 2, 'i': 3,
+    'w': 1, 'v': 1
   },
-  'Uk': {'o': 1, 'n': 1, 'e': 2, '!': 1, 'i': 1},
-  'ul': {
-    'l': 366, 't': 167, '!': 56, 'k': 53, 'd': 60, 'e': 127, 'v': 17, 's': 66,
-    'z': 11, 'i': 159, 'p': 10, 'b': 27, 'm': 18, 'c': 21, 'o': 76, 'a': 146,
-    'h': 14, 'x': 3, 'f': 16, 'u': 15, 'g': 13, 'w': 10, 'y': 9, 'n': 11,
-    'r': 8, 'j': 1, 'q': 1
+  'Oh': {
+    'a': 16, '!': 1, 'l': 18, 'm': 9, 'e': 4, 'o': 3, 't': 1, 'r': 5, 's': 1,
+    'n': 2, 'y': 1
   },
-  'Ul': {
-    'r': 3, 'm': 4, 'l': 10, 'i': 6, 'e': 3, 's': 6, 'y': 1, 'b': 3, 't': 3,
-    'a': 3, 'w': 1, 'c': 2, 'd': 1, 'v': 2, 'j': 1
+  'Oa': {'k': 10, 't': 9, 's': 1, 'r': 3, 'c': 1, 'j': 1, 'x': 1},
+  'gf': {'o': 9, 'i': 12, 'a': 2, 'e': 7, 'r': 3},
+  'lw': {'o': 23, 'e': 24, 'a': 35, 'i': 21, 'h': 1, 'r': 3, 'y': 2, 's': 1},
+  'gb': {
+    'l': 6, 'y': 8, 'e': 26, 'u': 7, 'o': 10, 'a': 7, 'i': 7, 'r': 2, 'h': 1
   },
-  'Um': {
-    'a': 3, 'b': 9, 's': 2, 'p': 4, 'l': 2, '!': 1, 'f': 1, 'i': 1, 'h': 1,
-    'e': 2, 'n': 1
+  'Yb': {'a': 5, 'o': 1},
+  'hs': {
+    '!': 49, 'o': 10, 't': 17, 'm': 4, 'l': 3, 'c': 4, 'e': 21, 'n': 1, 'i': 5,
+    'a': 2, 'h': 2, 'w': 1, 'p': 2, 'b': 1
   },
-  'um': {
-    'm': 107, 'p': 92, '!': 299, 'b': 131, 'a': 124, 'n': 6, 'f': 10, 'g': 16,
-    'e': 83, 'o': 28, 'l': 27, 'w': 6, 's': 28, 'r': 9, 't': 2, 'h': 5, 'u': 6,
-    'i': 41, 'k': 5, 'z': 1, 'v': 1, 'd': 1, 'y': 1
+  'bc': {'o': 1, 'z': 5, 'h': 1, 'k': 1},
+  'Kh': {'a': 33, 'o': 14, 'i': 3, 'e': 5, 'u': 4, 'n': 1, 'l': 1},
+  'uv': {'a': 22, 'i': 20, 'e': 44, 'o': 5, 'r': 3, '!': 1, 'k': 1},
+  'Xi': {'o': 1, 'e': 1, 'a': 3, 'm': 2},
+  'Yu': {
+    '!': 1, 'e': 5, 'n': 10, 'a': 2, 't': 1, 'h': 2, 'l': 1, 'r': 12, 's': 8,
+    'm': 2, 'p': 1, 'i': 1, 'k': 2, 'd': 1, 'z': 1, 'c': 1
   },
-  'Un': {
-    'd': 10, 'g': 12, 'r': 5, 'k': 2, 'z': 2, 's': 4, 't': 9, 'n': 3, 'o': 1,
-    'i': 4, 'c': 3, 'a': 2, 'l': 1, 'v': 2
+  'du': {
+    'e': 17, 'f': 11, 'c': 23, 'm': 7, 'x': 3, 'z': 5, 'l': 24, 's': 30, 't': 6,
+    'g': 5, 'j': 3, 'r': 21, 'n': 16, 'k': 6, 'a': 10, 'p': 3, 'y': 3, 'i': 1,
+    '!': 10, 'd': 3, 'h': 1, 'o': 1
   },
-  'un': {
-    'g': 131, 't': 123, 'n': 101, 'c': 57, 'o': 32, 'd': 314, 'e': 123, 'a': 75,
-    '!': 125, 'l': 21, 'b': 10, 'i': 82, 'h': 5, 'k': 95, 's': 92, 'y': 17,
-    'z': 43, 'r': 4, 'f': 9, 'p': 2, 'm': 8, 'w': 5, 'j': 2, 'q': 1, 'u': 4
+  'iu': {
+    's': 72, '!': 12, 'l': 18, 'n': 3, 'r': 6, 'd': 6, 'c': 5, 'f': 5, 'z': 4,
+    't': 6, 'k': 11, 'm': 7, 'b': 3, 'e': 3
   },
-  'Uo': {'n': 1, 'y': 1},
-  'uo': {
-    'n': 36, 'm': 7, 't': 10, '!': 11, 'h': 4, 'c': 4, 'f': 1, 'l': 8, 'r': 9,
-    'w': 1, 'z': 4, 'i': 2, 'y': 1, 'b': 1, 'p': 2, 'g': 1, 's': 4, 'd': 1,
-    'k': 3, 'a': 1
+  'hb': {'u': 10, 'y': 5, 'e': 32, 'o': 11, 'a': 34, 'r': 3, 'i': 5},
+  'vo': {
+    '!': 41, 'r': 44, 'i': 6, 's': 17, 'y': 9, 't': 11, 'e': 4, 'b': 3, 'n': 54,
   },
-  'up': {
-    'r': 20, 's': 12, 'u': 6, 'o': 12, 'p': 55, 'i': 30, '!': 71, 'e': 51,
-    't': 21, 'l': 14, 'a': 35, 'h': 6, 'k': 12, 'f': 6, 'b': 1, 'n': 2, 'c': 3,
-    'm': 1, 'y': 2
+  'Ec': {'h': 18, 'k': 41, 'c': 2, 't': 2, 'o': 7, 'l': 1},
+  'Wu': {
+    '!': 1, 'r': 13, 'n': 9, 'l': 5, 'e': 10, 's': 1, 't': 1, 'o': 2, 'j': 1,
+    'b': 5, 'i': 1, 'c': 1
   },
-  'Up': {
-    't': 7, 'c': 1, 's': 3, 'h': 4, 'd': 4, 'l': 1, 'r': 1, 'p': 3, 'm': 1,
-    'w': 1, 'a': 1, 'o': 1
+  'tb': {'r': 12, 'e': 16, 'y': 4, 'u': 3, 'o': 2, 'a': 5, 'i': 4, 'l': 1},
+  'my': {
+    '!': 45, 't': 2, 'e': 25, 'r': 7, 'a': 3, 'x': 1, 's': 2, 'l': 3, 'o': 2,
+    'n': 2, 'k': 2
   },
-  'uq': {'u': 19, 'd': 1},
-  'Ur': {
-    'b': 20, 'i': 15, 'e': 10, 'q': 7, 'r': 7, 's': 8, 'm': 4, 'a': 7, 't': 6,
-    'g': 1, 'd': 2, 'u': 1, 'f': 1, 'z': 1, 'w': 1, 'p': 1, 'l': 2, 'h': 1,
-    'c': 1, '!': 1, 'n': 1
+  'zz': {
+    'i': 124, 'o': 86, 'e': 43, 'a': 89, 'l': 7, 'u': 16, '!': 2, 'y': 2, 'n': 1
   },
-  'ur': {
-    'n': 232, 'p': 22, 'r': 174, 't': 159, 'k': 99, 'g': 246, 'a': 190,
-    'e': 208, 's': 106, 'h': 6, 'c': 71, 'l': 87, '!': 178, 'm': 34, 'd': 82,
-    'i': 179, 'v': 16, 'b': 53, 'y': 100, 'q': 2, 'o': 73, 'f': 19, 'w': 13,
-    'u': 18, 'z': 21, 'j': 3
+  'gm': {'a': 72, 'o': 12, 'i': 7, 'u': 2, 'e': 6, '!': 1, 'y': 2},
+  'Ou': {
+    'e': 4, 't': 13, 's': 2, 'b': 1, 'z': 1, 'r': 7, 'i': 4, 'l': 2, 'k': 1,
+    'm': 1, '!': 1, 'n': 2, 'd': 3, 'c': 2, 'y': 1
   },
-  'Us': {
-    'h': 3, 's': 1, 'r': 2, 'e': 4, 'i': 3, 'o': 1, '!': 1, 't': 1, 'm': 1,
-    'c': 1, 'a': 1
+  'Og': {
+    'd': 1, 'l': 6, 'r': 4, 'b': 3, 'i': 6, 'g': 1, 'o': 1, 'a': 14, 'u': 5,
+    'w': 2, 'e': 4, 'z': 1, 's': 1
   },
-  'us': {
-    's': 233, 'o': 59, 't': 209, 'h': 153, 'e': 285, '!': 539, 'k': 106,
-    'b': 18, 'c': 125, 'a': 72, 'i': 78, 'g': 4, 'l': 28, 'q': 4, 'm': 21,
-    'n': 17, 'u': 14, 'w': 5, 'z': 34, 'd': 6, 'y': 1, 'f': 1, 'r': 1
+  'gd': {'e': 9, 'o': 19, 'a': 21, 'i': 2, '!': 2, 'y': 1, 's': 1},
+  'yb': {
+    'e': 22, 'u': 17, 'a': 21, 'i': 7, 'o': 20, 'l': 2, 'y': 7, 'r': 10, 'b': 1,
+    'k': 1, 'c': 1, '!': 2, 's': 1
   },
-  'Ut': {'l': 1, 't': 5, 'e': 1, 'z': 3, 's': 2, 'h': 1, 'v': 1},
-  'ut': {
-    'l': 26, 'i': 63, 't': 215, 'c': 62, '!': 113, 'h': 169, 'z': 81, 'n': 20,
-    's': 47, 'u': 14, 'm': 17, 'r': 39, 'o': 69, 'e': 131, 'y': 15, 'w': 7,
-    'p': 2, 'k': 21, 'a': 55, 'f': 3, 'g': 4, 'j': 3, 'b': 2, 'v': 1
+  'lz': {
+    '!': 55, 'e': 50, 'a': 17, 'm': 7, 'i': 11, 'o': 8, 'y': 2, 'w': 4, 'g': 1,
+    'h': 4, 'b': 3, 'l': 5, 'u': 2, 'r': 1, 'n': 2
   },
-  'uu': {'!': 3, 'd': 1, 'r': 2, 'a': 1, 'l': 2, 's': 4, 'k': 1, 'n': 1},
-  'Uu': {'t': 1},
-  'uv': {'a': 22, 'i': 20, 'e': 44, 'o': 5, 'r': 3, '!': 1, 'k': 1},
-  'Uv': {'a': 3},
-  'uw': {
-    'e': 14, '!': 11, 'i': 2, 'a': 10, 's': 1, 'm': 1, 'k': 2, 'w': 1, 'h': 1
+  'Is': {
+    'a': 28, 'o': 4, 'b': 5, 'r': 5, 'h': 13, 'e': 14, 'l': 10, 'm': 3, 's': 4,
+    't': 2, 'k': 1, 'n': 1, 'i': 8, 'c': 1, 'g': 3
   },
+  'aq': {'u': 51, 'v': 1, '!': 4, 'r': 1},
   'ux': {
     '!': 135, 't': 4, 'i': 3, 'h': 2, 'b': 3, 'f': 1, 'm': 2, 'e': 2, 'o': 4,
     'l': 2, 'w': 1
   },
-  'Ux': {'a': 1},
-  'Uy': {'!': 1, 'e': 6},
-  'uy': {
-    'e': 27, '!': 21, 'n': 13, 't': 5, 'k': 3, 'l': 8, 'b': 1, 'd': 3, 's': 11,
-    'p': 3, 'a': 14, 'r': 3, 'm': 2, 'o': 7, 'v': 1, 'c': 2, 'g': 1, 'z': 1
-  },
-  'uz': {
-    '!': 28, 'm': 12, 'a': 33, 'c': 2, 'u': 4, 'z': 79, 'o': 7, 'i': 35, 't': 1,
-    'b': 4, 'y': 6, 'e': 27, 'l': 1, 'q': 1, 'n': 4, 'h': 1, 's': 1
-  },
-  'Uz': {'z': 3, 'e': 2, 'd': 1, 'i': 1, 'u': 1},
-  'va': {
-    'n': 219, 'r': 125, '!': 112, 'l': 126, 'g': 27, 's': 40, 'k': 13, 'z': 8,
-    't': 52, 'y': 12, 'c': 25, 'e': 3, 'd': 17, 'i': 23, 'j': 1, 'u': 9, 'o': 3,
-    'm': 2, 'a': 4, 'b': 1, 'v': 1, 'h': 2, 'p': 1
+  'Ez': {'e': 6, 'z': 3, 'a': 1, 'p': 2, 'd': 1},
+  'Cy': {'r': 6, 'p': 7, 'b': 2, 'g': 3, 'n': 2, 'w': 1, 'l': 2, 'f': 1, 'c': 1
   },
-  'Va': {
-    's': 52, 'r': 79, 'u': 20, 'l': 141, 'z': 5, 'n': 527, 'i': 16, 'c': 22,
-    'd': 7, 't': 9, 'v': 4, 'q': 4, 'w': 1, 'h': 3, 'y': 4, 'g': 9, 'k': 4,
-    'j': 3, '!': 1, 'm': 1, 'f': 2, 'e': 2
+  'Ap': {
+    'o': 12, 'p': 35, 'a': 8, 'e': 6, 'g': 1, 'r': 6, 'i': 2, 'u': 2, 'l': 5,
+    'f': 1, 't': 2, 's': 2, 'k': 3, 'y': 1
   },
-  'Vb': {'i': 1},
-  'vc': {'i': 1, 'e': 2, 'c': 1},
-  'vd': {'e': 4, 'a': 2, '!': 2},
-  'Ve': {
-    'g': 8, 'l': 54, 'n': 83, 'r': 144, 's': 25, 't': 11, 'a': 14, 'i': 15,
-    'd': 3, 'c': 8, 'z': 2, 'y': 4, 'v': 3, 'e': 8, 'j': 2, 'h': 2, 'k': 1,
-    'm': 1, 'b': 1, '!': 1
+  'Ze': {
+    'p': 6, 'i': 23, 'l': 41, 'r': 23, 'n': 25, 'h': 11, 'm': 13, 'b': 5,
+    'o': 2, 'c': 10, 't': 9, 'e': 5, 'f': 1, 'v': 2, 's': 2, 'd': 3, 'a': 6,
+    'g': 5, 'u': 1, 'y': 2, 'k': 1, 'z': 1
   },
-  've': {
-    'r': 627, 'n': 239, 'z': 18, 'y': 64, 's': 109, '!': 167, 'd': 28, 'l': 205,
-    't': 59, 'i': 13, 'j': 6, 'a': 23, 'c': 28, 'e': 19, 'v': 2, 'g': 4, 'u': 6,
-    'm': 5, 'q': 1, 'o': 2, 'h': 4, 'k': 4, 'b': 3
+  'wc': {
   },
-  'vf': {'a': 1},
-  'vg': {'r': 1, 'l': 1},
-  'vh': {'a': 1},
-  'Vi': {
-    'n': 45, 'l': 118, 'g': 28, 'c': 40, 'd': 22, 't': 44, 'e': 44, 'o': 8,
-    'r': 36, 'a': 17, 's': 33, 'v': 18, 'z': 10, 'b': 3, 'p': 2, 'm': 1, 'x': 3,
-    'k': 3, 'j': 2
+  'sd': {'a': 38, 'o': 28, 'e': 32, 'i': 5, 'y': 1},
+  'kt': {'o': 7, 'a': 3, 'e': 3, '!': 2, 'n': 1, 'i': 1, 'h': 1, 's': 1},
+  'zo': {
+    's': 17, '!': 177, 'g': 4, 'n': 50, 't': 8, 'l': 29, 'y': 1, 'r': 21,
   },
-  'vi': {
-    's': 87, 'd': 29, 'l': 181, 'n': 231, 'e': 75, 't': 91, 'g': 30, 'a': 52,
-    '!': 33, 'z': 9, 'c': 200, 'r': 17, 'h': 1, 'u': 3, 'v': 4, 'o': 23,
-    'k': 13, 'j': 1
+  'ln': {
+    '!': 8, 'e': 50, 'a': 16, 'i': 31, 'u': 4, 'y': 3, 'h': 1, 'o': 7, 'n': 1
   },
-  'vj': {'o': 1, 'e': 2},
-  'vk': {'i': 1, 'a': 6, 'e': 1, 'o': 1, '!': 1},
-  'Vl': {'c': 2, 'a': 6, 'l': 1, 'i': 2, 'j': 1, 'e': 1, 'k': 1},
-  'vl': {'i': 24, 'e': 14, 'a': 7, 'o': 7, 'y': 1, 'u': 1},
-  'vm': {'a': 1},
-  'vn': {'e': 12, 'a': 3, 'i': 2, 'o': 1, 'y': 1},
-  'vo': {
-    '!': 41, 'r': 44, 'i': 6, 's': 17, 'y': 9, 't': 11, 'e': 4, 'b': 3, 'n': 54,
-    'a': 1, 'u': 3, 'l': 35, 'c': 5, 'o': 8, 'g': 3, 'd': 1, 'w': 1, 'f': 1, 
-    'z': 1
+  'Ul': {
+    'r': 3, 'm': 4, 'l': 10, 'i': 6, 'e': 3, 's': 6, 'y': 1, 'b': 3, 't': 3,
+    'a': 3, 'w': 1, 'c': 2, 'd': 1, 'v': 2, 'j': 1
   },
-  'Vo': {
-    'g': 22, 's': 17, '!': 1, 'l': 56, 'i': 13, 'o': 7, 'y': 3, 'e': 14, 'w': 3,
-    'n': 48, 't': 10, 'r': 24, 'u': 2, 'h': 1, 'k': 1, 'd': 3, 'j': 3, 'c': 6,
-    'v': 2, 'p': 1
+  'Sq': {'u': 15},
+  'wb': {'y': 1, 'e': 14, 'r': 9, 'o': 8, 'u': 5, 'i': 1, 'a': 9, 'l': 1},
+  'tj': {'o': 5, 'e': 21, 'a': 3, 'u': 3},
+  'Et': {
+    'h': 10, 't': 8, 'i': 2, 'z': 3, 'c': 4, 's': 1, 'l': 1, 'k': 1, 'u': 1,
+    'r': 1, 'o': 1
   },
-  'vr': {'i': 11, 'e': 15, 'o': 13, 'a': 13, 'c': 1},
-  'Vr': {'o': 3, 'e': 7, 'a': 10, 'i': 3, 'b': 3},
-  'vs': {
-    'o': 1, 'k': 26, 'e': 5, 'h': 2, '!': 5, 'a': 3, 'v': 1, 'n': 1, 't': 1, 
-    'c': 1
+  'Py': {
+    'l': 5, 'e': 4, 'a': 2, 'n': 2, 'r': 3, 'b': 2, 'p': 1, 'k': 1, 'u': 1,
+    't': 4, 'o': 2, 's': 2, 'c': 2, '!': 1, 'w': 1, 'f': 2
   },
-  'vt': {'i': 1, 'y': 1},
-  'Vu': {
-    '!': 1, 'e': 1, 'o': 4, 'n': 1, 'y': 1, 'l': 4, 'k': 5, 'i': 1, 'g': 1,
-    'c': 1, 't': 1
+  'hc': {'o': 17, 'r': 7, 'u': 2, 'a': 4, 'h': 1, 'l': 2, 'e': 1},
+  'eu': {
+    '!': 41, 'm': 18, 'x': 20, 'r': 63, 'n': 27, 't': 44, 'f': 11, 'b': 21,
+    'e': 33, 'v': 11, 's': 51, 'd': 16, 'i': 10, 'l': 20, 'h': 6, 'c': 13,
+    'g': 8, 'z': 5, 'w': 7, 'k': 6, 'a': 10, 'p': 6, 'y': 2, 'j': 1
   },
-  'vu': {'z': 3, 'c': 1, 'h': 1, 'r': 1, 'e': 1, 'l': 1},
-  'vv': {'o': 1},
-  'vw': {'i': 2},
-  'vy': {'!': 36, 'e': 2, 'n': 1, 'a': 1, 'd': 1},
-  'Vy': {'a': 1, '!': 1, 'h': 1},
-  'vz': {'o': 1, 'e': 1, 'i': 1},
-  'Wa': {
-    'l': 210, 'r': 126, 't': 52, 's': 72, 'g': 36, 'd': 32, 'n': 57, 'i': 34,
-    'k': 20, 'y': 25, 'u': 11, 'h': 23, 'm': 11, 'c': 23, 'x': 3, 'f': 5,
-    'e': 6, 'w': 2, 'a': 6, 'j': 1, 'p': 3, 'v': 4, 'b': 2, 'z': 1
+  'Ur': {
+    'b': 20, 'i': 15, 'e': 10, 'q': 7, 'r': 7, 's': 8, 'm': 4, 'a': 7, 't': 6,
+    'g': 1, 'd': 2, 'u': 1, 'f': 1, 'z': 1, 'w': 1, 'p': 1, 'l': 2, 'h': 1,
+    'c': 1, '!': 1, 'n': 1
   },
-  'wa': {
-    'r': 157, 'n': 118, 'y': 132, 'i': 40, 'k': 12, 'l': 156, 'b': 11, 'f': 1,
-    't': 53, '!': 77, 'd': 18, 'x': 2, 's': 22, 'c': 13, 'm': 11, 'g': 18,
-    'p': 2, 'a': 3, 'j': 2, 'h': 7, 'o': 1, 'u': 1, 'v': 1, 'e': 2, 'z': 1
+  'Oj': {'e': 1, 'a': 5, 'i': 2},
+  'Up': {
+    't': 7, 'c': 1, 's': 3, 'h': 4, 'd': 4, 'l': 1, 'r': 1, 'p': 3, 'm': 1,
+    'w': 1, 'a': 1, 'o': 1
   },
-  'wb': {'y': 1, 'e': 14, 'r': 9, 'o': 8, 'u': 5, 'i': 1, 'a': 9, 'l': 1},
-  'wc': {
-    'o': 8, 'e': 2, 'z': 7, 'r': 2, 'h': 4, 'u': 2, 'l': 1, 'a': 1, 'k': 2, 
-    '!': 1
+  'dh': {
+    'a': 41, 'o': 27, 'e': 11, 'u': 16, 'i': 6, 'r': 3, 'y': 2, '!': 1, 'n': 1
   },
-  'wd': {
-    'e': 36, 'y': 8, '!': 5, 'l': 3, 'h': 1, 'o': 5, 'r': 3, 'i': 9, 'u': 1,
-    'z': 1, 'a': 4, 's': 1
+  'kf': {'o': 16, 'i': 9, 'e': 2},
+  'dc': {'o': 7, 'l': 2, 'a': 5, 'h': 3, 'u': 1, 'r': 2},
+  'Ai': {
+    'k': 6, 'n': 9, 'e': 2, 't': 8, 'c': 2, 's': 1, 'g': 1, 'r': 5, 'l': 9,
+    'o': 2, 'm': 2, 'v': 1, 'u': 3, 'd': 2, 'y': 1, 'h': 1, 'p': 3, 'a': 1
   },
-  'Wd': {'o': 1},
-  'we': {
-    'l': 255, 'n': 72, 'r': 152, '!': 52, 'e': 53, 'y': 16, 's': 20, 'a': 31,
-    'i': 61, 't': 31, 'h': 6, 'd': 20, 'g': 16, 'c': 8, 'b': 6, 'k': 6, 'm': 3,
-    'z': 2, 'p': 2, 'j': 1, 'f': 1
+  'yv': {'a': 4, 'i': 2, 'e': 7},
+  'cs': {
+    '!': 10, 'o': 7, 'w': 5, 'h': 6, 'p': 5, 'i': 4, 's': 1, 'a': 3, 'f': 1,
+    'm': 1, 'e': 1, 'k': 5, 't': 1
   },
-  'We': {
-    's': 115, 'l': 68, 'b': 9, 'a': 49, 'i': 167, 'e': 28, 'r': 57, 't': 26,
-    'n': 77, 'd': 28, 'g': 16, 'x': 2, 'y': 17, 'c': 10, 'h': 26, 'v': 1,
-    'm': 7, 'p': 1, 'k': 2, 'f': 1, 'u': 1, 'w': 1
+  'Ok': {
+    'e': 13, 'a': 9, 'u': 13, '!': 1, 'o': 12, 'i': 9, 't': 1, 'r': 2, 's': 1,
+    'k': 1, 'w': 1
   },
-  'wf': {'o': 4, 'i': 1, '!': 1, 'e': 1},
-  'wg': {'i': 2, 'e': 3, 'o': 1, 'l': 1, 'a': 1, 'r': 1},
-  'Wh': {'i': 174, 'e': 45, 'a': 19, 'y': 9, 'o': 7, 't': 1},
   'wh': {'o': 15, 'i': 16, 'a': 9, 'e': 4, 'u': 1, 'y': 1},
-  'Wi': {
-    'l': 259, 's': 70, 'g': 36, 'n': 189, 't': 86, 'c': 45, 'm': 19, 'r': 20,
-    'e': 93, 'd': 34, 'b': 7, 'k': 12, 'x': 5, 'a': 8, 'f': 1, 'p': 5, 'z': 3,
-    'o': 1, 'u': 1, 'i': 1
-  },
-  'wi': {
-    's': 33, 'n': 166, 't': 86, 'f': 2, 'l': 49, 'g': 29, 'c': 207, 'e': 58,
-    'a': 25, 'd': 11, 'm': 5, 'h': 1, 'k': 7, 'r': 15, '!': 7, 'z': 1, 'p': 1
+  'uo': {
+    'n': 36, 'm': 7, 't': 10, '!': 11, 'h': 4, 'c': 4, 'f': 1, 'l': 8, 'r': 9,
+    'w': 1, 'z': 4, 'i': 2, 'y': 1, 'b': 1, 'p': 2, 'g': 1, 's': 4, 'd': 1,
+    'k': 3, 'a': 1
   },
-  'wk': {'i': 11, '!': 5, 's': 4, 'e': 9, 'a': 10, 'w': 1, 'o': 2},
-  'wl': {
-    'e': 66, 'a': 15, 'i': 30, 's': 6, 't': 1, 'k': 1, 'o': 6, '!': 8, 'b': 1,
-    'd': 1, 'u': 4, 'y': 1
+  'pu': {
+    'r': 19, 'l': 18, 'i': 2, 't': 9, 'z': 7, 'a': 7, 's': 15, 'y': 3, 'e': 5,
+    '!': 4, 'c': 4, 'h': 1, 'n': 5, 'g': 1, 'd': 1, 'p': 1
   },
-  'Wl': {'o': 5, 'a': 2},
-  'wm': {'a': 20, 'e': 4, 'o': 1, '!': 1, 'y': 1},
-  'Wm': {'s': 1, 'i': 1},
-  'wn': {
-    '!': 41, 's': 16, 'i': 9, 'e': 29, 'l': 6, 'f': 1, 'o': 1, 'b': 2, 'a': 4,
-    'd': 4, 'u': 2, 'r': 1, 'h': 3, 'w': 1, 't': 2, 'z': 1, 'y': 2
+  'Aq': {'u': 9},
+  'Eb': {
   },
-  'Wn': {'u': 2, 'e': 1, 'o': 1},
-  'wo': {
-    'o': 111, 'r': 137, 'l': 25, 'p': 3, 'n': 15, 'm': 3, 'k': 1, 'f': 2,
-    'b': 1, 'z': 2, 'g': 3, 's': 4, 'u': 4, 'y': 2, 'h': 4, 'a': 2, '!': 6,
-    'w': 2, 'c': 2, 'e': 2, 'd': 3
+  'Vu': {
+    '!': 1, 'e': 1, 'o': 4, 'n': 1, 'y': 1, 'l': 4, 'k': 5, 'i': 1, 'g': 1,
+    'c': 1, 't': 1
   },
-  'Wo': {
-    'o': 116, 'l': 105, 'n': 13, 'r': 63, 'm': 11, 'f': 1, 'z': 5, 'j': 24,
-    't': 3, 'e': 16, 'h': 17, 'u': 4, 'b': 4, 'g': 2, 'd': 3, 'w': 1, 'i': 2,
-    'y': 5, 's': 3, 'k': 1
+  'bn': {'e': 31, 'a': 2, 'o': 1, 'y': 1, 'i': 3},
+  'fn': {'e': 33, 'a': 4, 'i': 1},
+  'Pf': {'e': 13, 'a': 14, 'i': 6, 'l': 15, 'o': 5, 'u': 3, 'r': 2, 'n': 1},
+  'mw': {'e': 7, 'a': 7, 'o': 3, 'i': 1, 'r': 1},
+  'sy': {
   },
-  'wp': {'o': 1, 'e': 1, 'r': 1},
-  'wq': {'u': 1},
-  'wr': {'e': 10, 'i': 24, 'y': 11, 'a': 6, 'o': 8, 'z': 1},
-  'Wr': {'i': 17, 'a': 8, 'e': 8, 'o': 10, 'z': 2, 'y': 4, 'u': 2},
-  'ws': {
-    '!': 40, 'o': 21, 't': 7, 'e': 20, 'k': 491, 'l': 2, 'b': 2, 'h': 4, 'm': 1,
-    'u': 1, 'a': 2
+  'Om': {
   },
-  'wt': {'o': 8, 'h': 16, 'e': 6, 'y': 1, 'i': 1, 'r': 2, 's': 1},
-  'Wu': {
-    '!': 1, 'r': 13, 'n': 9, 'l': 5, 'e': 10, 's': 1, 't': 1, 'o': 2, 'j': 1,
-    'b': 5, 'i': 1, 'c': 1
+  'gw': {'e': 15, 'a': 13, 'o': 19, 'i': 13, 'u': 1, 'y': 1},
+  'kr': {'e': 25, 'i': 22, 'u': 7, 'a': 30, 'z': 4, 'o': 18, 'y': 2, '!': 2},
+  'dq': {'u': 8},
+  'ao': {
+    '!': 82, 'n': 7, 'l': 25, 'r': 3, 'u': 5, 'k': 8, 'i': 6, 'o': 2, 'm': 3,
+    'a': 5, 's': 2, 'h': 1, 'p': 1, 'b': 2
   },
-  'wu': {'s': 1, 'l': 3, '!': 1, 'c': 1, 'r': 1, 'o': 2, 'n': 1, 'h': 1},
-  'wv': {'e': 4, 'i': 1},
-  'ww': {'i': 1, 'a': 4},
-  'Wy': {
-    'a': 4, 'n': 12, 'm': 4, 'l': 8, 'c': 4, 'r': 5, 's': 6, 'b': 3, 'g': 4,
-    'd': 6, 'e': 3, 'k': 5, 't': 2, 'z': 2, 'o': 1
+  'rx': {'!': 5, 'l': 1, 'e': 1, 's': 1},
+  'sr': {'a': 10, 'o': 10, 'e': 6, 'y': 1, 'u': 10, 'i': 5, '!': 2},
+  'pc': {'h': 7, 'i': 3, 'z': 3, 'a': 2},
+  'gp': {'e': 2, 'u': 2, 'h': 1, 'i': 1, 'r': 1, 'a': 2},
+  'Yi': {'!': 1, 'n': 4, 'm': 1, 'p': 1, 'e': 1, 'u': 1, 'l': 1, 'd': 1},
+  'mf': {'i': 10, 'o': 10, 'e': 7, 'l': 1, 'f': 1, 'r': 1, 'a': 1},
+  'mr': {'i': 26, 'o': 16, 'a': 10, 'e': 13, 'h': 1, 'y': 3, '!': 1, 'u': 1},
+  'hf': {'o': 13, 'i': 23, 'u': 2, 'e': 7},
+  'xe': {'y': 7, 'i': 2, 'l': 17, 'n': 14, 'r': 5, '!': 5, 'd': 1},
+  'Ny': {
+    'e': 2, 's': 4, 'b': 2, 'g': 4, 'm': 1, 'q': 1, 'l': 5, 'c': 2, 'h': 3,
+    'r': 1, 'd': 3, 'p': 1, '!': 1, 'u': 1, 'k': 1, 'a': 1
   },
-  'wy': {
-    'e': 13, 'm': 3, 'n': 13, 'k': 5, '!': 9, 'g': 1, 'l': 2, 'f': 1, 'h': 1,
-    'r': 1, 't': 1, 's': 1, 'c': 2, 'a': 1, 'i': 1
+  'ij': {'e': 7, 'o': 14, 'a': 24, '!': 2, 'u': 1, 'i': 3},
+  'oq': {'u': 22},
+  'Zo': {
+    'o': 1, 'r': 15, 'l': 22, 'e': 5, 'b': 2, 'n': 5, 'g': 4, 'd': 3, 'c': 2,
+    'h': 1, 'z': 1, 'u': 6, 't': 3, 's': 2, 'm': 7, 'q': 1
   },
-  'wz': {'e': 3, 'a': 1},
-  'Wz': {'o': 1},
-  'xa': {
-    'n': 9, 'd': 2, 's': 3, 'u': 1, 'm': 1, 'c': 2, 'l': 1, 'y': 8, '!': 4,
-    'k': 2, 'r': 1
+  'vl': {'i': 24, 'e': 14, 'a': 7, 'o': 7, 'y': 1, 'u': 1},
+  'Ah': {
+    'm': 5, 'r': 10, 'e': 3, 'n': 4, 'o': 3, 'l': 21, 'u': 3, 'a': 7, 's': 2,
+    'y': 2, 'i': 2, 'h': 1
   },
-  'Xa': {'v': 1, 'n': 2, 'y': 2, 'i': 1},
-  'xb': {'y': 3, 'a': 1, 'u': 5, 'e': 3, 'o': 2},
-  'xc': {'y': 1, 'e': 1, 'o': 1},
-  'xd': {'o': 1},
-  'xe': {'y': 7, 'i': 2, 'l': 17, 'n': 14, 'r': 5, '!': 5, 'd': 1},
-  'xf': {'i': 2, 'o': 6},
-  'xh': {'a': 3, 'o': 3, 'e': 1},
-  'xi': {
-    'e': 8, 's': 1, 'm': 3, 'o': 5, 'l': 4, 'd': 2, 'c': 4, '!': 2, 't': 1,
-    'n': 3, 'u': 1
+  'gy': {'!': 33, 'a': 2, 'e': 3, 'l': 1, 'i': 5, 'u': 1, 's': 1},
+  'tp': {'i': 4, 'h': 5, 'e': 4, 'a': 2, 'f': 1},
+  'cv': {'e': 6, 'a': 5, 'i': 5, 'o': 1},
+  'fl': {'e': 96, 'i': 30, 'a': 18, 'o': 14, 'u': 12, '!': 5, 'y': 2},
+  'Hs': {'u': 3, 'i': 6, 'y': 1},
+  'vr': {'i': 11, 'e': 15, 'o': 13, 'a': 13, 'c': 1},
+  'sg': {'o': 4, 'r': 19, 'e': 9, 'u': 6, 'a': 7, 'i': 3, 'l': 1},
+  'zl': {'e': 71, 'o': 16, 'a': 14, 'i': 6, '!': 5, 'y': 1},
+  'mg': {'a': 15, 'r': 6, 'o': 5, 'e': 2, '!': 1},
+  'Zh': {'a': 3, 'o': 2, 'u': 2, 'e': 2},
+  'Ut': {'l': 1, 't': 5, 'e': 1, 'z': 3, 's': 2, 'h': 1, 'v': 1},
+  'yh': {'e': 10, 'i': 3, 'r': 3, 'a': 14, 'u': 6, 'o': 7, 'n': 2, '!': 2},
+  'zs': {'i': 3, 'c': 11, '!': 4, 't': 2, 'a': 3},
+  'uq': {'u': 19, 'd': 1},
+  'Hw': {'a': 1, 'e': 1},
+  'ko': {
+    'u': 11, 'w': 227, 'y': 3, 'f': 27, 'l': 45, 'r': 46, '!': 257, 'x': 1,
+    'k': 6, 'p': 27, 'o': 8, 'v': 73, 't': 14, 's': 69, 'g': 7, 'b': 5, 'e': 3,
+    'n': 27, 'd': 5, 'm': 8, 'c': 10, 'j': 2, 'a': 2, 'h': 4, 'i': 1, 'z': 1
   },
-  'Xi': {'o': 1, 'e': 1, 'a': 3, 'm': 2},
-  'xk': {'i': 1},
+  'mk': {'e': 27, 'i': 12, 'o': 16, 'u': 8, 'a': 12},
+  'bv': {'r': 1, 'i': 1},
+  'sv': {'e': 6, 'o': 4, 'a': 4, 'i': 6},
+  'nv': {'i': 34, 'e': 22, 'a': 9, 'l': 3, 'o': 6, 'r': 1, 'u': 1},
   'xl': {'e': 22, 'i': 2, 'a': 1},
-  'xm': {'a': 8, 'o': 1},
-  'xn': {'a': 2, 'e': 6, 'd': 1},
-  'xo': {'n': 22, 'm': 2, 'p': 1, 't': 1, 'l': 1, '!': 1},
-  'xp': {'o': 1},
-  'xr': {'o': 3},
-  'xs': {'o': 17, 'a': 1, 'e': 1, 'm': 1, 'i': 1},
-  'xt': {'e': 13, 'o': 26, 'a': 3, '!': 3, 'h': 1, 'i': 1, 'r': 1, 'm': 1},
-  'Xu': {'!': 1, 'e': 1},
-  'xu': {'m': 3},
-  'xw': {'e': 5, 'o': 3, 'i': 1},
-  'xx': {'!': 2},
-  'xy': {'!': 2},
-  'Xy': {'o': 1},
-  'xz': {'a': 1},
-  'ya': {
-    'n': 104, 'l': 31, 't': 13, '!': 81, 'r': 53, 's': 28, 'm': 32, 'k': 15,
-    'w': 3, 'c': 9, 'h': 7, 'g': 6, 'z': 2, 'd': 6, 'y': 1, 'b': 4, 'v': 2,
-    'i': 2, 'o': 3, 'p': 1, 'e': 1, 'u': 1
-  },
-  'Ya': {
-    't': 4, 'n': 53, 'r': 28, 'z': 4, 'm': 24, 'g': 10, 'l': 2, 'p': 3, 'o': 1,
-    'e': 3, 'w': 3, 'u': 5, 'h': 5, 'd': 3, 's': 11, 'c': 12, 'b': 2, 'f': 6,
-    'k': 7, '!': 1, 'x': 1, 'i': 2, 'v': 1
+  'Us': {
+    'h': 3, 's': 1, 'r': 2, 'e': 4, 'i': 3, 'o': 1, '!': 1, 't': 1, 'm': 1,
+    'c': 1, 'a': 1
   },
-  'Yb': {'a': 5, 'o': 1},
-  'yb': {
-    'e': 22, 'u': 17, 'a': 21, 'i': 7, 'o': 20, 'l': 2, 'y': 7, 'r': 10, 'b': 1,
-    'k': 1, 'c': 1, '!': 2, 's': 1
+  'nq': {'u': 30},
+  'xf': {'i': 2, 'o': 6},
+  'xs': {'o': 17, 'a': 1, 'e': 1, 'm': 1, 'i': 1},
+  'hd': {'e': 8, 'r': 2, '!': 1, 'i': 4, 'o': 3, 'a': 4},
+  'Oq': {'u': 4},
+  'sj': {'a': 4, 'e': 1, 'o': 4},
+  'ku': {
+    's': 54, 'p': 8, 'm': 20, 'l': 26, 'b': 11, 'c': 7, 'd': 3, 'h': 5, '!': 11,
   },
-  'yc': {
-    'e': 14, 'u': 9, 'o': 15, 'k': 29, 'h': 30, 'r': 7, 'a': 6, '!': 1, 'i': 1, 
-    'z': 2
+  'hk': {'i': 8, 'o': 21, 'e': 41, 'r': 1, 'a': 4, 'h': 1, '!': 1},
+  'Gw': {'i': 6, 'a': 4, 'y': 3, 'o': 1, 'e': 1},
+  'Sz': {
+    'y': 14, 'a': 18, 'e': 14, 'c': 10, 'o': 8, 'i': 3, 'w': 6, 'u': 11, 'm': 2,
+    'n': 1, 'l': 1, 'p': 1, 'k': 1
   },
-  'yd': {
-    '!': 20, 'e': 58, 'o': 15, 'n': 5, 's': 2, 'a': 23, 'r': 4, 'b': 1, 'i': 8,
-    't': 5, 'l': 6, 'z': 2, 'g': 1, 'm': 2, 'u': 4, 'd': 1
+  'zy': {
+    'm': 10, 'k': 56, 'b': 10, '!': 26, 'n': 59, 'g': 4, 'c': 16, 'z': 4,
+    'd': 3, 'p': 3, 'w': 6, 'r': 2, 'l': 3, 's': 5, 'e': 1
   },
-  'Yd': {'a': 1},
-  'Ye': {
-    'a': 32, 'e': 3, 'h': 3, 'p': 4, 'u': 2, 'n': 12, 't': 6, 'l': 14, 'r': 22,
-    'o': 3, '!': 1, 'd': 3, 's': 4, 'c': 1, 'i': 3, 'b': 1, 'm': 2, 'w': 1,
-    'z': 1, 'k': 1, 'g': 1
+  'iw': {'e': 12, 'i': 8, 'a': 15, 'o': 4, '!': 3, 'r': 1, 'c': 2, 's': 2},
+  'yg': {
   },
-  'ye': {
-    's': 32, 'r': 334, 'n': 34, '!': 84, 't': 26, 'a': 28, 'u': 4, 'd': 9,
-    'k': 2, 'l': 12, 'h': 2, 'g': 1, 'm': 7, 'e': 2, 'z': 1, 'w': 1
+  'hh': {'o': 15, 'e': 9, 'a': 14, 'i': 2, 'u': 4},
+  'wp': {'o': 1, 'e': 1, 'r': 1},
+  'Kw': {'a': 10, 'o': 3, 'i': 6, 'e': 1},
+  'Eh': {'l': 11, 'r': 19, 'm': 5, 's': 1, 'n': 2, 'e': 1, 'o': 1, 'i': 3},
+  'Ts': {'o': 3, 'a': 8, 'e': 4, 'c': 9, 'u': 16, 'i': 5, 'h': 1},
+  'zf': {'u': 1, 'e': 4, 'a': 1},
+  'fu': {
+    's': 31, 'e': 10, 't': 8, 'm': 1, 'r': 11, 'c': 1, 'l': 5, 'n': 4, 'h': 2,
+    'k': 1, 'a': 1, 'z': 1
   },
-  'yf': {'i': 9, 'o': 11, 'e': 7, 'f': 1, 'r': 2, 'u': 2, 'a': 2},
-  'Yg': {'l': 1},
-  'yg': {
-    'o': 6, 'a': 16, 'e': 8, 'm': 1, 'r': 3, 'i': 6, 'g': 2, 'l': 2, 'h': 1, 
-    'n': 1
+  'Ei': {
+    's': 45, 'd': 9, 'c': 33, 'l': 11, 'n': 6, 'f': 2, 't': 4, 'm': 2, 'g': 4,
+    'k': 6, 'b': 3, 'r': 2, 'e': 1
   },
-  'yh': {'e': 10, 'i': 3, 'r': 3, 'a': 14, 'u': 6, 'o': 7, 'n': 2, '!': 2},
-  'Yi': {'!': 1, 'n': 4, 'm': 1, 'p': 1, 'e': 1, 'u': 1, 'l': 1, 'd': 1},
-  'yi': {'n': 6, '!': 10, 'r': 1, 'c': 2, 'k': 1, 'e': 3},
-  'yj': {'o': 1, 'e': 1},
-  'yk': {
-    'e': 37, 'i': 8, 's': 4, '!': 79, 'o': 16, 'a': 11, 'l': 2, 'h': 3, 'k': 2,
-    'r': 1, 't': 1
+  'Az': {'e': 5, 'u': 4, 'a': 5, 'i': 3, 'c': 1, 'b': 2, 'z': 7, 'h': 1, 'o': 4
   },
-  'Yl': {'o': 1},
-  'yl': {
-    'o': 38, 'e': 97, 'v': 12, 'i': 15, 'a': 43, 't': 2, 'l': 12, 's': 7,
-    '!': 16, 'w': 2, 'd': 2, 'y': 3, 'u': 2, 'k': 2, 'n': 2, 'm': 1
+  'zn': {'i': 13, 'y': 11, 'e': 22, 'o': 3, 'a': 7, '!': 1},
+  'Ox': {'f': 1, 'l': 1, 'e': 2, 'n': 2, 'b': 2, 'm': 1, 't': 1},
+  'Dv': {'o': 2},
+  'bd': {'u': 10, 'i': 4, 'y': 1, 'o': 7, 'e': 14, 'a': 5},
+  'Oz': {
+    'u': 1, 'm': 2, 'a': 6, 'i': 2, 'b': 2, 'l': 1, 'o': 3, 'g': 1, 'e': 2,
+    'z': 1, '!': 1
   },
-  'ym': {
-    'o': 39, 'a': 69, 'p': 4, 'e': 35, 'i': 10, 'u': 7, 'c': 2, 'k': 3, '!': 6,
-    's': 4, 'm': 2, 'y': 1
+  'Lh': {'e': 1, 'u': 1, 'o': 1},
+  'Ig': {'l': 5, 'n': 5, 'o': 3, 'b': 2, 'a': 1, 'e': 1, 'w': 1, 't': 1, 'u': 2
   },
-  'Yn': {'i': 1, 'o': 1, 'g': 1},
-  'yn': {
-    'o': 32, 'e': 125, 'c': 3, 'n': 16, 'a': 36, 'u': 5, 'h': 5, 't': 12,
-    '!': 68, 'i': 15, 'd': 20, 'k': 5, 's': 55, 'g': 9, 'v': 1
+  'lx': {'!': 3},
+  'pf': {'!': 47, 'o': 1, 'i': 3, 'e': 33, 'f': 2, 'a': 3, 'l': 9, 'n': 1},
+  'fc': {'o': 4, 'h': 2, 'a': 1, 'i': 1},
+  'Iz': {'z': 3, 'a': 7, 'q': 1, 'u': 1, 's': 1},
+  'zw': {'a': 12, 'i': 9, 'e': 9, 'o': 2, 's': 1},
+  'yp': {'o': 6, 'h': 8, 'e': 9, 'a': 4, 'p': 1, 'r': 3, 'n': 1, 'u': 2, 'i': 1
   },
-  'yo': {
-    'n': 42, '!': 35, 'r': 16, 'u': 13, 't': 12, 's': 13, 'c': 5, 'l': 7,
-    'a': 3, 'e': 1, 'm': 2, 'v': 2, 'k': 2, 'z': 1, 'o': 2, 'd': 2, 'w': 2
+  'jc': {'i': 9, 'z': 8, 'h': 2, 'a': 1, '!': 1, 'e': 3},
+  'Ex': {
+    'u': 1, 'l': 3, 'n': 1, 'c': 1, 'f': 1, 'e': 2, 'o': 1, 'i': 1, 't': 2,
+    'a': 1, 'p': 1
   },
-  'Yo': {
-    'u': 53, 'r': 15, 'd': 3, 's': 18, 'o': 2, 'c': 10, 'h': 5, 'n': 22, 'a': 2,
-    'w': 2, 'k': 8, 't': 3, 'p': 1, 'e': 3, 'x': 1, 'b': 1, 'z': 2, 'v': 3,
-    'm': 1, 'q': 1, '!': 1
+  'xu': {'m': 3},
+  'uu': {'!': 3, 'd': 1, 'r': 2, 'a': 1, 'l': 2, 's': 4, 'k': 1, 'n': 1},
+  'ky': {'!': 375, 'l': 1, 'e': 5, 'a': 6, 'n': 3, 'b': 1, 'm': 1, 't': 1},
+  'gk': {'i': 5, 'h': 5, 'a': 1, '!': 3, 'n': 1},
+  'xn': {'a': 2, 'e': 6, 'd': 1},
+  'wz': {'e': 3, 'a': 1},
+  'Oy': {'l': 1, 'o': 1, 'e': 4, 'a': 3, 's': 2, 'u': 1},
+  'Im': {
+    'h': 3, 'e': 3, '!': 1, 'l': 2, 'a': 7, 'm': 8, 'b': 14, 'p': 5, 'o': 2,
+    'r': 1, 'd': 1, 'i': 1, 'u': 1, 'f': 1, 'g': 1
   },
-  'Yp': {'i': 1},
-  'yp': {
-    'o': 6, 'h': 8, 'e': 9, 'a': 4, 'p': 1, 'r': 3, 'n': 1, 'u': 2, 'i': 1
+  'mh': {'o': 12, 'e': 3, 'a': 8, 'i': 1},
+  'sz': {
+    'e': 41, '!': 57, 'y': 21, 'a': 20, 'k': 14, 'l': 4, 'u': 5, 'o': 2, 'c': 7,
+    't': 2, 'i': 2, 'b': 1, 'm': 1, 'w': 1
   },
-  'yq': {'u': 2},
-  'Yr': {'a': 2, 'i': 1},
-  'yr': {
-    'd': 3, 'e': 44, 'n': 8, 'i': 11, '!': 6, 'o': 21, 'u': 5, 'r': 2, 'a': 23,
-    'g': 1, 'k': 2, 'l': 3, 's': 4, 't': 1, 'm': 1, 'c': 1
+  'xb': {'y': 3, 'a': 1, 'u': 5, 'e': 3, 'o': 2},
+  'mq': {'u': 9},
+  'Tw': {'o': 8, 'i': 23, 'e': 15, 'y': 3, 'a': 3},
+  'kd': {'a': 4, 'o': 2, 'u': 1, 'i': 1, 'e': 2, 'y': 1},
+  'cz': {
+    'y': 80, 'a': 41, 'm': 4, 'o': 7, '!': 142, 'n': 6, 'e': 40, 'k': 21,
+    'u': 5, 'b': 1, 'i': 1, 'w': 1
   },
-  'ys': {
-    '!': 53, 'o': 35, 't': 24, 'e': 42, 'a': 11, 'i': 16, 's': 7, 'd': 4,
-    'l': 10, 'h': 10, 'm': 4, 'k': 9, 'c': 4, 'z': 12, 'r': 1, 'u': 2, 'y': 1,
-    'n': 1, 'w': 1, 'q': 1, 'b': 1
+  'Id': {'e': 6, 'd': 1, 'a': 1, 'o': 1, 'l': 2, 'r': 3, 'i': 1},
+  'bh': {'a': 14, 'r': 1, 'o': 5, 'u': 1, 'e': 1, '!': 1},
+  'lq': {'u': 22},
+  'ih': {
+    'a': 60, '!': 4, 'i': 6, 'y': 1, 'e': 22, 'o': 10, 'm': 3, 'l': 13, 'u': 7,
+    'n': 3, 't': 1, 'k': 1, 'r': 1
   },
-  'Ys': {'l': 2, 'q': 1, 'b': 1, 'a': 1},
-  'yt': {
-    'o': 28, '!': 10, 'l': 5, 'h': 17, 'e': 29, 'a': 8, 't': 3, 's': 3, 'c': 4,
-    'u': 2, 'z': 1, 'i': 1, 'k': 1, 'r': 1, 'y': 1
+  'Uh': {'l': 9, 'r': 6, 'm': 1, 'y': 1, 'e': 1, 'a': 1, 'd': 1},
+  'yi': {'n': 6, '!': 10, 'r': 1, 'c': 2, 'k': 1, 'e': 3},
+  'Of': {'f': 16, 'a': 2, 't': 1, 'l': 3, 's': 1, 'e': 1},
+  'zh': {'u': 2, 'e': 4, 'a': 6, 'o': 2, 'k': 1, 'y': 1},
+  'kk': {'e': 34, 'i': 11, 'a': 11, 'o': 7, 'h': 1, 'u': 1},
+  'xi': {
+    'e': 8, 's': 1, 'm': 3, 'o': 5, 'l': 4, 'd': 2, 'c': 4, '!': 2, 't': 1,
+    'n': 3, 'u': 1
   },
-  'Yt': {'u': 1},
-  'Yu': {
-    '!': 1, 'e': 5, 'n': 10, 'a': 2, 't': 1, 'h': 2, 'l': 1, 'r': 12, 's': 8,
-    'm': 2, 'p': 1, 'i': 1, 'k': 2, 'd': 1, 'z': 1, 'c': 1
+  'Sv': {'o': 3, 'e': 15, 'a': 5, 'r': 1, 'i': 1},
+  'mt': {'i': 2, 'e': 4, 'h': 3, 'z': 1, 'o': 2},
+  'py': {'!': 30, 'r': 3, 'd': 1, 'u': 1, 'i': 1, 'c': 1},
+  'Ey': {'r': 2, 'l': 3, 'e': 5, 'm': 1, 'n': 1, 't': 3, 's': 1, 'c': 1, 'u': 1
   },
+  'gq': {'u': 6},
   'yu': {
     's': 4, 'n': 10, 'm': 4, 'a': 2, 'k': 2, '!': 2, 'd': 1, 'o': 1, 'g': 1,
     'e': 2, 'p': 2, 'l': 1, 'r': 1, 'b': 1
   },
-  'yv': {'a': 4, 'i': 2, 'e': 7},
-  'Yv': {'o': 1},
-  'yw': {'o': 12, 'a': 12, 'e': 6, 'i': 8, 'h': 1},
-  'yx': {'!': 2},
-  'yy': {'e': 1, 'a': 3},
-  'Yz': {'a': 2, 'q': 1},
-  'yz': {'e': 13, '!': 3, 'a': 4, 'l': 1, 'i': 2, 'g': 1, 'd': 1},
-  'za': {
-    'l': 50, '!': 230, 'r': 150, 'n': 89, 'd': 20, 'k': 72, 's': 11, 'b': 14,
-    'g': 14, 'w': 5, 'j': 4, 'm': 8, 'p': 9, 't': 14, 'i': 7, 'o': 1, 'c': 9,
-    'f': 9, 'h': 6, 'q': 2, 'y': 4, 'v': 2, 'u': 1, 'z': 2, 'e': 1
+  'Gh': {'o': 8, 'e': 14, 'i': 8, 'a': 13, 'r': 2},
+  'Ek': {
+    'l': 2, 's': 4, '!': 1, 'b': 1, 'k': 1, 'd': 1, 'h': 2, 'm': 2, 'i': 3,
+    'w': 1, 'e': 2, 'a': 1
   },
-  'Za': {
-    'm': 30, 'v': 13, 'p': 20, 'r': 44, 'c': 26, 'y': 4, 'h': 20, 'n': 41,
-    'k': 10, 'j': 4, 'b': 21, 'l': 17, 'g': 12, 'w': 5, 's': 4, 'z': 4, 'u': 6,
-    'i': 10, 'd': 12, 'f': 5, 't': 3, 'e': 1, 'x': 1
+  'wg': {'i': 2, 'e': 3, 'o': 1, 'l': 1, 'a': 1, 'r': 1},
+  'pn': {'e': 21, 'i': 7, 'o': 2, 'a': 1, 'u': 1},
+  'rj': {'a': 12, 'o': 8, 'u': 3, 'e': 10, 'i': 5},
+  'fg': {'a': 1, 'r': 4, 'o': 1, 'u': 1, 'e': 1},
+  'Fy': {'e': 1, 'f': 2, 'o': 1, 'k': 3, 'a': 1, 'l': 3, 'd': 1},
+  'vn': {'e': 12, 'a': 3, 'i': 2, 'o': 1, 'y': 1},
+  'It': {
   },
-  'zb': {'e': 17, 'i': 3, 'y': 2, 'u': 2, 'a': 10, 'r': 2, 'o': 1},
-  'Zb': {'o': 1, 'r': 1, 'e': 1, 'i': 3},
-  'zc': {'o': 7, 'l': 1, 'u': 1, 'a': 7, 'z': 17, 'h': 1},
-  'zd': {'!': 1, 'a': 5, 'z': 2, 'e': 6, 'o': 5, 'y': 2, 'i': 2},
-  'Zd': {'e': 1, 'a': 1, 'o': 1, 'r': 1},
-  'ze': {
-    'm': 14, 'l': 203, '!': 93, 'r': 227, 'n': 118, 'v': 3, 'e': 18, 'w': 62,
-    'a': 10, 'y': 21, 't': 13, 'c': 10, 'o': 4, 'k': 56, 'z': 4, 'j': 5, 'i': 2,
-    'p': 10, 'b': 8, 's': 22, 'g': 2, 'd': 1
+  'Ic': {'k': 2, 'e': 3, 'h': 3, 'a': 2},
+  'iy': {'a': 37, 'o': 6, 'u': 1, 'e': 3},
+  'Bj': {'o': 12, 'e': 6},
+  'eq': {'u': 28},
+  'Il': {'e': 2, 'i': 3, 'l': 17, 'd': 1, 'a': 7, 's': 1, 't': 1, 'g': 1},
+  'xx': {'!': 2},
+  'fk': {'o': 6, 'i': 4, 'a': 11, 'e': 7, 'n': 1},
+  'Ee': {'l': 2, 'k': 1, 'd': 1, 'r': 1, '!': 1},
+  'Vr': {'o': 3, 'e': 7, 'a': 10, 'i': 3, 'b': 3},
+  'Sr': {'o': 5, 'i': 3, 's': 2, 'n': 1, 'e': 2, 'a': 2, 'y': 1},
+  'wv': {'e': 4, 'i': 1},
+  'bg': {'o': 1, 'e': 2},
+  'md': {'e': 8, 'a': 8, 'i': 4, 'n': 2},
+  'Xu': {'!': 1, 'e': 1},
+  'Mr': {'a': 5, 'o': 9, 'u': 2, 'n': 1, 'v': 1, 'k': 1},
+  'Io': {
+    'r': 1, 'n': 2, 'v': 1, 'e': 1, 't': 1, 'l': 1, 'd': 1, 'a': 1, 'z': 2,
+    'p': 1, 's': 1
   },
-  'Ze': {
-    'p': 6, 'i': 23, 'l': 41, 'r': 23, 'n': 25, 'h': 11, 'm': 13, 'b': 5,
-    'o': 2, 'c': 10, 't': 9, 'e': 5, 'f': 1, 'v': 2, 's': 2, 'd': 3, 'a': 6,
-    'g': 5, 'u': 1, 'y': 2, 'k': 1, 'z': 1
+  'Ik': {'e': 9, 'n': 1, 'a': 1, 'u': 1, 'z': 1, 'k': 1},
+  'pd': {'i': 2, 'e': 5, 'y': 2, 'a': 1},
+  'Um': {
+    'a': 3, 'b': 9, 's': 2, 'p': 4, 'l': 2, '!': 1, 'f': 1, 'i': 1, 'h': 1,
+    'e': 2, 'n': 1
   },
-  'zf': {'u': 1, 'e': 4, 'a': 1},
-  'zg': {'e': 7, 'i': 2, 'a': 9, 'u': 2, 'r': 1, 'h': 1, 'o': 4},
-  'Zg': {'o': 1},
-  'Zh': {'a': 3, 'o': 2, 'u': 2, 'e': 2},
-  'zh': {'u': 2, 'e': 4, 'a': 6, 'o': 2, 'k': 1, 'y': 1},
-  'zi': {
-    'e': 77, 'l': 20, 'a': 51, 'o': 75, '!': 139, 'n': 115, 'z': 3, 'g': 20,
-    'c': 27, 'k': 21, 'm': 9, 's': 10, 't': 4, 'u': 5, 'q': 1, 'v': 1, 'r': 3,
-    'i': 1, 'w': 1, 'd': 2
+  'pw': {'o': 4, 'e': 3, 'a': 2},
+  'Ax': {'t': 5, 'f': 1, 'e': 6, 'l': 2, 's': 2, '!': 1, 'o': 1, 'm': 1},
+  'Ip': {'p': 1, 'o': 1, 's': 2, '!': 1},
+  'ii': {
+    '!': 13, 'n': 2, 's': 3, 'o': 1, 'g': 1, 'k': 1, 'h': 3, 'm': 1, 'u': 1,
+    'b': 1, 'p': 3, 'r': 1, 'v': 1, 'l': 1
   },
-  'Zi': {
-    'm': 19, 'e': 56, 'n': 29, 't': 8, 'r': 9, 'g': 5, 'c': 11, 'o': 4, 'p': 8,
-    'l': 12, 'f': 1, 'k': 2, 'z': 2, 'v': 1, 's': 4, 'd': 3, 'a': 5, 'b': 3,
-    'y': 1, 'h': 1
+  'Aw': {'a': 4, 'o': 1, 'e': 2, 'k': 2, 'b': 1, 't': 2, 'y': 1, '!': 1},
+  'Uc': {'h': 5, 'c': 4, '!': 1},
+  'cj': {'u': 2},
+  'ju': {
   },
-  'zk': {'e': 30, 'o': 25, 'a': 15, 'u': 1, 'i': 13, '!': 1, 'y': 4, 'l': 1},
-  'Zl': {'a': 2, 'o': 2},
-  'zl': {'e': 71, 'o': 16, 'a': 14, 'i': 6, '!': 5, 'y': 1},
-  'zm': {'a': 78, 'e': 6, 'i': 13, 'o': 2, 'u': 2, 'd': 1},
-  'Zm': {'u': 1, 'o': 1, 'i': 3, 'e': 1},
-  'Zn': {'i': 1},
-  'zn': {'i': 13, 'y': 11, 'e': 22, 'o': 3, 'a': 7, '!': 1},
-  'Zo': {
-    'o': 1, 'r': 15, 'l': 22, 'e': 5, 'b': 2, 'n': 5, 'g': 4, 'd': 3, 'c': 2,
-    'h': 1, 'z': 1, 'u': 6, 't': 3, 's': 2, 'm': 7, 'q': 1
+  'yz': {'e': 13, '!': 3, 'a': 4, 'l': 1, 'i': 2, 'g': 1, 'd': 1},
+  'Oe': {'s': 8, 'h': 10, 'r': 3, 'l': 6, 't': 3, 'c': 1, 'd': 2, 'n': 1, 'f': 1
   },
-  'zo': {
-    's': 17, '!': 177, 'g': 4, 'n': 50, 't': 8, 'l': 29, 'y': 1, 'r': 21,
-    'z': 2, 'w': 15, 'c': 5, 'p': 2, 'k': 2, 'v': 3, 'm': 2, 'b': 2, 'u': 2, 
-    'i': 1
+  'Cz': {'e': 12, 'a': 22, 'y': 4, 'u': 4, 'l': 1, 'o': 2, 'w': 1},
+  'Xa': {'v': 1, 'n': 2, 'y': 2, 'i': 1},
+  'Ef': {'i': 1, 'f': 6, 'a': 1, 'u': 1, 'r': 2, 't': 2, 'l': 1},
+  'mc': {'o': 4, 'z': 7, 'h': 14, 'k': 1, 'a': 2, '!': 1, 'i': 2},
+  'tv': {'i': 8, 'a': 3, 'e': 6, 'r': 1, '!': 1, 'o': 2},
+  'jt': {'o': 2, 'c': 1, 'k': 2, 'a': 8, '!': 1, 'e': 1},
+  'Dz': {'i': 13, 'u': 4, 'l': 1, 'w': 1, 'a': 1},
+  'dz': {
+    'i': 45, 'e': 7, '!': 9, 'w': 3, 'y': 3, 'u': 2, 'a': 3, 'o': 1, 'm': 1,
+    'l': 1, 'h': 1, 'k': 2
+  },
+  'jk': {'o': 10, 'a': 9, 'u': 1, '!': 1},
+  'Zw': {'i': 11, 'e': 4, 'a': 5, 'o': 4},
+  'Jh': {'o': 2, 'i': 1, 'a': 1},
+  'zd': {'!': 1, 'a': 5, 'z': 2, 'e': 6, 'o': 5, 'y': 2, 'i': 2},
+  'bk': {'e': 11, 'o': 4, 'i': 4, 'a': 6},
+  'Ue': {'c': 2, 'h': 1, 'm': 1, 'd': 1, 'n': 1, 'l': 1, 'r': 1, 'k': 1, 'b': 1
   },
-  'zp': {'a': 4, 'e': 1},
-  'zq': {'u': 10},
-  'Zr': {'a': 1, 'i': 1},
   'zr': {'a': 3, 'o': 2, 'i': 3},
-  'Zs': {'a': 1, 'o': 1, 'c': 1},
-  'zs': {'i': 3, 'c': 11, '!': 4, 't': 2, 'a': 3},
+  'hj': {'e': 6, 'i': 1, '!': 2},
+  'Op': {
+    'p': 11, 'i': 6, 'l': 2, 'e': 6, 'f': 1, 'd': 2, 'h': 3, 'a': 7, 's': 2,
+    'u': 2, 'o': 2, 'r': 1, 'y': 1, 't': 1
+  },
+  'Ug': {'a': 4, 'l': 3, 'o': 1},
   'zt': {'s': 1, 'a': 1, 'o': 1, '!': 1},
-  'zu': {
-    'e': 9, 'r': 20, 'n': 8, 'k': 7, '!': 5, 't': 11, 'm': 14, 'l': 14, 'c': 7,
-    'b': 11, 'a': 4, 'o': 2, 's': 5, 'f': 1, 'w': 1, 'g': 1, 'p': 1
+  'vs': {
   },
-  'Zu': {
-    'n': 7, 'b': 11, 'm': 14, 'c': 16, 'k': 8, 'r': 16, 'l': 8, 'e': 7, 'p': 5,
-    'f': 2, 'i': 1, 'v': 2, 't': 2, 'h': 1, 'a': 2, 'w': 1, 'g': 1, 'z': 1, 
-    's': 1
+  'uw': {
+    'e': 14, '!': 11, 'i': 2, 'a': 10, 's': 1, 'm': 1, 'k': 2, 'w': 1, 'h': 1
+  },
+  'Bh': {'a': 16, 'o': 1, 'u': 1},
+  'Eo': {'f': 1, 'n': 1, 'v': 1},
+  'zb': {'e': 17, 'i': 3, 'y': 2, 'u': 2, 'a': 10, 'r': 2, 'o': 1},
+  'Uy': {'!': 1, 'e': 6},
+  'yj': {'o': 1, 'e': 1},
+  'Hr': {
   },
-  'zv': {'i': 2, 'e': 1},
-  'Zv': {'o': 1},
-  'zw': {'a': 12, 'i': 9, 'e': 9, 'o': 2, 's': 1},
-  'Zw': {'i': 11, 'e': 4, 'a': 5, 'o': 4},
   'Zy': {'l': 3, 'g': 1, 'c': 1, 'n': 1, 's': 3, 'w': 1, 'm': 1, 'b': 1},
-  'zy': {
-    'm': 10, 'k': 56, 'b': 10, '!': 26, 'n': 59, 'g': 4, 'c': 16, 'z': 4,
-    'd': 3, 'p': 3, 'w': 6, 'r': 2, 'l': 3, 's': 5, 'e': 1
+  'yq': {'u': 2},
+  'xm': {'a': 8, 'o': 1},
+  'xr': {'o': 3},
+  'Ia': {
+    'c': 12, 'n': 12, 'd': 1, 'r': 4, 'l': 1, 'f': 1, 'm': 2, 'v': 1, 't': 1
   },
-  'zz': {
-    'i': 124, 'o': 86, 'e': 43, 'a': 89, 'l': 7, 'u': 16, '!': 2, 'y': 2, 'n': 1
+  'zk': {'e': 30, 'o': 25, 'a': 15, 'u': 1, 'i': 13, '!': 1, 'y': 4, 'l': 1},
+  'wq': {'u': 1},
+  'dv': {'e': 5, 'o': 4, 'i': 13, 'a': 6},
+  'pg': {'a': 1, 'o': 2},
+  'Ao': {'k': 1, 'a': 1, 'n': 1, '!': 1},
+  'Sj': {'o': 8, 'a': 1, 'u': 1, 'e': 1},
+  'hv': {'i': 5, 'e': 4, 'a': 1},
+  'mz': {'e': 4, 'o': 1, 'a': 6, '!': 2, 'i': 3},
+  'dj': {'o': 2, 'e': 2, 'i': 5, 'a': 1, 'u': 1, 'm': 1},
+  'bm': {'a': 11, 'e': 2, 'y': 1},
+  'Iw': {'a': 13},
+  'Ih': {'l': 2, 'r': 2, 'd': 1, 'a': 1, 'n': 2, 'm': 1, 'e': 2},
+  'jn': {'a': 6, 'i': 4, 'o': 4, 'y': 2, 'e': 1},
+  'Oo': {'t': 2, 'm': 1, 'l': 1, 's': 1},
+  'xh': {'a': 3, 'o': 3, 'e': 1},
+  'If': {'i': 2, 'f': 3, 'v': 1, 'e': 1, 'a': 1},
+  'Yz': {'a': 2, 'q': 1},
+  'yx': {'!': 2},
+  'Zd': {'e': 1, 'a': 1, 'o': 1, 'r': 1},
+  'Ub': {'e': 3, 'a': 2, 'o': 1, 'l': 1, 'r': 1, 'i': 1},
+  'Pt': {'a': 4, 'o': 1},
+  'Oi': {'l': 2, 's': 1, 'e': 2, 'n': 2},
+  'jd': {'u': 2, 'a': 8, 'e': 2},
+  'Ud': {'e': 2, 'y': 1, 'o': 2, 'd': 1, 'l': 1, 'a': 1, 'i': 2},
+  'Km': {'e': 3, 'i': 3, 'a': 2},
+  'td': {'o': 5, 'e': 4, '!': 1},
+  'Tj': {'a': 3, 'e': 2},
+  'Kj': {'o': 2, 'e': 7, 'a': 1},
+  'dp': {'a': 6, 'h': 1, 'r': 1},
+  'Af': {'a': 4, 'r': 1, 'f': 8, 't': 1, 'o': 2, 'z': 1, 's': 2, 'l': 1, 'u': 1
   },
+  'Uz': {'z': 3, 'e': 2, 'd': 1, 'i': 1, 'u': 1},
+  'js': {'k': 1, 'e': 1, 'i': 1, 'a': 1, 'n': 1},
+  'qi': {'!': 1},
+  'vu': {'z': 3, 'c': 1, 'h': 1, 'r': 1, 'e': 1, 'l': 1},
+  'Rm': {'!': 1},
+  'wu': {'s': 1, 'l': 3, '!': 1, 'c': 1, 'r': 1, 'o': 2, 'n': 1, 'h': 1},
+  'tq': {'u': 2},
+  'Ae': {'s': 3, 'g': 1, 'r': 3, 'l': 1, 'm': 1, 'i': 1},
+  'Sg': {'r': 3, 'a': 2, 'u': 1},
+  'Ml': {'e': 3, 'i': 1, 'y': 1, 'o': 1},
+  'kg': {'r': 1, 'o': 1},
+  'vv': {'o': 1},
+  'Jn': {'!': 1},
+  'Dh': {'i': 1, 'o': 2, 'e': 2, 'a': 4, 'r': 1},
+  'Wn': {'u': 2, 'e': 1, 'o': 1},
+  'Vl': {'c': 2, 'a': 6, 'l': 1, 'i': 2, 'j': 1, 'e': 1, 'k': 1},
+  'Uv': {'a': 3},
+  'Hj': {'o': 1, 'e': 3, 'a': 1},
+  'kc': {'o': 3, 'e': 1},
+  'bp': {'l': 1},
+  'fq': {'u': 1},
+  'lj': {'e': 8, 'u': 2, 'a': 6, '!': 1, 'o': 2},
+  'Yn': {'i': 1, 'o': 1, 'g': 1},
+  'Vy': {'a': 1, '!': 1, 'h': 1},
+  'Uo': {'n': 1, 'y': 1},
+  'Tk': {'a': 3},
+  'Ie': {'z': 1, 's': 1, 'n': 3},
+  'fp': {'a': 2},
+  'Ds': {'o': 1, 'p': 1, 'a': 1},
+  'Wm': {'s': 1, 'i': 1},
+  'Sf': {'o': 1, 'e': 3, 'a': 1},
+  'bj': {'i': 1, 'e': 1, 'o': 1},
+  'Iu': {'l': 4, 'r': 1, 'c': 1},
+  'Ij': {'a': 2},
+  'Ii': {'a': 1, 'd': 1, 'n': 1},
+  'fh': {'i': 3, 'a': 2, 'o': 2, 'e': 1},
+  'Ys': {'l': 2, 'q': 1, 'b': 1, 'a': 1},
+  'Yg': {'l': 1},
+  'xc': {'y': 1, 'e': 1, 'o': 1},
+  'Dk': {'!': 1},
+  'hg': {'a': 3, 'e': 6, 'i': 1, 'o': 1, 'h': 1},
+  'vk': {'i': 1, 'a': 6, 'e': 1, 'o': 1, '!': 1},
+  'gc': {'h': 2, 'o': 9, 'k': 1, 'a': 2, 'l': 1},
+  'mv': {'o': 1, 'i': 1, 'a': 1},
+  'Iy': {'e': 2, 'o': 1},
+  'Yt': {'u': 1},
+  'Wl': {'o': 5, 'a': 2},
+  'bw': {'o': 1, 'e': 1},
+  'Nj': {'o': 1, 'i': 1, 'a': 1},
+  'jm': {'a': 3, 'u': 1, 'e': 1, 'o': 1},
+  'vd': {'e': 4, 'a': 2, '!': 2},
+  'Hn': {'a': 2, 'y': 1, 'o': 1},
+  'Gs': {'c': 2, 'e': 1, 't': 1},
+  'Gj': {'e': 6, 'o': 2},
+  'vh': {'a': 1},
+  'Eq': {'u': 4},
+  'Dl': {'o': 2, 'u': 2, 'a': 1},
+  'Zb': {'o': 1, 'r': 1, 'e': 1, 'i': 3},
+  'Kv': {'a': 3, 'i': 1, 'z': 1, 'o': 1, 'e': 3},
+  'Gv': {'e': 1},
+  'Cs': {'a': 1, 'u': 2, 'i': 1, 'e': 2},
+  'jl': {'a': 1, 'y': 1, 'o': 1, '!': 1, 'i': 1},
+  'Aj': {'a': 4, 'e': 1, 'o': 2},
+  'hp': {'e': 1, 'a': 3, 'u': 1, 'o': 2},
+  'Uf': {'f': 2},
+  'jz': {'!': 1, 'a': 1, 'i': 1},
+  'fz': {'i': 4, 'a': 1, '!': 1, 'g': 1},
+  'Gy': {'l': 3, 'g': 1, 's': 1, 'a': 2, 'u': 1},
+  'kj': {'y': 1, 'e': 1, 'i': 2},
+  'jy': {'!': 1},
+  'kx': {'!': 2, 't': 1, 'l': 1},
+  'fd': {'e': 2},
+  'vj': {'o': 1, 'e': 2},
+  'Zm': {'u': 1, 'o': 1, 'i': 3, 'e': 1},
+  'xk': {'i': 1},
+  'zv': {'i': 2, 'e': 1},
+  'Qi': {'a': 1, 'u': 1, 'n': 1},
+  'xy': {'!': 2},
+  'Mw': {'a': 2},
+  'Gf': {'e': 1, 'r': 1},
+  'Fj': {'e': 3},
+  'Cw': {'i': 5, 'a': 1},
+  'kq': {'u': 1},
+  'Ui': {'t': 1, 'm': 1, 'h': 1},
+  'vc': {'i': 1, 'e': 2, 'c': 1},
+  'Sb': {'e': 1, 'a': 2, 'o': 1},
+  'Rz': {'e': 4, 'a': 1, 'u': 1},
+  'Qa': {'z': 1, 'd': 2, 's': 1, 'r': 1},
+  'Nh': {'e': 2, 'a': 2},
+  'gv': {'y': 1, 'a': 2, 'o': 3, 'i': 6},
+  'Mt': {'!': 1, 'h': 1},
+  'kv': {'e': 3, 'l': 1, 'i': 2},
+  'bf': {'r': 1, 'l': 1},
+  'ww': {'i': 1, 'a': 4},
+  'bz': {'a': 1, 'i': 2, 'd': 1},
+  'Iq': {'b': 1},
+  'qb': {'a': 1},
+  'Hl': {'a': 8, 'u': 1, 'e': 1, 'y': 1},
+  'Gn': {'e': 3, 'i': 1, 'a': 5, 'o': 1},
+  'Gd': {'o': 1, 'u': 1},
+  'jw': {'a': 2},
+  'Wd': {'o': 1},
+  'fw': {'e': 1, 'a': 1},
+  'Uk': {'o': 1, 'n': 1, 'e': 2, '!': 1, 'i': 1},
+  'Tz': {'e': 2},
+  'Nw': {'a': 6},
+  'vw': {'i': 2},
+  'fv': {'i': 1, 'e': 1},
+  'qv': {'i': 1},
+  'Cd': {'e': 1},
+  'Zv': {'o': 1},
+  'Zn': {'i': 1},
+  'Zl': {'a': 2, 'o': 2},
+  'vm': {'a': 1},
+  'Tl': {'u': 2, 'l': 1, 'a': 3},
+  'Nq': {'u': 1},
+  'vz': {'o': 1, 'e': 1, 'i': 1},
+  'Ks': {'i': 1, 'h': 1, 'z': 1},
+  'fb': {'a': 1, 'o': 2},
+  'jj': {'a': 2},
+  'Zg': {'o': 1},
+  'Yv': {'o': 1},
+  'mj': {'a': 3, 'i': 1, 'u': 1, 'h': 1},
+  'Tc': {'h': 1},
+  'jb': {'k': 1},
+  'Rv': {'i': 1},
+  'Mh': {'o': 1},
+  'kz': {'a': 1, 'e': 1, 'd': 1},
+  'vg': {'r': 1, 'l': 1},
+  'Hv': {'i': 1},
+  'Cv': {'e': 1},
+  'qd': {'a': 1},
+  'Zs': {'a': 1, 'o': 1, 'c': 1},
+  'Zr': {'a': 1, 'i': 1},
+  'Yr': {'a': 2, 'i': 1},
+  'Xy': {'o': 1},
+  'gx': {'a': 4},
+  'Vb': {'i': 1},
+  'Uu': {'t': 1},
+  'Uj': {'a': 1},
+  'yy': {'e': 1, 'a': 3},
+  'Ps': {'o': 1, 'e': 1, 'u': 2, 'i': 1},
+  'gz': {'e': 1},
+  'Mg': {'u': 1},
+  'Mb': {'o': 1, 'a': 1},
+  'Lj': {'u': 1},
+  'gj': {'e': 1},
+  'vt': {'i': 1, 'y': 1},
+  'Gm': {'e': 1},
+  'xz': {'a': 1},
+  'hz': {'i': 1, 'e': 1, '!': 1},
+  'Yp': {'i': 1},
+  'Yl': {'o': 1},
+  'Yd': {'a': 1},
+  'Wz': {'o': 1},
+  'jg': {'r': 1, 'e': 1},
+  'Ux': {'a': 1},
+  'Tv': {'e': 1},
+  'pv': {'l': 1, 'a': 1},
+  'Sd': {'o': 1},
+  'jh': {'o': 2},
+  'Pn': {'i': 1},
+  'Pj': {'e': 1},
+  'Nk': {'u': 1, 'o': 1},
+  'Nc': {'n': 1},
+  'xd': {'o': 1},
+  'Lw': {'e': 1},
+  'vf': {'a': 1},
+  'pz': {'e': 1},
+  'Ht': {'w': 1},
+  'fj': {'o': 1},
+  'Gz': {'y': 1},
+  'Gb': {'u': 1},
+  'Fv': {'e': 1},
+  'xp': {'o': 1},
+  'Ej': {'i': 1},
+  'Dm': {'i': 1},
+  'Dj': {'u': 1},
+  'Cm': {'i': 1},
+  'Bz': {'h': 1},
+  'Bv': {'e': 1},
+  'qr': {'i': 1
+  }
 }
 
 def f():
   q3_keys = sorted(list(q3.keys()))
   q3_keys_where_first_char_in_AZ = q3_keys[:q3_keys.index('aa')]
   _z = choice(q3_keys_where_first_char_in_AZ)
   _2 = q3[_z[-2:]]
   while _2 != '!':
-    choices = q3[_z[-2:]]
-    _2 = choose(choices)
+    _2 = choose(q3[_z[-2:]])
     _z += _2
   return _z[:-1]
 
 t = lambda: is_a_family_name(f())
```

### Comparing `hak-0.0.88/hak/one/string/format.py` & `hak-0.0.9/hak/string/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .replace.triple_new_line_with_double_new_line import f as replace_triple_newlines_with_double_newlines
 from .insert.new_line_before_new_line_and_cea_ import f as insert_nl_before_nl_and_cea_
 from .indent.run_if_class_method import f as indent_if_is_run_method
 from .remove.whitespace_between_newlines import f as remove_whitespace_between_newlines
 from .colour.bright.yellow import f as yellow
 from .colour.bright.cyan import f as cy
 from .colour.bright.magenta import f as magenta
-from hak.many.strings.compare import f as compare_strings
+from hak.list.strings.compare import f as compare_strings
 
 def f(x: str):
   for fn in [
     append_new_line,
     replace_double_nl_with_single_new_line,
     remove_empty_line_spaces,
     insert_nl_before_def,
```

### Comparing `hak-0.0.88/hak/one/string/insert/new_line_after_last_import_line.py` & `hak-0.0.9/hak/string/insert/new_line_after_last_import_line.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/one/string/insert/new_line_before_def.py` & `hak-0.0.9/hak/string/insert/new_line_before_def.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/one/string/insert/new_line_before_lambda.py` & `hak-0.0.9/hak/string/insert/new_line_before_lambda.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from hak.one.string.contains.l import f as contains_lambda
+from hak.string.contains.l import f as contains_lambda
 
 def f(x):
   lines_containing_lambda = [_l for _l in x.split('\n') if contains_lambda(_l)]
   if lines_containing_lambda:
     for _l in lines_containing_lambda:
       x = x.replace(_l, '\n'+_l)
   return x
```

### Comparing `hak-0.0.88/hak/one/string/lambdarise.py` & `hak-0.0.9/hak/string/lambdarise.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from hak.one.string.single_line_function.to_lambda_str import f as to_l_str
+from hak.string.single_line_function.to_lambda_str import f as to_l_str
 
 def f(x):
   y = '\n'.join([to_l_str(_l) for _l in x.split('\n')])
   return len(x) > len(y), y
 
 def t():
   change_made, z = f('\n'.join([
```

### Comparing `hak-0.0.88/hak/one/string/password/create.py` & `hak-0.0.9/hak/string/password/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from string import ascii_lowercase as l
 from string import ascii_uppercase as u
 from string import digits as d
 from string import punctuation as p
 from random import choice
 from random import shuffle
-from hak.one.string.colour.tgfr import f as tgfr
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.colour.tgfr import f as tgfr
+from hak.string.print_and_return_false import f as pf
 
 def f(n=8):
   base = [choice(_) for _ in [d, l, p, u]]
   extra = [choice(l+u+d+p) for _ in range(n-len(base))]
   result = base + extra
   shuffle(result)
   return ''.join(result)
```

### Comparing `hak-0.0.88/hak/one/string/password/has_chars_from_3_sets.py` & `hak-0.0.9/hak/string/password/has_chars_from_3_sets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.many.bools.count_true import f as count_true
-from hak.one.string.has_digit import f as has_09
-from hak.one.string.has_lowercase import f as has_az
-from hak.one.string.has_uppercase import f as has_AZ
-from hak.one.string.has_other_char import f as has_other
+from hak.bools.count_true import f as count_true
+from hak.string.has_digit import f as has_09
+from hak.string.has_lowercase import f as has_az
+from hak.string.has_uppercase import f as has_AZ
+from hak.string.has_other_char import f as has_other
 
 f = lambda x: count_true([has_09(x), has_az(x), has_AZ(x), has_other(x)]) >= 3
 
 t = lambda: all([
   not any([
     f('12345678'),
     f('abcdefgh'),
```

### Comparing `hak-0.0.88/hak/one/string/print_and_return_false.py` & `hak-0.0.9/hak/string/print_and_return_false.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/one/string/refactor/by_two_char_combinations.py` & `hak-0.0.9/hak/string/refactor/by_two_char_combinations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from subprocess import run as sprun
-from hak.many.strings.two_char_combinations import f as prepare_combinations
+from hak.list.strings.two_char_combinations import f as prepare_combinations
 
 def f(original):
   data = original
   chars = ''.join(sorted(list(set(data))))
   _L = prepare_combinations(chars)
   for _l in _L:
     candidate_data = data.replace(_l, '')
```

### Comparing `hak-0.0.88/hak/one/string/separate_function_from_context.py` & `hak-0.0.9/hak/string/separate_function_from_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ignore_overlength_lines
-from hak.one.string.remove.empty_lines import f as remove_empty_lines
+from hak.string.remove.empty_lines import f as remove_empty_lines
 
 def f(content):
   first_def = content.find('def ')
   if first_def < 0: return ('', content)
 
   second_def = content.find('def ', first_def+1)
   if second_def < 0: second_def = len(content)
```

### Comparing `hak-0.0.88/hak/one/string/token/substitute.py` & `hak-0.0.9/hak/string/token/substitute.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/one/system/git/commit/run.py` & `hak-0.0.9/hak/system/git/commit/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from hak.one.directory.remove import f as rmdir
+from hak.directory.remove import f as rmdir
 from os.path import exists
 from subprocess import run as sprun
-from hak.one.file.zip.extract import f as extract
+from hak.file.zip.extract import f as extract
 from time import sleep as time_sleep
 from hak.fake.sleep import f as fake_sleep
 
 _dir_name = '../temp'
-base = './hak/one/system/git/commit'
+base = './hak/system/git/commit'
 
 codes = {'A ': 'Added', 'D ': 'Removed', 'R ': 'Renamed', 'M ': 'Modified'}
 
 def f(do_pull=True, cwd='.', do_push=True, cap_out=True, sleep=time_sleep):
   if do_pull:
     sprun(['git', 'pull'], cwd=cwd, capture_output=cap_out)
     sleep(0.05)
```

### Comparing `hak-0.0.88/hak/one/system/git/gitignore/make.py` & `hak-0.0.9/hak/system/git/gitignore/make.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdir
-from hak.one.file.load import f as load
-from hak.one.file.save import f as save
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdir
+from hak.file.load import f as load
+from hak.file.save import f as save
 
 data = '\n'.join([
   "__pycache__",
   "*.html",
   "*.pkl",
   "*.pickle",
   "*.xlsx",
```

### Comparing `hak-0.0.88/hak/one/system/git/log_oneline.py` & `hak-0.0.9/hak/system/git/log_oneline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from subprocess import run as sprun
-from hak.one.directory.make import f as mkdir
-from hak.one.directory.remove import f as rmdir
-from hak.one.system.git.init import f as git_init
-from hak.one.file.save import f as save
-from hak.one.system.git.commit.run import f as git_commit
+from hak.directory.make import f as mkdir
+from hak.directory.remove import f as rmdir
+from hak.system.git.init import f as git_init
+from hak.file.save import f as save
+from hak.system.git.commit.run import f as git_commit
 
 _root = '../temp_git_log_oneline'
 
 def up():
   mkdir(_root)
   git_init(_root)
   save(_root+'/foo.py', 'foo')
```

### Comparing `hak-0.0.88/hak/one/system/git/push_after_delay.py` & `hak-0.0.9/hak/system/git/push_after_delay.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from subprocess import run as sprun
 from time import sleep
 from time import time
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.print_and_return_false import f as pf
 
 def f(delay_s=5):
   sleep(delay_s)
   return sprun(['git', 'push'], capture_output=True)
 
 def t():
   delay_s = 0.5
```

### Comparing `hak-0.0.88/hak/one/system/screen/clear.py` & `hak-0.0.9/hak/system/screen/clear.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.88/hak/one/terminal.py` & `hak-0.0.9/hak/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from hak.one.system.screen.clear import f as clear_screen
-from hak.one.string.print_and_return_false import f as pf
+from hak.system.screen.clear import f as clear_screen
+from hak.string.print_and_return_false import f as pf
 
 class Terminal:
   __init__ = lambda self, mode='run': self.reset(mode)
 
   def print(self, string:str='', end='\n'):
     if self.mode == 'test':
       self.output_stream_as_list.append(string+end)
```

### Comparing `hak-0.0.88/hak/other/patch/do.py` & `hak-0.0.9/hak/patch/do.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,39 @@
-from copy import deepcopy
-from hak.one.directory.empty import f as empty_directory
-from hak.one.directory.make import f as mkdir
-from hak.one.directory.remove import f as rmdirie
-from hak.one.file.load import f as load
-from hak.one.file.save import f as save
-from hak.one.string.print_and_return_false import f as pf
-from hak.one.system.git.commit.run import f as add_to_git
-from hak.one.system.git.commit.run import t as t_add_to_git
-from hak.other.pip.dist_tar.make import f as generate_new_dist_tar
-from hak.other.pip.dist_tar.make import t as t_generate_new_dist_tar
-from hak.other.pip.dist_tar.remove import t as t_remove_dist_tar
-from hak.other.pip.upload import f as start_upload
-from hak.other.pip.upload import t as t_start_upload
-from hak.other.pip.version.get import f as get_pip_version
-from hak.other.pip.version.get import t as t_get_pip_version
-from hak.other.setup.cfg.update import f as update_setup_cfg
-from hak.other.setup.cfg.update import t as t_update_setup_cfg
-from hak.other.setup.py.update import f as update_setup_py
-from hak.other.setup.py.update import t as t_update_setup_py
+from hak.pip.version.get import f as get_pip_version
+from hak.pip.version.get import t as t_get_pip_version
+
+from hak.setup.cfg.update import f as update_setup_cfg
+from hak.setup.cfg.update import t as t_update_setup_cfg
+
+from hak.setup.py.update import f as update_setup_py
+from hak.setup.py.update import t as t_update_setup_py
+
+from hak.pip.dist_tar.make import f as generate_new_dist_tar
+from hak.pip.dist_tar.make import t as t_generate_new_dist_tar
+
+from hak.system.git.commit.run import f as add_to_git
+from hak.system.git.commit.run import t as t_add_to_git
+
+from hak.pip.upload import f as start_upload
+from hak.pip.upload import t as t_start_upload
+
+from hak.directory.remove import f as rmdirie
+
+from hak.file.save import f as save
+
+from hak.pip.dist_tar.remove import f as remove_dist_tar
+from hak.pip.dist_tar.remove import t as t_remove_dist_tar
+
 from subprocess import run as sprun
+from hak.string.print_and_return_false import f as pf
+
+from hak.directory.make import f as mkdir
+from hak.file.load import f as load
+
+from copy import deepcopy
 
 def up():
   x = {}
   x['root'] = f"./hak_test"
   x['cfg_path'] = f"{x['root']}/setup.cfg"
   x['py_path'] = f"{x['root']}/setup.py"
 
@@ -97,16 +108,15 @@
   z['py_path'] = f'{z["root"]}/setup.py'
 
   z['v'] = z['v'] or get_pip_version('hak')
   z['v']['patch'] += 1
 
   update_setup_cfg({'v': z['v'], 'filename': z['cfg_path']})
   update_setup_py({'v': z['v'], 'filename': z['py_path']})
-  empty_directory('./dist/')
-  
+  remove_dist_tar(x)
   generate_new_dist_tar(x)
   # add_to_git(cwd=_root, cap_out=True)
   if 'local_test_only' not in x: z['upload_result'] = start_upload(x)
   return z
 
 def t():
   x = up()
```

### Comparing `hak-0.0.88/hak/other/pip/dist_tar/make.py` & `hak-0.0.9/hak/pip/dist_tar/make.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from copy import deepcopy
 from subprocess import run as sprun
-
-from hak.one.directory.make import f as mkdir
-from hak.one.directory.remove import f as rmdir
-from hak.one.file.save import f as save
-from hak.one.file.zip.extract import f as extract
-from hak.one.string.print_and_return_false import f as pf
+from hak.string.colour.primary import f as primary
+from hak.directory.remove import f as rmdir
+from hak.directory.make import f as mkdir
+from hak.file.save import f as save
+from hak.file.zip.extract import f as extract
+from copy import deepcopy
+from hak.string.print_and_return_false import f as pf
 
 def f(x):
   x = deepcopy(x)
   cwd = x['root'] if 'root' in x else '.'
   return sprun(['python3', 'setup.py', 'sdist'], cwd=cwd, capture_output=True)
 
 def up():
   _root = '../temp'
   mkdir(_root)
   mkdir(_root+'/hak')
   save(_root+'/hak/__init__.py', '')
 
-  _base = './hak/one/system/git/commit'
+  _base = './hak/system/git/commit'
   extract(f'{_base}/added_file_pre_commit.zip', '..')
 
   _setup_filepath = _root + '/setup.py'
   save(_setup_filepath, "\n".join([
     'from setuptools import setup',
     'from pathlib import Path',
     '',
```

### Comparing `hak-0.0.88/hak/other/pip/dist_tar/remove.py` & `hak-0.0.9/hak/pip/dist_tar/remove.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from os.path import exists
 
-from hak.one.directory.make import f as mkdir
-from hak.one.directory.empty import f as empty_directory
-from hak.one.directory.remove import f as rmdirie
-from hak.one.file.save import f as save
-from hak.one.string.print_and_return_false import f as pf
+from hak.directory.make import f as mkdir
+from hak.directory.empty import f as empty_directory
+from hak.directory.remove import f as rmdirie
+from hak.file.save import f as save
+from hak.string.print_and_return_false import f as pf
 
 from copy import deepcopy
 
 def f(x):
   x = deepcopy(x)
   root = x['root'] if 'root' in x else '.'
   return empty_directory(root)
 
 def up():
   temp_root = './_dist_tars_remove'
-  filename = f'{temp_root}/junk.tar'
-  x = {'filename': filename, 'root': temp_root}
   mkdir(temp_root)
+  print(temp_root)
+  filename = f'{temp_root}/junk.tar'
   save(filename, 'junk')
-  return x
+  return {'filename': filename, 'root': temp_root}
 
 dn = lambda x: rmdirie(x['root'])
 
 def t():
   x = up()
   f(x)
-  if exists(x['filename']): return pf(f'exists({x["filename"]})')
+  if not exists(x['filename']): return pf(f'not exists({x["filename"]})')
   dn(x)
   if exists(x["root"]): return pf(f'exists({x["root"]})')
   return True
```

### Comparing `hak-0.0.88/hak/other/pip/setup/update.py` & `hak-0.0.9/hak/pip/setup/update.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.one.file.save import f as save
-from hak.one.file.remove import f as remove
-from hak.one.file.load import f as read_file
-from hak.one.file.save_lines import f as apply_change_to_file
-from hak.many.strings.make_patch_version_change_to_py import f as patch_setup_py
+from hak.file.save import f as save
+from hak.file.remove import f as remove
+from hak.file.load import f as read_file
+from hak.file.save_lines import f as apply_change_to_file
+from hak.list.strings.make_patch_version_change_to_py import f as patch_setup_py
 
 f = lambda version, filename: apply_change_to_file(
   filename,
   '\n'.join(patch_setup_py(version, read_file(filename).split('\n')))
 )
 
 filename='./fake_setup.py'
```

### Comparing `hak-0.0.88/hak/other/pip/upload.py` & `hak-0.0.9/hak/pip/upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from subprocess import run as sprun
 from hak.fake.subprocess.run import f as fake_sprun
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdirie
-from hak.one.file.load import f as load
-from hak.one.string.print_and_return_false import f as pf
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdirie
+from hak.file.load import f as load
+from hak.string.print_and_return_false import f as pf
 
 _dir = '../start_upload'
 
 up = lambda: mkdirine(_dir)
 
 dn = lambda: rmdirie(_dir)
```

### Comparing `hak-0.0.88/hak/other/pip/version/get.py` & `hak-0.0.9/hak/pip/version/get.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from requests import get
-from hak.one.file.pickle.load_if_exists import f as load
-from hak.one.dict.make_from_key_value_lists import f as make_from_key_val_lists
-from hak.one.string.print_and_return_false import f as pf
+from hak.file.pickle.load_if_exists import f as load
+from hak.dict.make_from_key_value_lists import f as make_from_key_value_lists
+from hak.string.print_and_return_false import f as pf
 
 def f(name, response=None):
   response = response or get(f"https://pypi.org/project/{name}/")
   lines = [l for l in response.text.split('\n') if all([
     '<h2>Initiate a new hak project</h2>' not in l,
     'hak ' in l,
     'title' not in l
   ])]
   v_line = lines[0] if lines else '0.0.4'
   v_str = v_line.split('hak ')[-1]
-  return make_from_key_val_lists(
+  return make_from_key_value_lists(
     ['major', 'minor', 'patch'],
     [int(_) for _ in v_str.split('.')]
   )
 
 def t():
-  x = {
-    'name': "hak",
-    'response': load('./hak/other/pip/version/test_response.pkl')
-  }
   y = {'major': 0, 'minor': 0, 'patch': 4}
-  z = f(**x) 
-  return y == z or pf([f'y == z: {y == z}', f'x: {x}', f'y: {y}', f'z: {z}'])
+  z = f("hak", response=load('./hak/pip/version/test_response.pkl')) 
+  return y == z or pf([f'y == z: {y == z}', f'z: {z}', f'y: {y}'])
```

### Comparing `hak-0.0.88/hak/other/report/fail/no_xyz.py` & `hak-0.0.9/hak/report/fail/z_return_neq_y_return.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,46 @@
-from hak.one.string.colour.bright.red import f as danger
-from hak.one.duration import f as duration
+from hak.string.colour.bright.red import f as danger
+from hak.duration import f as duration
+from hak.string.colour.primary import f as pri
+from hak.string.colour.secondary import f as sec
+from hak.report.summarise_file import f as summarise_file
 from time import time
 
-f = lambda name, mode, time_started, w: (
-  False, '\n'.join(['|'.join([
-    "\r",
-    f"{danger('  FAIL  ')}",
-    f" {name:{w}} ",
-    f" {duration(time_started, name)} ",
-    "",
-  ]),
-  f"{danger('mode:')} {mode}",
-]))
+f = lambda name, x_args, y_return, z_return, time_started, max_filename_len: (
+  False, '\n'.join([
+    '|'.join([
+      "\r",
+      f"{danger('  FAIL  ')}",
+      f" {name:{max_filename_len}} ",
+      f" {duration(time_started, name)} ",
+      ""
+    ]),
+    f"{danger('mode:')} {'y_return != z_return'}",
+    f"{pri('Input       x_args: ')} {summarise_file(str(x_args))}",
+    f"{pri('y y_return: ')} {summarise_file(str(y_return))}",
+    f"{pri('z z_return: ')} {summarise_file(str(z_return))}",
+  ])
+)
 
 def t():
   e_result = False
   e_message_l = '|'.join([
     "\r",
     "\x1b[1;31m  FAIL  \x1b[0;0m",
     " fake_name ",
     " \x1b[1;32m                           "
   ])
-  e_message_r = '\n'.join(["\x1b[0;0m |", "\x1b[1;31mmode:\x1b[0;0m fake_mode"])
+  e_message_r = '\n'.join([
+    "\x1b[0;0m |",
+    "\x1b[1;31mmode:\x1b[0;0m y_return != z_return",
+    "\x1b[1;34mInput       x_args: \x1b[0;0m {'a': 0, 'b': 1}",
+    "\x1b[1;34my y_return: \x1b[0;0m 0.5",
+    "\x1b[1;34mz z_return: \x1b[0;0m 0.5",
+  ])
 
-  o_result, o_message = f('fake_name', 'fake_mode', time(), 9)
+  o_result, o_message = f('fake_name', {'a': 0, 'b': 1}, 0.5, 0.5, time(), 9)
 
   return all([
     e_result == o_result,
     e_message_l == o_message[:len(e_message_l)],
     e_message_r == o_message[len(o_message) - len(e_message_r):]
   ])
```

### Comparing `hak-0.0.88/hak/other/report/fail/xyz.py` & `hak-0.0.9/hak/report/fail/xyz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.one.string.colour.bright.red import f as danger
-from hak.one.duration import f as duration
-from hak.one.string.colour.primary import f as pri
-from hak.one.string.colour.secondary import f as sec
-from hak.other.report.summarise_file import f as summarise_file
+from hak.string.colour.bright.red import f as danger
+from hak.duration import f as duration
+from hak.string.colour.primary import f as pri
+from hak.string.colour.secondary import f as sec
+from hak.report.summarise_file import f as summarise_file
 from time import time
 
 f = lambda name, xyz, mode, time_started, max_filename_length: (
   False, '\n'.join([
     '|'.join([
       "\r",
       f"{danger('  FAIL  ')}",
```

### Comparing `hak-0.0.88/hak/other/report/fail/z_return_neq_y_return.py` & `hak-0.0.9/hak/report/property_failure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,38 @@
-from hak.one.string.colour.bright.red import f as danger
-from hak.one.duration import f as duration
-from hak.one.string.colour.primary import f as pri
-from hak.one.string.colour.secondary import f as sec
-from hak.other.report.summarise_file import f as summarise_file
+from hak.string.colour.bright.red import f as danger
+from hak.duration import f as duration
 from time import time
 
-f = lambda name, x_args, y_return, z_return, time_started, max_filename_len: (
-  False, '\n'.join([
+f = lambda name, mode, time_started, max_filename_length: (
+  False,
+  '\n'.join([
     '|'.join([
       "\r",
       f"{danger('  FAIL  ')}",
-      f" {name:{max_filename_len}} ",
+      f" {name:{max_filename_length}} ",
       f" {duration(time_started, name)} ",
       ""
     ]),
-    f"{danger('mode:')} {'y_return != z_return'}",
-    f"{pri('Input       x_args: ')} {summarise_file(str(x_args))}",
-    f"{pri('y y_return: ')} {summarise_file(str(y_return))}",
-    f"{pri('z z_return: ')} {summarise_file(str(z_return))}",
+    f"{danger('mode:')} {mode}",
   ])
 )
 
 def t():
   e_result = False
   e_message_l = '|'.join([
-    "\r",
-    "\x1b[1;31m  FAIL  \x1b[0;0m",
-    " fake_name ",
-    " \x1b[1;32m                           "
+    '\r',
+    '\x1b[1;31m  FAIL  \x1b[0;0m',
+    ' fake_name ',
+    ' \x1b[1;32m                           '
   ])
-  e_message_r = '\n'.join([
-    "\x1b[0;0m |",
-    "\x1b[1;31mmode:\x1b[0;0m y_return != z_return",
-    "\x1b[1;34mInput       x_args: \x1b[0;0m {'a': 0, 'b': 1}",
-    "\x1b[1;34my y_return: \x1b[0;0m 0.5",
-    "\x1b[1;34mz z_return: \x1b[0;0m 0.5",
+  e_message_r = '|'.join([
+    '\x1b[0;0m ',
+    '\n\x1b[1;31mmode:\x1b[0;0m fake_mode'
   ])
-
-  o_result, o_message = f('fake_name', {'a': 0, 'b': 1}, 0.5, 0.5, time(), 9)
+  
+  o_result, o_message = f('fake_name', 'fake_mode', time(), 9)
 
   return all([
-    e_result == o_result,
     e_message_l == o_message[:len(e_message_l)],
-    e_message_r == o_message[len(o_message) - len(e_message_r):]
+    e_message_r == o_message[len(o_message) - len(e_message_r):],
+    e_result == o_result
   ])
```

### Comparing `hak-0.0.88/hak/other/report/fail/z_stdo_neq_y_stdo.py` & `hak-0.0.9/hak/report/fail/z_stdo_neq_y_stdo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.one.string.colour.bright.red import f as danger
-from hak.one.duration import f as duration
-from hak.one.string.colour.primary import f as pri
-from hak.one.string.colour.secondary import f as sec
-from hak.other.report.summarise_file import f as summarise_file
+from hak.string.colour.bright.red import f as danger
+from hak.duration import f as duration
+from hak.string.colour.primary import f as pri
+from hak.string.colour.secondary import f as sec
+from hak.report.summarise_file import f as summarise_file
 from time import time
 
 f = lambda name, x_args, x_stdi, y_stdo, z_stdo, t_0, max_filename_len: (
   False, '\n'.join([
     '|'.join([
       "\r",
       f"{danger('  FAIL  ')}",
```

### Comparing `hak-0.0.88/hak/other/report/property_failure.py` & `hak-0.0.9/hak/report/fail/no_xyz.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-from hak.one.string.colour.bright.red import f as danger
-from hak.one.duration import f as duration
+from hak.string.colour.bright.red import f as danger
+from hak.duration import f as duration
 from time import time
 
-f = lambda name, mode, time_started, max_filename_length: (
-  False,
-  '\n'.join([
-    '|'.join([
-      "\r",
-      f"{danger('  FAIL  ')}",
-      f" {name:{max_filename_length}} ",
-      f" {duration(time_started, name)} ",
-      ""
-    ]),
-    f"{danger('mode:')} {mode}",
-  ])
-)
+f = lambda name, mode, time_started, w: (
+  False, '\n'.join(['|'.join([
+    "\r",
+    f"{danger('  FAIL  ')}",
+    f" {name:{w}} ",
+    f" {duration(time_started, name)} ",
+    "",
+  ]),
+  f"{danger('mode:')} {mode}",
+]))
 
 def t():
   e_result = False
   e_message_l = '|'.join([
-    '\r',
-    '\x1b[1;31m  FAIL  \x1b[0;0m',
-    ' fake_name ',
-    ' \x1b[1;32m                           '
-  ])
-  e_message_r = '|'.join([
-    '\x1b[0;0m ',
-    '\n\x1b[1;31mmode:\x1b[0;0m fake_mode'
+    "\r",
+    "\x1b[1;31m  FAIL  \x1b[0;0m",
+    " fake_name ",
+    " \x1b[1;32m                           "
   ])
-  
+  e_message_r = '\n'.join(["\x1b[0;0m |", "\x1b[1;31mmode:\x1b[0;0m fake_mode"])
+
   o_result, o_message = f('fake_name', 'fake_mode', time(), 9)
 
   return all([
+    e_result == o_result,
     e_message_l == o_message[:len(e_message_l)],
-    e_message_r == o_message[len(o_message) - len(e_message_r):],
-    e_result == o_result
+    e_message_r == o_message[len(o_message) - len(e_message_r):]
   ])
```

### Comparing `hak-0.0.88/hak/other/report/success.py` & `hak-0.0.9/hak/report/success.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from hak.one.string.colour.bright.green import f as success
-from hak.one.duration import f as duration
+from hak.string.colour.bright.green import f as success
+from hak.duration import f as duration
 from time import time
 
 f = lambda name, time_started, max_filename_length: (
   True, '|'.join([
     "\r",
     f"{success('  PASS  ')}",
     f" {name:{max_filename_length}} ",
```

### Comparing `hak-0.0.88/hak/other/setup/cfg/update.py` & `hak-0.0.9/hak/setup/cfg/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.one.file.load import f as load
-from hak.one.file.save import f as save
-from hak.many.strings.patch_setup_cfg import f as increment_patch_in_setup_cfg
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdirie
+from hak.file.load import f as load
+from hak.file.save import f as save
+from hak.list.strings.patch_setup_cfg import f as increment_patch_in_setup_cfg
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdirie
 from copy import deepcopy
 
 def f(x):
   x = deepcopy(x)
   v = x['v']
   filename = x['filename'] if 'filename' in x else 'setup.cfg'
   lines = load(filename).split('\n')
```

### Comparing `hak-0.0.88/hak/other/setup/py/update.py` & `hak-0.0.9/hak/setup/py/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from hak.one.file.load import f as load
-from hak.one.file.save import f as save
-from hak.many.strings.patch_setup_py import f as increment_patch_in_setup_py
-from hak.one.directory.make import f as mkdirine
-from hak.one.directory.remove import f as rmdirie
-from hak.one.string.print_and_return_false import f as pf
+from hak.file.load import f as load
+from hak.file.save import f as save
+from hak.list.strings.patch_setup_py import f as increment_patch_in_setup_py
+from hak.directory.make import f as mkdirine
+from hak.directory.remove import f as rmdirie
+from hak.string.print_and_return_false import f as pf
 from copy import deepcopy
 
 def f(x):
   x = deepcopy(x)
   filename = x['filename'] if 'filename' in x else 'setup.py'
   lines = load(filename).split('\n')
   new_lines = increment_patch_in_setup_py(x['v'], lines)
```

### Comparing `hak-0.0.88/hak/test/final_line/check.py` & `hak-0.0.9/hak/test/check_final_line.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from hak.one.file.load import f as load
-from hak.one.file.remove import f as remove
-from hak.one.file.save import f as save_file
-from hak.many.strings.filepaths.py.testables.get import f as list_testables
-from hak.one.string.colour.bright.green import f as success
-from hak.one.string.colour.bright.red import f as danger
-from hak.one.string.print_and_return_false import f as pf
-from hak.one.terminal import Terminal
+from hak.string.colour.bright.green import f as success
+from hak.list.strings.filepaths.py.testables.get import f as list_testables
+from hak.file.load import f as load
+from hak.string.colour.bright.red import f as danger
+from hak.string.print_and_return_false import f as pf
+from hak.file.save import f as save_file
+from hak.terminal import Terminal
+from hak.file.remove import f as remove
 
 # check_final_line
 
 def f(filepaths=None, term=None):
   term = term or Terminal()
   term.print('Checking final lines...', end='\r')
   filepaths = filepaths or list_testables()
   for pi in filepaths:
     _lines = load(pi).split('\n')
-    _last_index = len(_lines)-1
-    l = _lines[_last_index]
-    if l != '': return pf([f'{pi}:{_last_index}', danger([l])], p=term.print)
+    _last_line_index = len(_lines)-1
+    _line = _lines[_last_line_index]
+    if _line != '': return pf([
+      f'{pi}:{_last_line_index}',
+      danger([_line])
+    ], p=term.print)
   term.print(f"{success('PASS')} Final lines "+' '*20)
   return True
 
 def t_expected_false():
   _test_files = {
     './a.pz': "\n".join(["abc", "xyz"]),
     './b.pz': "\n".join(["abc", "xyz", '']),
@@ -36,15 +39,19 @@
     "./a.pz:1\n\x1b[1;31m['xyz']\x1b[0;0m\n"
   ]
   term = Terminal(mode='test')
   z = f(x, term=term)
   
   for k in _test_files: remove(k)
 
-  if y != z: return pf([f'x: {x}', f'y: {y}', f'z: {z}'])
+  if y != z: return pf([
+    'y != z',
+    f'y: {y}',
+    f'z: {z}'
+  ])
   if term.output_stream_as_list != y_out_stream_list: return pf([
     'term.output_stream_as_list != y_out_stream_list',
     f'term.output_stream_as_list: {term.output_stream_as_list}',
     f'y_out_stream_list:          {y_out_stream_list}',
   ])
   return True
 
@@ -63,15 +70,19 @@
     '\x1b[1;32mPASS\x1b[0;0m Final lines                     \n'
   ]
   term = Terminal(mode='test')
   z = f(x, term=term)
   
   for k in _test_files: remove(k)
 
-  if y != z: return pf([f'x: {x}', f'y: {y}', f'z: {z}'])
+  if y != z: return pf([
+    'y != z',
+    f'y: {y}',
+    f'z: {z}'
+  ])
   if term.output_stream_as_list != y_out_stream_list: return pf([
     'term.output_stream_as_list != y_out_stream_list',
     f'term.output_stream_as_list: {term.output_stream_as_list}',
     f'y_out_stream_list:          {y_out_stream_list}',
   ])
   return True
```

### Comparing `hak-0.0.88/hak/test/line_lengths/check.py` & `hak-0.0.9/hak/test/check_line_lengths.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from hak.one.string.colour.bright.green import f as success
-from hak.many.strings.filepaths.py.testables.get import f as list_testables
-from hak.one.file.load import f as load
-from hak.one.string.print_and_return_false import f as pf
-from hak.one.string.colour.bright.red import f as danger
-from hak.one.file.save import f as save
-from hak.one.terminal import Terminal
-from hak.one.file.remove import f as remove
+from hak.string.colour.bright.green import f as success
+from hak.list.strings.filepaths.py.testables.get import f as list_testables
+from hak.file.load import f as load
+from hak.string.print_and_return_false import f as pf
+from hak.string.colour.bright.red import f as danger
+from hak.file.save import f as save
+from hak.terminal import Terminal
+from hak.file.remove import f as remove
 
 # check_line_lengths
 
 def f(filepaths=None, term=None):
   term = term or Terminal()
   term.print('Checking line lengths...', end='\r')
   filepaths = filepaths or list_testables()
```

### Comparing `hak-0.0.88/hak/test/line_lengths_check.py` & `hak-0.0.9/hak/test/line_lengths_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from hak.many.strings.filepaths.py.testables.get import f as list_testables
-from hak.one.file.load import f as load
-from hak.one.string.print_and_return_false import f as pf
-from hak.one.string.colour.bright.red import f as danger
-from hak.one.string.colour.bright.green import f as success
+from hak.list.strings.filepaths.py.testables.get import f as list_testables
+from hak.file.load import f as load
+from hak.string.print_and_return_false import f as pf
+from hak.string.colour.bright.red import f as danger
+from hak.string.colour.bright.green import f as success
 
 def f(_Pi=None):
   print('Checking line lengths...', end='\r')
   _Pi = list_testables() or _Pi
   for _pi in _Pi:
     ignore_line_lengths = False
     for line_index, line in enumerate(load(_pi).split('\n')):
```

### Comparing `hak-0.0.88/hak/test/oldest_file_print.py` & `hak-0.0.9/hak/test/oldest_file_print.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from hak.many.strings.filepaths.py.testables.get import f as list_testables
+from hak.list.strings.filepaths.py.testables.get import f as list_testables
 from os.path import getmtime
-from hak.one.file.pickle.load_if_exists import f as load_pickle
-from hak.one.file.remove import f as remove
-from hak.one.file.pickle.save import f as save
-from hak.many.strings.filepaths.py.testables.get import f as make_Pi_t
-from hak.one.dict.durations.to_tuple_list_sorted_by_duration import f as srt
+from hak.file.pickle.load_if_exists import f as load_pickle
+from hak.file.remove import f as remove
+from hak.file.pickle.save import f as save
+from hak.list.strings.filepaths.py.testables.get import f as make_Pi_t
+from hak.dict.test_durations.to_tuple_list_sorted_by_duration import f as srt
 
 def f(_Pi=None):
   _Pi = list_testables()
   try: prev = load_pickle('./last_modified.pickle') or set()
   except EOFError as eofe: remove('./last_modified.pickle'); prev = set()
   last_mods = {py_filename: getmtime(py_filename) for py_filename in _Pi}
   save(last_mods, './last_modified.pickle')
```

### Comparing `hak-0.0.88/setup.cfg` & `hak-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hak
-version = 0.0.88
+version = 0.0.9
 author = John Forbes
 author_email = john.robert.forbes@gmail.com
 description = Function Test Pair Toolbox
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JohnForbes/hak
 license_files = LICENSE
```

