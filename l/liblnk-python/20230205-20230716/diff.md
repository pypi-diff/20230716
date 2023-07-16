# Comparing `tmp/liblnk-python-20230205.tar.gz` & `tmp/liblnk-python-20230716.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liblnk-python-20230205.tar", last modified: Sun Feb  5 16:45:09 2023, max compression
+gzip compressed data, was "liblnk-python-20230716.tar", last modified: Sun Jul 16 06:58:33 2023, max compression
```

## Comparing `liblnk-python-20230205.tar` & `liblnk-python-20230716.tar`

### file list

```diff
@@ -1,906 +1,915 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_format_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_format_class_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_property_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1142 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_libfole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31561 2023-02-05 14:12:55.000000 liblnk-20230205/libfwps/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45991 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-02-05 14:12:38.000000 liblnk-20230205/libfwps/libfwps_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/common/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-02-04 09:58:08.000000 liblnk-20230205/common/config_msc.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-02-04 09:58:08.000000 liblnk-20230205/common/byte_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-02-04 09:58:08.000000 liblnk-20230205/common/common.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-02-04 09:58:08.000000 liblnk-20230205/common/system_string.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-02-04 09:58:03.000000 liblnk-20230205/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7233 2023-02-05 14:13:06.000000 liblnk-20230205/common/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7236 2023-02-04 09:58:08.000000 liblnk-20230205/common/types.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2243 2023-02-04 09:58:08.000000 liblnk-20230205/common/config_winapi.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-02-04 09:58:08.000000 liblnk-20230205/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16814 2023-02-05 14:13:06.000000 liblnk-20230205/common/config.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-02-04 09:58:08.000000 liblnk-20230205/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25063 2023-02-05 14:12:55.000000 liblnk-20230205/common/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-02-04 09:58:08.000000 liblnk-20230205/common/file_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-02-04 09:58:08.000000 liblnk-20230205/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15873 2023-02-05 14:12:54.000000 liblnk-20230205/common/config.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-02-04 09:58:08.000000 liblnk-20230205/common/wide_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      630 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29386 2023-02-05 14:12:55.000000 liblnk-20230205/libfole/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2023-02-05 14:12:37.000000 liblnk-20230205/libfole/libfole_types.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/pylnk/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2420 2023-02-04 10:14:36.000000 liblnk-20230205/pylnk/pylnk_data_blocks.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6747 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_drive_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2023-02-04 16:18:22.000000 liblnk-20230205/pylnk/pylnk_strings_data_block.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1586 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_data_flags.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10926 2023-02-04 16:53:14.000000 liblnk-20230205/pylnk/pylnk_data_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6547 2023-02-04 16:14:17.000000 liblnk-20230205/pylnk/pylnk_file.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_error.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_datetime.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10206 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_file_attribute_flags.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1576 2023-02-04 16:23:50.000000 liblnk-20230205/pylnk/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_drive_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    86746 2023-02-04 16:52:31.000000 liblnk-20230205/pylnk/pylnk_file.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_datetime.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2262 2023-02-04 16:44:55.000000 liblnk-20230205/pylnk/pylnk_distributed_link_tracking_data_block.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13848 2023-02-04 16:59:04.000000 liblnk-20230205/pylnk/pylnk_distributed_link_tracking_data_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1352 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9307 2023-02-04 10:14:36.000000 liblnk-20230205/pylnk/pylnk_data_blocks.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_liblnk.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11473 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_data_flags.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    33697 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_file_object_io_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_file_attribute_flags.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1165 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_guid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54747 2023-02-05 14:12:56.000000 liblnk-20230205/pylnk/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5511 2023-02-04 16:21:20.000000 liblnk-20230205/pylnk/pylnk_strings_data_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16922 2023-02-04 16:52:14.000000 liblnk-20230205/pylnk/pylnk.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_file_object_io_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_codepage.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2881 2023-02-04 09:58:09.000000 liblnk-20230205/pylnk/pylnk_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2131 2023-02-04 16:14:59.000000 liblnk-20230205/pylnk/pylnk_data_block.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29463 2023-02-05 14:12:55.000000 liblnk-20230205/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-02-05 14:12:35.000000 liblnk-20230205/libfguid/libfguid_extern.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9663 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_distributed_link_tracker_properties.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14741 2023-02-04 10:56:22.000000 liblnk-20230205/tests/pylnk_test_file.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3956 2023-02-04 10:16:41.000000 liblnk-20230205/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125663 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_file.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_liblnk.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19470 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_data_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_unused.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-02-04 10:19:11.000000 liblnk-20230205/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7293 2023-02-04 09:59:15.000000 liblnk-20230205/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15540 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_file_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7856 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_io_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_memory.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13235 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_functions.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_getopt.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14071 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25666 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_data_string.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     2148 2023-02-04 09:58:09.000000 liblnk-20230205/tests/test_lnkinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13532 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_special_folder_location.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_macros.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_libbfio.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3788 2023-02-04 10:16:41.000000 liblnk-20230205/tests/test_tools.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3236 2023-02-04 10:19:03.000000 liblnk-20230205/tests/pylnk_test_support.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1645 2023-02-04 09:58:09.000000 liblnk-20230205/tests/test_manpage.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_tools_output.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14125 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_known_folder_location.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37784 2023-02-04 09:58:09.000000 liblnk-20230205/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8456 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_link_target_identifier.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65088 2023-02-05 14:12:56.000000 liblnk-20230205/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8362 2023-02-04 09:59:15.000000 liblnk-20230205/tests/lnk_test_location_information.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_tools_signal.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_notify.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-02-04 09:58:09.000000 liblnk-20230205/tests/lnk_test_libclocale.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30019 2023-02-05 14:12:55.000000 liblnk-20230205/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-02-05 14:12:27.000000 liblnk-20230205/libclocale/libclocale_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-02-05 14:12:55.000000 liblnk-20230205/missing
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      734 2023-02-04 09:58:04.000000 liblnk-20230205/liblnk.pc.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3571 2022-04-28 04:23:51.000000 liblnk-20230205/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56019 2023-02-05 14:12:51.000000 liblnk-20230205/aclocal.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33525 2023-02-05 14:12:55.000000 liblnk-20230205/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-02-05 14:12:21.000000 liblnk-20230205/libbfio/libbfio_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-02-04 09:58:05.000000 liblnk-20230205/COPYING
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2023-02-04 09:58:05.000000 liblnk-20230205/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/include/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      464 2023-02-04 09:58:05.000000 liblnk-20230205/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/include/liblnk/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4928 2023-02-04 09:58:08.000000 liblnk-20230205/include/liblnk/definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-02-04 09:58:08.000000 liblnk-20230205/include/liblnk/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4831 2023-02-05 14:13:06.000000 liblnk-20230205/include/liblnk/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2023-02-04 09:58:08.000000 liblnk-20230205/include/liblnk/features.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4962 2023-02-04 09:58:08.000000 liblnk-20230205/include/liblnk/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2023-02-05 14:13:06.000000 liblnk-20230205/include/liblnk/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4926 2023-02-05 14:13:06.000000 liblnk-20230205/include/liblnk/definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2023-02-04 09:58:08.000000 liblnk-20230205/include/liblnk/codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2023-02-04 09:58:08.000000 liblnk-20230205/include/liblnk/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28026 2023-02-05 14:12:55.000000 liblnk-20230205/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36827 2023-02-05 14:13:06.000000 liblnk-20230205/include/liblnk.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36827 2023-02-04 15:52:54.000000 liblnk-20230205/include/liblnk.h.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-02-05 14:12:55.000000 liblnk-20230205/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-02-05 14:12:55.000000 liblnk-20230205/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/liblnk.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      119 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/changelog.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       27 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/liblnk-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2023-02-05 14:13:06.000000 liblnk-20230205/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2023-02-04 09:58:09.000000 liblnk-20230205/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/liblnk-python3.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/source/format
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      754 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/rules
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/liblnk-dev.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2040 2023-02-04 09:58:05.000000 liblnk-20230205/dpkg/control
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32634 2023-02-05 14:12:55.000000 liblnk-20230205/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-02-05 14:12:34.000000 liblnk-20230205/libfdatetime/libfdatetime_filetime.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30783 2023-02-05 14:12:55.000000 liblnk-20230205/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-02-05 14:12:26.000000 liblnk-20230205/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2570 2023-02-05 14:13:06.000000 liblnk-20230205/liblnk.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32873 2023-02-05 14:12:55.000000 liblnk-20230205/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-02-05 14:12:33.000000 liblnk-20230205/libcthreads/libcthreads_queue.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       90 2023-02-04 09:58:08.000000 liblnk-20230205/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/lnktools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69191 2023-02-04 09:59:42.000000 liblnk-20230205/lnktools/info_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_liblnk.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libfdatetime.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2340 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/shell_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1595 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/property_store.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2023-01-29 14:00:19.000000 liblnk-20230205/lnktools/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_getopt.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1708 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libfwps.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26318 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/property_store.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    38310 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/shell_items.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_output.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3952 2023-02-04 09:59:42.000000 liblnk-20230205/lnktools/info_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4143 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32095 2023-02-05 14:12:56.000000 liblnk-20230205/lnktools/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_signal.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6925 2023-02-04 09:59:42.000000 liblnk-20230205/lnktools/lnkinfo.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5659 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_signal.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2023-02-04 09:58:09.000000 liblnk-20230205/lnktools/lnktools_getopt.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/pylnk-python3/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2044 2023-02-04 16:24:18.000000 liblnk-20230205/pylnk-python3/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54771 2023-02-05 14:12:56.000000 liblnk-20230205/pylnk-python3/Makefile.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-02-05 14:12:55.000000 liblnk-20230205/config.sub
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30061 2023-02-05 14:12:55.000000 liblnk-20230205/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-02-05 14:12:30.000000 liblnk-20230205/libcpath/libcpath_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      154 2010-06-19 10:23:30.000000 liblnk-20230205/manuals/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4351 2023-02-04 09:58:09.000000 liblnk-20230205/manuals/lnkinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12980 2023-02-04 10:14:36.000000 liblnk-20230205/manuals/liblnk.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27017 2023-02-05 14:12:56.000000 liblnk-20230205/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-13 02:34:46.000000 liblnk-20230205/ABOUT-NLS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6294 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libfwps/libfwps.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_special_folder_location/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5909 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_special_folder_location/lnk_test_special_folder_location.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libfole/libfole.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/pylnk/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7791 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/pylnk/pylnk.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6508 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_support/lnk_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_location_information/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5900 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_location_information/lnk_test_location_information.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6420 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_file/lnk_test_file.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1579 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5803 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_tools_output/lnk_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_link_target_identifier/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5906 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_link_target_identifier/lnk_test_link_target_identifier.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_data_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6117 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_data_string/lnk_test_data_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5700 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_notify/lnk_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5803 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_tools_signal/lnk_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5615 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_error/lnk_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libcpath/libcpath.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32633 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/liblnk.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_known_folder_location/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5903 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_known_folder_location/lnk_test_known_folder_location.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/liblnk/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9740 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/liblnk/liblnk.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libuna/libuna.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13549 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libfwsi/libfwsi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_distributed_link_tracker_properties/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5945 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_distributed_link_tracker_properties/lnk_test_distributed_link_tracker_properties.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_file_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6117 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_file_header/lnk_test_file_header.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23598 2023-02-05 14:12:56.000000 liblnk-20230205/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5867 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_io_handle/lnk_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_data_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6114 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_data_block/lnk_test_data_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnkinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7248 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnkinfo/lnkinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/lnk_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6286 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/lnk_test_tools_info_handle/lnk_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2023-02-04 16:24:23.000000 liblnk-20230205/msvscpp/libcsplit/libcsplit.vcproj
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3504 2023-02-04 09:58:05.000000 liblnk-20230205/liblnk.spec.in
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11454 2023-02-04 09:58:36.000000 liblnk-20230205/setup.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-02-05 14:12:55.000000 liblnk-20230205/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-04 09:58:05.000000 liblnk-20230205/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/ossfuzz/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2023-02-04 09:58:09.000000 liblnk-20230205/ossfuzz/file_fuzzer.cc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2020-07-14 05:11:41.000000 liblnk-20230205/ossfuzz/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      962 2023-02-04 09:58:09.000000 liblnk-20230205/ossfuzz/ossfuzz_liblnk.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32242 2023-02-05 14:12:56.000000 liblnk-20230205/ossfuzz/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-02-04 09:58:09.000000 liblnk-20230205/ossfuzz/ossfuzz_libbfio.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/liblnk/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_extern.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17708 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_data_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1569 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1081 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk.rc.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2098 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_special_folder_location.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_data_string.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4484 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_distributed_link_tracker_properties.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2599 2023-02-04 08:33:09.000000 liblnk-20230205/liblnk/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11471 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_file_header.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6216 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    52878 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_location_information.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9315 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_support.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2071 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_known_folder_location.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    21041 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_data_string.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3429 2023-02-05 12:56:30.000000 liblnk-20230205/liblnk/liblnk_data_block.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libfwsi.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9265 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_link_target_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16518 2023-02-04 15:53:43.000000 liblnk-20230205/liblnk/liblnk_strings_data_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2558 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_debug.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_location_information.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2082 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/lnk_network_share_information.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3914 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_io_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23325 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_distributed_link_tracker_properties.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1511 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libfwps.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2010 2023-02-04 15:53:39.000000 liblnk-20230205/liblnk/liblnk_strings_data_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3104 2023-02-05 06:49:23.000000 liblnk-20230205/liblnk/liblnk_distributed_link_tracking_data_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_distributed_link_tracking_data_block.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   172569 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_file.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libfguid.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1840 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_io_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/lnk_volume_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15324 2023-02-05 07:37:28.000000 liblnk-20230205/liblnk/liblnk_file.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_file_header.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7870 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_known_folder_location.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1947 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_link_target_identifier.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1079 2023-02-05 14:13:06.000000 liblnk-20230205/liblnk/liblnk.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36757 2023-02-05 14:12:55.000000 liblnk-20230205/liblnk/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2218 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/lnk_location_information.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_notify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_support.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_notify.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2256 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/lnk_file_header.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7263 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_special_folder_location.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    21242 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_debug.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/liblnk_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6214 2023-02-05 14:13:06.000000 liblnk-20230205/liblnk/liblnk_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2023-02-04 10:14:36.000000 liblnk-20230205/liblnk/liblnk_libcdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3775 2023-02-04 09:58:09.000000 liblnk-20230205/liblnk/lnk_data_blocks.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/pylnk-python2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2044 2023-02-04 16:24:07.000000 liblnk-20230205/pylnk-python2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54771 2023-02-05 14:12:56.000000 liblnk-20230205/pylnk-python2/Makefile.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-02-05 14:12:56.000000 liblnk-20230205/test-driver
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1690975 2023-02-05 14:12:53.000000 liblnk-20230205/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53585 2023-02-05 14:12:56.000000 liblnk-20230205/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-02-05 14:12:42.000000 liblnk-20230205/libuna/libuna_codepage_iso_8859_16.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:07.000000 liblnk-20230205/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16822 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_entry_extension_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9231 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0014_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2305 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_entry_extension_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0013_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1744 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_control_panel_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6567 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0025_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0001_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_root_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_delegate_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_libfole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1770 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_root_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_mtp_volume_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6191 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0006_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_users_property_view_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3716 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15176 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8865 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_volume_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_shell_folder_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3266 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_control_panel_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef000a_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5972 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0003_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7247 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_delegate_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_entry_extension.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_network_location_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2421 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_item_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11686 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_compressed_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0000_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0014_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5954 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0013_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_game_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0019_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13984 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_cdburn_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10520 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_unknown_0x74_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_uri_sub_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14432 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10190 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_shell_folder_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11581 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0025_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1609 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_uri_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_known_folder_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_unknown_0x74_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5435 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0005_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3432 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_network_location.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17745 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_mtp_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_game_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16884 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_mtp_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5811 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_root_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14083 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_uri_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11244 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_users_property_view_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3769 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_compressed_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_control_panel_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef000a_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3098 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_root_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5780 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_control_panel_category_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2625 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48264 2023-02-05 14:12:55.000000 liblnk-20230205/libfwsi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6748 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0000_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0001_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5584 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_control_panel_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12649 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_network_location_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0003_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_cdburn_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23730 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0005_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_uri_sub_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_control_panel_cpl_file_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2792 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_known_folder_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_control_panel_category_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_control_panel_cpl_file_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12685 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3429 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25658 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_entry_extension.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6205 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0019_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0006_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24416 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_network_location.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2117 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_file_entry_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_mtp_file_entry_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40951 2023-02-05 14:12:39.000000 liblnk-20230205/libfwsi/libfwsi_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42189 2023-02-05 14:12:55.000000 liblnk-20230205/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-02-04 10:34:18.000000 liblnk-20230205/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/m4/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-09-09 04:52:22.000000 liblnk-20230205/m4/libuna.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7867 2023-01-30 06:11:21.000000 liblnk-20230205/m4/libfwps.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-13 02:34:46.000000 liblnk-20230205/m4/gettext.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-07-14 05:14:28.000000 liblnk-20230205/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-13 02:34:46.000000 liblnk-20230205/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-02-05 14:12:48.000000 liblnk-20230205/m4/ltoptions.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-13 02:34:46.000000 liblnk-20230205/m4/lib-ld.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-13 02:34:46.000000 liblnk-20230205/m4/lib-link.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-11-14 13:23:54.000000 liblnk-20230205/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-02-05 14:12:48.000000 liblnk-20230205/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-13 02:34:46.000000 liblnk-20230205/m4/nls.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libclocale.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-13 02:34:46.000000 liblnk-20230205/m4/host-cpu-c-abi.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-02-05 14:12:48.000000 liblnk-20230205/m4/ltversion.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-01-18 05:34:57.000000 liblnk-20230205/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-13 02:34:46.000000 liblnk-20230205/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-02-05 14:12:48.000000 liblnk-20230205/m4/lt~obsolete.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-13 02:34:46.000000 liblnk-20230205/m4/po.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2016-03-27 06:27:18.000000 liblnk-20230205/m4/pthread.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2018-11-20 06:29:06.000000 liblnk-20230205/m4/common.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libcerror.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-13 02:34:46.000000 liblnk-20230205/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-02-05 14:12:48.000000 liblnk-20230205/m4/ltsugar.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libcsplit.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libfole.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-13 02:34:46.000000 liblnk-20230205/m4/intlmacosx.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-08-08 20:05:58.000000 liblnk-20230205/m4/types.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4850 2019-07-17 07:52:28.000000 liblnk-20230205/m4/libfwsi.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2020-11-29 10:24:48.000000 liblnk-20230205/m4/libbfio.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-02-04 09:58:05.000000 liblnk-20230205/COPYING.LESSER
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29408 2023-02-05 14:12:55.000000 liblnk-20230205/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-02-05 14:12:24.000000 liblnk-20230205/libcerror/libcerror_system.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29895 2023-02-05 14:12:55.000000 liblnk-20230205/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-02-05 14:12:29.000000 liblnk-20230205/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-02-05 14:12:48.000000 liblnk-20230205/ltmain.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-02-05 14:12:55.000000 liblnk-20230205/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-13 02:34:46.000000 liblnk-20230205/config.rpath
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-02-05 14:12:56.000000 liblnk-20230205/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:08.000000 liblnk-20230205/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-13 02:34:46.000000 liblnk-20230205/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-13 02:34:46.000000 liblnk-20230205/po/Rules-quot
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       59 2010-08-02 11:55:48.000000 liblnk-20230205/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-13 02:34:46.000000 liblnk-20230205/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2010-12-28 20:13:01.000000 liblnk-20230205/po/Makevars.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-08 08:32:51.000000 liblnk-20230205/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-13 02:34:46.000000 liblnk-20230205/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2010-08-02 11:55:48.000000 liblnk-20230205/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2023-02-05 14:13:06.000000 liblnk-20230205/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-13 02:34:46.000000 liblnk-20230205/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-13 02:34:46.000000 liblnk-20230205/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2010-08-02 11:55:48.000000 liblnk-20230205/po/boldquot.sed
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32467 2023-02-05 14:12:55.000000 liblnk-20230205/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-02-05 14:12:23.000000 liblnk-20230205/libcdata/libcdata_btree.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2023-02-04 09:58:05.000000 liblnk-20230205/acinclude.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-02-05 16:45:06.000000 liblnk-20230205/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30841 2023-02-05 14:12:55.000000 liblnk-20230205/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-02-05 14:12:31.000000 liblnk-20230205/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7677 2023-02-05 13:16:06.000000 liblnk-20230205/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2023-02-05 16:45:09.588361 liblnk-20230205/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:31.000000 liblnk-20230716/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5115 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_format_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_format_class_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_property_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1142 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_libfole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31561 2023-07-16 06:36:51.000000 liblnk-20230716/libfwps/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60078 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-16 06:36:35.000000 liblnk-20230716/libfwps/libfwps_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:29.000000 liblnk-20230716/common/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-07-16 05:57:45.000000 liblnk-20230716/common/config_msc.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-07-16 05:57:45.000000 liblnk-20230716/common/byte_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-07-16 05:57:45.000000 liblnk-20230716/common/common.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-07-16 05:57:45.000000 liblnk-20230716/common/system_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-07-16 05:57:42.000000 liblnk-20230716/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2023-07-16 06:37:02.000000 liblnk-20230716/common/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-07-16 05:57:45.000000 liblnk-20230716/common/types.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2023-07-16 05:57:45.000000 liblnk-20230716/common/config_winapi.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-07-16 05:57:45.000000 liblnk-20230716/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16814 2023-07-16 06:37:02.000000 liblnk-20230716/common/config.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-07-16 05:57:45.000000 liblnk-20230716/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25063 2023-07-16 06:36:51.000000 liblnk-20230716/common/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-07-16 05:57:45.000000 liblnk-20230716/common/file_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-07-16 05:57:45.000000 liblnk-20230716/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15873 2023-07-16 06:36:50.000000 liblnk-20230716/common/config.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-07-16 05:57:45.000000 liblnk-20230716/common/wide_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:31.000000 liblnk-20230716/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      630 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29386 2023-07-16 06:36:51.000000 liblnk-20230716/libfole/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2023-07-16 06:36:34.000000 liblnk-20230716/libfole/libfole_types.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:31.000000 liblnk-20230716/pylnk/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2420 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_data_blocks.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6747 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_drive_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_strings_data_block.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1586 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_data_flags.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10926 2023-07-16 05:58:36.000000 liblnk-20230716/pylnk/pylnk_data_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6547 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_file.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_error.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_datetime.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10206 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_file_attribute_flags.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-07-12 03:50:27.000000 liblnk-20230716/pylnk/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_drive_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    87923 2023-07-16 05:58:36.000000 liblnk-20230716/pylnk/pylnk_file.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8011 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_string.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2262 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_distributed_link_tracking_data_block.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13812 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_distributed_link_tracking_data_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1352 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9307 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_data_blocks.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_liblnk.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11473 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_data_flags.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_file_attribute_flags.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1165 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_guid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56200 2023-07-16 06:36:52.000000 liblnk-20230716/pylnk/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8443 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_strings_data_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17182 2023-07-16 05:58:36.000000 liblnk-20230716/pylnk/pylnk.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_file_object_io_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3218 2023-07-16 05:57:46.000000 liblnk-20230716/pylnk/pylnk_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2842 2023-07-16 05:58:36.000000 liblnk-20230716/pylnk/pylnk_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2131 2023-07-16 05:58:36.000000 liblnk-20230716/pylnk/pylnk_data_block.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:31.000000 liblnk-20230716/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29463 2023-07-16 06:36:51.000000 liblnk-20230716/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-07-16 06:36:33.000000 liblnk-20230716/libfguid/libfguid_extern.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5546 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9663 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_distributed_link_tracker_properties.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14741 2023-07-16 05:58:36.000000 liblnk-20230716/tests/pylnk_test_file.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3964 2023-07-16 05:58:36.000000 liblnk-20230716/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125663 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_file.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_liblnk.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19470 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_data_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_unused.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3420 2023-07-16 05:58:36.000000 liblnk-20230716/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7692 2023-07-16 05:58:36.000000 liblnk-20230716/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15540 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_file_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7856 2023-07-16 05:57:46.000000 liblnk-20230716/tests/lnk_test_io_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_memory.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13235 2023-07-16 05:57:46.000000 liblnk-20230716/tests/lnk_test_functions.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2023-07-16 05:57:46.000000 liblnk-20230716/tests/lnk_test_getopt.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14071 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25876 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_data_string.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     2156 2023-07-16 05:57:46.000000 liblnk-20230716/tests/test_lnkinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13532 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_special_folder_location.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7191 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_tools_path_string.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_macros.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2023-07-16 05:57:46.000000 liblnk-20230716/tests/lnk_test_libbfio.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3808 2023-07-16 05:58:36.000000 liblnk-20230716/tests/test_tools.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2023-07-16 05:57:46.000000 liblnk-20230716/tests/lnk_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3236 2023-07-16 05:58:36.000000 liblnk-20230716/tests/pylnk_test_support.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-07-16 05:57:46.000000 liblnk-20230716/tests/test_manpage.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_tools_output.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14125 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_known_folder_location.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-07-16 05:57:46.000000 liblnk-20230716/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8456 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_link_target_identifier.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2023-07-16 05:57:46.000000 liblnk-20230716/tests/lnk_test_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2023-07-16 05:57:46.000000 liblnk-20230716/tests/lnk_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66697 2023-07-16 06:36:52.000000 liblnk-20230716/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8362 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_location_information.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_tools_signal.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_notify.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-07-16 05:58:36.000000 liblnk-20230716/tests/lnk_test_libcpath.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-07-16 05:57:47.000000 liblnk-20230716/tests/lnk_test_libclocale.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30019 2023-07-16 06:36:51.000000 liblnk-20230716/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-07-16 06:36:24.000000 liblnk-20230716/libclocale/libclocale_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-07-16 06:36:51.000000 liblnk-20230716/missing
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      734 2023-07-16 05:57:42.000000 liblnk-20230716/liblnk.pc.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3571 2022-04-28 04:23:51.000000 liblnk-20230716/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56019 2023-07-16 06:36:48.000000 liblnk-20230716/aclocal.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33525 2023-07-16 06:36:51.000000 liblnk-20230716/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-07-16 06:36:18.000000 liblnk-20230716/libbfio/libbfio_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-07-16 05:57:42.000000 liblnk-20230716/COPYING
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      399 2023-07-16 05:57:42.000000 liblnk-20230716/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:29.000000 liblnk-20230716/include/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      464 2023-07-16 05:57:42.000000 liblnk-20230716/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:29.000000 liblnk-20230716/include/liblnk/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4928 2023-07-16 05:57:45.000000 liblnk-20230716/include/liblnk/definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-16 05:57:45.000000 liblnk-20230716/include/liblnk/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4831 2023-07-16 06:37:02.000000 liblnk-20230716/include/liblnk/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2023-07-16 05:57:45.000000 liblnk-20230716/include/liblnk/features.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4962 2023-07-16 05:57:45.000000 liblnk-20230716/include/liblnk/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2023-07-16 06:37:02.000000 liblnk-20230716/include/liblnk/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4926 2023-07-16 06:37:02.000000 liblnk-20230716/include/liblnk/definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2023-07-16 05:57:45.000000 liblnk-20230716/include/liblnk/codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2023-07-16 05:57:45.000000 liblnk-20230716/include/liblnk/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28026 2023-07-16 06:36:51.000000 liblnk-20230716/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40961 2023-07-16 06:37:02.000000 liblnk-20230716/include/liblnk.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40961 2023-07-16 05:57:45.000000 liblnk-20230716/include/liblnk.h.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-07-16 06:36:51.000000 liblnk-20230716/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-07-16 06:36:51.000000 liblnk-20230716/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:29.000000 liblnk-20230716/dpkg/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/liblnk.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      119 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/changelog.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       27 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/liblnk-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2023-07-16 06:37:02.000000 liblnk-20230716/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2023-07-16 05:57:47.000000 liblnk-20230716/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/liblnk-python3.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:29.000000 liblnk-20230716/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/source/format
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      754 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/rules
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/liblnk-dev.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2040 2023-07-16 05:57:42.000000 liblnk-20230716/dpkg/control
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:31.000000 liblnk-20230716/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32634 2023-07-16 06:36:51.000000 liblnk-20230716/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2023-07-16 06:36:31.000000 liblnk-20230716/libfdatetime/libfdatetime_filetime.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30783 2023-07-16 06:36:51.000000 liblnk-20230716/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-07-16 06:36:22.000000 liblnk-20230716/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2303 2023-07-16 06:37:02.000000 liblnk-20230716/liblnk.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32873 2023-07-16 06:36:51.000000 liblnk-20230716/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-07-16 06:36:30.000000 liblnk-20230716/libcthreads/libcthreads_queue.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       90 2023-07-16 05:57:45.000000 liblnk-20230716/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:31.000000 liblnk-20230716/lnktools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    75915 2023-07-16 05:58:36.000000 liblnk-20230716/lnktools/info_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      965 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_liblnk.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libfdatetime.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2521 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/shell_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/property_store.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1518 2023-07-10 04:18:02.000000 liblnk-20230716/lnktools/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_getopt.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libcnotify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1708 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1517 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libfwps.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29927 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/property_store.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    40269 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/shell_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8698 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/path_string.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1283 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/path_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4140 2023-07-16 05:58:36.000000 liblnk-20230716/lnktools/info_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4143 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32309 2023-07-16 06:36:51.000000 liblnk-20230716/lnktools/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_signal.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6925 2023-07-16 05:58:36.000000 liblnk-20230716/lnktools/lnkinfo.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5659 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_signal.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2023-07-16 05:57:46.000000 liblnk-20230716/lnktools/lnktools_getopt.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/pylnk-python3/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2095 2023-07-16 05:57:44.000000 liblnk-20230716/pylnk-python3/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56182 2023-07-16 06:36:52.000000 liblnk-20230716/pylnk-python3/Makefile.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-07-16 06:36:51.000000 liblnk-20230716/config.sub
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30061 2023-07-16 06:36:51.000000 liblnk-20230716/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-07-16 06:36:27.000000 liblnk-20230716/libcpath/libcpath_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      154 2010-06-19 10:23:30.000000 liblnk-20230716/manuals/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4351 2023-07-16 05:57:47.000000 liblnk-20230716/manuals/lnkinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13616 2023-07-16 05:59:15.000000 liblnk-20230716/manuals/liblnk.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27017 2023-07-16 06:36:51.000000 liblnk-20230716/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-13 02:34:46.000000 liblnk-20230716/ABOUT-NLS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6294 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libfwps/libfwps.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_special_folder_location/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5909 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_special_folder_location/lnk_test_special_folder_location.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libfole/libfole.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/pylnk/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8051 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/pylnk/pylnk.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6508 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_support/lnk_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_location_information/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5900 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_location_information/lnk_test_location_information.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6420 2023-07-16 05:58:36.000000 liblnk-20230716/msvscpp/lnk_test_file/lnk_test_file.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1643 2023-07-16 05:58:36.000000 liblnk-20230716/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5803 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_tools_output/lnk_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_link_target_identifier/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5906 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_link_target_identifier/lnk_test_link_target_identifier.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_data_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6117 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_data_string/lnk_test_data_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5700 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_notify/lnk_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5803 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_tools_signal/lnk_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5615 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_error/lnk_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_tools_path_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5891 2023-07-16 05:58:36.000000 liblnk-20230716/msvscpp/lnk_test_tools_path_string/lnk_test_tools_path_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libcpath/libcpath.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33478 2023-07-16 05:58:36.000000 liblnk-20230716/msvscpp/liblnk.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_known_folder_location/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5903 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_known_folder_location/lnk_test_known_folder_location.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/liblnk/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9740 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/liblnk/liblnk.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libuna/libuna.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13549 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libfwsi/libfwsi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_distributed_link_tracker_properties/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5945 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_distributed_link_tracker_properties/lnk_test_distributed_link_tracker_properties.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_file_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6117 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_file_header/lnk_test_file_header.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23662 2023-07-16 06:36:51.000000 liblnk-20230716/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5867 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnk_test_io_handle/lnk_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_data_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6114 2023-07-16 05:58:36.000000 liblnk-20230716/msvscpp/lnk_test_data_block/lnk_test_data_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnkinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7404 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/lnkinfo/lnkinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/lnk_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6442 2023-07-16 05:58:36.000000 liblnk-20230716/msvscpp/lnk_test_tools_info_handle/lnk_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2023-07-16 05:58:12.000000 liblnk-20230716/msvscpp/libcsplit/libcsplit.vcproj
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3237 2023-07-16 05:57:42.000000 liblnk-20230716/liblnk.spec.in
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-07-16 05:58:12.000000 liblnk-20230716/setup.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-07-16 06:36:51.000000 liblnk-20230716/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 05:57:42.000000 liblnk-20230716/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/ossfuzz/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2023-07-16 05:57:45.000000 liblnk-20230716/ossfuzz/file_fuzzer.cc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      884 2020-07-14 05:11:41.000000 liblnk-20230716/ossfuzz/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      962 2023-07-16 05:57:45.000000 liblnk-20230716/ossfuzz/ossfuzz_liblnk.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32242 2023-07-16 06:36:51.000000 liblnk-20230716/ossfuzz/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-07-16 05:57:45.000000 liblnk-20230716/ossfuzz/ossfuzz_libbfio.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:31.000000 liblnk-20230716/liblnk/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_extern.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17708 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_data_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1569 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1081 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk.rc.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2098 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_special_folder_location.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3627 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_data_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4484 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_distributed_link_tracker_properties.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2599 2023-02-04 08:33:09.000000 liblnk-20230716/liblnk/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11471 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_file_header.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6216 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    52878 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_location_information.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9315 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_support.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2071 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_known_folder_location.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    29187 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_data_string.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3429 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_data_block.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libfwsi.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9265 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_link_target_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25486 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_strings_data_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2558 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_debug.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2891 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_location_information.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2082 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/lnk_network_share_information.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3914 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_io_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23325 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_distributed_link_tracker_properties.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1511 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libfwps.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_strings_data_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3104 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_distributed_link_tracking_data_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_distributed_link_tracking_data_block.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   175933 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_file.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libfguid.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1840 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_io_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/lnk_volume_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15324 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_file.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2429 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_file_header.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7870 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_known_folder_location.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1947 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_link_target_identifier.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1079 2023-07-16 06:37:02.000000 liblnk-20230716/liblnk/liblnk.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36757 2023-07-16 06:36:51.000000 liblnk-20230716/liblnk/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2218 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/lnk_location_information.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_notify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1986 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_support.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_notify.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2256 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/lnk_file_header.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7263 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_special_folder_location.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    21242 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_debug.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6214 2023-07-16 06:37:02.000000 liblnk-20230716/liblnk/liblnk_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/liblnk_libcdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3775 2023-07-16 05:57:45.000000 liblnk-20230716/liblnk/lnk_data_blocks.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/pylnk-python2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2095 2023-07-16 05:57:44.000000 liblnk-20230716/pylnk-python2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56182 2023-07-16 06:36:52.000000 liblnk-20230716/pylnk-python2/Makefile.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-07-16 06:36:52.000000 liblnk-20230716/test-driver
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1761565 2023-07-16 06:36:49.000000 liblnk-20230716/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53585 2023-07-16 06:36:51.000000 liblnk-20230716/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-07-16 06:36:39.000000 liblnk-20230716/libuna/libuna_codepage_iso_8859_16.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:31.000000 liblnk-20230716/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16822 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_entry_extension_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9231 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0014_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2305 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_entry_extension_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0013_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1744 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_control_panel_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6567 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0025_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0001_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_root_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_delegate_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_libfole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1770 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_root_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_mtp_volume_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6191 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0006_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1865 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_users_property_view_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3716 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15176 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8865 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_volume_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_shell_folder_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3266 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_control_panel_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef000a_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5972 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0003_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7247 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_delegate_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_entry_extension.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_network_location_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2421 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_item_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11686 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_compressed_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0000_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0014_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5954 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0013_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_game_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0019_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14734 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_cdburn_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10520 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_unknown_0x74_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_uri_sub_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14432 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10190 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_shell_folder_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11581 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0025_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1609 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_uri_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6183 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_known_folder_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_unknown_0x74_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5435 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0005_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3432 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_network_location.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17745 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_mtp_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_game_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16884 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_mtp_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5811 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_root_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14083 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_uri_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11244 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_users_property_view_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3769 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_compressed_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_control_panel_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef000a_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3098 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_root_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5780 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_control_panel_category_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2625 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48264 2023-07-16 06:36:51.000000 liblnk-20230716/libfwsi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6748 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0000_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0001_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5584 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_control_panel_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12649 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_network_location_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0003_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_cdburn_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23730 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0005_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_uri_sub_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_control_panel_cpl_file_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2792 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_known_folder_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_control_panel_category_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_control_panel_cpl_file_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12685 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3429 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26408 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_entry_extension.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6205 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0019_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0006_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24416 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_network_location.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2117 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_file_entry_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_mtp_file_entry_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40951 2023-07-16 06:36:37.000000 liblnk-20230716/libfwsi/libfwsi_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42189 2023-07-16 06:36:51.000000 liblnk-20230716/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-07-10 18:36:28.000000 liblnk-20230716/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:29.000000 liblnk-20230716/m4/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-07-10 03:54:36.000000 liblnk-20230716/m4/libuna.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8519 2023-07-11 15:49:48.000000 liblnk-20230716/m4/libfwps.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-13 02:34:46.000000 liblnk-20230716/m4/gettext.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2020-07-14 05:14:28.000000 liblnk-20230716/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-13 02:34:46.000000 liblnk-20230716/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-07-16 06:36:44.000000 liblnk-20230716/m4/ltoptions.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-13 02:34:46.000000 liblnk-20230716/m4/lib-ld.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-13 02:34:46.000000 liblnk-20230716/m4/lib-link.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-11-14 13:23:54.000000 liblnk-20230716/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-07-16 06:36:44.000000 liblnk-20230716/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-13 02:34:46.000000 liblnk-20230716/m4/nls.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libclocale.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2022-07-13 02:34:46.000000 liblnk-20230716/m4/host-cpu-c-abi.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-07-16 06:36:45.000000 liblnk-20230716/m4/ltversion.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-01-18 05:34:57.000000 liblnk-20230716/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-13 02:34:46.000000 liblnk-20230716/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-07-16 06:36:45.000000 liblnk-20230716/m4/lt~obsolete.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-13 02:34:46.000000 liblnk-20230716/m4/po.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2016-03-27 06:27:18.000000 liblnk-20230716/m4/pthread.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2018-11-20 06:29:06.000000 liblnk-20230716/m4/common.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libcerror.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-13 02:34:46.000000 liblnk-20230716/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-07-16 06:36:45.000000 liblnk-20230716/m4/ltsugar.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libcsplit.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libfole.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-13 02:34:46.000000 liblnk-20230716/m4/intlmacosx.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2018-08-08 20:05:58.000000 liblnk-20230716/m4/types.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4850 2019-07-17 07:52:28.000000 liblnk-20230716/m4/libfwsi.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2020-11-29 10:24:48.000000 liblnk-20230716/m4/libbfio.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-07-16 05:57:42.000000 liblnk-20230716/COPYING.LESSER
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:29.000000 liblnk-20230716/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29408 2023-07-16 06:36:51.000000 liblnk-20230716/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-07-16 06:36:21.000000 liblnk-20230716/libcerror/libcerror_system.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29895 2023-07-16 06:36:51.000000 liblnk-20230716/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-07-16 06:36:25.000000 liblnk-20230716/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-07-16 06:36:44.000000 liblnk-20230716/ltmain.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-07-16 06:36:51.000000 liblnk-20230716/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-13 02:34:46.000000 liblnk-20230716/config.rpath
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-07-16 06:36:52.000000 liblnk-20230716/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:32.000000 liblnk-20230716/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-13 02:34:46.000000 liblnk-20230716/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-13 02:34:46.000000 liblnk-20230716/po/Rules-quot
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       59 2010-08-02 11:55:48.000000 liblnk-20230716/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-13 02:34:46.000000 liblnk-20230716/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2010-12-28 20:13:01.000000 liblnk-20230716/po/Makevars.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       50 2016-11-08 08:32:51.000000 liblnk-20230716/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-13 02:34:46.000000 liblnk-20230716/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2010-08-02 11:55:48.000000 liblnk-20230716/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2023-07-16 06:37:02.000000 liblnk-20230716/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-13 02:34:46.000000 liblnk-20230716/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-13 02:34:46.000000 liblnk-20230716/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2010-08-02 11:55:48.000000 liblnk-20230716/po/boldquot.sed
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32467 2023-07-16 06:36:51.000000 liblnk-20230716/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-07-16 06:36:19.000000 liblnk-20230716/libcdata/libcdata_btree.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1186 2023-07-16 05:57:42.000000 liblnk-20230716/acinclude.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-07-16 06:58:30.000000 liblnk-20230716/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30841 2023-07-16 06:36:51.000000 liblnk-20230716/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-07-16 06:36:29.000000 liblnk-20230716/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7677 2023-07-16 05:57:42.000000 liblnk-20230716/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2023-07-16 06:58:33.569212 liblnk-20230716/PKG-INFO
```

### Comparing `liblnk-20230205/libfwps/libfwps_record.h` & `liblnk-20230716/libfwps/libfwps_record.h`

 * *Files 15% similar despite different names*

```diff
@@ -164,14 +164,40 @@
 int libfwps_record_get_data_as_utf16_string(
      libfwps_record_t *record,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error );
 
 LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf8_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf8_path_string(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf16_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
+int libfwps_record_get_data_as_utf16_path_string(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error );
+
+LIBFWPS_EXTERN \
 int libfwps_record_get_data_as_guid(
      libfwps_record_t *record,
      uint8_t *guid_data,
      size_t guid_data_size,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
```

### Comparing `liblnk-20230205/libfwps/libfwps_format_class_identifier.c` & `liblnk-20230716/libfwps/libfwps_format_class_identifier.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_libcdata.h` & `liblnk-20230716/libfwps/libfwps_libcdata.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_extern.h` & `liblnk-20230716/libfwps/libfwps_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_store.c` & `liblnk-20230716/libfwps/libfwps_store.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_codepage.h` & `liblnk-20230716/libfwps/libfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_format_class_identifier.h` & `liblnk-20230716/libfwps/libfwps_format_class_identifier.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_property_identifier.h` & `liblnk-20230716/libfwps/libfwps_property_identifier.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_libcnotify.h` & `liblnk-20230716/libfwps/libfwps_libcnotify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/Makefile.am` & `liblnk-20230716/libfwps/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_libfguid.h` & `liblnk-20230716/libfwps/libfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_set.c` & `liblnk-20230716/libfwps/libfwps_set.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_definitions.h` & `liblnk-20230716/libfwps/libfwps_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwps/definitions.h> are copied here
  * for local use of libfwps
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWPS_VERSION					20230202
+#define LIBFWPS_VERSION					20230711
 
 /* The version string
  */
-#define LIBFWPS_VERSION_STRING				"20230202"
+#define LIBFWPS_VERSION_STRING				"20230711"
 
 /* The byte order definitions
  */
 #define LIBFWPS_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWPS_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The value types
```

### Comparing `liblnk-20230205/libfwps/libfwps_libuna.h` & `liblnk-20230716/libfwps/libfwps_libuna.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_libfole.h` & `liblnk-20230716/libfwps/libfwps_libfole.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_store.h` & `liblnk-20230716/libfwps/libfwps_store.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_error.c` & `liblnk-20230716/libfwps/libfwps_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_support.c` & `liblnk-20230716/libfwps/libfwps_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/Makefile.in` & `liblnk-20230716/libfwps/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_libcerror.h` & `liblnk-20230716/libfwps/libfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_property_identifier.c` & `liblnk-20230716/libfwps/libfwps_property_identifier.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_types.h` & `liblnk-20230716/libfwps/libfwps_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_record.c` & `liblnk-20230716/libfwps/libfwps_record.c`

 * *Files 14% similar despite different names*

```diff
@@ -1275,14 +1275,15 @@
 
 		*value_floating_point = value_double.floating_point;
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the data formatted as an UTF-8 string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
  * The returned size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwps_record_get_data_as_utf8_string_size(
      libfwps_record_t *record,
      size_t *utf8_string_size,
      libcerror_error_t **error )
@@ -1525,14 +1526,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the data formatted as an UTF-16 string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
  * The returned size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwps_record_get_data_as_utf16_string_size(
      libfwps_record_t *record,
      size_t *utf16_string_size,
      libcerror_error_t **error )
@@ -1733,14 +1735,520 @@
 		          error );
 	}
 	/* Codepage 65000 represents UTF-7
 	 */
 	else if( internal_record->ascii_codepage == 65000 )
 	{
 		result = libuna_utf16_string_copy_from_utf7_stream(
+		          utf16_string,
+		          utf16_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          error );
+	}
+	/* Codepage 65001 represents UTF-8
+	 */
+	else if( internal_record->ascii_codepage == 65001 )
+	{
+		result = libuna_utf16_string_copy_from_utf8_stream(
+		          utf16_string,
+		          utf16_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          error );
+	}
+	else
+	{
+		result = libuna_utf16_string_copy_from_byte_stream(
+		          utf16_string,
+		          utf16_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          internal_record->ascii_codepage,
+		          error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy value data to UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the data formatted as an UTF-8 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_utf8_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf8_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_utf8_path_string_size";
+	uint8_t is_ascii_string                    = 0;
+	int result                                 = 0;
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string size.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_record->value_data == NULL )
+	 || ( internal_record->value_data_size == 0 ) )
+	{
+		*utf8_string_size = 0;
+
+		return( 1 );
+	}
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	{
+		is_ascii_string = 1;
+	}
+	/* String is in UTF-16 little-endian
+	 */
+	if( is_ascii_string == 0 )
+	{
+		result = libuna_utf8_string_size_from_utf16_stream(
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+		          utf8_string_size,
+		          error );
+	}
+	/* Codepage 65000 represents UTF-7
+	 */
+	else if( internal_record->ascii_codepage == 65000 )
+	{
+		result = libuna_utf8_string_size_from_utf7_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  utf8_string_size,
+			  error );
+	}
+	/* Codepage 65001 represents UTF-8
+	 */
+	else if( internal_record->ascii_codepage == 65001 )
+	{
+		result = libuna_utf8_string_size_from_utf8_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  utf8_string_size,
+			  error );
+	}
+	else
+	{
+		result = libuna_utf8_string_size_from_byte_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  internal_record->ascii_codepage,
+			  utf8_string_size,
+			  error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to determine size of value data as UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the data formatted as an UTF-8 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_utf8_path_string(
+     libfwps_record_t *record,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_utf8_path_string";
+	uint8_t is_ascii_string                    = 0;
+	int result                                 = 0;
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( utf8_string_size == 0 )
+	 || ( utf8_string_size > (size_t) SSIZE_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid UTF-8 string size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_record->value_data == NULL )
+	 || ( internal_record->value_data_size == 0 ) )
+	{
+		utf8_string[ 0 ] = 0;
+
+		return( 1 );
+	}
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	{
+		is_ascii_string = 1;
+	}
+	/* String is in UTF-16 little-endian
+	 */
+	if( is_ascii_string == 0 )
+	{
+		result = libuna_utf8_string_copy_from_utf16_stream(
+		          utf8_string,
+		          utf8_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+		          error );
+	}
+	/* Codepage 65000 represents UTF-7
+	 */
+	else if( internal_record->ascii_codepage == 65000 )
+	{
+		result = libuna_utf8_string_copy_from_utf7_stream(
+		          utf8_string,
+		          utf8_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          error );
+	}
+	/* Codepage 65001 represents UTF-8
+	 */
+	else if( internal_record->ascii_codepage == 65001 )
+	{
+		result = libuna_utf8_string_copy_from_utf8_stream(
+		          utf8_string,
+		          utf8_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          error );
+	}
+	else
+	{
+		result = libuna_utf8_string_copy_from_byte_stream(
+		          utf8_string,
+		          utf8_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          internal_record->ascii_codepage,
+		          error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy value data to UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the data formatted as an UTF-16 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The returned size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_utf16_path_string_size(
+     libfwps_record_t *record,
+     size_t *utf16_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_utf16_path_string_size";
+	uint8_t is_ascii_string                    = 0;
+	int result                                 = 0;
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf16_string_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-16 string size.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_record->value_data == NULL )
+	 || ( internal_record->value_data_size == 0 ) )
+	{
+		*utf16_string_size = 0;
+
+		return( 1 );
+	}
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	{
+		is_ascii_string = 1;
+	}
+	/* String is in UTF-16 little-endian
+	 */
+	if( is_ascii_string == 0 )
+	{
+		result = libuna_utf16_string_size_from_utf16_stream(
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+		          utf16_string_size,
+		          error );
+	}
+	/* Codepage 65000 represents UTF-7
+	 */
+	else if( internal_record->ascii_codepage == 65000 )
+	{
+		result = libuna_utf16_string_size_from_utf7_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  utf16_string_size,
+			  error );
+	}
+	/* Codepage 65001 represents UTF-8
+	 */
+	else if( internal_record->ascii_codepage == 65001 )
+	{
+		result = libuna_utf16_string_size_from_utf8_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  utf16_string_size,
+			  error );
+	}
+	else
+	{
+		result = libuna_utf16_string_size_from_byte_stream(
+			  internal_record->value_data,
+			  internal_record->value_data_size,
+			  internal_record->ascii_codepage,
+			  utf16_string_size,
+			  error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to determine size of value data as UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the data formatted as an UTF-16 path string
+ * The function uses a codepage if necessary, it uses the codepage set for the library
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int libfwps_record_get_data_as_utf16_path_string(
+     libfwps_record_t *record,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error )
+{
+	libfwps_internal_record_t *internal_record = NULL;
+	static char *function                      = "libfwps_record_get_data_as_utf16_path_string";
+	uint8_t is_ascii_string                    = 0;
+	int result                                 = 0;
+
+	if( record == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid record entry.",
+		 function );
+
+		return( -1 );
+	}
+	internal_record = (libfwps_internal_record_t *) record;
+
+	if( ( internal_record->value_type != LIBFWPS_VALUE_TYPE_BINARY_STRING )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	 && ( internal_record->value_type != LIBFWPS_VALUE_TYPE_STRING_UNICODE ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid record entry - unsupported value type.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf16_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( utf16_string_size == 0 )
+	 || ( utf16_string_size > (size_t) SSIZE_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid UTF-16 string size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_record->value_data == NULL )
+	 || ( internal_record->value_data_size == 0 ) )
+	{
+		utf16_string[ 0 ] = 0;
+
+		return( 1 );
+	}
+	if( internal_record->value_type == LIBFWPS_VALUE_TYPE_STRING_ASCII )
+	{
+		is_ascii_string = 1;
+	}
+	/* String is in UTF-16 little-endian
+	 */
+	if( is_ascii_string == 0 )
+	{
+		result = libuna_utf16_string_copy_from_utf16_stream(
+		          utf16_string,
+		          utf16_string_size,
+		          internal_record->value_data,
+		          internal_record->value_data_size,
+		          LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+		          error );
+	}
+	/* Codepage 65000 represents UTF-7
+	 */
+	else if( internal_record->ascii_codepage == 65000 )
+	{
+		result = libuna_utf16_string_copy_from_utf7_stream(
 		          utf16_string,
 		          utf16_string_size,
 		          internal_record->value_data,
 		          internal_record->value_data_size,
 		          error );
 	}
 	/* Codepage 65001 represents UTF-8
```

### Comparing `liblnk-20230205/libfwps/libfwps_unused.h` & `liblnk-20230716/libfwps/libfwps_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_support.h` & `liblnk-20230716/libfwps/libfwps_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_set.h` & `liblnk-20230716/libfwps/libfwps_set.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwps/libfwps_error.h` & `liblnk-20230716/libfwps/libfwps_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/config_msc.h` & `liblnk-20230716/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/byte_stream.h` & `liblnk-20230716/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/common.h` & `liblnk-20230716/common/common.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/system_string.h` & `liblnk-20230716/common/system_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/types.h` & `liblnk-20230716/common/types.h`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
 #define PRIc_SYSTEM "c"
 #define PRIs_SYSTEM "s"
 
 #endif /* defined( WINAPI ) && ( defined( _UNICODE ) || defined( UNICODE ) ) */
 
 /* Fallback for systems without PRI definitions
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( PRId8 )
 #define PRId8 "d"
 #endif
 
 #if !defined( PRId16 )
 #define PRId16 "d"
 #endif
@@ -212,14 +215,16 @@
 
 #else
 #define PRIx64 "llx"
 
 #endif
 #endif /* !defined( PRIx64 ) */
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Fallback for systems without printf %jd definition
  */
 #if defined( HAVE_PRINTF_JD )
 #define PRIjd	"jd"
 #define PRIji	"ji"
 #define PRIju	"ju"
 #define PRIjx	"jx"
```

### Comparing `liblnk-20230205/common/types.h.in` & `liblnk-20230716/common/types.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
 #define PRIc_SYSTEM "c"
 #define PRIs_SYSTEM "s"
 
 #endif /* defined( WINAPI ) && ( defined( _UNICODE ) || defined( UNICODE ) ) */
 
 /* Fallback for systems without PRI definitions
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( PRId8 )
 #define PRId8 "d"
 #endif
 
 #if !defined( PRId16 )
 #define PRId16 "d"
 #endif
@@ -212,14 +215,16 @@
 
 #else
 #define PRIx64 "llx"
 
 #endif
 #endif /* !defined( PRIx64 ) */
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Fallback for systems without printf %jd definition
  */
 #if defined( HAVE_PRINTF_JD )
 #define PRIjd	"jd"
 #define PRIji	"ji"
 #define PRIju	"ju"
 #define PRIjx	"jx"
```

### Comparing `liblnk-20230205/common/config_winapi.h` & `liblnk-20230716/common/config_winapi.h`

 * *Files 11% similar despite different names*

```diff
@@ -41,23 +41,28 @@
 /* Define the size of the integer for WINAPI
  */
 #if !defined( SIZEOF_INT )
 #define SIZEOF_INT			4
 #endif
 
 /* Define the size of size_t for WINAPI
+ * Do not define when pyconfig.h has been included via python.h
  */
+#if !defined( HAVE_PYCONFIG_H )
+
 #if !defined( SIZEOF_SIZE_T )
 #if __WORDSIZE == 64
 #define SIZEOF_SIZE_T			8
 #else
 #define SIZEOF_SIZE_T			4
 #endif
 #endif
 
+#endif /* !defined( HAVE_PYCONFIG_H ) */
+
 /* Define the size of the wide character for WINAPI
  */
 #if !defined( SIZEOF_WCHAR_T )
 #define SIZEOF_WCHAR_T			2
 #endif
 
 /* Enable the DllMain function
```

### Comparing `liblnk-20230205/common/memory.h` & `liblnk-20230716/common/memory.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/config.h` & `liblnk-20230716/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -523,24 +523,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "liblnk"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "liblnk 20230205"
+#define PACKAGE_STRING "liblnk 20230716"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "liblnk"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20230205"
+#define PACKAGE_VERSION "20230716"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -558,15 +558,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20230205"
+#define VERSION "20230716"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `liblnk-20230205/common/narrow_string.h` & `liblnk-20230716/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/Makefile.in` & `liblnk-20230716/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/file_stream.h` & `liblnk-20230716/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/config_borlandc.h` & `liblnk-20230716/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/config.h.in` & `liblnk-20230716/common/config.h.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/common/wide_string.h` & `liblnk-20230716/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_definitions.h` & `liblnk-20230716/libfole/libfole_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/Makefile.am` & `liblnk-20230716/libfole/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_support.h` & `liblnk-20230716/libfole/libfole_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_extern.h` & `liblnk-20230716/libfole/libfole_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_error.c` & `liblnk-20230716/libfole/libfole_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_libcerror.h` & `liblnk-20230716/libfole/libfole_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_value_type.h` & `liblnk-20230716/libfole/libfole_value_type.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_unused.h` & `liblnk-20230716/libfole/libfole_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_value_type.c` & `liblnk-20230716/libfole/libfole_value_type.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_error.h` & `liblnk-20230716/libfole/libfole_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/Makefile.in` & `liblnk-20230716/libfole/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_support.c` & `liblnk-20230716/libfole/libfole_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfole/libfole_types.h` & `liblnk-20230716/libfole/libfole_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_integer.h` & `liblnk-20230716/pylnk/pylnk_integer.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_data_blocks.h` & `liblnk-20230716/pylnk/pylnk_data_blocks.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_drive_types.c` & `liblnk-20230716/pylnk/pylnk_drive_types.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_strings_data_block.h` & `liblnk-20230716/pylnk/pylnk_strings_data_block.h`

 * *Files 6% similar despite different names*

```diff
@@ -36,13 +36,17 @@
 extern PyMethodDef pylnk_strings_data_block_object_methods[];
 extern PyTypeObject pylnk_strings_data_block_type_object;
 
 PyObject *pylnk_strings_data_block_get_string(
            pylnk_data_block_t *pylnk_data_block,
            PyObject *arguments );
 
+PyObject *pylnk_strings_data_block_get_path_string(
+           pylnk_data_block_t *pylnk_data_block,
+           PyObject *arguments );
+
 #if defined( __cplusplus )
 }
 #endif
 
 #endif /* !defined( _PYLNK_STRINGS_DATA_BLOCK_H ) */
```

### Comparing `liblnk-20230205/pylnk/pylnk_data_flags.h` & `liblnk-20230716/pylnk/pylnk_data_flags.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_data_block.c` & `liblnk-20230716/pylnk/pylnk_data_block.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_file.h` & `liblnk-20230716/pylnk/pylnk_file.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_error.h` & `liblnk-20230716/pylnk/pylnk_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_libclocale.h` & `liblnk-20230716/pylnk/pylnk_libclocale.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_datetime.h` & `liblnk-20230716/pylnk/pylnk_datetime.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_unused.h` & `liblnk-20230716/pylnk/pylnk_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_error.c` & `liblnk-20230716/pylnk/pylnk_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_file_attribute_flags.c` & `liblnk-20230716/pylnk/pylnk_file_attribute_flags.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/Makefile.am` & `liblnk-20230716/pylnk/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 	pylnk_guid.c pylnk_guid.h \
 	pylnk_integer.c pylnk_integer.h \
 	pylnk_libbfio.h \
 	pylnk_libcerror.h \
 	pylnk_libclocale.h \
 	pylnk_libfguid.h \
 	pylnk_liblnk.h \
+	pylnk_libuna.h \
 	pylnk_python.h \
+	pylnk_string.c pylnk_string.h \
 	pylnk_strings_data_block.c pylnk_strings_data_block.h \
 	pylnk_unused.h
 
 pylnk_la_LIBADD = \
 	@LIBCERROR_LIBADD@ \
 	../liblnk/liblnk.la \
 	@LIBCDATA_LIBADD@ \
```

### Comparing `liblnk-20230205/pylnk/pylnk_drive_types.h` & `liblnk-20230716/pylnk/pylnk_drive_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_file.c` & `liblnk-20230716/pylnk/pylnk_file.c`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 #include "pylnk_guid.h"
 #include "pylnk_integer.h"
 #include "pylnk_libbfio.h"
 #include "pylnk_libcerror.h"
 #include "pylnk_libclocale.h"
 #include "pylnk_liblnk.h"
 #include "pylnk_python.h"
+#include "pylnk_string.h"
 #include "pylnk_unused.h"
 
 #if !defined( LIBLNK_HAVE_BFIO )
 
 LIBLNK_EXTERN \
 int liblnk_file_open_file_io_handle(
      liblnk_file_t *file,
@@ -840,25 +841,36 @@
 		return( NULL );
 	}
 	else if( result != 0 )
 	{
 		PyErr_Clear();
 
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+		filename_wide = (wchar_t *) PyUnicode_AsWideCharString(
+		                             string_object,
+		                             NULL );
+#else
 		filename_wide = (wchar_t *) PyUnicode_AsUnicode(
 		                             string_object );
+#endif
 		Py_BEGIN_ALLOW_THREADS
 
 		result = liblnk_file_open_wide(
 		          pylnk_file->file,
 		          filename_wide,
 		          LIBLNK_OPEN_READ,
 		          &error );
 
 		Py_END_ALLOW_THREADS
+
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+		PyMem_Free(
+		 filename_wide );
+#endif
 #else
 		utf8_string_object = PyUnicode_AsUTF8String(
 		                      string_object );
 
 		if( utf8_string_object == NULL )
 		{
 			pylnk_error_fetch_and_raise(
@@ -2346,15 +2358,14 @@
  */
 PyObject *pylnk_file_get_volume_label(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_volume_label";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -2434,15 +2445,15 @@
 	}
 	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
 	 * the end of string character is part of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
+	                 NULL );
 
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
@@ -2468,15 +2479,14 @@
  */
 PyObject *pylnk_file_get_local_path(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_local_path";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -2550,22 +2560,28 @@
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
-	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
-	 * the end of string character is part of the string
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pylnk_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
-
+	                 NULL );
+#endif
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
 
@@ -2590,15 +2606,14 @@
  */
 PyObject *pylnk_file_get_network_path(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_network_path";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -2672,22 +2687,28 @@
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
-	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
-	 * the end of string character is part of the string
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pylnk_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
-
+	                 NULL );
+#endif
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
 
@@ -2712,15 +2733,14 @@
  */
 PyObject *pylnk_file_get_description(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_description";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -2800,15 +2820,15 @@
 	}
 	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
 	 * the end of string character is part of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
+	                 NULL );
 
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
@@ -2834,15 +2854,14 @@
  */
 PyObject *pylnk_file_get_relative_path(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_relative_path";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -2916,22 +2935,28 @@
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
-	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
-	 * the end of string character is part of the string
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pylnk_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
-
+	                 NULL );
+#endif
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
 
@@ -2956,15 +2981,14 @@
  */
 PyObject *pylnk_file_get_working_directory(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_working_directory";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -3038,22 +3062,28 @@
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
-	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
-	 * the end of string character is part of the string
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pylnk_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
-
+	                 NULL );
+#endif
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
 
@@ -3078,15 +3108,14 @@
  */
 PyObject *pylnk_file_get_command_line_arguments(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_command_line_arguments";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -3160,22 +3189,28 @@
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
-	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
-	 * the end of string character is part of the string
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pylnk_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
-
+	                 NULL );
+#endif
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
 
@@ -3200,15 +3235,14 @@
  */
 PyObject *pylnk_file_get_icon_location(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_icon_location";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -3282,22 +3316,28 @@
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
-	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
-	 * the end of string character is part of the string
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pylnk_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
-
+	                 NULL );
+#endif
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
 
@@ -3322,15 +3362,14 @@
  */
 PyObject *pylnk_file_get_environment_variables_location(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_environment_variables_location";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -3404,22 +3443,28 @@
 		 function );
 
 		libcerror_error_free(
 		 &error );
 
 		goto on_error;
 	}
-	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
-	 * the end of string character is part of the string
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+	string_object = pylnk_string_new_from_utf8_rfc2279(
+			 (uint8_t *) utf8_string,
+			 utf8_string_size );
+#else
+	/* Pass the string length to PyUnicode_DecodeUTF8
+	 * otherwise it makes the end of string character is part
+	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
-
+	                 NULL );
+#endif
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
 
@@ -3568,15 +3613,14 @@
  */
 PyObject *pylnk_file_get_machine_identifier(
            pylnk_file_t *pylnk_file,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_file_get_machine_identifier";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -3656,15 +3700,15 @@
 	}
 	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
 	 * the end of string character is part of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
+	                 NULL );
 
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
```

### Comparing `liblnk-20230205/pylnk/pylnk_libbfio.h` & `liblnk-20230716/pylnk/pylnk_libbfio.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk.h` & `liblnk-20230716/pylnk/pylnk.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_datetime.c` & `liblnk-20230716/pylnk/pylnk_datetime.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_python.h` & `liblnk-20230716/pylnk/pylnk_python.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_distributed_link_tracking_data_block.h` & `liblnk-20230716/pylnk/pylnk_distributed_link_tracking_data_block.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_codepage.h` & `liblnk-20230716/pylnk/pylnk_codepage.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_distributed_link_tracking_data_block.c` & `liblnk-20230716/pylnk/pylnk_distributed_link_tracking_data_block.c`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,14 @@
  */
 PyObject *pylnk_distributed_link_tracking_data_block_get_machine_identifier(
            pylnk_data_block_t *pylnk_data_block,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
 	PyObject *string_object  = NULL;
 	libcerror_error_t *error = NULL;
-	const char *errors       = NULL;
 	static char *function    = "pylnk_distributed_link_tracking_data_block_get_machine_identifier";
 	char *utf8_string        = NULL;
 	size_t utf8_string_size  = 0;
 	int result               = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
@@ -301,15 +300,15 @@
 	}
 	/* Pass the string length to PyUnicode_DecodeUTF8 otherwise it makes
 	 * the end of string character is part of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 	                 utf8_string,
 	                 (Py_ssize_t) utf8_string_size - 1,
-	                 errors );
+	                 NULL );
 
 	if( string_object == NULL )
 	{
 		PyErr_Format(
 		 PyExc_IOError,
 		 "%s: unable to convert UTF-8 string into Unicode object.",
 		 function );
```

### Comparing `liblnk-20230205/pylnk/pylnk_libfguid.h` & `liblnk-20230716/pylnk/pylnk_libfguid.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_data_blocks.c` & `liblnk-20230716/pylnk/pylnk_data_blocks.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_liblnk.h` & `liblnk-20230716/pylnk/pylnk_liblnk.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_data_flags.c` & `liblnk-20230716/pylnk/pylnk_data_flags.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_file_object_io_handle.c` & `liblnk-20230716/pylnk/pylnk_file_object_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -574,15 +574,15 @@
 		     safe_buffer,
 		     read_count ) == NULL )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_MEMORY,
 			 LIBCERROR_MEMORY_ERROR_COPY_FAILED,
-			 "%s: unable to data to buffer.",
+			 "%s: unable to copy data to buffer.",
 			 function );
 
 			goto on_error;
 		}
 		Py_DecRef(
 		 method_result );
```

### Comparing `liblnk-20230205/pylnk/pylnk_file_attribute_flags.h` & `liblnk-20230716/pylnk/pylnk_file_attribute_flags.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_guid.h` & `liblnk-20230716/pylnk/pylnk_guid.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_integer.c` & `liblnk-20230716/pylnk/pylnk_integer.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/Makefile.in` & `liblnk-20230716/pylnk/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -154,31 +154,32 @@
 	pylnk_distributed_link_tracking_data_block.h \
 	pylnk_drive_types.c pylnk_drive_types.h pylnk_error.c \
 	pylnk_error.h pylnk_file.c pylnk_file.h \
 	pylnk_file_attribute_flags.c pylnk_file_attribute_flags.h \
 	pylnk_file_object_io_handle.c pylnk_file_object_io_handle.h \
 	pylnk_guid.c pylnk_guid.h pylnk_integer.c pylnk_integer.h \
 	pylnk_libbfio.h pylnk_libcerror.h pylnk_libclocale.h \
-	pylnk_libfguid.h pylnk_liblnk.h pylnk_python.h \
-	pylnk_strings_data_block.c pylnk_strings_data_block.h \
-	pylnk_unused.h
+	pylnk_libfguid.h pylnk_liblnk.h pylnk_libuna.h pylnk_python.h \
+	pylnk_string.c pylnk_string.h pylnk_strings_data_block.c \
+	pylnk_strings_data_block.h pylnk_unused.h
 @HAVE_PYTHON_TRUE@am_pylnk_la_OBJECTS = pylnk_la-pylnk.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_codepage.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_data_block.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_data_blocks.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_data_flags.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_datetime.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_distributed_link_tracking_data_block.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_drive_types.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_error.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_file.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_file_attribute_flags.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_file_object_io_handle.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_guid.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_integer.lo \
+@HAVE_PYTHON_TRUE@	pylnk_la-pylnk_string.lo \
 @HAVE_PYTHON_TRUE@	pylnk_la-pylnk_strings_data_block.lo
 pylnk_la_OBJECTS = $(am_pylnk_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 pylnk_la_LINK = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
@@ -210,14 +211,15 @@
 	./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_error.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_guid.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_integer.Plo \
+	./$(DEPDIR)/pylnk_la-pylnk_string.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
@@ -632,15 +634,17 @@
 @HAVE_PYTHON_TRUE@	pylnk_guid.c pylnk_guid.h \
 @HAVE_PYTHON_TRUE@	pylnk_integer.c pylnk_integer.h \
 @HAVE_PYTHON_TRUE@	pylnk_libbfio.h \
 @HAVE_PYTHON_TRUE@	pylnk_libcerror.h \
 @HAVE_PYTHON_TRUE@	pylnk_libclocale.h \
 @HAVE_PYTHON_TRUE@	pylnk_libfguid.h \
 @HAVE_PYTHON_TRUE@	pylnk_liblnk.h \
+@HAVE_PYTHON_TRUE@	pylnk_libuna.h \
 @HAVE_PYTHON_TRUE@	pylnk_python.h \
+@HAVE_PYTHON_TRUE@	pylnk_string.c pylnk_string.h \
 @HAVE_PYTHON_TRUE@	pylnk_strings_data_block.c pylnk_strings_data_block.h \
 @HAVE_PYTHON_TRUE@	pylnk_unused.h
 
 @HAVE_PYTHON_TRUE@pylnk_la_LIBADD = \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_PYTHON_TRUE@	../liblnk/liblnk.la \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_LIBADD@ \
@@ -745,14 +749,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_error.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_integer.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_string.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
@@ -872,14 +877,21 @@
 pylnk_la-pylnk_integer.lo: pylnk_integer.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_integer.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_integer.Tpo -c -o pylnk_la-pylnk_integer.lo `test -f 'pylnk_integer.c' || echo '$(srcdir)/'`pylnk_integer.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_integer.Tpo $(DEPDIR)/pylnk_la-pylnk_integer.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_integer.c' object='pylnk_la-pylnk_integer.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_integer.lo `test -f 'pylnk_integer.c' || echo '$(srcdir)/'`pylnk_integer.c
 
+pylnk_la-pylnk_string.lo: pylnk_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_string.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_string.Tpo -c -o pylnk_la-pylnk_string.lo `test -f 'pylnk_string.c' || echo '$(srcdir)/'`pylnk_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_string.Tpo $(DEPDIR)/pylnk_la-pylnk_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_string.c' object='pylnk_la-pylnk_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_string.lo `test -f 'pylnk_string.c' || echo '$(srcdir)/'`pylnk_string.c
+
 pylnk_la-pylnk_strings_data_block.lo: pylnk_strings_data_block.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_strings_data_block.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Tpo -c -o pylnk_la-pylnk_strings_data_block.lo `test -f 'pylnk_strings_data_block.c' || echo '$(srcdir)/'`pylnk_strings_data_block.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Tpo $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_strings_data_block.c' object='pylnk_la-pylnk_strings_data_block.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_strings_data_block.lo `test -f 'pylnk_strings_data_block.c' || echo '$(srcdir)/'`pylnk_strings_data_block.c
 
@@ -1070,14 +1082,15 @@
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_error.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_guid.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_integer.Plo
+	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_string.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
```

### Comparing `liblnk-20230205/pylnk/pylnk_libcerror.h` & `liblnk-20230716/pylnk/pylnk_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk.c` & `liblnk-20230716/pylnk/pylnk.c`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,14 @@
 /* Retrieves the pylnk/liblnk version
  * Returns a Python object if successful or NULL on error
  */
 PyObject *pylnk_get_version(
            PyObject *self PYLNK_ATTRIBUTE_UNUSED,
            PyObject *arguments PYLNK_ATTRIBUTE_UNUSED )
 {
-	const char *errors           = NULL;
 	const char *version_string   = NULL;
 	size_t version_string_length = 0;
 
 	PYLNK_UNREFERENCED_PARAMETER( self )
 	PYLNK_UNREFERENCED_PARAMETER( arguments )
 
 	Py_BEGIN_ALLOW_THREADS
@@ -121,15 +120,15 @@
 	/* Pass the string length to PyUnicode_DecodeUTF8
 	 * otherwise it makes the end of string character is part
 	 * of the string
 	 */
 	return( PyUnicode_DecodeUTF8(
 	         version_string,
 	         (Py_ssize_t) version_string_length,
-	         errors ) );
+	         NULL ) );
 }
 
 /* Checks if a file has a Windows Shortcut File (LNK) signature
  * Returns a Python object if successful or NULL on error
  */
 PyObject *pylnk_check_file_signature(
            PyObject *self PYLNK_ATTRIBUTE_UNUSED,
@@ -181,23 +180,34 @@
 		return( NULL );
 	}
 	else if( result != 0 )
 	{
 		PyErr_Clear();
 
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+		filename_wide = (wchar_t *) PyUnicode_AsWideCharString(
+		                             string_object,
+		                             NULL );
+#else
 		filename_wide = (wchar_t *) PyUnicode_AsUnicode(
 		                             string_object );
+#endif
 		Py_BEGIN_ALLOW_THREADS
 
 		result = liblnk_check_file_signature_wide(
 		          filename_wide,
 		          &error );
 
 		Py_END_ALLOW_THREADS
+
+#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
+		PyMem_Free(
+		 filename_wide );
+#endif
 #else
 		utf8_string_object = PyUnicode_AsUTF8String(
 		                      string_object );
 
 		if( utf8_string_object == NULL )
 		{
 			pylnk_error_fetch_and_raise(
```

### Comparing `liblnk-20230205/pylnk/pylnk_file_object_io_handle.h` & `liblnk-20230716/pylnk/pylnk_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_codepage.c` & `liblnk-20230716/pylnk/pylnk_codepage.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk/pylnk_guid.c` & `liblnk-20230716/pylnk/pylnk_guid.c`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
            size_t guid_buffer_size )
 {
 	char guid_string[ 48 ];
 
 	libcerror_error_t *error    = NULL;
 	libfguid_identifier_t *guid = NULL;
 	PyObject *string_object     = NULL;
-	const char *errors          = NULL;
 	static char *function       = "pylnk_string_new_from_guid";
 
 	if( libfguid_identifier_initialize(
 	     &guid,
 	     &error ) != 1 )
 	{
 		pylnk_error_raise(
@@ -111,15 +110,15 @@
 	/* Pass the string length to PyUnicode_DecodeUTF8
 	 * otherwise it makes the end of string character is part
 	 * of the string
 	 */
 	string_object = PyUnicode_DecodeUTF8(
 			 guid_string,
 			 (Py_ssize_t) 36,
-			 errors );
+			 NULL );
 
 	return( string_object );
 
 on_error:
 	if( guid != NULL )
 	{
 		libfguid_identifier_free(
```

### Comparing `liblnk-20230205/pylnk/pylnk_data_block.h` & `liblnk-20230716/pylnk/pylnk_data_block.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_identifier.c` & `liblnk-20230716/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_support.c` & `liblnk-20230716/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/Makefile.am` & `liblnk-20230716/libfguid/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_support.h` & `liblnk-20230716/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_definitions.h` & `liblnk-20230716/libfguid/libfguid_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_identifier.h` & `liblnk-20230716/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_unused.h` & `liblnk-20230716/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_error.h` & `liblnk-20230716/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_libcerror.h` & `liblnk-20230716/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/Makefile.in` & `liblnk-20230716/libfguid/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_error.c` & `liblnk-20230716/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_types.h` & `liblnk-20230716/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfguid/libfguid_extern.h` & `liblnk-20230716/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_tools_info_handle.c` & `liblnk-20230716/tests/lnk_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_distributed_link_tracker_properties.c` & `liblnk-20230716/tests/lnk_test_distributed_link_tracker_properties.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/pylnk_test_file.py` & `liblnk-20230716/tests/pylnk_test_file.py`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/test_library.sh` & `liblnk-20230716/tests/test_library.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20200705
+# Version: 20230410
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="data_block data_string distributed_link_tracker_properties error file_header io_handle known_folder_location link_target_identifier location_information notify special_folder_location";
 LIBRARY_TESTS_WITH_INPUT="file support";
```

### Comparing `liblnk-20230205/tests/lnk_test_file.c` & `liblnk-20230716/tests/lnk_test_file.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_liblnk.h` & `liblnk-20230716/tests/lnk_test_liblnk.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_libcerror.h` & `liblnk-20230716/tests/lnk_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_data_block.c` & `liblnk-20230716/tests/lnk_test_data_block.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_unused.h` & `liblnk-20230716/tests/lnk_test_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/test_python_module.sh` & `liblnk-20230716/tests/test_python_module.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20200705
+# Version: 20230410
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="";
 TEST_FUNCTIONS_WITH_INPUT="file support";
```

### Comparing `liblnk-20230205/tests/Makefile.am` & `liblnk-20230716/tests/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 	lnk_test_link_target_identifier \
 	lnk_test_location_information \
 	lnk_test_notify \
 	lnk_test_special_folder_location \
 	lnk_test_support \
 	lnk_test_tools_info_handle \
 	lnk_test_tools_output \
+	lnk_test_tools_path_string \
 	lnk_test_tools_signal
 
 lnk_test_data_block_SOURCES = \
 	lnk_test_data_block.c \
 	lnk_test_functions.c lnk_test_functions.h \
 	lnk_test_libbfio.h \
 	lnk_test_libcerror.h \
@@ -272,14 +273,15 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../liblnk/liblnk.la \
 	@LIBCERROR_LIBADD@
 
 lnk_test_tools_info_handle_SOURCES = \
 	../lnktools/info_handle.c ../lnktools/info_handle.h \
+	../lnktools/path_string.c ../lnktools/path_string.h \
 	../lnktools/property_store.c ../lnktools/property_store.h \
 	../lnktools/shell_items.c ../lnktools/shell_items.h \
 	lnk_test_libcerror.h \
 	lnk_test_macros.h \
 	lnk_test_memory.c lnk_test_memory.h \
 	lnk_test_tools_info_handle.c \
 	lnk_test_unused.h
@@ -302,14 +304,27 @@
 	lnk_test_tools_output.c \
 	lnk_test_unused.h
 
 lnk_test_tools_output_LDADD = \
 	../liblnk/liblnk.la \
 	@LIBCERROR_LIBADD@
 
+lnk_test_tools_path_string_SOURCES = \
+	../lnktools/path_string.c ../lnktools/path_string.h \
+	lnk_test_libcerror.h \
+	lnk_test_libcpath.h \
+	lnk_test_macros.h \
+	lnk_test_tools_path_string.c \
+	lnk_test_unused.h
+
+lnk_test_tools_path_string_LDADD = \
+	@LIBUNA_LIBADD@ \
+	../liblnk/liblnk.la \
+	@LIBCERROR_LIBADD@
+
 lnk_test_tools_signal_SOURCES = \
 	../lnktools/lnktools_signal.c ../lnktools/lnktools_signal.h \
 	lnk_test_libcerror.h \
 	lnk_test_macros.h \
 	lnk_test_tools_signal.c \
 	lnk_test_unused.h
```

### Comparing `liblnk-20230205/tests/lnk_test_file_header.c` & `liblnk-20230716/tests/lnk_test_file_header.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_io_handle.c` & `liblnk-20230716/tests/lnk_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_memory.c` & `liblnk-20230716/tests/lnk_test_memory.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_libuna.h` & `liblnk-20230716/tests/lnk_test_libuna.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_functions.c` & `liblnk-20230716/tests/lnk_test_functions.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_getopt.c` & `liblnk-20230716/tests/lnk_test_getopt.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_support.c` & `liblnk-20230716/tests/lnk_test_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_data_string.c` & `liblnk-20230716/tests/lnk_test_data_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -330,14 +330,15 @@
 	/* Test regular cases
 	 */
 	result = liblnk_data_string_read_data(
 	          data_string,
 	          io_handle,
 	          lnk_test_data_string_data1,
 	          60,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -348,14 +349,15 @@
 	/* Test error cases
 	 */
 	result = liblnk_data_string_read_data(
 	          data_string,
 	          io_handle,
 	          lnk_test_data_string_data1,
 	          60,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -407,14 +409,15 @@
 	/* Test error cases
 	 */
 	result = liblnk_data_string_read_data(
 	          NULL,
 	          io_handle,
 	          lnk_test_data_string_data1,
 	          60,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -426,14 +429,15 @@
 	 &error );
 
 	result = liblnk_data_string_read_data(
 	          data_string,
 	          NULL,
 	          lnk_test_data_string_data1,
 	          60,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -445,14 +449,15 @@
 	 &error );
 
 	result = liblnk_data_string_read_data(
 	          data_string,
 	          io_handle,
 	          NULL,
 	          60,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -464,14 +469,15 @@
 	 &error );
 
 	result = liblnk_data_string_read_data(
 	          data_string,
 	          io_handle,
 	          lnk_test_data_string_data1,
 	          (size_t) SSIZE_MAX + 1,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -483,14 +489,15 @@
 	 &error );
 
 	result = liblnk_data_string_read_data(
 	          data_string,
 	          io_handle,
 	          lnk_test_data_string_data1,
 	          0,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -634,14 +641,15 @@
 	/* Test regular cases
 	 */
 	result = liblnk_data_string_read_file_io_handle(
 	          data_string,
 	          io_handle,
 	          file_io_handle,
 	          0,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
 
@@ -652,14 +660,15 @@
 	/* Test error cases
 	 */
 	result = liblnk_data_string_read_file_io_handle(
 	          data_string,
 	          io_handle,
 	          file_io_handle,
 	          0,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -711,14 +720,15 @@
 	/* Test error cases
 	 */
 	result = liblnk_data_string_read_file_io_handle(
 	          NULL,
 	          io_handle,
 	          file_io_handle,
 	          0,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -730,14 +740,15 @@
 	 &error );
 
 	result = liblnk_data_string_read_file_io_handle(
 	          data_string,
 	          NULL,
 	          file_io_handle,
 	          0,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -749,14 +760,15 @@
 	 &error );
 
 	result = liblnk_data_string_read_file_io_handle(
 	          data_string,
 	          io_handle,
 	          NULL,
 	          0,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -768,14 +780,15 @@
 	 &error );
 
 	result = liblnk_data_string_read_file_io_handle(
 	          data_string,
 	          io_handle,
 	          file_io_handle,
 	          -1,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -823,14 +836,15 @@
 	 error );
 
 	result = liblnk_data_string_read_file_io_handle(
 	          data_string,
 	          io_handle,
 	          file_io_handle,
 	          0,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 -1 );
 
@@ -1360,14 +1374,15 @@
 	 error );
 
 	result = liblnk_data_string_read_data(
 	          data_string,
 	          io_handle,
 	          lnk_test_data_string_data1,
 	          60,
+	          0,
 	          &error );
 
 	LNK_TEST_ASSERT_EQUAL_INT(
 	 "result",
 	 result,
 	 1 );
```

### Comparing `liblnk-20230205/tests/test_lnkinfo.sh` & `liblnk-20230716/tests/test_lnkinfo.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20200705
+# Version: 20230410
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("lnkinfo");
 OPTIONS_PER_PROFILE=("");
```

### Comparing `liblnk-20230205/tests/lnk_test_special_folder_location.c` & `liblnk-20230716/tests/lnk_test_special_folder_location.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_macros.h` & `liblnk-20230716/tests/lnk_test_macros.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_libbfio.h` & `liblnk-20230716/tests/lnk_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/test_tools.sh` & `liblnk-20230716/tests/test_tools.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20200705
+# Version: 20230410
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-TOOLS_TESTS="info_handle output signal";
+TOOLS_TESTS="info_handle output path_string signal";
 TOOLS_TESTS_WITH_INPUT="";
 OPTION_SETS="";
 
 INPUT_GLOB="*";
 
 run_test()
 {
```

### Comparing `liblnk-20230205/tests/lnk_test_getopt.h` & `liblnk-20230716/tests/lnk_test_getopt.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/pylnk_test_support.py` & `liblnk-20230716/tests/pylnk_test_support.py`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/test_manpage.sh` & `liblnk-20230716/tests/test_manpage.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Tests man pages.
 #
-# Version: 20190302
+# Version: 20230410
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 run_test()
 {
```

### Comparing `liblnk-20230205/tests/lnk_test_tools_output.c` & `liblnk-20230716/tests/lnk_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_memory.h` & `liblnk-20230716/tests/lnk_test_memory.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_known_folder_location.c` & `liblnk-20230716/tests/lnk_test_known_folder_location.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/test_runner.sh` & `liblnk-20230716/tests/test_runner.sh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/bin/bash
+#!/usr/bin/env bash
 # Bash functions to run an executable for testing.
 #
-# Version: 20220924
+# Version: 20230410
 #
 # When CHECK_WITH_ASAN is set to a non-empty value the test executable
 # is run with asan, otherwise it is run without.
 #
 # When CHECK_WITH_GDB is set to a non-empty value the test executable
 # is run with gdb, otherwise it is run without.
 #
```

### Comparing `liblnk-20230205/tests/lnk_test_link_target_identifier.c` & `liblnk-20230716/tests/lnk_test_link_target_identifier.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_error.c` & `liblnk-20230716/tests/lnk_test_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_functions.h` & `liblnk-20230716/tests/lnk_test_functions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/Makefile.in` & `liblnk-20230716/tests/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,17 @@
 	lnk_test_file_header$(EXEEXT) lnk_test_io_handle$(EXEEXT) \
 	lnk_test_known_folder_location$(EXEEXT) \
 	lnk_test_link_target_identifier$(EXEEXT) \
 	lnk_test_location_information$(EXEEXT) \
 	lnk_test_notify$(EXEEXT) \
 	lnk_test_special_folder_location$(EXEEXT) \
 	lnk_test_support$(EXEEXT) lnk_test_tools_info_handle$(EXEEXT) \
-	lnk_test_tools_output$(EXEEXT) lnk_test_tools_signal$(EXEEXT)
+	lnk_test_tools_output$(EXEEXT) \
+	lnk_test_tools_path_string$(EXEEXT) \
+	lnk_test_tools_signal$(EXEEXT)
 subdir = tests
 ACLOCAL_M4 = $(top_srcdir)/aclocal.m4
 am__aclocal_m4_deps = $(top_srcdir)/m4/common.m4 \
 	$(top_srcdir)/m4/gettext.m4 $(top_srcdir)/m4/host-cpu-c-abi.m4 \
 	$(top_srcdir)/m4/iconv.m4 $(top_srcdir)/m4/intlmacosx.m4 \
 	$(top_srcdir)/m4/lib-ld.m4 $(top_srcdir)/m4/lib-link.m4 \
 	$(top_srcdir)/m4/lib-prefix.m4 $(top_srcdir)/m4/libbfio.m4 \
@@ -193,25 +195,32 @@
 	lnk_test_getopt.$(OBJEXT) lnk_test_memory.$(OBJEXT) \
 	lnk_test_support.$(OBJEXT)
 lnk_test_support_OBJECTS = $(am_lnk_test_support_OBJECTS)
 lnk_test_support_DEPENDENCIES = ../liblnk/liblnk.la
 am__dirstamp = $(am__leading_dot)dirstamp
 am_lnk_test_tools_info_handle_OBJECTS =  \
 	../lnktools/info_handle.$(OBJEXT) \
+	../lnktools/path_string.$(OBJEXT) \
 	../lnktools/property_store.$(OBJEXT) \
 	../lnktools/shell_items.$(OBJEXT) lnk_test_memory.$(OBJEXT) \
 	lnk_test_tools_info_handle.$(OBJEXT)
 lnk_test_tools_info_handle_OBJECTS =  \
 	$(am_lnk_test_tools_info_handle_OBJECTS)
 lnk_test_tools_info_handle_DEPENDENCIES = ../liblnk/liblnk.la
 am_lnk_test_tools_output_OBJECTS =  \
 	../lnktools/lnktools_output.$(OBJEXT) \
 	lnk_test_tools_output.$(OBJEXT)
 lnk_test_tools_output_OBJECTS = $(am_lnk_test_tools_output_OBJECTS)
 lnk_test_tools_output_DEPENDENCIES = ../liblnk/liblnk.la
+am_lnk_test_tools_path_string_OBJECTS =  \
+	../lnktools/path_string.$(OBJEXT) \
+	lnk_test_tools_path_string.$(OBJEXT)
+lnk_test_tools_path_string_OBJECTS =  \
+	$(am_lnk_test_tools_path_string_OBJECTS)
+lnk_test_tools_path_string_DEPENDENCIES = ../liblnk/liblnk.la
 am_lnk_test_tools_signal_OBJECTS =  \
 	../lnktools/lnktools_signal.$(OBJEXT) \
 	lnk_test_tools_signal.$(OBJEXT)
 lnk_test_tools_signal_OBJECTS = $(am_lnk_test_tools_signal_OBJECTS)
 lnk_test_tools_signal_DEPENDENCIES = ../liblnk/liblnk.la
 AM_V_P = $(am__v_P_@AM_V@)
 am__v_P_ = $(am__v_P_@AM_DEFAULT_V@)
@@ -227,14 +236,15 @@
 am__v_at_1 = 
 DEFAULT_INCLUDES = -I.@am__isrc@ -I$(top_builddir)/common
 depcomp = $(SHELL) $(top_srcdir)/depcomp
 am__maybe_remake_depfiles = depfiles
 am__depfiles_remade = ../lnktools/$(DEPDIR)/info_handle.Po \
 	../lnktools/$(DEPDIR)/lnktools_output.Po \
 	../lnktools/$(DEPDIR)/lnktools_signal.Po \
+	../lnktools/$(DEPDIR)/path_string.Po \
 	../lnktools/$(DEPDIR)/property_store.Po \
 	../lnktools/$(DEPDIR)/shell_items.Po \
 	./$(DEPDIR)/lnk_test_data_block.Po \
 	./$(DEPDIR)/lnk_test_data_string.Po \
 	./$(DEPDIR)/lnk_test_distributed_link_tracker_properties.Po \
 	./$(DEPDIR)/lnk_test_error.Po ./$(DEPDIR)/lnk_test_file.Po \
 	./$(DEPDIR)/lnk_test_file_header.Po \
@@ -245,14 +255,15 @@
 	./$(DEPDIR)/lnk_test_link_target_identifier.Po \
 	./$(DEPDIR)/lnk_test_location_information.Po \
 	./$(DEPDIR)/lnk_test_memory.Po ./$(DEPDIR)/lnk_test_notify.Po \
 	./$(DEPDIR)/lnk_test_special_folder_location.Po \
 	./$(DEPDIR)/lnk_test_support.Po \
 	./$(DEPDIR)/lnk_test_tools_info_handle.Po \
 	./$(DEPDIR)/lnk_test_tools_output.Po \
+	./$(DEPDIR)/lnk_test_tools_path_string.Po \
 	./$(DEPDIR)/lnk_test_tools_signal.Po
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
@@ -278,28 +289,30 @@
 	$(lnk_test_link_target_identifier_SOURCES) \
 	$(lnk_test_location_information_SOURCES) \
 	$(lnk_test_notify_SOURCES) \
 	$(lnk_test_special_folder_location_SOURCES) \
 	$(lnk_test_support_SOURCES) \
 	$(lnk_test_tools_info_handle_SOURCES) \
 	$(lnk_test_tools_output_SOURCES) \
+	$(lnk_test_tools_path_string_SOURCES) \
 	$(lnk_test_tools_signal_SOURCES)
 DIST_SOURCES = $(lnk_test_data_block_SOURCES) \
 	$(lnk_test_data_string_SOURCES) \
 	$(lnk_test_distributed_link_tracker_properties_SOURCES) \
 	$(lnk_test_error_SOURCES) $(lnk_test_file_SOURCES) \
 	$(lnk_test_file_header_SOURCES) $(lnk_test_io_handle_SOURCES) \
 	$(lnk_test_known_folder_location_SOURCES) \
 	$(lnk_test_link_target_identifier_SOURCES) \
 	$(lnk_test_location_information_SOURCES) \
 	$(lnk_test_notify_SOURCES) \
 	$(lnk_test_special_folder_location_SOURCES) \
 	$(lnk_test_support_SOURCES) \
 	$(lnk_test_tools_info_handle_SOURCES) \
 	$(lnk_test_tools_output_SOURCES) \
+	$(lnk_test_tools_path_string_SOURCES) \
 	$(lnk_test_tools_signal_SOURCES)
 am__can_run_installinfo = \
   case $$AM_UPDATE_INFO_DIR in \
     n|no|NO) false;; \
     *) (install-info --version) >/dev/null 2>&1;; \
   esac
 am__tagged_files = $(HEADERS) $(SOURCES) $(TAGS_FILES) $(LISP)
@@ -1121,14 +1134,15 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../liblnk/liblnk.la \
 	@LIBCERROR_LIBADD@
 
 lnk_test_tools_info_handle_SOURCES = \
 	../lnktools/info_handle.c ../lnktools/info_handle.h \
+	../lnktools/path_string.c ../lnktools/path_string.h \
 	../lnktools/property_store.c ../lnktools/property_store.h \
 	../lnktools/shell_items.c ../lnktools/shell_items.h \
 	lnk_test_libcerror.h \
 	lnk_test_macros.h \
 	lnk_test_memory.c lnk_test_memory.h \
 	lnk_test_tools_info_handle.c \
 	lnk_test_unused.h
@@ -1151,14 +1165,27 @@
 	lnk_test_tools_output.c \
 	lnk_test_unused.h
 
 lnk_test_tools_output_LDADD = \
 	../liblnk/liblnk.la \
 	@LIBCERROR_LIBADD@
 
+lnk_test_tools_path_string_SOURCES = \
+	../lnktools/path_string.c ../lnktools/path_string.h \
+	lnk_test_libcerror.h \
+	lnk_test_libcpath.h \
+	lnk_test_macros.h \
+	lnk_test_tools_path_string.c \
+	lnk_test_unused.h
+
+lnk_test_tools_path_string_LDADD = \
+	@LIBUNA_LIBADD@ \
+	../liblnk/liblnk.la \
+	@LIBCERROR_LIBADD@
+
 lnk_test_tools_signal_SOURCES = \
 	../lnktools/lnktools_signal.c ../lnktools/lnktools_signal.h \
 	lnk_test_libcerror.h \
 	lnk_test_macros.h \
 	lnk_test_tools_signal.c \
 	lnk_test_unused.h
 
@@ -1267,28 +1294,34 @@
 	@$(MKDIR_P) ../lnktools
 	@: > ../lnktools/$(am__dirstamp)
 ../lnktools/$(DEPDIR)/$(am__dirstamp):
 	@$(MKDIR_P) ../lnktools/$(DEPDIR)
 	@: > ../lnktools/$(DEPDIR)/$(am__dirstamp)
 ../lnktools/info_handle.$(OBJEXT): ../lnktools/$(am__dirstamp) \
 	../lnktools/$(DEPDIR)/$(am__dirstamp)
+../lnktools/path_string.$(OBJEXT): ../lnktools/$(am__dirstamp) \
+	../lnktools/$(DEPDIR)/$(am__dirstamp)
 ../lnktools/property_store.$(OBJEXT): ../lnktools/$(am__dirstamp) \
 	../lnktools/$(DEPDIR)/$(am__dirstamp)
 ../lnktools/shell_items.$(OBJEXT): ../lnktools/$(am__dirstamp) \
 	../lnktools/$(DEPDIR)/$(am__dirstamp)
 
 lnk_test_tools_info_handle$(EXEEXT): $(lnk_test_tools_info_handle_OBJECTS) $(lnk_test_tools_info_handle_DEPENDENCIES) $(EXTRA_lnk_test_tools_info_handle_DEPENDENCIES) 
 	@rm -f lnk_test_tools_info_handle$(EXEEXT)
 	$(AM_V_CCLD)$(LINK) $(lnk_test_tools_info_handle_OBJECTS) $(lnk_test_tools_info_handle_LDADD) $(LIBS)
 ../lnktools/lnktools_output.$(OBJEXT): ../lnktools/$(am__dirstamp) \
 	../lnktools/$(DEPDIR)/$(am__dirstamp)
 
 lnk_test_tools_output$(EXEEXT): $(lnk_test_tools_output_OBJECTS) $(lnk_test_tools_output_DEPENDENCIES) $(EXTRA_lnk_test_tools_output_DEPENDENCIES) 
 	@rm -f lnk_test_tools_output$(EXEEXT)
 	$(AM_V_CCLD)$(LINK) $(lnk_test_tools_output_OBJECTS) $(lnk_test_tools_output_LDADD) $(LIBS)
+
+lnk_test_tools_path_string$(EXEEXT): $(lnk_test_tools_path_string_OBJECTS) $(lnk_test_tools_path_string_DEPENDENCIES) $(EXTRA_lnk_test_tools_path_string_DEPENDENCIES) 
+	@rm -f lnk_test_tools_path_string$(EXEEXT)
+	$(AM_V_CCLD)$(LINK) $(lnk_test_tools_path_string_OBJECTS) $(lnk_test_tools_path_string_LDADD) $(LIBS)
 ../lnktools/lnktools_signal.$(OBJEXT): ../lnktools/$(am__dirstamp) \
 	../lnktools/$(DEPDIR)/$(am__dirstamp)
 
 lnk_test_tools_signal$(EXEEXT): $(lnk_test_tools_signal_OBJECTS) $(lnk_test_tools_signal_DEPENDENCIES) $(EXTRA_lnk_test_tools_signal_DEPENDENCIES) 
 	@rm -f lnk_test_tools_signal$(EXEEXT)
 	$(AM_V_CCLD)$(LINK) $(lnk_test_tools_signal_OBJECTS) $(lnk_test_tools_signal_LDADD) $(LIBS)
 
@@ -1298,14 +1331,15 @@
 
 distclean-compile:
 	-rm -f *.tab.c
 
 @AMDEP_TRUE@@am__include@ @am__quote@../lnktools/$(DEPDIR)/info_handle.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@../lnktools/$(DEPDIR)/lnktools_output.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@../lnktools/$(DEPDIR)/lnktools_signal.Po@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@../lnktools/$(DEPDIR)/path_string.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@../lnktools/$(DEPDIR)/property_store.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@../lnktools/$(DEPDIR)/shell_items.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_data_block.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_data_string.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_distributed_link_tracker_properties.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_error.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_file.Po@am__quote@ # am--include-marker
@@ -1318,14 +1352,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_location_information.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_memory.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_notify.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_special_folder_location.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_support.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_tools_info_handle.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_tools_output.Po@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_tools_path_string.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnk_test_tools_signal.Po@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
@@ -1718,14 +1753,15 @@
 
 installcheck-am:
 
 maintainer-clean: maintainer-clean-am
 		-rm -f ../lnktools/$(DEPDIR)/info_handle.Po
 	-rm -f ../lnktools/$(DEPDIR)/lnktools_output.Po
 	-rm -f ../lnktools/$(DEPDIR)/lnktools_signal.Po
+	-rm -f ../lnktools/$(DEPDIR)/path_string.Po
 	-rm -f ../lnktools/$(DEPDIR)/property_store.Po
 	-rm -f ../lnktools/$(DEPDIR)/shell_items.Po
 	-rm -f ./$(DEPDIR)/lnk_test_data_block.Po
 	-rm -f ./$(DEPDIR)/lnk_test_data_string.Po
 	-rm -f ./$(DEPDIR)/lnk_test_distributed_link_tracker_properties.Po
 	-rm -f ./$(DEPDIR)/lnk_test_error.Po
 	-rm -f ./$(DEPDIR)/lnk_test_file.Po
@@ -1738,14 +1774,15 @@
 	-rm -f ./$(DEPDIR)/lnk_test_location_information.Po
 	-rm -f ./$(DEPDIR)/lnk_test_memory.Po
 	-rm -f ./$(DEPDIR)/lnk_test_notify.Po
 	-rm -f ./$(DEPDIR)/lnk_test_special_folder_location.Po
 	-rm -f ./$(DEPDIR)/lnk_test_support.Po
 	-rm -f ./$(DEPDIR)/lnk_test_tools_info_handle.Po
 	-rm -f ./$(DEPDIR)/lnk_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/lnk_test_tools_path_string.Po
 	-rm -f ./$(DEPDIR)/lnk_test_tools_signal.Po
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
```

### Comparing `liblnk-20230205/tests/lnk_test_location_information.c` & `liblnk-20230716/tests/lnk_test_location_information.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_tools_signal.c` & `liblnk-20230716/tests/lnk_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_notify.c` & `liblnk-20230716/tests/lnk_test_notify.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_libcnotify.h` & `liblnk-20230716/tests/lnk_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/tests/lnk_test_libclocale.h` & `liblnk-20230716/tests/lnk_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_wide_string.h` & `liblnk-20230716/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_support.c` & `liblnk-20230716/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_locale.h` & `liblnk-20230716/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/Makefile.am` & `liblnk-20230716/libclocale/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_locale.c` & `liblnk-20230716/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_extern.h` & `liblnk-20230716/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_unused.h` & `liblnk-20230716/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_support.h` & `liblnk-20230716/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_definitions.h` & `liblnk-20230716/libclocale/libclocale_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_codepage.h` & `liblnk-20230716/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_codepage.c` & `liblnk-20230716/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/Makefile.in` & `liblnk-20230716/libclocale/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_wide_string.c` & `liblnk-20230716/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libclocale/libclocale_libcerror.h` & `liblnk-20230716/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/missing` & `liblnk-20230716/missing`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk.pc.in` & `liblnk-20230716/liblnk.pc.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/Makefile.am` & `liblnk-20230716/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/aclocal.m4` & `liblnk-20230716/aclocal.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_handle.h` & `liblnk-20230716/libbfio/libbfio_handle.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_libcerror.h` & `liblnk-20230716/libbfio/libbfio_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_handle.c` & `liblnk-20230716/libbfio/libbfio_handle.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_libuna.h` & `liblnk-20230716/libbfio/libbfio_libuna.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_definitions.h` & `liblnk-20230716/libbfio/libbfio_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_libclocale.h` & `liblnk-20230716/libbfio/libbfio_libclocale.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_codepage.h` & `liblnk-20230716/libbfio/libbfio_codepage.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_libcdata.h` & `liblnk-20230716/libbfio/libbfio_libcdata.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_extern.h` & `liblnk-20230716/libbfio/libbfio_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file_range.c` & `liblnk-20230716/libbfio/libbfio_file_range.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file_range_io_handle.c` & `liblnk-20230716/libbfio/libbfio_file_range_io_handle.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/Makefile.am` & `liblnk-20230716/libbfio/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file_pool.c` & `liblnk-20230716/libbfio/libbfio_file_pool.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file.c` & `liblnk-20230716/libbfio/libbfio_file.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_pool.h` & `liblnk-20230716/libbfio/libbfio_pool.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file_range.h` & `liblnk-20230716/libbfio/libbfio_file_range.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_system_string.h` & `liblnk-20230716/libbfio/libbfio_system_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file_io_handle.h` & `liblnk-20230716/libbfio/libbfio_file_io_handle.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_memory_range_io_handle.c` & `liblnk-20230716/libbfio/libbfio_memory_range_io_handle.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file.h` & `liblnk-20230716/libbfio/libbfio_file.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_support.c` & `liblnk-20230716/libbfio/libbfio_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file_pool.h` & `liblnk-20230716/libbfio/libbfio_file_pool.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_memory_range_io_handle.h` & `liblnk-20230716/libbfio/libbfio_memory_range_io_handle.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_error.h` & `liblnk-20230716/libbfio/libbfio_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_libcthreads.h` & `liblnk-20230716/libbfio/libbfio_libcthreads.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_system_string.c` & `liblnk-20230716/libbfio/libbfio_system_string.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_memory_range.h` & `liblnk-20230716/libbfio/libbfio_memory_range.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file_range_io_handle.h` & `liblnk-20230716/libbfio/libbfio_file_range_io_handle.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_memory_range.c` & `liblnk-20230716/libbfio/libbfio_memory_range.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/Makefile.in` & `liblnk-20230716/libbfio/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_pool.c` & `liblnk-20230716/libbfio/libbfio_pool.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_unused.h` & `liblnk-20230716/libbfio/libbfio_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_libcpath.h` & `liblnk-20230716/libbfio/libbfio_libcpath.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_libcfile.h` & `liblnk-20230716/libbfio/libbfio_libcfile.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_support.h` & `liblnk-20230716/libbfio/libbfio_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_file_io_handle.c` & `liblnk-20230716/libbfio/libbfio_file_io_handle.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_error.c` & `liblnk-20230716/libbfio/libbfio_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libbfio/libbfio_types.h` & `liblnk-20230716/libbfio/libbfio_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/COPYING` & `liblnk-20230716/COPYING`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk/definitions.h.in` & `liblnk-20230716/include/liblnk/definitions.h.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk/extern.h` & `liblnk-20230716/include/liblnk/extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk/types.h` & `liblnk-20230716/include/liblnk/types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk/features.h.in` & `liblnk-20230716/include/liblnk/features.h.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk/types.h.in` & `liblnk-20230716/include/liblnk/types.h.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk/features.h` & `liblnk-20230716/include/liblnk/features.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk/definitions.h` & `liblnk-20230716/include/liblnk/definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBLNK_DEFINITIONS_H )
 #define _LIBLNK_DEFINITIONS_H
 
 #include <liblnk/types.h>
 
-#define LIBLNK_VERSION							20230205
+#define LIBLNK_VERSION							20230716
 
 /* The liblnk version string
  */
-#define LIBLNK_VERSION_STRING						"20230205"
+#define LIBLNK_VERSION_STRING						"20230716"
 
 /* The liblnk file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBLNK_ACCESS_FLAGS
```

### Comparing `liblnk-20230205/include/liblnk/codepage.h` & `liblnk-20230716/include/liblnk/codepage.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk/error.h` & `liblnk-20230716/include/liblnk/error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/Makefile.in` & `liblnk-20230716/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/include/liblnk.h` & `liblnk-20230716/include/liblnk.h`

 * *Files 8% similar despite different names*

```diff
@@ -448,94 +448,102 @@
 int liblnk_file_get_utf16_volume_label(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded local path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_local_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded local path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_local_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded local path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_local_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded local path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_local_path(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded network path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_network_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded network path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_network_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded network path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_network_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded network path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_network_path(
      liblnk_file_t *file,
@@ -582,196 +590,214 @@
 int liblnk_file_get_utf16_description(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded relative path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_relative_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded relative path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_relative_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded relative path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_relative_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded relative path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_relative_path(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded working directory
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_working_directory_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded working directory
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_working_directory(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded working directory
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_working_directory_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded working directory
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_working_directory(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded command line arguments
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_command_line_arguments_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded command line arguments
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_command_line_arguments(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded command line arguments
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_command_line_arguments_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded command line arguments
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_command_line_arguments(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded icon location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_icon_location_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded icon location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_icon_location(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded icon location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_icon_location_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded icon location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_icon_location(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded environment variables location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  *
  * This function is deprecated use liblnk_strings_data_block_get_utf8_string_size instead
  *
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_DEPRECATED \
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_environment_variables_location_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded environment variables location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  *
  * This function is deprecated use liblnk_strings_data_block_get_utf8_string instead
  *
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_DEPRECATED \
@@ -779,28 +805,30 @@
 int liblnk_file_get_utf8_environment_variables_location(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded environment variables location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  *
  * This function is deprecated use liblnk_strings_data_block_get_utf16_string_size instead
  *
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_DEPRECATED \
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_environment_variables_location_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded environment variables location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  *
  * This function is deprecated use liblnk_strings_data_block_get_utf16_string instead
  *
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_DEPRECATED \
@@ -1067,14 +1095,60 @@
 LIBLNK_EXTERN \
 int liblnk_strings_data_block_get_utf16_string(
      liblnk_data_block_t *data_block,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
+/* Retrieves the size of the UTF-8 path string
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBLNK_EXTERN \
+int liblnk_strings_data_block_get_utf8_path_string_size(
+     liblnk_data_block_t *data_block,
+     size_t *utf8_string_size,
+     liblnk_error_t **error );
+
+/* Retrieves the UTF-8 path string
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBLNK_EXTERN \
+int liblnk_strings_data_block_get_utf8_path_string(
+     liblnk_data_block_t *data_block,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     liblnk_error_t **error );
+
+/* Retrieves the size of the UTF-16 path string
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBLNK_EXTERN \
+int liblnk_strings_data_block_get_utf16_path_string_size(
+     liblnk_data_block_t *data_block,
+     size_t *utf16_string_size,
+     liblnk_error_t **error );
+
+/* Retrieves the UTF-16 path string
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBLNK_EXTERN \
+int liblnk_strings_data_block_get_utf16_path_string(
+     liblnk_data_block_t *data_block,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     liblnk_error_t **error );
+
 /* -------------------------------------------------------------------------
  * Distributed link tracking data block functions
  * ------------------------------------------------------------------------- */
 
 /* Retrieves the size of the UTF-8 encoded machine identifier
  * The size includes the end of string character
  * Returns 1 if successful or -1 on error
```

### Comparing `liblnk-20230205/include/liblnk.h.in` & `liblnk-20230716/include/liblnk.h.in`

 * *Files 8% similar despite different names*

```diff
@@ -448,94 +448,102 @@
 int liblnk_file_get_utf16_volume_label(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded local path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_local_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded local path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_local_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded local path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_local_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded local path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_local_path(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded network path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_network_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded network path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_network_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded network path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_network_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded network path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_network_path(
      liblnk_file_t *file,
@@ -582,196 +590,214 @@
 int liblnk_file_get_utf16_description(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded relative path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_relative_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded relative path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_relative_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded relative path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_relative_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded relative path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_relative_path(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded working directory
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_working_directory_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded working directory
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_working_directory(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded working directory
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_working_directory_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded working directory
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_working_directory(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded command line arguments
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_command_line_arguments_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded command line arguments
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_command_line_arguments(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded command line arguments
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_command_line_arguments_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded command line arguments
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_command_line_arguments(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded icon location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_icon_location_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded icon location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_icon_location(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded icon location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_icon_location_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded icon location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_icon_location(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-8 encoded environment variables location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  *
  * This function is deprecated use liblnk_strings_data_block_get_utf8_string_size instead
  *
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_DEPRECATED \
 LIBLNK_EXTERN \
 int liblnk_file_get_utf8_environment_variables_location_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-8 encoded environment variables location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  *
  * This function is deprecated use liblnk_strings_data_block_get_utf8_string instead
  *
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_DEPRECATED \
@@ -779,28 +805,30 @@
 int liblnk_file_get_utf8_environment_variables_location(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the size of the UTF-16 encoded environment variables location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  *
  * This function is deprecated use liblnk_strings_data_block_get_utf16_string_size instead
  *
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_DEPRECATED \
 LIBLNK_EXTERN \
 int liblnk_file_get_utf16_environment_variables_location_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      liblnk_error_t **error );
 
 /* Retrieves the UTF-16 encoded environment variables location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  *
  * This function is deprecated use liblnk_strings_data_block_get_utf16_string instead
  *
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 LIBLNK_DEPRECATED \
@@ -1067,14 +1095,60 @@
 LIBLNK_EXTERN \
 int liblnk_strings_data_block_get_utf16_string(
      liblnk_data_block_t *data_block,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      liblnk_error_t **error );
 
+/* Retrieves the size of the UTF-8 path string
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBLNK_EXTERN \
+int liblnk_strings_data_block_get_utf8_path_string_size(
+     liblnk_data_block_t *data_block,
+     size_t *utf8_string_size,
+     liblnk_error_t **error );
+
+/* Retrieves the UTF-8 path string
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBLNK_EXTERN \
+int liblnk_strings_data_block_get_utf8_path_string(
+     liblnk_data_block_t *data_block,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     liblnk_error_t **error );
+
+/* Retrieves the size of the UTF-16 path string
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBLNK_EXTERN \
+int liblnk_strings_data_block_get_utf16_path_string_size(
+     liblnk_data_block_t *data_block,
+     size_t *utf16_string_size,
+     liblnk_error_t **error );
+
+/* Retrieves the UTF-16 path string
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+LIBLNK_EXTERN \
+int liblnk_strings_data_block_get_utf16_path_string(
+     liblnk_data_block_t *data_block,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     liblnk_error_t **error );
+
 /* -------------------------------------------------------------------------
  * Distributed link tracking data block functions
  * ------------------------------------------------------------------------- */
 
 /* Retrieves the size of the UTF-8 encoded machine identifier
  * The size includes the end of string character
  * Returns 1 if successful or -1 on error
```

### Comparing `liblnk-20230205/install-sh` & `liblnk-20230716/install-sh`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/INSTALL` & `liblnk-20230716/INSTALL`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/dpkg/copyright` & `liblnk-20230716/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/dpkg/rules` & `liblnk-20230716/dpkg/rules`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/dpkg/control` & `liblnk-20230716/dpkg/control`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_support.c` & `liblnk-20230716/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_systemtime.h` & `liblnk-20230716/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_error.h` & `liblnk-20230716/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/Makefile.am` & `liblnk-20230716/libfdatetime/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_unused.h` & `liblnk-20230716/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_error.c` & `liblnk-20230716/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_posix_time.c` & `liblnk-20230716/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_fat_date_time.h` & `liblnk-20230716/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_types.h` & `liblnk-20230716/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_floatingtime.c` & `liblnk-20230716/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_hfs_time.h` & `liblnk-20230716/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_support.h` & `liblnk-20230716/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_extern.h` & `liblnk-20230716/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_filetime.h` & `liblnk-20230716/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_date_time_values.c` & `liblnk-20230716/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_floatingtime.h` & `liblnk-20230716/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_libcerror.h` & `liblnk-20230716/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/Makefile.in` & `liblnk-20230716/libfdatetime/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_nsf_timedate.c` & `liblnk-20230716/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_date_time_values.h` & `liblnk-20230716/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_hfs_time.c` & `liblnk-20230716/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_posix_time.h` & `liblnk-20230716/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_fat_date_time.c` & `liblnk-20230716/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_nsf_timedate.h` & `liblnk-20230716/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_definitions.h` & `liblnk-20230716/libfdatetime/libfdatetime_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_systemtime.c` & `liblnk-20230716/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfdatetime/libfdatetime_filetime.c` & `liblnk-20230716/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_file.c` & `liblnk-20230716/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_libclocale.h` & `liblnk-20230716/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_support.c` & `liblnk-20230716/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_support.h` & `liblnk-20230716/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_error.c` & `liblnk-20230716/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_winapi.c` & `liblnk-20230716/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/Makefile.am` & `liblnk-20230716/libcfile/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_libcerror.h` & `liblnk-20230716/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_unused.h` & `liblnk-20230716/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_winapi.h` & `liblnk-20230716/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_types.h` & `liblnk-20230716/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_extern.h` & `liblnk-20230716/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_notify.h` & `liblnk-20230716/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_definitions.h` & `liblnk-20230716/libcfile/libcfile_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_file.h` & `liblnk-20230716/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_error.h` & `liblnk-20230716/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_system_string.c` & `liblnk-20230716/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/Makefile.in` & `liblnk-20230716/libcfile/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_system_string.h` & `liblnk-20230716/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_libcnotify.h` & `liblnk-20230716/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_libuna.h` & `liblnk-20230716/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcfile/libcfile_notify.c` & `liblnk-20230716/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk.spec` & `liblnk-20230716/liblnk.spec`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Name: liblnk
-Version: 20230205
+Version: 20230716
 Release: 1
 Summary: Library to access the Windows Shortcut File (LNK) format
 Group: System Environment/Libraries
-License: LGPLv3+
+License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/liblnk
-BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
                
 BuildRequires: gcc               
 
 %description -n liblnk
 Library to access the Windows Shortcut File (LNK) format
 
 %package -n liblnk-static
@@ -61,45 +60,40 @@
 rm -rf %{buildroot}
 
 %post -p /sbin/ldconfig
 
 %postun -p /sbin/ldconfig
 
 %files -n liblnk
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.so.*
+%{_libdir}/*.so.*
 
 %files -n liblnk-static
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.a
+%{_libdir}/*.a
 
 %files -n liblnk-devel
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/*.so
 %{_libdir}/pkgconfig/liblnk.pc
 %{_includedir}/*
 %{_mandir}/man3/*
 
 %files -n liblnk-python3
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %files -n liblnk-tools
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_bindir}/*
+%{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sun Feb  5 2023 Joachim Metz <joachim.metz@gmail.com> 20230205-1
+* Sun Jul 16 2023 Joachim Metz <joachim.metz@gmail.com> 20230716-1
 - Auto-generated
```

### Comparing `liblnk-20230205/libcthreads/libcthreads_thread_pool.h` & `liblnk-20230716/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_thread_pool.c` & `liblnk-20230716/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_repeating_thread.c` & `liblnk-20230716/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_error.c` & `liblnk-20230716/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/Makefile.am` & `liblnk-20230716/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_unused.h` & `liblnk-20230716/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_condition.h` & `liblnk-20230716/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_definitions.h` & `liblnk-20230716/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_thread.h` & `liblnk-20230716/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_repeating_thread.h` & `liblnk-20230716/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_read_write_lock.c` & `liblnk-20230716/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_mutex.h` & `liblnk-20230716/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_support.h` & `liblnk-20230716/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_thread.c` & `liblnk-20230716/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_mutex.c` & `liblnk-20230716/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_types.h` & `liblnk-20230716/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_lock.h` & `liblnk-20230716/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_extern.h` & `liblnk-20230716/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_error.h` & `liblnk-20230716/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_queue.c` & `liblnk-20230716/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_condition.c` & `liblnk-20230716/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/Makefile.in` & `liblnk-20230716/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_thread_attributes.c` & `liblnk-20230716/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_libcerror.h` & `liblnk-20230716/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_lock.c` & `liblnk-20230716/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_support.c` & `liblnk-20230716/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_read_write_lock.h` & `liblnk-20230716/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_thread_attributes.h` & `liblnk-20230716/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcthreads/libcthreads_queue.h` & `liblnk-20230716/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/info_handle.c` & `liblnk-20230716/lnktools/info_handle.c`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 #include "lnktools_libcerror.h"
 #include "lnktools_libclocale.h"
 #include "lnktools_libfdatetime.h"
 #include "lnktools_libfguid.h"
 #include "lnktools_libfwps.h"
 #include "lnktools_libfwsi.h"
 #include "lnktools_liblnk.h"
+#include "path_string.h"
 #include "property_store.h"
 #include "shell_items.h"
 
 #define INFO_HANDLE_NOTIFY_STREAM	stdout
 
 /* Prints the file attribute flags to the notify stream
  */
@@ -697,14 +698,84 @@
 		libfguid_identifier_free(
 		 &guid,
 		 NULL );
 	}
 	return( -1 );
 }
 
+/* Prints a path string
+ * Returns 1 if successful or -1 on error
+ */
+int info_handle_path_string_value_fprint(
+     info_handle_t *info_handle,
+     const system_character_t *value_string,
+     size_t value_string_length,
+     libcerror_error_t **error )
+{
+	system_character_t *escaped_value_string = NULL;
+	static char *function                    = "info_handle_path_string_value_fprint";
+	size_t escaped_value_string_size         = 0;
+
+	if( info_handle == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid info handle.",
+		 function );
+
+		return( -1 );
+	}
+	if( path_string_copy_from_file_entry_path(
+	     &escaped_value_string,
+	     &escaped_value_string_size,
+	     value_string,
+	     value_string_length,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy path from file entry path.",
+		 function );
+
+		goto on_error;
+	}
+	if( escaped_value_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: missing escaped value string.",
+		 function );
+
+		goto on_error;
+	}
+	fprintf(
+	 info_handle->notify_stream,
+	 "%" PRIs_SYSTEM "",
+	 escaped_value_string );
+
+	memory_free(
+	 escaped_value_string );
+
+	return( 1 );
+
+on_error:
+	if( escaped_value_string != NULL )
+	{
+		memory_free(
+		 escaped_value_string );
+	}
+	return( -1 );
+}
+
 /* Prints the data flags
  * Returns 1 if successful or -1 on error
  */
 int info_handle_data_flags_fprint(
      info_handle_t *info_handle,
      libcerror_error_t **error )
 {
@@ -1157,15 +1228,15 @@
 			 function );
 
 			goto on_error;
 		}
 		else if( ( result != 0 )
 		      && ( value_string_size > 0 ) )
 		{
-			if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+			if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 				 "%s: invalid volume label string size value exceeds maximum.",
 				 function );
@@ -1241,15 +1312,15 @@
 			 function );
 
 			goto on_error;
 		}
 		else if( ( result != 0 )
 		      && ( value_string_size > 0 ) )
 		{
-			if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+			if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 				 "%s: invalid local path string size value exceeds maximum.",
 				 function );
@@ -1292,16 +1363,34 @@
 				 "%s: unable to retrieve local path.",
 				 function );
 
 				goto on_error;
 			}
 			fprintf(
 			 info_handle->notify_stream,
-			 "\tLocal path\t\t\t: %" PRIs_SYSTEM "\n",
-			 value_string );
+			 "\tLocal path\t\t\t: " );
+
+			if( info_handle_path_string_value_fprint(
+			     info_handle,
+			     value_string,
+			     value_string_size - 1,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print local path string.",
+				 function );
+
+				goto on_error;
+			}
+			fprintf(
+			 info_handle->notify_stream,
+			 "\n" );
 
 			memory_free(
 			 value_string );
 
 			value_string = NULL;
 		}
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
@@ -1325,15 +1414,15 @@
 			 function );
 
 			goto on_error;
 		}
 		else if( ( result != 0 )
 		      && ( value_string_size > 0 ) )
 		{
-			if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+			if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 			{
 				libcerror_error_set(
 				 error,
 				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 				 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 				 "%s: invalid network path string size value exceeds maximum.",
 				 function );
@@ -1376,16 +1465,34 @@
 				 "%s: unable to retrieve local path.",
 				 function );
 
 				goto on_error;
 			}
 			fprintf(
 			 info_handle->notify_stream,
-			 "\tNetwork path\t\t\t: %" PRIs_SYSTEM "\n",
-			 value_string );
+			 "\tNetwork path\t\t\t: " );
+
+			if( info_handle_path_string_value_fprint(
+			     info_handle,
+			     value_string,
+			     value_string_size - 1,
+			     error ) != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+				 "%s: unable to print network path string.",
+				 function );
+
+				goto on_error;
+			}
+			fprintf(
+			 info_handle->notify_stream,
+			 "\n" );
 
 			memory_free(
 			 value_string );
 
 			value_string = NULL;
 		}
 	}
@@ -1444,15 +1551,15 @@
 		 function );
 
 		goto on_error;
 	}
 	else if( ( result != 0 )
 	      && ( value_string_size > 0 ) )
 	{
-		if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+		if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 			 "%s: invalid description string size value exceeds maximum.",
 			 function );
@@ -1562,15 +1669,15 @@
 		 function );
 
 		goto on_error;
 	}
 	else if( ( result != 0 )
 	      && ( value_string_size > 0 ) )
 	{
-		if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+		if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 			 "%s: invalid relative path string size value exceeds maximum.",
 			 function );
@@ -1613,16 +1720,34 @@
 			 "%s: unable to retrieve relative path.",
 			 function );
 
 			goto on_error;
 		}
 		fprintf(
 		 info_handle->notify_stream,
-		 "\tRelative path\t\t\t: %" PRIs_SYSTEM "\n",
-		 value_string );
+		 "\tRelative path\t\t\t: " );
+
+		if( info_handle_path_string_value_fprint(
+		     info_handle,
+		     value_string,
+		     value_string_size - 1,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+			 "%s: unable to print relative path string.",
+			 function );
+
+			goto on_error;
+		}
+		fprintf(
+		 info_handle->notify_stream,
+		 "\n" );
 
 		memory_free(
 		 value_string );
 
 		value_string = NULL;
 	}
 	return( 1 );
@@ -1680,15 +1805,15 @@
 		 function );
 
 		goto on_error;
 	}
 	else if( ( result != 0 )
 	      && ( value_string_size > 0 ) )
 	{
-		if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+		if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 			 "%s: invalid working directory string size value exceeds maximum.",
 			 function );
@@ -1731,16 +1856,34 @@
 			 "%s: unable to retrieve working directory.",
 			 function );
 
 			goto on_error;
 		}
 		fprintf(
 		 info_handle->notify_stream,
-		 "\tWorking directory\t\t: %" PRIs_SYSTEM "\n",
-		 value_string );
+		 "\tWorking directory\t\t: " );
+
+		if( info_handle_path_string_value_fprint(
+		     info_handle,
+		     value_string,
+		     value_string_size - 1,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+			 "%s: unable to print working directory string.",
+			 function );
+
+			goto on_error;
+		}
+		fprintf(
+		 info_handle->notify_stream,
+		 "\n" );
 
 		memory_free(
 		 value_string );
 
 		value_string = NULL;
 	}
 	return( 1 );
@@ -1798,15 +1941,15 @@
 		 function );
 
 		goto on_error;
 	}
 	else if( ( result != 0 )
 	      && ( value_string_size > 0 ) )
 	{
-		if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+		if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 			 "%s: invalid command line arguments string size value exceeds maximum.",
 			 function );
@@ -1849,16 +1992,34 @@
 			 "%s: unable to retrieve command line arguments.",
 			 function );
 
 			goto on_error;
 		}
 		fprintf(
 		 info_handle->notify_stream,
-		 "\tCommand line arguments\t\t: %" PRIs_SYSTEM "\n",
-		 value_string );
+		 "\tCommand line arguments\t\t: " );
+
+		if( info_handle_path_string_value_fprint(
+		     info_handle,
+		     value_string,
+		     value_string_size - 1,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+			 "%s: unable to print command line arguments string.",
+			 function );
+
+			goto on_error;
+		}
+		fprintf(
+		 info_handle->notify_stream,
+		 "\n" );
 
 		memory_free(
 		 value_string );
 
 		value_string = NULL;
 	}
 	return( 1 );
@@ -1916,15 +2077,15 @@
 		 function );
 
 		goto on_error;
 	}
 	else if( ( result != 0 )
 	      && ( value_string_size > 0 ) )
 	{
-		if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+		if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 			 "%s: invalid icon location string size value exceeds maximum.",
 			 function );
@@ -1967,16 +2128,34 @@
 			 "%s: unable to retrieve icon location.",
 			 function );
 
 			goto on_error;
 		}
 		fprintf(
 		 info_handle->notify_stream,
-		 "\tIcon location\t\t\t: %" PRIs_SYSTEM "\n",
-		 value_string );
+		 "\tIcon location\t\t\t: " );
+
+		if( info_handle_path_string_value_fprint(
+		     info_handle,
+		     value_string,
+		     value_string_size - 1,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+			 "%s: unable to print icon location string.",
+			 function );
+
+			goto on_error;
+		}
+		fprintf(
+		 info_handle->notify_stream,
+		 "\n" );
 
 		memory_free(
 		 value_string );
 
 		value_string = NULL;
 	}
 	return( 1 );
@@ -2274,17 +2453,15 @@
 	}
 	fprintf(
 	 info_handle->notify_stream,
 	 "\n" );
 
 	switch( signature )
 	{
-		case LIBLNK_DATA_BLOCK_SIGNATURE_ENVIRONMENT_VARIABLES_LOCATION:
 		case LIBLNK_DATA_BLOCK_SIGNATURE_DARWIN_PROPERTIES:
-		case LIBLNK_DATA_BLOCK_SIGNATURE_ICON_LOCATION:
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
 			result = liblnk_strings_data_block_get_utf16_string_size(
 				  data_block,
 				  &value_string_size,
 				  error );
 #else
 			result = liblnk_strings_data_block_get_utf8_string_size(
@@ -2301,15 +2478,15 @@
 				 "%s: unable to retrieve strings data block string size.",
 				 function );
 
 				goto on_error;
 			}
 			else if( value_string_size > 0 )
 			{
-				if( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE )
+				if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
 					 "%s: invalid strings data block string size value exceeds maximum.",
 					 function );
@@ -2366,14 +2543,123 @@
 			}
 			fprintf(
 			 info_handle->notify_stream,
 			 "\n" );
 
 			break;
 
+		case LIBLNK_DATA_BLOCK_SIGNATURE_ENVIRONMENT_VARIABLES_LOCATION:
+		case LIBLNK_DATA_BLOCK_SIGNATURE_ICON_LOCATION:
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+			result = liblnk_strings_data_block_get_utf16_path_string_size(
+				  data_block,
+				  &value_string_size,
+				  error );
+#else
+			result = liblnk_strings_data_block_get_utf8_path_string_size(
+				  data_block,
+				  &value_string_size,
+				  error );
+#endif
+			if( result != 1 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+				 "%s: unable to retrieve strings data block string size.",
+				 function );
+
+				goto on_error;
+			}
+			else if( value_string_size > 0 )
+			{
+				if( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) )
+				{
+					libcerror_error_set(
+					 error,
+					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+					 LIBCERROR_RUNTIME_ERROR_VALUE_EXCEEDS_MAXIMUM,
+					 "%s: invalid strings data block string size value exceeds maximum.",
+					 function );
+
+					goto on_error;
+				}
+				value_string = system_string_allocate(
+						value_string_size );
+
+				if( value_string == NULL )
+				{
+					libcerror_error_set(
+					 error,
+					 LIBCERROR_ERROR_DOMAIN_MEMORY,
+					 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+					 "%s: unable to create strings data block string.",
+					 function );
+
+					goto on_error;
+				}
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+				result = liblnk_strings_data_block_get_utf16_path_string(
+					  data_block,
+					  (uint16_t *) value_string,
+					  value_string_size,
+					  error );
+#else
+				result = liblnk_strings_data_block_get_utf8_path_string(
+					  data_block,
+					  (uint8_t *) value_string,
+					  value_string_size,
+					  error );
+#endif
+				if( result != 1 )
+				{
+					libcerror_error_set(
+					 error,
+					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+					 "%s: unable to retrieve strings data block string.",
+					 function );
+
+					goto on_error;
+				}
+				fprintf(
+				 info_handle->notify_stream,
+				 "\tString\t\t\t\t: " );
+
+				if( info_handle_path_string_value_fprint(
+				     info_handle,
+				     value_string,
+				     value_string_size - 1,
+				     error ) != 1 )
+				{
+					libcerror_error_set(
+					 error,
+					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+					 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+					 "%s: unable to print strings data block string.",
+					 function );
+
+					goto on_error;
+				}
+				fprintf(
+				 info_handle->notify_stream,
+				 "\n" );
+
+				memory_free(
+				 value_string );
+
+				value_string = NULL;
+			}
+			fprintf(
+			 info_handle->notify_stream,
+			 "\n" );
+
+			break;
+
 		case LIBLNK_DATA_BLOCK_SIGNATURE_DISTRIBUTED_LINK_TRACKER_PROPERTIES:
 			if( info_handle_distributed_link_tracking_data_block_fprint(
 			     info_handle,
 			     data_block,
 			     error ) != 1 )
 			{
 				libcerror_error_set(
@@ -2469,15 +2755,15 @@
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve machine identifier string size.",
 		 function );
 
 		goto on_error;
 	}
 	if( ( value_string_size == 0 )
-	 || ( value_string_size > MEMORY_MAXIMUM_ALLOCATION_SIZE ) )
+	 || ( value_string_size > ( (size_t) MEMORY_MAXIMUM_ALLOCATION_SIZE / sizeof( system_character_t ) ) ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 		 "%s: invalid machine identifier size value out of bounds.",
 		 function );
```

### Comparing `liblnk-20230205/lnktools/lnktools_liblnk.h` & `liblnk-20230716/lnktools/lnktools_liblnk.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_libfdatetime.h` & `liblnk-20230716/lnktools/lnktools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/shell_items.h` & `liblnk-20230716/lnktools/shell_items.h`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 extern "C" {
 #endif
 
 void shell_items_file_attribute_flags_fprint(
       uint32_t file_attribute_flags,
       FILE *notify_stream );
 
+int shell_items_path_string_fprint(
+     const system_character_t *file_entry_path,
+     size_t file_entry_path_length,
+     FILE *notify_stream,
+     libcerror_error_t **error );
+
 int shell_items_extension_block_fprint(
      libfwsi_extension_block_t *extension_block,
      int extension_block_index,
      FILE *notify_stream,
      libcerror_error_t **error );
 
 int shell_items_file_entry_extension_fprint(
```

### Comparing `liblnk-20230205/lnktools/property_store.h` & `liblnk-20230716/lnktools/lnktools_output.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Property store functions
+ * Common output functions for the lnktools
  *
  * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -15,43 +15,41 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _PROPERTY_STORE_H )
-#define _PROPERTY_STORE_H
+#if !defined( _LNKTOOLS_OUTPUT_H )
+#define _LNKTOOLS_OUTPUT_H
 
 #include <common.h>
 #include <file_stream.h>
 #include <types.h>
 
-#include "lnktools_libfwps.h"
+#include "lnktools_libcerror.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int property_store_record_fprint(
-     const uint8_t *property_set_identifier,
-     const system_character_t *property_set_identifier_string,
-     libfwps_record_t *property_record,
-     FILE *notify_stream,
+int lnktools_output_initialize(
+     int stdio_mode,
      libcerror_error_t **error );
 
-int property_store_set_fprint(
-     libfwps_set_t *property_set,
-     FILE *notify_stream,
-     libcerror_error_t **error );
+void lnktools_output_copyright_fprint(
+      FILE *stream );
 
-int property_store_fprint(
-     libfwps_store_t *property_store,
-     FILE *notify_stream,
-     libcerror_error_t **error );
+void lnktools_output_version_fprint(
+      FILE *stream,
+      const char *program );
+
+void lnktools_output_version_detailed_fprint(
+      FILE *stream,
+      const char *program );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _PROPERTY_STORE_H ) */
+#endif /* !defined( _LNKTOOLS_OUTPUT_H ) */
```

### Comparing `liblnk-20230205/lnktools/Makefile.am` & `liblnk-20230716/lnktools/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 	lnktools_libfwps.h \
 	lnktools_libfwsi.h \
 	lnktools_liblnk.h \
 	lnktools_libuna.h \
 	lnktools_output.c lnktools_output.h \
 	lnktools_signal.c lnktools_signal.h \
 	lnktools_unused.h \
+	path_string.c path_string.h \
 	property_store.c property_store.h \
 	shell_items.c shell_items.h
 
 lnkinfo_LDADD = \
 	@LIBFWSI_LIBADD@ \
 	@LIBFWPS_LIBADD@ \
 	@LIBFOLE_LIBADD@ \
```

### Comparing `liblnk-20230205/lnktools/lnktools_libbfio.h` & `liblnk-20230716/lnktools/lnktools_libbfio.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_getopt.c` & `liblnk-20230716/lnktools/lnktools_getopt.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_unused.h` & `liblnk-20230716/lnktools/lnktools_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_libcnotify.h` & `liblnk-20230716/lnktools/lnktools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_libfwsi.h` & `liblnk-20230716/lnktools/lnktools_libfwsi.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_libfwps.h` & `liblnk-20230716/lnktools/lnktools_libfwps.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_libclocale.h` & `liblnk-20230716/lnktools/lnktools_libclocale.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/property_store.c` & `liblnk-20230716/lnktools/property_store.c`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 #include <types.h>
 #include <wide_string.h>
 
 #include "lnktools_libcerror.h"
 #include "lnktools_libfdatetime.h"
 #include "lnktools_libfguid.h"
 #include "lnktools_libfwps.h"
+#include "lnktools_libuna.h"
+#include "path_string.h"
 #include "property_store.h"
 
 /* 446d16b1-8dad-4870-a748-402ea43d788c */
 uint8_t property_store_format_class_identifier_system1[ 16 ] = {
 	0xb1, 0x16, 0x6d, 0x44, 0xad, 0x8d, 0x70, 0x48, 0xa7, 0x48, 0x40, 0x2e, 0xa4, 0x3d, 0x78, 0x8c };
 
 /* b725f130-47ef-101a-a5f1-02608c9eebac */
@@ -61,14 +63,73 @@
 uint8_t property_store_format_class_identifier_tile[ 16 ] = {
 	0x4d, 0x0b, 0xd4, 0x86, 0x69, 0x90, 0x3c, 0x44, 0x81, 0x9a, 0x2a, 0x54, 0x09, 0x0d, 0xcc, 0xec };
 
 /* fb8d2d7b-90d1-4e34-bf60-6eac09922bbf */
 uint8_t property_store_format_class_identifier_winx_hash[ 16 ] = {
 	0x7b, 0x2d, 0x8d, 0xfb, 0xd1, 0x90, 0x34, 0x4e, 0xbf, 0x60, 0x6e, 0xac, 0x09, 0x92, 0x2b, 0xbf };
 
+/* Prints a path string
+ * Returns 1 if successful or -1 on error
+ */
+int property_store_path_string_fprint(
+     const system_character_t *file_entry_path,
+     size_t file_entry_path_length,
+     FILE *notify_stream,
+     libcerror_error_t **error )
+{
+	system_character_t *escaped_path_string = NULL;
+	static char *function                   = "property_store_path_string_print";
+	size_t escaped_path_string_size         = 0;
+
+	if( path_string_copy_from_file_entry_path(
+	     &escaped_path_string,
+	     &escaped_path_string_size,
+	     file_entry_path,
+	     file_entry_path_length,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy path from file entry path.",
+		 function );
+
+		goto on_error;
+	}
+	if( escaped_path_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: missing escaped path string.",
+		 function );
+
+		goto on_error;
+	}
+	fprintf(
+	 notify_stream,
+	 " %" PRIs_SYSTEM "",
+	 escaped_path_string );
+
+	memory_free(
+	 escaped_path_string );
+
+	return( 1 );
+
+on_error:
+	if( escaped_path_string != NULL )
+	{
+		memory_free(
+		 escaped_path_string );
+	}
+	return( -1 );
+}
+
 /* Prints the property record to the notify stream
  * Returns 1 if successful or -1 on error
  */
 int property_store_record_fprint(
      const uint8_t *property_set_identifier,
      const system_character_t *property_set_identifier_string,
      libfwps_record_t *property_record,
@@ -89,14 +150,15 @@
 	uint64_t value_64bit              = 0;
 	uint32_t entry_type               = 0;
 	uint32_t value_32bit              = 0;
 	uint32_t value_type               = 0;
 	uint16_t value_16bit              = 0;
 	uint8_t value_8bit                = 0;
 	double value_floating_point       = 0.0;
+	int is_path_string                = 0;
 	int result                        = 0;
 
 	if( property_set_identifier == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -147,15 +209,16 @@
 			switch( entry_type )
 			{
 				case 4:
 					description = "PKEY_ItemTypeText";
 					break;
 
 				case 10:
-					description = "PKEY_ItemNameDisplay";
+					description    = "PKEY_ItemNameDisplay";
+					is_path_string = 1;
 					break;
 
 				case 14:
 					description = "PKEY_DateModified";
 					break;
 
 				case 15:
@@ -261,15 +324,16 @@
 		          property_set_identifier,
 		          property_store_format_class_identifier_system4,
 		          16 ) == 0 )
 		{
 			switch( entry_type )
 			{
 				case 30:
-					description = "PKEY_ParsingPath";
+					description    = "PKEY_ParsingPath";
+					is_path_string = 1;
 					break;
 
 				default:
 					break;
 			}
 		}
 		else if( memory_compare(
@@ -605,86 +669,175 @@
 			 value_floating_point );
 
 			break;
 
 		case LIBFWPS_VALUE_TYPE_BINARY_STRING:
 		case LIBFWPS_VALUE_TYPE_STRING_ASCII:
 		case LIBFWPS_VALUE_TYPE_STRING_UNICODE:
+			if( is_path_string == 0 )
+			{
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-			result = libfwps_record_get_data_as_utf16_string_size(
-			          property_record,
-				  &value_string_size,
-				  error );
+				result = libfwps_record_get_data_as_utf16_string_size(
+				          property_record,
+					  &value_string_size,
+					  error );
 #else
-			result = libfwps_record_get_data_as_utf8_string_size(
-			          property_record,
-				  &value_string_size,
-				  error );
+				result = libfwps_record_get_data_as_utf8_string_size(
+				          property_record,
+					  &value_string_size,
+					  error );
 #endif
-			if( result == -1 )
-			{
-				libcerror_error_set(
-				 error,
-				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-				 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-				 "%s: unable to retrieve value string size.",
-				 function );
-
-				goto on_error;
-			}
-			if( ( result != 0 )
-			 && ( value_string_size > 0 ) )
-			{
-				value_string = system_string_allocate(
-				                value_string_size );
-
-				if( value_string == NULL )
+				if( result == -1 )
 				{
 					libcerror_error_set(
 					 error,
-					 LIBCERROR_ERROR_DOMAIN_MEMORY,
-					 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
-					 "%s: unable to create value string.",
+					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+					 "%s: unable to retrieve value string size.",
 					 function );
 
 					goto on_error;
 				}
+				if( ( result != 0 )
+				 && ( value_string_size > 0 ) )
+				{
+					value_string = system_string_allocate(
+					                value_string_size );
+
+					if( value_string == NULL )
+					{
+						libcerror_error_set(
+						 error,
+						 LIBCERROR_ERROR_DOMAIN_MEMORY,
+						 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+						 "%s: unable to create value string.",
+						 function );
+
+						goto on_error;
+					}
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+					result = libfwps_record_get_data_as_utf16_string(
+					          property_record,
+						  (uint16_t *) value_string,
+						  value_string_size,
+						  error );
+#else
+					result = libfwps_record_get_data_as_utf8_string(
+					          property_record,
+						  (uint8_t *) value_string,
+						  value_string_size,
+						  error );
+#endif
+					if( result == -1 )
+					{
+						libcerror_error_set(
+						 error,
+						 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+						 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+						 "%s: unable to retrieve value string.",
+						 function );
+
+						goto on_error;
+					}
+					fprintf(
+					 notify_stream,
+					 " %" PRIs_SYSTEM "",
+					 value_string );
+
+					memory_free(
+					 value_string );
+
+					value_string = NULL;
+				}
+			}
+			else
+			{
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
-				result = libfwps_record_get_data_as_utf16_string(
+				result = libfwps_record_get_data_as_utf16_path_string_size(
 				          property_record,
-					  (uint16_t *) value_string,
-					  value_string_size,
+					  &value_string_size,
 					  error );
 #else
-				result = libfwps_record_get_data_as_utf8_string(
+				result = libfwps_record_get_data_as_utf8_path_string_size(
 				          property_record,
-					  (uint8_t *) value_string,
-					  value_string_size,
+					  &value_string_size,
 					  error );
 #endif
 				if( result == -1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-					 "%s: unable to retrieve value string.",
+					 "%s: unable to retrieve path string size.",
 					 function );
 
 					goto on_error;
 				}
-				fprintf(
-				 notify_stream,
-				 " %" PRIs_SYSTEM "",
-				 value_string );
+				if( ( result != 0 )
+				 && ( value_string_size > 0 ) )
+				{
+					value_string = system_string_allocate(
+					                value_string_size );
+
+					if( value_string == NULL )
+					{
+						libcerror_error_set(
+						 error,
+						 LIBCERROR_ERROR_DOMAIN_MEMORY,
+						 LIBCERROR_MEMORY_ERROR_INSUFFICIENT,
+						 "%s: unable to create path string.",
+						 function );
 
-				memory_free(
-				 value_string );
+						goto on_error;
+					}
+#if defined( HAVE_WIDE_SYSTEM_CHARACTER )
+					result = libfwps_record_get_data_as_utf16_path_string(
+					          property_record,
+						  (uint16_t *) value_string,
+						  value_string_size,
+						  error );
+#else
+					result = libfwps_record_get_data_as_utf8_path_string(
+					          property_record,
+						  (uint8_t *) value_string,
+						  value_string_size,
+						  error );
+#endif
+					if( result == -1 )
+					{
+						libcerror_error_set(
+						 error,
+						 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+						 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+						 "%s: unable to retrieve path string.",
+						 function );
+
+						goto on_error;
+					}
+					if( property_store_path_string_fprint(
+					     value_string,
+					     value_string_size - 1,
+					     notify_stream,
+					     error ) != 1 )
+					{
+						libcerror_error_set(
+						 error,
+						 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+						 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+						 "%s: unable to print path string.",
+						 function );
+
+						goto on_error;
+					}
+					memory_free(
+					 value_string );
 
-				value_string = NULL;
+					value_string = NULL;
+				}
 			}
 			break;
 
 		case LIBFWPS_VALUE_TYPE_FILETIME:
 			if( libfwps_record_get_data_as_filetime(
 			     property_record,
 			     &value_64bit,
```

### Comparing `liblnk-20230205/lnktools/shell_items.c` & `liblnk-20230716/lnktools/shell_items.c`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 #include <wide_string.h>
 
 #include "lnktools_libcerror.h"
 #include "lnktools_libfdatetime.h"
 #include "lnktools_libfguid.h"
 #include "lnktools_libfwsi.h"
 #include "lnktools_libuna.h"
+#include "path_string.h"
 #include "shell_items.h"
 
 /* Prints the file attribute flags to the notify stream
  */
 void shell_items_file_attribute_flags_fprint(
       uint32_t file_attribute_flags,
       FILE *notify_stream )
@@ -130,14 +131,73 @@
 	{
 		fprintf(
 		 notify_stream,
 		 "\t\t\tIs virtual (FILE_ATTRIBUTE_VIRTUAL)\n" );
 	}
 }
 
+/* Prints a path string
+ * Returns 1 if successful or -1 on error
+ */
+int shell_items_path_string_fprint(
+     const system_character_t *file_entry_path,
+     size_t file_entry_path_length,
+     FILE *notify_stream,
+     libcerror_error_t **error )
+{
+	system_character_t *escaped_path_string = NULL;
+	static char *function                   = "shell_items_path_string_print";
+	size_t escaped_path_string_size         = 0;
+
+	if( path_string_copy_from_file_entry_path(
+	     &escaped_path_string,
+	     &escaped_path_string_size,
+	     file_entry_path,
+	     file_entry_path_length,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_COPY_FAILED,
+		 "%s: unable to copy path from file entry path.",
+		 function );
+
+		goto on_error;
+	}
+	if( escaped_path_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: missing escaped path string.",
+		 function );
+
+		goto on_error;
+	}
+	fprintf(
+	 notify_stream,
+	 "%" PRIs_SYSTEM "",
+	 escaped_path_string );
+
+	memory_free(
+	 escaped_path_string );
+
+	return( 1 );
+
+on_error:
+	if( escaped_path_string != NULL )
+	{
+		memory_free(
+		 escaped_path_string );
+	}
+	return( -1 );
+}
+
 /* Prints the extension block to the notify stream
  * Returns 1 if successful or -1 on error
  */
 int shell_items_extension_block_fprint(
      libfwsi_extension_block_t *extension_block,
      int extension_block_index,
      FILE *notify_stream,
@@ -289,16 +349,34 @@
 			 "%s: unable to retrieve long name.",
 			 function );
 
 			goto on_error;
 		}
 		fprintf(
 		 notify_stream,
-		 "\t\tLong name\t\t: %" PRIs_SYSTEM "\n",
-		 value_string );
+		 "\t\tLong name\t\t: " );
+
+		if( shell_items_path_string_fprint(
+		     value_string,
+		     value_string_size - 1,
+		     notify_stream,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+			 "%s: unable to print name string.",
+			 function );
+
+			goto on_error;
+		}
+		fprintf(
+		 notify_stream,
+		 "\n" );
 
 		memory_free(
 		 value_string );
 
 		value_string = NULL;
 	}
 #if defined( HAVE_WIDE_SYSTEM_CHARACTER )
@@ -1277,16 +1355,34 @@
 			 "%s: unable to retrieve name.",
 			 function );
 
 			goto on_error;
 		}
 		fprintf(
 		 notify_stream,
-		 "\t\tName\t\t\t: %" PRIs_SYSTEM "\n",
-		 value_string );
+		 "\t\tName\t\t\t: " );
+
+		if( shell_items_path_string_fprint(
+		     value_string,
+		     value_string_size - 1,
+		     notify_stream,
+		     error ) != 1 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
+			 "%s: unable to print name string.",
+			 function );
+
+			goto on_error;
+		}
+		fprintf(
+		 notify_stream,
+		 "\n" );
 
 		memory_free(
 		 value_string );
 
 		value_string = NULL;
 	}
 	if( libfdatetime_fat_date_time_initialize(
```

### Comparing `liblnk-20230205/lnktools/lnktools_output.h` & `liblnk-20230716/lnktools/path_string.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Common output functions for the lnktools
+ * Path string functions
  *
  * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
@@ -15,41 +15,32 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LNKTOOLS_OUTPUT_H )
-#define _LNKTOOLS_OUTPUT_H
+#if !defined( _PATH_STRING_H )
+#define _PATH_STRING_H
 
 #include <common.h>
-#include <file_stream.h>
 #include <types.h>
 
 #include "lnktools_libcerror.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int lnktools_output_initialize(
-     int stdio_mode,
+int path_string_copy_from_file_entry_path(
+     system_character_t **path,
+     size_t *path_size,
+     const system_character_t *file_entry_path,
+     size_t file_entry_path_length,
      libcerror_error_t **error );
 
-void lnktools_output_copyright_fprint(
-      FILE *stream );
-
-void lnktools_output_version_fprint(
-      FILE *stream,
-      const char *program );
-
-void lnktools_output_version_detailed_fprint(
-      FILE *stream,
-      const char *program );
-
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LNKTOOLS_OUTPUT_H ) */
+#endif /* !defined( _PATH_STRING_H ) */
```

### Comparing `liblnk-20230205/lnktools/lnktools_i18n.h` & `liblnk-20230716/lnktools/lnktools_i18n.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/info_handle.h` & `liblnk-20230716/lnktools/info_handle.h`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,20 @@
 
 int info_handle_guid_value_fprint(
      info_handle_t *info_handle,
      const char *value_name,
      const uint8_t *guid_data,
      libcerror_error_t **error );
 
+int info_handle_path_string_value_fprint(
+     info_handle_t *info_handle,
+     const system_character_t *value_string,
+     size_t value_string_length,
+     libcerror_error_t **error );
+
 int info_handle_data_flags_fprint(
      info_handle_t *info_handle,
      libcerror_error_t **error );
 
 int info_handle_link_information_fprint(
      info_handle_t *info_handle,
      libcerror_error_t **error );
```

### Comparing `liblnk-20230205/lnktools/lnktools_output.c` & `liblnk-20230716/lnktools/lnktools_output.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/Makefile.in` & `liblnk-20230716/lnktools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
 CONFIG_HEADER = $(top_builddir)/common/config.h
 CONFIG_CLEAN_FILES =
 CONFIG_CLEAN_VPATH_FILES =
 am__installdirs = "$(DESTDIR)$(bindir)"
 PROGRAMS = $(bin_PROGRAMS)
 am_lnkinfo_OBJECTS = info_handle.$(OBJEXT) lnkinfo.$(OBJEXT) \
 	lnktools_getopt.$(OBJEXT) lnktools_output.$(OBJEXT) \
-	lnktools_signal.$(OBJEXT) property_store.$(OBJEXT) \
-	shell_items.$(OBJEXT)
+	lnktools_signal.$(OBJEXT) path_string.$(OBJEXT) \
+	property_store.$(OBJEXT) shell_items.$(OBJEXT)
 lnkinfo_OBJECTS = $(am_lnkinfo_OBJECTS)
 lnkinfo_DEPENDENCIES = ../liblnk/liblnk.la
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 AM_V_P = $(am__v_P_@AM_V@)
@@ -143,15 +143,16 @@
 am__v_at_1 = 
 DEFAULT_INCLUDES = -I.@am__isrc@ -I$(top_builddir)/common
 depcomp = $(SHELL) $(top_srcdir)/depcomp
 am__maybe_remake_depfiles = depfiles
 am__depfiles_remade = ./$(DEPDIR)/info_handle.Po \
 	./$(DEPDIR)/lnkinfo.Po ./$(DEPDIR)/lnktools_getopt.Po \
 	./$(DEPDIR)/lnktools_output.Po ./$(DEPDIR)/lnktools_signal.Po \
-	./$(DEPDIR)/property_store.Po ./$(DEPDIR)/shell_items.Po
+	./$(DEPDIR)/path_string.Po ./$(DEPDIR)/property_store.Po \
+	./$(DEPDIR)/shell_items.Po
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
 	$(AM_CFLAGS) $(CFLAGS)
@@ -568,14 +569,15 @@
 	lnktools_libfwps.h \
 	lnktools_libfwsi.h \
 	lnktools_liblnk.h \
 	lnktools_libuna.h \
 	lnktools_output.c lnktools_output.h \
 	lnktools_signal.c lnktools_signal.h \
 	lnktools_unused.h \
+	path_string.c path_string.h \
 	property_store.c property_store.h \
 	shell_items.c shell_items.h
 
 lnkinfo_LDADD = \
 	@LIBFWSI_LIBADD@ \
 	@LIBFWPS_LIBADD@ \
 	@LIBFOLE_LIBADD@ \
@@ -686,14 +688,15 @@
 	-rm -f *.tab.c
 
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/info_handle.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnkinfo.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnktools_getopt.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnktools_output.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/lnktools_signal.Po@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/path_string.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/property_store.Po@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/shell_items.Po@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
@@ -897,14 +900,15 @@
 
 maintainer-clean: maintainer-clean-am
 		-rm -f ./$(DEPDIR)/info_handle.Po
 	-rm -f ./$(DEPDIR)/lnkinfo.Po
 	-rm -f ./$(DEPDIR)/lnktools_getopt.Po
 	-rm -f ./$(DEPDIR)/lnktools_output.Po
 	-rm -f ./$(DEPDIR)/lnktools_signal.Po
+	-rm -f ./$(DEPDIR)/path_string.Po
 	-rm -f ./$(DEPDIR)/property_store.Po
 	-rm -f ./$(DEPDIR)/shell_items.Po
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
```

### Comparing `liblnk-20230205/lnktools/lnktools_signal.h` & `liblnk-20230716/lnktools/lnktools_signal.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_libfguid.h` & `liblnk-20230716/lnktools/lnktools_libfguid.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnkinfo.c` & `liblnk-20230716/lnktools/lnkinfo.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_signal.c` & `liblnk-20230716/lnktools/lnktools_signal.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_libuna.h` & `liblnk-20230716/lnktools/lnktools_libuna.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_libcerror.h` & `liblnk-20230716/lnktools/lnktools_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/lnktools/lnktools_getopt.h` & `liblnk-20230716/lnktools/lnktools_getopt.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk-python3/Makefile.am` & `liblnk-20230716/pylnk-python3/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 	pylnk_guid.c pylnk_guid.h \
 	pylnk_integer.c pylnk_integer.h \
 	pylnk_libbfio.h \
 	pylnk_libcerror.h \
 	pylnk_libclocale.h \
 	pylnk_libfguid.h \
 	pylnk_liblnk.h \
+	pylnk_libuna.h \
 	pylnk_python.h \
+	pylnk_string.c pylnk_string.h \
 	pylnk_strings_data_block.c pylnk_strings_data_block.h \
 	pylnk_unused.h
 
 pyexec_LTLIBRARIES = pylnk.la
 
 nodist_pylnk_la_SOURCES = $(BUILT_SOURCES)
```

### Comparing `liblnk-20230205/pylnk-python3/Makefile.in` & `liblnk-20230716/pylnk-python3/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 @HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_drive_types.lo \
 @HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_error.lo \
 @HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_file.lo \
 @HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_file_attribute_flags.lo \
 @HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_file_object_io_handle.lo \
 @HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_guid.lo \
 @HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_integer.lo \
+@HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_string.lo \
 @HAVE_PYTHON3_TRUE@	pylnk_la-pylnk_strings_data_block.lo
 @HAVE_PYTHON3_TRUE@nodist_pylnk_la_OBJECTS = $(am__objects_1)
 pylnk_la_OBJECTS = $(nodist_pylnk_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
@@ -194,14 +195,15 @@
 	./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_error.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_guid.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_integer.Plo \
+	./$(DEPDIR)/pylnk_la-pylnk_string.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
@@ -621,15 +623,17 @@
 @HAVE_PYTHON3_TRUE@	pylnk_guid.c pylnk_guid.h \
 @HAVE_PYTHON3_TRUE@	pylnk_integer.c pylnk_integer.h \
 @HAVE_PYTHON3_TRUE@	pylnk_libbfio.h \
 @HAVE_PYTHON3_TRUE@	pylnk_libcerror.h \
 @HAVE_PYTHON3_TRUE@	pylnk_libclocale.h \
 @HAVE_PYTHON3_TRUE@	pylnk_libfguid.h \
 @HAVE_PYTHON3_TRUE@	pylnk_liblnk.h \
+@HAVE_PYTHON3_TRUE@	pylnk_libuna.h \
 @HAVE_PYTHON3_TRUE@	pylnk_python.h \
+@HAVE_PYTHON3_TRUE@	pylnk_string.c pylnk_string.h \
 @HAVE_PYTHON3_TRUE@	pylnk_strings_data_block.c pylnk_strings_data_block.h \
 @HAVE_PYTHON3_TRUE@	pylnk_unused.h
 
 @HAVE_PYTHON3_TRUE@pyexec_LTLIBRARIES = pylnk.la
 @HAVE_PYTHON3_TRUE@nodist_pylnk_la_SOURCES = $(BUILT_SOURCES)
 @HAVE_PYTHON3_TRUE@pylnk_la_LIBADD = \
 @HAVE_PYTHON3_TRUE@	@LIBCERROR_LIBADD@ \
@@ -737,14 +741,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_error.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_integer.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_string.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
@@ -864,14 +869,21 @@
 pylnk_la-pylnk_integer.lo: pylnk_integer.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_integer.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_integer.Tpo -c -o pylnk_la-pylnk_integer.lo `test -f 'pylnk_integer.c' || echo '$(srcdir)/'`pylnk_integer.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_integer.Tpo $(DEPDIR)/pylnk_la-pylnk_integer.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_integer.c' object='pylnk_la-pylnk_integer.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_integer.lo `test -f 'pylnk_integer.c' || echo '$(srcdir)/'`pylnk_integer.c
 
+pylnk_la-pylnk_string.lo: pylnk_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_string.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_string.Tpo -c -o pylnk_la-pylnk_string.lo `test -f 'pylnk_string.c' || echo '$(srcdir)/'`pylnk_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_string.Tpo $(DEPDIR)/pylnk_la-pylnk_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_string.c' object='pylnk_la-pylnk_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_string.lo `test -f 'pylnk_string.c' || echo '$(srcdir)/'`pylnk_string.c
+
 pylnk_la-pylnk_strings_data_block.lo: pylnk_strings_data_block.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_strings_data_block.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Tpo -c -o pylnk_la-pylnk_strings_data_block.lo `test -f 'pylnk_strings_data_block.c' || echo '$(srcdir)/'`pylnk_strings_data_block.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Tpo $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_strings_data_block.c' object='pylnk_la-pylnk_strings_data_block.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_strings_data_block.lo `test -f 'pylnk_strings_data_block.c' || echo '$(srcdir)/'`pylnk_strings_data_block.c
 
@@ -1066,14 +1078,15 @@
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_error.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_guid.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_integer.Plo
+	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_string.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
```

### Comparing `liblnk-20230205/config.sub` & `liblnk-20230716/config.sub`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_unused.h` & `liblnk-20230716/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_support.c` & `liblnk-20230716/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_libclocale.h` & `liblnk-20230716/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/Makefile.am` & `liblnk-20230716/libcpath/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_error.h` & `liblnk-20230716/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_system_string.h` & `liblnk-20230716/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_error.c` & `liblnk-20230716/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_libcsplit.h` & `liblnk-20230716/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_path.h` & `liblnk-20230716/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/Makefile.in` & `liblnk-20230716/libcpath/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_definitions.h` & `liblnk-20230716/libcpath/libcpath_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_libcerror.h` & `liblnk-20230716/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_extern.h` & `liblnk-20230716/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_path.c` & `liblnk-20230716/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_system_string.c` & `liblnk-20230716/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_support.h` & `liblnk-20230716/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcpath/libcpath_libuna.h` & `liblnk-20230716/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/manuals/lnkinfo.1` & `liblnk-20230716/manuals/lnkinfo.1`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/manuals/liblnk.3` & `liblnk-20230716/manuals/liblnk.3`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.Dd February  4, 2023
+.Dd July 16, 2023
 .Dt liblnk 3
 .Os liblnk
 .Sh NAME
 .Nm liblnk.h
 .Nd Library to access the Windows Shortcut File (LNK) format
 .Sh SYNOPSIS
 .In liblnk.h
@@ -194,14 +194,22 @@
 .Fn liblnk_strings_data_block_get_utf8_string_size "liblnk_data_block_t *data_block" "size_t *utf8_string_size" "liblnk_error_t **error"
 .Ft int
 .Fn liblnk_strings_data_block_get_utf8_string "liblnk_data_block_t *data_block" "uint8_t *utf8_string" "size_t utf8_string_size" "liblnk_error_t **error"
 .Ft int
 .Fn liblnk_strings_data_block_get_utf16_string_size "liblnk_data_block_t *data_block" "size_t *utf16_string_size" "liblnk_error_t **error"
 .Ft int
 .Fn liblnk_strings_data_block_get_utf16_string "liblnk_data_block_t *data_block" "uint16_t *utf16_string" "size_t utf16_string_size" "liblnk_error_t **error"
+.Ft int
+.Fn liblnk_strings_data_block_get_utf8_path_string_size "liblnk_data_block_t *data_block" "size_t *utf8_string_size" "liblnk_error_t **error"
+.Ft int
+.Fn liblnk_strings_data_block_get_utf8_path_string "liblnk_data_block_t *data_block" "uint8_t *utf8_string" "size_t utf8_string_size" "liblnk_error_t **error"
+.Ft int
+.Fn liblnk_strings_data_block_get_utf16_path_string_size "liblnk_data_block_t *data_block" "size_t *utf16_string_size" "liblnk_error_t **error"
+.Ft int
+.Fn liblnk_strings_data_block_get_utf16_path_string "liblnk_data_block_t *data_block" "uint16_t *utf16_string" "size_t utf16_string_size" "liblnk_error_t **error"
 .Pp
 Distributed link tracking data block functions
 .Ft int
 .Fn liblnk_distributed_link_tracking_data_block_get_utf8_machine_identifier_size "liblnk_data_block_t *data_block" "size_t *utf8_string_size" "liblnk_error_t **error"
 .Ft int
 .Fn liblnk_distributed_link_tracking_data_block_get_utf8_machine_identifier "liblnk_data_block_t *data_block" "uint8_t *utf8_string" "size_t utf8_string_size" "liblnk_error_t **error"
 .Ft int
```

### Comparing `liblnk-20230205/manuals/Makefile.in` & `liblnk-20230716/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libfwps/libfwps.vcproj` & `liblnk-20230716/msvscpp/libfwps/libfwps.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_special_folder_location/lnk_test_special_folder_location.vcproj` & `liblnk-20230716/msvscpp/lnk_test_special_folder_location/lnk_test_special_folder_location.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libfole/libfole.vcproj` & `liblnk-20230716/msvscpp/libfole/libfole.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/pylnk/pylnk.vcproj` & `liblnk-20230716/msvscpp/pylnk/pylnk.vcproj`

 * *Files 5% similar despite different names*

#### Comparing `liblnk-20230205/msvscpp/pylnk/pylnk.vcproj` & `liblnk-20230716/msvscpp/pylnk/pylnk.vcproj`

```diff
@@ -7,15 +7,15 @@
   <Configurations>
     <Configuration Name="Release|Win32" OutputDirectory="$(SolutionDir)$(ConfigurationName)" IntermediateDirectory="$(ConfigurationName)" ConfigurationType="2" CharacterSet="1">
       <Tool Name="VCPreBuildEventTool"/>
       <Tool Name="VCCustomBuildTool"/>
       <Tool Name="VCXMLDataGeneratorTool"/>
       <Tool Name="VCWebServiceProxyGeneratorTool"/>
       <Tool Name="VCMIDLTool"/>
-      <Tool Name="VCCLCompilerTool" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libcsplit;..\..\libuna;..\..\libcfile;..\..\libcpath;..\..\libbfio;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBCSPLIT;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBCFILE;HAVE_LOCAL_LIBCPATH;HAVE_LOCAL_LIBBFIO;HAVE_LOCAL_LIBFGUID;LIBLNK_DLL_IMPORT" RuntimeLibrary="2" WarningLevel="4" CompileAs="1"/>
+      <Tool Name="VCCLCompilerTool" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libcsplit;..\..\libuna;..\..\libcfile;..\..\libcpath;..\..\libbfio;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_PYCONFIG_H;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBCSPLIT;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBCFILE;HAVE_LOCAL_LIBCPATH;HAVE_LOCAL_LIBBFIO;HAVE_LOCAL_LIBFGUID;LIBLNK_DLL_IMPORT" RuntimeLibrary="2" WarningLevel="4" CompileAs="1"/>
       <Tool Name="VCManagedResourceCompilerTool"/>
       <Tool Name="VCResourceCompilerTool"/>
       <Tool Name="VCPreLinkEventTool"/>
       <Tool Name="VCLinkerTool" OutputFile="$(OutDir)\$(ProjectName).pyd" AdditionalLibraryDirectories="&quot;$(OutDir)&quot;;C:\Python27\libs" RandomizedBaseAddress="2" DataExecutionPrevention="2" TargetMachine="1" ImportLibrary="$(OutDir)\$(ProjectName).lib"/>
       <Tool Name="VCALinkTool"/>
       <Tool Name="VCManifestTool"/>
       <Tool Name="VCXDCMakeTool"/>
@@ -26,15 +26,15 @@
     </Configuration>
     <Configuration Name="VSDebug|Win32" OutputDirectory="$(SolutionDir)$(ConfigurationName)" IntermediateDirectory="$(ConfigurationName)" ConfigurationType="2" CharacterSet="1">
       <Tool Name="VCPreBuildEventTool"/>
       <Tool Name="VCCustomBuildTool"/>
       <Tool Name="VCXMLDataGeneratorTool"/>
       <Tool Name="VCWebServiceProxyGeneratorTool"/>
       <Tool Name="VCMIDLTool"/>
-      <Tool Name="VCCLCompilerTool" Optimization="0" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libcsplit;..\..\libuna;..\..\libcfile;..\..\libcpath;..\..\libbfio;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBCSPLIT;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBCFILE;HAVE_LOCAL_LIBCPATH;HAVE_LOCAL_LIBBFIO;HAVE_LOCAL_LIBFGUID;LIBLNK_DLL_IMPORT" BasicRuntimeChecks="3" SmallerTypeCheck="true" RuntimeLibrary="3" WarningLevel="4" DebugInformationFormat="3" CompileAs="1"/>
+      <Tool Name="VCCLCompilerTool" Optimization="0" AdditionalIncludeDirectories="..\..\include;..\..\common;..\..\libcerror;..\..\libcdata;..\..\libclocale;..\..\libcsplit;..\..\libuna;..\..\libcfile;..\..\libcpath;..\..\libbfio;..\..\libfguid;C:\Python27\include" PreprocessorDefinitions="_CRT_SECURE_NO_DEPRECATE;HAVE_PYCONFIG_H;HAVE_LOCAL_LIBCERROR;HAVE_LOCAL_LIBCDATA;HAVE_LOCAL_LIBCLOCALE;HAVE_LOCAL_LIBCSPLIT;HAVE_LOCAL_LIBUNA;HAVE_LOCAL_LIBCFILE;HAVE_LOCAL_LIBCPATH;HAVE_LOCAL_LIBBFIO;HAVE_LOCAL_LIBFGUID;LIBLNK_DLL_IMPORT" BasicRuntimeChecks="3" SmallerTypeCheck="true" RuntimeLibrary="3" WarningLevel="4" DebugInformationFormat="3" CompileAs="1"/>
       <Tool Name="VCManagedResourceCompilerTool"/>
       <Tool Name="VCResourceCompilerTool"/>
       <Tool Name="VCPreLinkEventTool"/>
       <Tool Name="VCLinkerTool" OutputFile="$(OutDir)\$(ProjectName).pyd" AdditionalLibraryDirectories="&quot;$(OutDir)&quot;;C:\Python27\libs" GenerateDebugInformation="true" RandomizedBaseAddress="1" DataExecutionPrevention="1" TargetMachine="1" ImportLibrary="$(OutDir)\$(ProjectName).lib"/>
       <Tool Name="VCALinkTool"/>
       <Tool Name="VCManifestTool"/>
       <Tool Name="VCXDCMakeTool"/>
@@ -57,14 +57,15 @@
       <File RelativePath="..\..\pylnk\pylnk_drive_types.c"/>
       <File RelativePath="..\..\pylnk\pylnk_error.c"/>
       <File RelativePath="..\..\pylnk\pylnk_file.c"/>
       <File RelativePath="..\..\pylnk\pylnk_file_attribute_flags.c"/>
       <File RelativePath="..\..\pylnk\pylnk_file_object_io_handle.c"/>
       <File RelativePath="..\..\pylnk\pylnk_guid.c"/>
       <File RelativePath="..\..\pylnk\pylnk_integer.c"/>
+      <File RelativePath="..\..\pylnk\pylnk_string.c"/>
       <File RelativePath="..\..\pylnk\pylnk_strings_data_block.c"/>
     </Filter>
     <Filter Name="Header Files" Filter="h;hpp;hxx;hm;inl;inc;xsd" UniqueIdentifier="{93995380-89BD-4b04-88EB-625FBE52EBFB}">
       <File RelativePath="..\..\pylnk\pylnk.h"/>
       <File RelativePath="..\..\pylnk\pylnk_codepage.h"/>
       <File RelativePath="..\..\pylnk\pylnk_data_block.h"/>
       <File RelativePath="..\..\pylnk\pylnk_data_blocks.h"/>
@@ -79,15 +80,17 @@
       <File RelativePath="..\..\pylnk\pylnk_guid.h"/>
       <File RelativePath="..\..\pylnk\pylnk_integer.h"/>
       <File RelativePath="..\..\pylnk\pylnk_libbfio.h"/>
       <File RelativePath="..\..\pylnk\pylnk_libcerror.h"/>
       <File RelativePath="..\..\pylnk\pylnk_libclocale.h"/>
       <File RelativePath="..\..\pylnk\pylnk_libfguid.h"/>
       <File RelativePath="..\..\pylnk\pylnk_liblnk.h"/>
+      <File RelativePath="..\..\pylnk\pylnk_libuna.h"/>
       <File RelativePath="..\..\pylnk\pylnk_python.h"/>
+      <File RelativePath="..\..\pylnk\pylnk_string.h"/>
       <File RelativePath="..\..\pylnk\pylnk_strings_data_block.h"/>
       <File RelativePath="..\..\pylnk\pylnk_unused.h"/>
     </Filter>
     <Filter Name="Resource Files" Filter="rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav" UniqueIdentifier="{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}"/>
   </Files>
   <Globals/>
 </VisualStudioProject>
```

### Comparing `liblnk-20230205/msvscpp/libfguid/libfguid.vcproj` & `liblnk-20230716/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_support/lnk_test_support.vcproj` & `liblnk-20230716/msvscpp/lnk_test_support/lnk_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_location_information/lnk_test_location_information.vcproj` & `liblnk-20230716/msvscpp/lnk_test_location_information/lnk_test_location_information.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libclocale/libclocale.vcproj` & `liblnk-20230716/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_file/lnk_test_file.vcproj` & `liblnk-20230716/msvscpp/lnk_test_file/lnk_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/Makefile.am` & `liblnk-20230716/msvscpp/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 	lnk_test_link_target_identifier/lnk_test_link_target_identifier.vcproj \
 	lnk_test_location_information/lnk_test_location_information.vcproj \
 	lnk_test_notify/lnk_test_notify.vcproj \
 	lnk_test_special_folder_location/lnk_test_special_folder_location.vcproj \
 	lnk_test_support/lnk_test_support.vcproj \
 	lnk_test_tools_info_handle/lnk_test_tools_info_handle.vcproj \
 	lnk_test_tools_output/lnk_test_tools_output.vcproj \
+	lnk_test_tools_path_string/lnk_test_tools_path_string.vcproj \
 	lnk_test_tools_signal/lnk_test_tools_signal.vcproj \
 	lnkinfo/lnkinfo.vcproj \
 	pylnk/pylnk.vcproj \
 	liblnk.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
```

### Comparing `liblnk-20230205/msvscpp/libbfio/libbfio.vcproj` & `liblnk-20230716/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_tools_output/lnk_test_tools_output.vcproj` & `liblnk-20230716/msvscpp/lnk_test_tools_output/lnk_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_link_target_identifier/lnk_test_link_target_identifier.vcproj` & `liblnk-20230716/msvscpp/lnk_test_link_target_identifier/lnk_test_link_target_identifier.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_data_string/lnk_test_data_string.vcproj` & `liblnk-20230716/msvscpp/lnk_test_data_string/lnk_test_data_string.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_notify/lnk_test_notify.vcproj` & `liblnk-20230716/msvscpp/lnk_test_notify/lnk_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_tools_signal/lnk_test_tools_signal.vcproj` & `liblnk-20230716/msvscpp/lnk_test_tools_signal/lnk_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_error/lnk_test_error.vcproj` & `liblnk-20230716/msvscpp/lnk_test_error/lnk_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libfdatetime/libfdatetime.vcproj` & `liblnk-20230716/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libcfile/libcfile.vcproj` & `liblnk-20230716/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libcthreads/libcthreads.vcproj` & `liblnk-20230716/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libcpath/libcpath.vcproj` & `liblnk-20230716/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/liblnk.sln` & `liblnk-20230716/msvscpp/liblnk.sln`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,21 @@
 EndProject
 Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "lnk_test_tools_output", "lnk_test_tools_output\lnk_test_tools_output.vcproj", "{A87ACAF1-6398-4F34-B928-D5F152EC77EE}"
 	ProjectSection(ProjectDependencies) = postProject
 		{460AAFDF-4A19-4187-9A48-F11A78D3BD79} = {460AAFDF-4A19-4187-9A48-F11A78D3BD79}
 		{BD3A95FA-A3DE-4B79-A889-A7E5ECA4B69C} = {BD3A95FA-A3DE-4B79-A889-A7E5ECA4B69C}
 	EndProjectSection
 EndProject
+Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "lnk_test_tools_path_string", "lnk_test_tools_path_string\lnk_test_tools_path_string.vcproj", "{3FEA089C-DC89-46A5-9883-8F2CCFDBD381}"
+	ProjectSection(ProjectDependencies) = postProject
+		{BC27FF34-C859-4A1A-95D6-FC89952E1910} = {BC27FF34-C859-4A1A-95D6-FC89952E1910}
+		{460AAFDF-4A19-4187-9A48-F11A78D3BD79} = {460AAFDF-4A19-4187-9A48-F11A78D3BD79}
+		{BD3A95FA-A3DE-4B79-A889-A7E5ECA4B69C} = {BD3A95FA-A3DE-4B79-A889-A7E5ECA4B69C}
+	EndProjectSection
+EndProject
 Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "lnk_test_tools_signal", "lnk_test_tools_signal\lnk_test_tools_signal.vcproj", "{2F0AF625-C1AC-4B9E-A8ED-F14221D02FEC}"
 	ProjectSection(ProjectDependencies) = postProject
 		{460AAFDF-4A19-4187-9A48-F11A78D3BD79} = {460AAFDF-4A19-4187-9A48-F11A78D3BD79}
 		{BD3A95FA-A3DE-4B79-A889-A7E5ECA4B69C} = {BD3A95FA-A3DE-4B79-A889-A7E5ECA4B69C}
 	EndProjectSection
 EndProject
 Project("{8BC9CEB8-8B4A-11D0-8D11-00A0C91BC942}") = "libclocale", "libclocale\libclocale.vcproj", "{CEDF8919-00B2-4D8A-88CC-84ADB2D2FF89}"
@@ -371,14 +378,18 @@
 		{D0F8EDC2-037E-492B-9CE7-6E5AC75178E2}.Release|Win32.Build.0 = Release|Win32
 		{D0F8EDC2-037E-492B-9CE7-6E5AC75178E2}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
 		{D0F8EDC2-037E-492B-9CE7-6E5AC75178E2}.VSDebug|Win32.Build.0 = VSDebug|Win32
 		{A87ACAF1-6398-4F34-B928-D5F152EC77EE}.Release|Win32.ActiveCfg = Release|Win32
 		{A87ACAF1-6398-4F34-B928-D5F152EC77EE}.Release|Win32.Build.0 = Release|Win32
 		{A87ACAF1-6398-4F34-B928-D5F152EC77EE}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
 		{A87ACAF1-6398-4F34-B928-D5F152EC77EE}.VSDebug|Win32.Build.0 = VSDebug|Win32
+		{3FEA089C-DC89-46A5-9883-8F2CCFDBD381}.Release|Win32.ActiveCfg = Release|Win32
+		{3FEA089C-DC89-46A5-9883-8F2CCFDBD381}.Release|Win32.Build.0 = Release|Win32
+		{3FEA089C-DC89-46A5-9883-8F2CCFDBD381}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
+		{3FEA089C-DC89-46A5-9883-8F2CCFDBD381}.VSDebug|Win32.Build.0 = VSDebug|Win32
 		{2F0AF625-C1AC-4B9E-A8ED-F14221D02FEC}.Release|Win32.ActiveCfg = Release|Win32
 		{2F0AF625-C1AC-4B9E-A8ED-F14221D02FEC}.Release|Win32.Build.0 = Release|Win32
 		{2F0AF625-C1AC-4B9E-A8ED-F14221D02FEC}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
 		{2F0AF625-C1AC-4B9E-A8ED-F14221D02FEC}.VSDebug|Win32.Build.0 = VSDebug|Win32
 		{CEDF8919-00B2-4D8A-88CC-84ADB2D2FF89}.Release|Win32.ActiveCfg = Release|Win32
 		{CEDF8919-00B2-4D8A-88CC-84ADB2D2FF89}.Release|Win32.Build.0 = Release|Win32
 		{CEDF8919-00B2-4D8A-88CC-84ADB2D2FF89}.VSDebug|Win32.ActiveCfg = VSDebug|Win32
```

### Comparing `liblnk-20230205/msvscpp/lnk_test_known_folder_location/lnk_test_known_folder_location.vcproj` & `liblnk-20230716/msvscpp/lnk_test_known_folder_location/lnk_test_known_folder_location.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/liblnk/liblnk.vcproj` & `liblnk-20230716/msvscpp/liblnk/liblnk.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libuna/libuna.vcproj` & `liblnk-20230716/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libfwsi/libfwsi.vcproj` & `liblnk-20230716/msvscpp/libfwsi/libfwsi.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_distributed_link_tracker_properties/lnk_test_distributed_link_tracker_properties.vcproj` & `liblnk-20230716/msvscpp/lnk_test_distributed_link_tracker_properties/lnk_test_distributed_link_tracker_properties.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_file_header/lnk_test_file_header.vcproj` & `liblnk-20230716/msvscpp/lnk_test_file_header/lnk_test_file_header.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/Makefile.in` & `liblnk-20230716/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -506,14 +506,15 @@
 	lnk_test_link_target_identifier/lnk_test_link_target_identifier.vcproj \
 	lnk_test_location_information/lnk_test_location_information.vcproj \
 	lnk_test_notify/lnk_test_notify.vcproj \
 	lnk_test_special_folder_location/lnk_test_special_folder_location.vcproj \
 	lnk_test_support/lnk_test_support.vcproj \
 	lnk_test_tools_info_handle/lnk_test_tools_info_handle.vcproj \
 	lnk_test_tools_output/lnk_test_tools_output.vcproj \
+	lnk_test_tools_path_string/lnk_test_tools_path_string.vcproj \
 	lnk_test_tools_signal/lnk_test_tools_signal.vcproj \
 	lnkinfo/lnkinfo.vcproj \
 	pylnk/pylnk.vcproj \
 	liblnk.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
```

### Comparing `liblnk-20230205/msvscpp/lnk_test_io_handle/lnk_test_io_handle.vcproj` & `liblnk-20230716/msvscpp/lnk_test_io_handle/lnk_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libcerror/libcerror.vcproj` & `liblnk-20230716/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnk_test_data_block/lnk_test_data_block.vcproj` & `liblnk-20230716/msvscpp/lnk_test_data_block/lnk_test_data_block.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libcnotify/libcnotify.vcproj` & `liblnk-20230716/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/lnkinfo/lnkinfo.vcproj` & `liblnk-20230716/msvscpp/lnkinfo/lnkinfo.vcproj`

 * *Files 2% similar despite different names*

#### Comparing `liblnk-20230205/msvscpp/lnkinfo/lnkinfo.vcproj` & `liblnk-20230716/msvscpp/lnkinfo/lnkinfo.vcproj`

```diff
@@ -48,14 +48,15 @@
   <Files>
     <Filter Name="Source Files" Filter="cpp;c;cc;cxx;def;odl;idl;hpj;bat;asm;asmx" UniqueIdentifier="{4FC737F1-C7A5-4376-A066-2A32D752A2FF}">
       <File RelativePath="..\..\lnktools\info_handle.c"/>
       <File RelativePath="..\..\lnktools\lnkinfo.c"/>
       <File RelativePath="..\..\lnktools\lnktools_getopt.c"/>
       <File RelativePath="..\..\lnktools\lnktools_output.c"/>
       <File RelativePath="..\..\lnktools\lnktools_signal.c"/>
+      <File RelativePath="..\..\lnktools\path_string.c"/>
       <File RelativePath="..\..\lnktools\property_store.c"/>
       <File RelativePath="..\..\lnktools\shell_items.c"/>
     </Filter>
     <Filter Name="Header Files" Filter="h;hpp;hxx;hm;inl;inc;xsd" UniqueIdentifier="{93995380-89BD-4b04-88EB-625FBE52EBFB}">
       <File RelativePath="..\..\lnktools\info_handle.h"/>
       <File RelativePath="..\..\lnktools\lnktools_getopt.h"/>
       <File RelativePath="..\..\lnktools\lnktools_i18n.h"/>
@@ -68,14 +69,15 @@
       <File RelativePath="..\..\lnktools\lnktools_libfwps.h"/>
       <File RelativePath="..\..\lnktools\lnktools_libfwsi.h"/>
       <File RelativePath="..\..\lnktools\lnktools_liblnk.h"/>
       <File RelativePath="..\..\lnktools\lnktools_libuna.h"/>
       <File RelativePath="..\..\lnktools\lnktools_output.h"/>
       <File RelativePath="..\..\lnktools\lnktools_signal.h"/>
       <File RelativePath="..\..\lnktools\lnktools_unused.h"/>
+      <File RelativePath="..\..\lnktools\path_string.h"/>
       <File RelativePath="..\..\lnktools\property_store.h"/>
       <File RelativePath="..\..\lnktools\shell_items.h"/>
     </Filter>
     <Filter Name="Resource Files" Filter="rc;ico;cur;bmp;dlg;rc2;rct;bin;rgs;gif;jpg;jpeg;jpe;resx;tiff;tif;png;wav" UniqueIdentifier="{67DA6AB6-F800-4c08-8B7A-83BB121AAD01}"/>
   </Files>
   <Globals/>
 </VisualStudioProject>
```

### Comparing `liblnk-20230205/msvscpp/lnk_test_tools_info_handle/lnk_test_tools_info_handle.vcproj` & `liblnk-20230716/msvscpp/lnk_test_tools_info_handle/lnk_test_tools_info_handle.vcproj`

 * *Files 2% similar despite different names*

#### Comparing `liblnk-20230205/msvscpp/lnk_test_tools_info_handle/lnk_test_tools_info_handle.vcproj` & `liblnk-20230716/msvscpp/lnk_test_tools_info_handle/lnk_test_tools_info_handle.vcproj`

```diff
@@ -44,21 +44,23 @@
       <Tool Name="VCPostBuildEventTool"/>
     </Configuration>
   </Configurations>
   <References/>
   <Files>
     <Filter Name="Source Files" Filter="cpp;c;cc;cxx;def;odl;idl;hpj;bat;asm;asmx" UniqueIdentifier="{4FC737F1-C7A5-4376-A066-2A32D752A2FF}">
       <File RelativePath="..\..\lnktools\info_handle.c"/>
+      <File RelativePath="..\..\lnktools\path_string.c"/>
       <File RelativePath="..\..\lnktools\property_store.c"/>
       <File RelativePath="..\..\lnktools\shell_items.c"/>
       <File RelativePath="..\..\tests\lnk_test_memory.c"/>
       <File RelativePath="..\..\tests\lnk_test_tools_info_handle.c"/>
     </Filter>
     <Filter Name="Header Files" Filter="h;hpp;hxx;hm;inl;inc;xsd" UniqueIdentifier="{93995380-89BD-4b04-88EB-625FBE52EBFB}">
       <File RelativePath="..\..\lnktools\info_handle.h"/>
+      <File RelativePath="..\..\lnktools\path_string.h"/>
       <File RelativePath="..\..\lnktools\property_store.h"/>
       <File RelativePath="..\..\lnktools\shell_items.h"/>
       <File RelativePath="..\..\tests\lnk_test_libcerror.h"/>
       <File RelativePath="..\..\tests\lnk_test_macros.h"/>
       <File RelativePath="..\..\tests\lnk_test_memory.h"/>
       <File RelativePath="..\..\tests\lnk_test_unused.h"/>
     </Filter>
```

### Comparing `liblnk-20230205/msvscpp/libcdata/libcdata.vcproj` & `liblnk-20230716/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/msvscpp/libcsplit/libcsplit.vcproj` & `liblnk-20230716/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk.spec.in` & `liblnk-20230716/liblnk.spec.in`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Name: liblnk
 Version: @VERSION@
 Release: 1
 Summary: Library to access the Windows Shortcut File (LNK) format
 Group: System Environment/Libraries
-License: LGPLv3+
+License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/liblnk
-BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
 @liblnk_spec_requires@ @ax_libbfio_spec_requires@ @ax_libcdata_spec_requires@ @ax_libcerror_spec_requires@ @ax_libcfile_spec_requires@ @ax_libclocale_spec_requires@ @ax_libcnotify_spec_requires@ @ax_libcpath_spec_requires@ @ax_libcsplit_spec_requires@ @ax_libcthreads_spec_requires@ @ax_libfdatetime_spec_requires@ @ax_libfguid_spec_requires@ @ax_libfole_spec_requires@ @ax_libfwps_spec_requires@ @ax_libfwsi_spec_requires@ @ax_libuna_spec_requires@
 BuildRequires: gcc @ax_libbfio_spec_build_requires@ @ax_libcdata_spec_build_requires@ @ax_libcerror_spec_build_requires@ @ax_libcfile_spec_build_requires@ @ax_libclocale_spec_build_requires@ @ax_libcnotify_spec_build_requires@ @ax_libcpath_spec_build_requires@ @ax_libcsplit_spec_build_requires@ @ax_libcthreads_spec_build_requires@ @ax_libfdatetime_spec_build_requires@ @ax_libfguid_spec_build_requires@ @ax_libfole_spec_build_requires@ @ax_libfwps_spec_build_requires@ @ax_libfwsi_spec_build_requires@ @ax_libuna_spec_build_requires@
 
 %description -n liblnk
 Library to access the Windows Shortcut File (LNK) format
 
 %package -n liblnk-static
@@ -61,45 +60,40 @@
 rm -rf %{buildroot}
 
 %post -p /sbin/ldconfig
 
 %postun -p /sbin/ldconfig
 
 %files -n liblnk
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.so.*
+%{_libdir}/*.so.*
 
 %files -n liblnk-static
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_libdir}/*.a
+%{_libdir}/*.a
 
 %files -n liblnk-devel
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/*.so
 %{_libdir}/pkgconfig/liblnk.pc
 %{_includedir}/*
 %{_mandir}/man3/*
 
 %files -n liblnk-python3
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %files -n liblnk-tools
-%defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
-%attr(755,root,root) %{_bindir}/*
+%{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
 * @SPEC_DATE@ Joachim Metz <joachim.metz@gmail.com> @VERSION@-1
 - Auto-generated
```

### Comparing `liblnk-20230205/setup.py` & `liblnk-20230716/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 #
 # Script to build and install Python-bindings.
-# Version: 20221217
+# Version: 20230411
 
 from __future__ import print_function
 
 import copy
 import datetime
 import glob
 import gzip
@@ -91,14 +91,15 @@
     build_ext.build_extensions(self)
 
   def run(self):
     """Runs the build extension."""
     compiler = new_compiler(compiler=self.compiler)
     if compiler.compiler_type == "msvc":
       self.define = [
+          ("_CRT_SECURE_NO_WARNINGS", ""),
           ("UNICODE", ""),
       ]
 
     else:
       command = "sh configure --disable-nls --disable-shared-libs"
       output = self._RunCommand(command)
```

### Comparing `liblnk-20230205/config.guess` & `liblnk-20230716/config.guess`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/ossfuzz/file_fuzzer.cc` & `liblnk-20230716/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/ossfuzz/Makefile.am` & `liblnk-20230716/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/ossfuzz/ossfuzz_liblnk.h` & `liblnk-20230716/ossfuzz/ossfuzz_liblnk.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/ossfuzz/Makefile.in` & `liblnk-20230716/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/ossfuzz/ossfuzz_libbfio.h` & `liblnk-20230716/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_extern.h` & `liblnk-20230716/liblnk/liblnk_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_data_block.c` & `liblnk-20230716/liblnk/liblnk_data_block.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_libuna.h` & `liblnk-20230716/liblnk/liblnk_libuna.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_types.h` & `liblnk-20230716/liblnk/liblnk_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk.rc.in` & `liblnk-20230716/liblnk/liblnk.rc.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_special_folder_location.h` & `liblnk-20230716/liblnk/liblnk_special_folder_location.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_data_string.h` & `liblnk-20230716/liblnk/liblnk_data_string.h`

 * *Files 23% similar despite different names*

```diff
@@ -59,21 +59,23 @@
      libcerror_error_t **error );
 
 int liblnk_data_string_read_data(
      liblnk_data_string_t *data_string,
      liblnk_io_handle_t *io_handle,
      const uint8_t *data,
      size_t data_size,
+     uint32_t encoding_flags,
      libcerror_error_t **error );
 
 int liblnk_data_string_read_file_io_handle(
      liblnk_data_string_t *data_string,
      liblnk_io_handle_t *io_handle,
      libbfio_handle_t *file_io_handle,
      off64_t file_offset,
+     uint32_t encoding_flags,
      libcerror_error_t **error );
 
 int liblnk_data_string_get_utf8_string_size(
      liblnk_data_string_t *data_string,
      int ascii_codepage,
      size_t *utf8_string_size,
      libcerror_error_t **error );
@@ -94,13 +96,39 @@
 int liblnk_data_string_get_utf16_string(
      liblnk_data_string_t *data_string,
      int ascii_codepage,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error );
 
+int liblnk_data_string_get_utf8_path_string_size(
+     liblnk_data_string_t *data_string,
+     int ascii_codepage,
+     size_t *utf8_string_size,
+     libcerror_error_t **error );
+
+int liblnk_data_string_get_utf8_path_string(
+     liblnk_data_string_t *data_string,
+     int ascii_codepage,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error );
+
+int liblnk_data_string_get_utf16_path_string_size(
+     liblnk_data_string_t *data_string,
+     int ascii_codepage,
+     size_t *utf16_string_size,
+     libcerror_error_t **error );
+
+int liblnk_data_string_get_utf16_path_string(
+     liblnk_data_string_t *data_string,
+     int ascii_codepage,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error );
+
 #if defined( __cplusplus )
 }
 #endif
 
 #endif /* !defined( _LIBLNK_DATA_STRING_H ) */
```

### Comparing `liblnk-20230205/liblnk/liblnk_distributed_link_tracker_properties.h` & `liblnk-20230716/liblnk/liblnk_distributed_link_tracker_properties.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_libcerror.h` & `liblnk-20230716/liblnk/liblnk_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/Makefile.am` & `liblnk-20230716/liblnk/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_file_header.c` & `liblnk-20230716/liblnk/liblnk_file_header.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_definitions.h.in` & `liblnk-20230716/liblnk/liblnk_definitions.h.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_location_information.c` & `liblnk-20230716/liblnk/liblnk_location_information.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_support.c` & `liblnk-20230716/liblnk/liblnk_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_unused.h` & `liblnk-20230716/liblnk/liblnk_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_libbfio.h` & `liblnk-20230716/liblnk/liblnk_libbfio.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_known_folder_location.h` & `liblnk-20230716/liblnk/liblnk_known_folder_location.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_data_string.c` & `liblnk-20230716/liblnk/liblnk_data_string.c`

 * *Files 19% similar despite different names*

```diff
@@ -147,14 +147,15 @@
  * Returns 1 if successful or -1 on error
  */
 int liblnk_data_string_read_data(
      liblnk_data_string_t *data_string,
      liblnk_io_handle_t *io_handle,
      const uint8_t *data,
      size_t data_size,
+     uint32_t encoding_flags,
      libcerror_error_t **error )
 {
 	static char *function = "liblnk_data_string_read_data";
 
 	if( data_string == NULL )
 	{
 		libcerror_error_set(
@@ -330,15 +331,15 @@
 			if( data_string->is_unicode != 0 )
 			{
 				if( liblnk_debug_print_utf16_string_value(
 				     function,
 				     "data string\t\t\t",
 				     data_string->data,
 				     data_string->data_size,
-				     LIBUNA_ENDIAN_LITTLE,
+				     LIBUNA_ENDIAN_LITTLE | encoding_flags,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 					 "%s: unable to print UTF-16 string value.",
@@ -389,14 +390,15 @@
  * Returns 1 if successful or -1 on error
  */
 int liblnk_data_string_read_file_io_handle(
      liblnk_data_string_t *data_string,
      liblnk_io_handle_t *io_handle,
      libbfio_handle_t *file_io_handle,
      off64_t file_offset,
+     uint32_t encoding_flags,
      libcerror_error_t **error )
 {
 	uint8_t data_string_size_data[ 2 ];
 
 	static char *function = "liblnk_data_string_read_file_io_handle";
 	ssize_t read_count    = 0;
 
@@ -549,15 +551,15 @@
 			if( data_string->is_unicode != 0 )
 			{
 				if( liblnk_debug_print_utf16_string_value(
 				     function,
 				     "data string\t\t\t",
 				     data_string->data,
 				     data_string->data_size,
-				     LIBUNA_ENDIAN_LITTLE,
+				     LIBUNA_ENDIAN_LITTLE | encoding_flags,
 				     error ) != 1 )
 				{
 					libcerror_error_set(
 					 error,
 					 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 					 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 					 "%s: unable to print UTF-16 string value.",
@@ -600,15 +602,15 @@
 		 data_string->data );
 
 		data_string->data = NULL;
 	}
 	return( -1 );
 }
 
-/* Retrieves the size of the UTF-8 encoded data string
+/* Retrieves the size of the UTF-8 encoded string
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_data_string_get_utf8_string_size(
      liblnk_data_string_t *data_string,
      int ascii_codepage,
      size_t *utf8_string_size,
@@ -670,23 +672,23 @@
 	}
 	if( result != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-		 "%s: unable to retrieve UTF-8 data string size.",
+		 "%s: unable to retrieve UTF-8 string size.",
 		 function );
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
-/* Retrieves the UTF-8 encoded data string
+/* Retrieves the UTF-8 encoded string
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_data_string_get_utf8_string(
      liblnk_data_string_t *data_string,
      int ascii_codepage,
      uint8_t *utf8_string,
@@ -762,23 +764,23 @@
 	}
 	if( result != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
-		 "%s: unable to set UTF-8 data string.",
+		 "%s: unable to set UTF-8 string.",
 		 function );
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
-/* Retrieves the size of the UTF-16 encoded data string
+/* Retrieves the size of the UTF-16 encoded string
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_data_string_get_utf16_string_size(
      liblnk_data_string_t *data_string,
      int ascii_codepage,
      size_t *utf16_string_size,
@@ -840,23 +842,23 @@
 	}
 	if( result != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
-		 "%s: unable to retrieve UTF-16 data string size.",
+		 "%s: unable to retrieve UTF-16 string size.",
 		 function );
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
-/* Retrieves the UTF-16 encoded data string
+/* Retrieves the UTF-16 encoded string
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_data_string_get_utf16_string(
      liblnk_data_string_t *data_string,
      int ascii_codepage,
      uint16_t *utf16_string,
@@ -932,15 +934,359 @@
 	}
 	if( result != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
-		 "%s: unable to set UTF-16 data string.",
+		 "%s: unable to set UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the UTF-8 encoded path string
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
+ * Returns 1 if successful, 0 if value is not available or -1 on error
+ */
+int liblnk_data_string_get_utf8_path_string_size(
+     liblnk_data_string_t *data_string,
+     int ascii_codepage,
+     size_t *utf8_string_size,
+     libcerror_error_t **error )
+{
+	static char *function = "liblnk_data_string_get_utf8_path_string_size";
+	int result            = 0;
+
+	if( data_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data string.",
+		 function );
+
+		return( -1 );
+	}
+	if( data_string->data == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid data string - missing data.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string size.",
+		 function );
+
+		return( -1 );
+	}
+	if( data_string->is_unicode != 0 )
+	{
+		result = libuna_utf8_string_size_from_utf16_stream(
+			  data_string->data,
+			  data_string->data_size,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+			  utf8_string_size,
+			  error );
+	}
+	else
+	{
+		result = libuna_utf8_string_size_from_byte_stream(
+			  data_string->data,
+			  data_string->data_size,
+			  ascii_codepage,
+			  utf8_string_size,
+			  error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve UTF-8 string size.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the UTF-8 encoded path string
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful, 0 if value is not available or -1 on error
+ */
+int liblnk_data_string_get_utf8_path_string(
+     liblnk_data_string_t *data_string,
+     int ascii_codepage,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error )
+{
+	static char *function = "liblnk_data_string_get_utf8_path_string";
+	int result            = 0;
+
+	if( data_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data string.",
+		 function );
+
+		return( -1 );
+	}
+	if( data_string->data == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid data string - missing data.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UTF-8 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( data_string->is_unicode != 0 )
+	{
+		result = libuna_utf8_string_copy_from_utf16_stream(
+			  utf8_string,
+			  utf8_string_size,
+			  data_string->data,
+			  data_string->data_size,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+			  error );
+	}
+	else
+	{
+		result = libuna_utf8_string_copy_from_byte_stream(
+			  utf8_string,
+			  utf8_string_size,
+			  data_string->data,
+			  data_string->data_size,
+			  ascii_codepage,
+			  error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+		 "%s: unable to set UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the UTF-16 encoded path string
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
+ * Returns 1 if successful, 0 if value is not available or -1 on error
+ */
+int liblnk_data_string_get_utf16_path_string_size(
+     liblnk_data_string_t *data_string,
+     int ascii_codepage,
+     size_t *utf16_string_size,
+     libcerror_error_t **error )
+{
+	static char *function = "liblnk_data_string_get_utf16_path_string_size";
+	int result            = 0;
+
+	if( data_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data string.",
+		 function );
+
+		return( -1 );
+	}
+	if( data_string->data == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid data string - missing data.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf16_string_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-16 string size.",
+		 function );
+
+		return( -1 );
+	}
+	if( data_string->is_unicode != 0 )
+	{
+		result = libuna_utf16_string_size_from_utf16_stream(
+			  data_string->data,
+			  data_string->data_size,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+			  utf16_string_size,
+			  error );
+	}
+	else
+	{
+		result = libuna_utf16_string_size_from_byte_stream(
+			  data_string->data,
+			  data_string->data_size,
+			  ascii_codepage,
+			  utf16_string_size,
+			  error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve UTF-16 string size.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the UTF-16 encoded path string
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful, 0 if value is not available or -1 on error
+ */
+int liblnk_data_string_get_utf16_path_string(
+     liblnk_data_string_t *data_string,
+     int ascii_codepage,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error )
+{
+	static char *function = "liblnk_data_string_get_utf16_path_string";
+	int result            = 0;
+
+	if( data_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data string.",
+		 function );
+
+		return( -1 );
+	}
+	if( data_string->data == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid data string - missing data.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf16_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf16_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UTF-16 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( data_string->is_unicode != 0 )
+	{
+		result = libuna_utf16_string_copy_from_utf16_stream(
+			  utf16_string,
+			  utf16_string_size,
+			  data_string->data,
+			  data_string->data_size,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+			  error );
+	}
+	else
+	{
+		result = libuna_utf16_string_copy_from_byte_stream(
+			  utf16_string,
+			  utf16_string_size,
+			  data_string->data,
+			  data_string->data_size,
+			  ascii_codepage,
+			  error );
+	}
+	if( result != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
+		 "%s: unable to set UTF-16 string.",
 		 function );
 
 		return( -1 );
 	}
 	return( 1 );
 }
```

### Comparing `liblnk-20230205/liblnk/liblnk_data_block.h` & `liblnk-20230716/liblnk/liblnk_data_block.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_libfwsi.h` & `liblnk-20230716/liblnk/liblnk_libfwsi.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_link_target_identifier.c` & `liblnk-20230716/liblnk/liblnk_link_target_identifier.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_strings_data_block.c` & `liblnk-20230716/liblnk/liblnk_strings_data_block.c`

 * *Files 15% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 	liblnk_internal_data_block_t *internal_data_block = NULL;
 	const uint8_t *string_data                        = NULL;
 	const uint8_t *unicode_string_data                = NULL;
 	static char *function                             = "liblnk_data_block_strings_read";
 	size_t string_size                                = 0;
 	size_t unicode_string_size                        = 0;
 
+#if defined( HAVE_DEBUG_OUTPUT )
+	uint32_t encoding_flags                           = 0;
+#endif
+
 	if( data_block == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid data block.",
@@ -193,28 +197,33 @@
 	else
 	{
 		unicode_string_size += 2;
 	}
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
+		if( ( internal_data_block->signature == LIBLNK_DATA_BLOCK_SIGNATURE_ENVIRONMENT_VARIABLES_LOCATION )
+		 || ( internal_data_block->signature == LIBLNK_DATA_BLOCK_SIGNATURE_ICON_LOCATION ) )
+		{
+			encoding_flags = LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE;
+		}
 		libcnotify_printf(
 		 "%s: Unicode string data:\n",
 		 function );
 		libcnotify_print_data(
 		 unicode_string_data,
 		 520,
 		 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 
 		if( liblnk_debug_print_utf16_string_value(
 		     function,
 		     "Unicode string\t\t\t\t",
 		     unicode_string_data,
 		     520,
-		     LIBUNA_ENDIAN_LITTLE,
+		     LIBUNA_ENDIAN_LITTLE | encoding_flags,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_PRINT_FAILED,
 			 "%s: unable to print UTF-16 string value.",
@@ -307,16 +316,16 @@
 			 &( internal_data_block->data[ sizeof( lnk_data_block_strings_t ) ] ),
 			 internal_data_block->data_size - sizeof( lnk_data_block_strings_t ),
 			 LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA );
 		}
 	}
 #endif /* defined( HAVE_DEBUG_OUTPUT ) */
 
-	internal_data_block->value          = (intptr_t *) data_string;
-	internal_data_block->free_value     = (int(*)(intptr_t **, libcerror_error_t **)) &liblnk_data_string_free;
+	internal_data_block->value      = (intptr_t *) data_string;
+	internal_data_block->free_value = (int(*)(intptr_t **, libcerror_error_t **)) &liblnk_data_string_free;
 
 	return( 1 );
 
 on_error:
 	if( data_string != NULL )
 	{
 		liblnk_data_string_free(
@@ -627,14 +636,330 @@
 	     (liblnk_data_string_t *) internal_data_block->value,
 	     internal_data_block->ascii_codepage,
 	     utf16_string,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve UTF-16 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the UTF-8 path string
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int liblnk_strings_data_block_get_utf8_path_string_size(
+     liblnk_data_block_t *data_block,
+     size_t *utf8_string_size,
+     libcerror_error_t **error )
+{
+	liblnk_internal_data_block_t *internal_data_block = NULL;
+	static char *function                             = "liblnk_strings_data_block_get_utf8_path_string_size";
+
+	if( data_block == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data block.",
+		 function );
+
+		return( -1 );
+	}
+	internal_data_block = (liblnk_internal_data_block_t *) data_block;
+
+	if( internal_data_block->value == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid data block - missing value.",
+		 function );
+
+		return( -1 );
+	}
+	if( internal_data_block->data_size < 4 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid data block - data size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_data_block->signature != LIBLNK_DATA_BLOCK_SIGNATURE_ENVIRONMENT_VARIABLES_LOCATION )
+	 && ( internal_data_block->signature != LIBLNK_DATA_BLOCK_SIGNATURE_ICON_LOCATION ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid data block - unsupported signature.",
+		 function );
+
+		return( -1 );
+	}
+	if( liblnk_data_string_get_utf8_path_string_size(
+	     (liblnk_data_string_t *) internal_data_block->value,
+	     internal_data_block->ascii_codepage,
+	     utf8_string_size,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve UTF-8 string size.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the UTF-8 path string
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int liblnk_strings_data_block_get_utf8_path_string(
+     liblnk_data_block_t *data_block,
+     uint8_t *utf8_string,
+     size_t utf8_string_size,
+     libcerror_error_t **error )
+{
+	liblnk_internal_data_block_t *internal_data_block = NULL;
+	static char *function                             = "liblnk_strings_data_block_get_utf8_path_string";
+
+	if( data_block == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data block.",
+		 function );
+
+		return( -1 );
+	}
+	internal_data_block = (liblnk_internal_data_block_t *) data_block;
+
+	if( internal_data_block->value == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid data block - missing value.",
+		 function );
+
+		return( -1 );
+	}
+	if( internal_data_block->data_size < 4 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid data block - data size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_data_block->signature != LIBLNK_DATA_BLOCK_SIGNATURE_ENVIRONMENT_VARIABLES_LOCATION )
+	 && ( internal_data_block->signature != LIBLNK_DATA_BLOCK_SIGNATURE_ICON_LOCATION ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid data block - unsupported signature.",
+		 function );
+
+		return( -1 );
+	}
+	if( liblnk_data_string_get_utf8_path_string(
+	     (liblnk_data_string_t *) internal_data_block->value,
+	     internal_data_block->ascii_codepage,
+	     utf8_string,
+	     utf8_string_size,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the size of the UTF-16 path string
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int liblnk_strings_data_block_get_utf16_path_string_size(
+     liblnk_data_block_t *data_block,
+     size_t *utf16_string_size,
+     libcerror_error_t **error )
+{
+	liblnk_internal_data_block_t *internal_data_block = NULL;
+	static char *function                             = "liblnk_strings_data_block_get_utf16_path_string_size";
+
+	if( data_block == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data block.",
+		 function );
+
+		return( -1 );
+	}
+	internal_data_block = (liblnk_internal_data_block_t *) data_block;
+
+	if( internal_data_block->value == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid data block - missing value.",
+		 function );
+
+		return( -1 );
+	}
+	if( internal_data_block->data_size < 4 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid data block - data size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_data_block->signature != LIBLNK_DATA_BLOCK_SIGNATURE_ENVIRONMENT_VARIABLES_LOCATION )
+	 && ( internal_data_block->signature != LIBLNK_DATA_BLOCK_SIGNATURE_ICON_LOCATION ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid data block - unsupported signature.",
+		 function );
+
+		return( -1 );
+	}
+	if( liblnk_data_string_get_utf16_path_string_size(
+	     (liblnk_data_string_t *) internal_data_block->value,
+	     internal_data_block->ascii_codepage,
+	     utf16_string_size,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
+		 "%s: unable to retrieve UTF-16 string size.",
+		 function );
+
+		return( -1 );
+	}
+	return( 1 );
+}
+
+/* Retrieves the UTF-16 path string
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
+ * Returns 1 if successful or -1 on error
+ */
+int liblnk_strings_data_block_get_utf16_path_string(
+     liblnk_data_block_t *data_block,
+     uint16_t *utf16_string,
+     size_t utf16_string_size,
+     libcerror_error_t **error )
+{
+	liblnk_internal_data_block_t *internal_data_block = NULL;
+	static char *function                             = "liblnk_strings_data_block_get_utf16_path_string";
+
+	if( data_block == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid data block.",
+		 function );
+
+		return( -1 );
+	}
+	internal_data_block = (liblnk_internal_data_block_t *) data_block;
+
+	if( internal_data_block->value == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_MISSING,
+		 "%s: invalid data block - missing value.",
+		 function );
+
+		return( -1 );
+	}
+	if( internal_data_block->data_size < 4 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
+		 "%s: invalid data block - data size value out of bounds.",
+		 function );
+
+		return( -1 );
+	}
+	if( ( internal_data_block->signature != LIBLNK_DATA_BLOCK_SIGNATURE_ENVIRONMENT_VARIABLES_LOCATION )
+	 && ( internal_data_block->signature != LIBLNK_DATA_BLOCK_SIGNATURE_ICON_LOCATION ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid data block - unsupported signature.",
+		 function );
+
+		return( -1 );
+	}
+	if( liblnk_data_string_get_utf16_path_string(
+	     (liblnk_data_string_t *) internal_data_block->value,
+	     internal_data_block->ascii_codepage,
+	     utf16_string,
+	     utf16_string_size,
+	     error ) != 1 )
+	{
+		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
 		 "%s: unable to retrieve UTF-16 string.",
 		 function );
 
 		return( -1 );
```

### Comparing `liblnk-20230205/liblnk/liblnk_debug.h` & `liblnk-20230716/liblnk/liblnk_debug.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_location_information.h` & `liblnk-20230716/liblnk/liblnk_location_information.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/lnk_network_share_information.h` & `liblnk-20230716/liblnk/lnk_network_share_information.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_io_handle.c` & `liblnk-20230716/liblnk/liblnk_io_handle.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_distributed_link_tracker_properties.c` & `liblnk-20230716/liblnk/liblnk_distributed_link_tracker_properties.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_libfwps.h` & `liblnk-20230716/liblnk/liblnk_libfwps.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_libfdatetime.h` & `liblnk-20230716/liblnk/liblnk_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_strings_data_block.h` & `liblnk-20230716/libfwsi/libfwsi_volume.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Strings data block functions
+ * Volume (shell item) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,57 +15,67 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBLNK_STRINGS_DATA_BLOCK_H )
-#define _LIBLNK_STRINGS_DATA_BLOCK_H
+#if !defined( _LIBFWSI_VOLUME_H )
+#define _LIBFWSI_VOLUME_H
 
 #include <common.h>
 #include <types.h>
 
-#include "liblnk_extern.h"
-#include "liblnk_libcerror.h"
-#include "liblnk_types.h"
+#include "libfwsi_extern.h"
+#include "libfwsi_libcerror.h"
+#include "libfwsi_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int liblnk_strings_data_block_read(
-     liblnk_data_block_t *data_block,
-     libcerror_error_t **error );
-
-LIBLNK_EXTERN \
-int liblnk_strings_data_block_get_utf8_string_size(
-     liblnk_data_block_t *data_block,
+LIBFWSI_EXTERN \
+int libfwsi_volume_get_utf8_name_size(
+     libfwsi_item_t *volume,
      size_t *utf8_string_size,
      libcerror_error_t **error );
 
-LIBLNK_EXTERN \
-int liblnk_strings_data_block_get_utf8_string(
-     liblnk_data_block_t *data_block,
+LIBFWSI_EXTERN \
+int libfwsi_volume_get_utf8_name(
+     libfwsi_item_t *volume,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libcerror_error_t **error );
 
-LIBLNK_EXTERN \
-int liblnk_strings_data_block_get_utf16_string_size(
-     liblnk_data_block_t *data_block,
+LIBFWSI_EXTERN \
+int libfwsi_volume_get_utf16_name_size(
+     libfwsi_item_t *volume,
      size_t *utf16_string_size,
      libcerror_error_t **error );
 
-LIBLNK_EXTERN \
-int liblnk_strings_data_block_get_utf16_string(
-     liblnk_data_block_t *data_block,
+LIBFWSI_EXTERN \
+int libfwsi_volume_get_utf16_name(
+     libfwsi_item_t *volume,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error );
 
+LIBFWSI_EXTERN \
+int libfwsi_volume_get_identifier(
+     libfwsi_item_t *volume,
+     uint8_t *guid_data,
+     size_t guid_data_size,
+     libcerror_error_t **error );
+
+LIBFWSI_EXTERN \
+int libfwsi_volume_get_shell_folder_identifier(
+     libfwsi_item_t *volume,
+     uint8_t *guid_data,
+     size_t guid_data_size,
+     libcerror_error_t **error );
+
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBLNK_STRINGS_DATA_BLOCK_H ) */
+#endif /* !defined( _LIBFWSI_VOLUME_H ) */
```

### Comparing `liblnk-20230205/liblnk/liblnk_distributed_link_tracking_data_block.h` & `liblnk-20230716/liblnk/liblnk_distributed_link_tracking_data_block.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_distributed_link_tracking_data_block.c` & `liblnk-20230716/liblnk/liblnk_distributed_link_tracking_data_block.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_libcnotify.h` & `liblnk-20230716/liblnk/liblnk_libcnotify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_file.c` & `liblnk-20230716/liblnk/liblnk_file.c`

 * *Files 3% similar despite different names*

```diff
@@ -1293,14 +1293,15 @@
 		}
 #endif
 		if( liblnk_data_string_read_file_io_handle(
 		     internal_file->description,
 		     internal_file->io_handle,
 		     file_io_handle,
 		     file_offset,
+		     0,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_IO,
 			 LIBCERROR_IO_ERROR_READ_FAILED,
 			 "%s: unable to read description data string.",
@@ -1333,14 +1334,15 @@
 		}
 #endif
 		if( liblnk_data_string_read_file_io_handle(
 		     internal_file->relative_path,
 		     internal_file->io_handle,
 		     file_io_handle,
 		     file_offset,
+		     LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_IO,
 			 LIBCERROR_IO_ERROR_READ_FAILED,
 			 "%s: unable to read relative path data string.",
@@ -1373,14 +1375,15 @@
 		}
 #endif
 		if( liblnk_data_string_read_file_io_handle(
 		     internal_file->working_directory,
 		     internal_file->io_handle,
 		     file_io_handle,
 		     file_offset,
+		     LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_IO,
 			 LIBCERROR_IO_ERROR_READ_FAILED,
 			 "%s: unable to read working directory data string.",
@@ -1413,14 +1416,15 @@
 		}
 #endif
 		if( liblnk_data_string_read_file_io_handle(
 		     internal_file->command_line_arguments,
 		     internal_file->io_handle,
 		     file_io_handle,
 		     file_offset,
+		     LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_IO,
 			 LIBCERROR_IO_ERROR_READ_FAILED,
 			 "%s: unable to read command line arguments data string.",
@@ -1453,14 +1457,15 @@
 		}
 #endif
 		if( liblnk_data_string_read_file_io_handle(
 		     internal_file->icon_location,
 		     internal_file->io_handle,
 		     file_io_handle,
 		     file_offset,
+		     LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_IO,
 			 LIBCERROR_IO_ERROR_READ_FAILED,
 			 "%s: unable to read icon location data string.",
@@ -3324,14 +3329,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 encoded local path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_local_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
@@ -3387,15 +3393,15 @@
 		return( 0 );
 	}
 	if( ( internal_file->location_information->string_flags & LIBLNK_LOCATION_INFORMATION_STRING_FLAG_LOCAL_PATH_IS_UNICODE ) != 0 )
 	{
 		result = libuna_utf8_string_size_from_utf16_stream(
 			  internal_file->location_information->local_path,
 			  internal_file->location_information->local_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  &utf8_local_path_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_size_from_byte_stream(
 			  internal_file->location_information->local_path,
@@ -3469,15 +3475,15 @@
 		utf8_local_path_size += 1;
 	}
 	if( ( internal_file->location_information->string_flags & LIBLNK_LOCATION_INFORMATION_STRING_FLAG_COMMON_PATH_IS_UNICODE ) != 0 )
 	{
 		result = libuna_utf8_string_size_from_utf16_stream(
 			  internal_file->location_information->common_path,
 			  internal_file->location_information->common_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  &utf8_common_path_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_size_from_byte_stream(
 			  internal_file->location_information->common_path,
@@ -3499,14 +3505,15 @@
 	}
 	*utf8_string_size = utf8_local_path_size + utf8_common_path_size - 1;
 
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 encoded local path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_local_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
@@ -3576,15 +3583,15 @@
 	{
 		result = libuna_utf8_string_with_index_copy_from_utf16_stream(
 			  utf8_string,
 			  utf8_string_size,
 			  &string_index,
 			  internal_file->location_information->local_path,
 			  internal_file->location_information->local_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_with_index_copy_from_byte_stream(
 			  utf8_string,
 			  utf8_string_size,
@@ -3675,15 +3682,15 @@
 	{
 		result = libuna_utf8_string_with_index_copy_from_utf16_stream(
 			  utf8_string,
 			  utf8_string_size,
 			  &string_index,
 			  internal_file->location_information->common_path,
 			  internal_file->location_information->common_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_with_index_copy_from_byte_stream(
 			  utf8_string,
 			  utf8_string_size,
@@ -3704,14 +3711,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 encoded local path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_local_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
@@ -3767,15 +3775,15 @@
 		return( 0 );
 	}
 	if( ( internal_file->location_information->string_flags & LIBLNK_LOCATION_INFORMATION_STRING_FLAG_LOCAL_PATH_IS_UNICODE ) != 0 )
 	{
 		result = libuna_utf16_string_size_from_utf16_stream(
 			  internal_file->location_information->local_path,
 			  internal_file->location_information->local_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  &utf16_local_path_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_size_from_byte_stream(
 			  internal_file->location_information->local_path,
@@ -3849,15 +3857,15 @@
 		utf16_local_path_size += 1;
 	}
 	if( ( internal_file->location_information->string_flags & LIBLNK_LOCATION_INFORMATION_STRING_FLAG_COMMON_PATH_IS_UNICODE ) != 0 )
 	{
 		result = libuna_utf16_string_size_from_utf16_stream(
 			  internal_file->location_information->common_path,
 			  internal_file->location_information->common_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  &utf16_common_path_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_size_from_byte_stream(
 			  internal_file->location_information->common_path,
@@ -3879,14 +3887,15 @@
 	}
 	*utf16_string_size = utf16_local_path_size + utf16_common_path_size - 1;
 
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 encoded local path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * The local path is only set if the link refers to a file on a local volume
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_local_path(
      liblnk_file_t *file,
      uint16_t *utf16_string,
@@ -3956,15 +3965,15 @@
 	{
 		result = libuna_utf16_string_with_index_copy_from_utf16_stream(
 			  utf16_string,
 			  utf16_string_size,
 			  &string_index,
 			  internal_file->location_information->local_path,
 			  internal_file->location_information->local_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_with_index_copy_from_byte_stream(
 			  utf16_string,
 			  utf16_string_size,
@@ -4055,15 +4064,15 @@
 	{
 		result = libuna_utf16_string_with_index_copy_from_utf16_stream(
 			  utf16_string,
 			  utf16_string_size,
 			  &string_index,
 			  internal_file->location_information->common_path,
 			  internal_file->location_information->common_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_with_index_copy_from_byte_stream(
 			  utf16_string,
 			  utf16_string_size,
@@ -4084,14 +4093,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 encoded network path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_network_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
@@ -4229,15 +4239,15 @@
 		utf8_network_share_name_size += 1;
 	}
 	if( ( internal_file->location_information->string_flags & LIBLNK_LOCATION_INFORMATION_STRING_FLAG_COMMON_PATH_IS_UNICODE ) != 0 )
 	{
 		result = libuna_utf8_string_size_from_utf16_stream(
 			  internal_file->location_information->common_path,
 			  internal_file->location_information->common_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  &utf8_common_path_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_size_from_byte_stream(
 			  internal_file->location_information->common_path,
@@ -4259,14 +4269,15 @@
 	}
 	*utf8_string_size = utf8_network_share_name_size + utf8_common_path_size - 1;
 
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 encoded network path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_network_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
@@ -4435,15 +4446,15 @@
 	{
 		result = libuna_utf8_string_with_index_copy_from_utf16_stream(
 			  utf8_string,
 			  utf8_string_size,
 		          &string_index,
 			  internal_file->location_information->common_path,
 			  internal_file->location_information->common_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_with_index_copy_from_byte_stream(
 			  utf8_string,
 			  utf8_string_size,
@@ -4464,14 +4475,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 encoded network path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_network_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
@@ -4609,15 +4621,15 @@
 		utf16_network_share_name_size += 1;
 	}
 	if( ( internal_file->location_information->string_flags & LIBLNK_LOCATION_INFORMATION_STRING_FLAG_COMMON_PATH_IS_UNICODE ) != 0 )
 	{
 		result = libuna_utf16_string_size_from_utf16_stream(
 			  internal_file->location_information->common_path,
 			  internal_file->location_information->common_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  &utf16_common_path_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_size_from_byte_stream(
 			  internal_file->location_information->common_path,
@@ -4639,14 +4651,15 @@
 	}
 	*utf16_string_size = utf16_network_share_name_size + utf16_common_path_size - 1;
 
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 encoded network path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * The network path is only set if the link refers to a file on a network share
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_network_path(
      liblnk_file_t *file,
      uint16_t *utf16_string,
@@ -4815,15 +4828,15 @@
 	{
 		result = libuna_utf16_string_with_index_copy_from_utf16_stream(
 			  utf16_string,
 			  utf16_string_size,
 			  &string_index,
 			  internal_file->location_information->common_path,
 			  internal_file->location_information->common_path_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_with_index_copy_from_byte_stream(
 			  utf16_string,
 			  utf16_string_size,
@@ -5080,14 +5093,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 encoded relative path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_relative_path_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      libcerror_error_t **error )
@@ -5119,15 +5133,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->relative_path == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf8_string_size(
+	if( liblnk_data_string_get_utf8_path_string_size(
 	     internal_file->relative_path,
 	     internal_file->io_handle->ascii_codepage,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -5138,14 +5152,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 encoded relative path
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_relative_path(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
@@ -5178,15 +5193,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->relative_path == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf8_string(
+	if( liblnk_data_string_get_utf8_path_string(
 	     internal_file->relative_path,
 	     internal_file->io_handle->ascii_codepage,
 	     utf8_string,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -5198,14 +5213,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 encoded relative path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_relative_path_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      libcerror_error_t **error )
@@ -5237,15 +5253,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->relative_path == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf16_string_size(
+	if( liblnk_data_string_get_utf16_path_string_size(
 	     internal_file->relative_path,
 	     internal_file->io_handle->ascii_codepage,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -5256,14 +5272,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 encoded relative path
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_relative_path(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
@@ -5296,15 +5313,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->relative_path == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf16_string(
+	if( liblnk_data_string_get_utf16_path_string(
 	     internal_file->relative_path,
 	     internal_file->io_handle->ascii_codepage,
 	     utf16_string,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -5316,14 +5333,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 encoded working directory
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_working_directory_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      libcerror_error_t **error )
@@ -5355,15 +5373,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->working_directory == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf8_string_size(
+	if( liblnk_data_string_get_utf8_path_string_size(
 	     internal_file->working_directory,
 	     internal_file->io_handle->ascii_codepage,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -5374,14 +5392,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 encoded working directory
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_working_directory(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
@@ -5414,15 +5433,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->working_directory == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf8_string(
+	if( liblnk_data_string_get_utf8_path_string(
 	     internal_file->working_directory,
 	     internal_file->io_handle->ascii_codepage,
 	     utf8_string,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -5434,14 +5453,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 encoded working directory
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_working_directory_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      libcerror_error_t **error )
@@ -5473,15 +5493,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->working_directory == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf16_string_size(
+	if( liblnk_data_string_get_utf16_path_string_size(
 	     internal_file->working_directory,
 	     internal_file->io_handle->ascii_codepage,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -5492,14 +5512,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 encoded working directory
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_working_directory(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
@@ -5532,15 +5553,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->working_directory == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf16_string(
+	if( liblnk_data_string_get_utf16_path_string(
 	     internal_file->working_directory,
 	     internal_file->io_handle->ascii_codepage,
 	     utf16_string,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -5552,14 +5573,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 encoded command line arguments
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_command_line_arguments_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      libcerror_error_t **error )
@@ -5591,15 +5613,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->command_line_arguments == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf8_string_size(
+	if( liblnk_data_string_get_utf8_path_string_size(
 	     internal_file->command_line_arguments,
 	     internal_file->io_handle->ascii_codepage,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -5610,14 +5632,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 encoded command line arguments
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_command_line_arguments(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
@@ -5650,15 +5673,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->command_line_arguments == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf8_string(
+	if( liblnk_data_string_get_utf8_path_string(
 	     internal_file->command_line_arguments,
 	     internal_file->io_handle->ascii_codepage,
 	     utf8_string,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -5670,14 +5693,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 encoded command line arguments
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_command_line_arguments_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      libcerror_error_t **error )
@@ -5709,15 +5733,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->command_line_arguments == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf16_string_size(
+	if( liblnk_data_string_get_utf16_path_string_size(
 	     internal_file->command_line_arguments,
 	     internal_file->io_handle->ascii_codepage,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -5728,14 +5752,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 encoded command line arguments
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_command_line_arguments(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
@@ -5768,15 +5793,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->command_line_arguments == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf16_string(
+	if( liblnk_data_string_get_utf16_path_string(
 	     internal_file->command_line_arguments,
 	     internal_file->io_handle->ascii_codepage,
 	     utf16_string,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -5788,14 +5813,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 encoded icon location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_icon_location_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      libcerror_error_t **error )
@@ -5827,15 +5853,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->icon_location == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf8_string_size(
+	if( liblnk_data_string_get_utf8_path_string_size(
 	     internal_file->icon_location,
 	     internal_file->io_handle->ascii_codepage,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -5846,14 +5872,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 encoded icon location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_icon_location(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
@@ -5886,15 +5913,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->icon_location == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf8_string(
+	if( liblnk_data_string_get_utf8_path_string(
 	     internal_file->icon_location,
 	     internal_file->io_handle->ascii_codepage,
 	     utf8_string,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -5906,14 +5933,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 encoded icon location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_icon_location_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      libcerror_error_t **error )
@@ -5945,15 +5973,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->icon_location == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf16_string_size(
+	if( liblnk_data_string_get_utf16_path_string_size(
 	     internal_file->icon_location,
 	     internal_file->io_handle->ascii_codepage,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -5964,14 +5992,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 encoded icon location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_icon_location(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
@@ -6004,15 +6033,15 @@
 
 		return( -1 );
 	}
 	if( internal_file->icon_location == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_data_string_get_utf16_string(
+	if( liblnk_data_string_get_utf16_path_string(
 	     internal_file->icon_location,
 	     internal_file->io_handle->ascii_codepage,
 	     utf16_string,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -6024,14 +6053,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 encoded environment variables location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_environment_variables_location_size(
      liblnk_file_t *file,
      size_t *utf8_string_size,
      libcerror_error_t **error )
@@ -6052,15 +6082,15 @@
 	}
 	internal_file = (liblnk_internal_file_t *) file;
 
 	if( internal_file->environment_variables_location_data_block == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_strings_data_block_get_utf8_string_size(
+	if( liblnk_strings_data_block_get_utf8_path_string_size(
 	     internal_file->environment_variables_location_data_block,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -6070,14 +6100,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 encoded environment variables location
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf8_environment_variables_location(
      liblnk_file_t *file,
      uint8_t *utf8_string,
      size_t utf8_string_size,
@@ -6099,15 +6130,15 @@
 	}
 	internal_file = (liblnk_internal_file_t *) file;
 
 	if( internal_file->environment_variables_location_data_block == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_strings_data_block_get_utf8_string(
+	if( liblnk_strings_data_block_get_utf8_path_string(
 	     internal_file->environment_variables_location_data_block,
 	     utf8_string,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
@@ -6118,14 +6149,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 encoded environment variables location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size includes the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_environment_variables_location_size(
      liblnk_file_t *file,
      size_t *utf16_string_size,
      libcerror_error_t **error )
@@ -6146,15 +6178,15 @@
 	}
 	internal_file = (liblnk_internal_file_t *) file;
 
 	if( internal_file->environment_variables_location_data_block == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_strings_data_block_get_utf16_string_size(
+	if( liblnk_strings_data_block_get_utf16_path_string_size(
 	     internal_file->environment_variables_location_data_block,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -6164,14 +6196,15 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 encoded environment variables location
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
  * The size should include the end of string character
  * Returns 1 if successful, 0 if value is not available or -1 on error
  */
 int liblnk_file_get_utf16_environment_variables_location(
      liblnk_file_t *file,
      uint16_t *utf16_string,
      size_t utf16_string_size,
@@ -6193,15 +6226,15 @@
 	}
 	internal_file = (liblnk_internal_file_t *) file;
 
 	if( internal_file->environment_variables_location_data_block == NULL )
 	{
 		return( 0 );
 	}
-	if( liblnk_strings_data_block_get_utf16_string(
+	if( liblnk_strings_data_block_get_utf16_path_string(
 	     internal_file->environment_variables_location_data_block,
 	     utf16_string,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
```

### Comparing `liblnk-20230205/liblnk/liblnk_libfguid.h` & `liblnk-20230716/liblnk/liblnk_libfguid.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_io_handle.h` & `liblnk-20230716/liblnk/liblnk_io_handle.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/lnk_volume_information.h` & `liblnk-20230716/liblnk/lnk_volume_information.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_file.h` & `liblnk-20230716/liblnk/liblnk_file.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_codepage.h` & `liblnk-20230716/liblnk/liblnk_codepage.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_file_header.h` & `liblnk-20230716/liblnk/liblnk_file_header.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_known_folder_location.c` & `liblnk-20230716/liblnk/liblnk_known_folder_location.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_link_target_identifier.h` & `liblnk-20230716/liblnk/liblnk_link_target_identifier.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk.c` & `liblnk-20230716/liblnk/liblnk.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk.rc` & `liblnk-20230716/liblnk/liblnk.rc`

 * *Files 23% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Shortcut File (LNK) format\0"
-      VALUE "FileVersion",		"20230205" "\0"
+      VALUE "FileVersion",		"20230716" "\0"
       VALUE "InternalName",		"liblnk.dll\0"
       VALUE "LegalCopyright",		"(C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"liblnk.dll\0"
       VALUE "ProductName",		"liblnk\0"
-      VALUE "ProductVersion",		"20230205" "\0"
+      VALUE "ProductVersion",		"20230716" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/liblnk/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `liblnk-20230205/liblnk/Makefile.in` & `liblnk-20230716/liblnk/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_error.c` & `liblnk-20230716/liblnk/liblnk_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/lnk_location_information.h` & `liblnk-20230716/liblnk/lnk_location_information.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_notify.h` & `liblnk-20230716/liblnk/liblnk_notify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_support.h` & `liblnk-20230716/liblnk/liblnk_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_notify.c` & `liblnk-20230716/liblnk/liblnk_notify.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/lnk_file_header.h` & `liblnk-20230716/liblnk/lnk_file_header.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_libclocale.h` & `liblnk-20230716/liblnk/liblnk_libclocale.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_special_folder_location.c` & `liblnk-20230716/liblnk/liblnk_special_folder_location.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_debug.c` & `liblnk-20230716/liblnk/liblnk_debug.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_error.h` & `liblnk-20230716/liblnk/liblnk_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/liblnk_definitions.h` & `liblnk-20230716/liblnk/liblnk_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBLNK )
 #include <liblnk/definitions.h>
 
 /* The definitions in <liblnk/definitions.h> are copied here
  * for local use of liblnk
  */
 #else
-#define LIBLNK_VERSION								20230205
+#define LIBLNK_VERSION								20230716
 
 /* The liblnk version string
  */
-#define LIBLNK_VERSION_STRING							"20230205"
+#define LIBLNK_VERSION_STRING							"20230716"
 
 /* The liblnk file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBLNK_ACCESS_FLAGS
```

### Comparing `liblnk-20230205/liblnk/liblnk_libcdata.h` & `liblnk-20230716/liblnk/liblnk_libcdata.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/liblnk/lnk_data_blocks.h` & `liblnk-20230716/liblnk/lnk_data_blocks.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/pylnk-python2/Makefile.am` & `liblnk-20230716/pylnk-python2/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 	pylnk_guid.c pylnk_guid.h \
 	pylnk_integer.c pylnk_integer.h \
 	pylnk_libbfio.h \
 	pylnk_libcerror.h \
 	pylnk_libclocale.h \
 	pylnk_libfguid.h \
 	pylnk_liblnk.h \
+	pylnk_libuna.h \
 	pylnk_python.h \
+	pylnk_string.c pylnk_string.h \
 	pylnk_strings_data_block.c pylnk_strings_data_block.h \
 	pylnk_unused.h
 
 pyexec_LTLIBRARIES = pylnk.la
 
 nodist_pylnk_la_SOURCES = $(BUILT_SOURCES)
```

### Comparing `liblnk-20230205/pylnk-python2/Makefile.in` & `liblnk-20230716/pylnk-python2/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 @HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_drive_types.lo \
 @HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_error.lo \
 @HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_file.lo \
 @HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_file_attribute_flags.lo \
 @HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_file_object_io_handle.lo \
 @HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_guid.lo \
 @HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_integer.lo \
+@HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_string.lo \
 @HAVE_PYTHON2_TRUE@	pylnk_la-pylnk_strings_data_block.lo
 @HAVE_PYTHON2_TRUE@nodist_pylnk_la_OBJECTS = $(am__objects_1)
 pylnk_la_OBJECTS = $(nodist_pylnk_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
@@ -194,14 +195,15 @@
 	./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_error.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_guid.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_integer.Plo \
+	./$(DEPDIR)/pylnk_la-pylnk_string.Plo \
 	./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 am__mv = mv -f
 COMPILE = $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) \
 	$(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS)
 LTCOMPILE = $(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) \
 	$(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) \
 	$(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(CPPFLAGS) \
@@ -621,15 +623,17 @@
 @HAVE_PYTHON2_TRUE@	pylnk_guid.c pylnk_guid.h \
 @HAVE_PYTHON2_TRUE@	pylnk_integer.c pylnk_integer.h \
 @HAVE_PYTHON2_TRUE@	pylnk_libbfio.h \
 @HAVE_PYTHON2_TRUE@	pylnk_libcerror.h \
 @HAVE_PYTHON2_TRUE@	pylnk_libclocale.h \
 @HAVE_PYTHON2_TRUE@	pylnk_libfguid.h \
 @HAVE_PYTHON2_TRUE@	pylnk_liblnk.h \
+@HAVE_PYTHON2_TRUE@	pylnk_libuna.h \
 @HAVE_PYTHON2_TRUE@	pylnk_python.h \
+@HAVE_PYTHON2_TRUE@	pylnk_string.c pylnk_string.h \
 @HAVE_PYTHON2_TRUE@	pylnk_strings_data_block.c pylnk_strings_data_block.h \
 @HAVE_PYTHON2_TRUE@	pylnk_unused.h
 
 @HAVE_PYTHON2_TRUE@pyexec_LTLIBRARIES = pylnk.la
 @HAVE_PYTHON2_TRUE@nodist_pylnk_la_SOURCES = $(BUILT_SOURCES)
 @HAVE_PYTHON2_TRUE@pylnk_la_LIBADD = \
 @HAVE_PYTHON2_TRUE@	@LIBCERROR_LIBADD@ \
@@ -737,14 +741,15 @@
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_error.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_guid.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_integer.Plo@am__quote@ # am--include-marker
+@AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_string.Plo@am__quote@ # am--include-marker
 @AMDEP_TRUE@@am__include@ @am__quote@./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo@am__quote@ # am--include-marker
 
 $(am__depfiles_remade):
 	@$(MKDIR_P) $(@D)
 	@echo '# dummy' >$@-t && $(am__mv) $@-t $@
 
 am--depfiles: $(am__depfiles_remade)
@@ -864,14 +869,21 @@
 pylnk_la-pylnk_integer.lo: pylnk_integer.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_integer.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_integer.Tpo -c -o pylnk_la-pylnk_integer.lo `test -f 'pylnk_integer.c' || echo '$(srcdir)/'`pylnk_integer.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_integer.Tpo $(DEPDIR)/pylnk_la-pylnk_integer.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_integer.c' object='pylnk_la-pylnk_integer.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_integer.lo `test -f 'pylnk_integer.c' || echo '$(srcdir)/'`pylnk_integer.c
 
+pylnk_la-pylnk_string.lo: pylnk_string.c
+@am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_string.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_string.Tpo -c -o pylnk_la-pylnk_string.lo `test -f 'pylnk_string.c' || echo '$(srcdir)/'`pylnk_string.c
+@am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_string.Tpo $(DEPDIR)/pylnk_la-pylnk_string.Plo
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_string.c' object='pylnk_la-pylnk_string.lo' libtool=yes @AMDEPBACKSLASH@
+@AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
+@am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_string.lo `test -f 'pylnk_string.c' || echo '$(srcdir)/'`pylnk_string.c
+
 pylnk_la-pylnk_strings_data_block.lo: pylnk_strings_data_block.c
 @am__fastdepCC_TRUE@	$(AM_V_CC)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -MT pylnk_la-pylnk_strings_data_block.lo -MD -MP -MF $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Tpo -c -o pylnk_la-pylnk_strings_data_block.lo `test -f 'pylnk_strings_data_block.c' || echo '$(srcdir)/'`pylnk_strings_data_block.c
 @am__fastdepCC_TRUE@	$(AM_V_at)$(am__mv) $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Tpo $(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	$(AM_V_CC)source='pylnk_strings_data_block.c' object='pylnk_la-pylnk_strings_data_block.lo' libtool=yes @AMDEPBACKSLASH@
 @AMDEP_TRUE@@am__fastdepCC_FALSE@	DEPDIR=$(DEPDIR) $(CCDEPMODE) $(depcomp) @AMDEPBACKSLASH@
 @am__fastdepCC_FALSE@	$(AM_V_CC@am__nodep@)$(LIBTOOL) $(AM_V_lt) --tag=CC $(AM_LIBTOOLFLAGS) $(LIBTOOLFLAGS) --mode=compile $(CC) $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(pylnk_la_CPPFLAGS) $(CPPFLAGS) $(AM_CFLAGS) $(CFLAGS) -c -o pylnk_la-pylnk_strings_data_block.lo `test -f 'pylnk_strings_data_block.c' || echo '$(srcdir)/'`pylnk_strings_data_block.c
 
@@ -1066,14 +1078,15 @@
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_drive_types.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_error.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file_attribute_flags.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_file_object_io_handle.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_guid.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_integer.Plo
+	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_string.Plo
 	-rm -f ./$(DEPDIR)/pylnk_la-pylnk_strings_data_block.Plo
 	-rm -f Makefile
 maintainer-clean-am: distclean-am maintainer-clean-generic
 
 mostlyclean: mostlyclean-am
 
 mostlyclean-am: mostlyclean-compile mostlyclean-generic \
```

### Comparing `liblnk-20230205/test-driver` & `liblnk-20230716/test-driver`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/configure` & `liblnk-20230716/configure`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for liblnk 20230205.
+# Generated by GNU Autoconf 2.71 for liblnk 20230716.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='liblnk'
 PACKAGE_TARNAME='liblnk'
-PACKAGE_VERSION='20230205'
-PACKAGE_STRING='liblnk 20230205'
+PACKAGE_VERSION='20230716'
+PACKAGE_STRING='liblnk 20230716'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/liblnk.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1685,15 +1685,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures liblnk 20230205 to adapt to many kinds of systems.
+\`configure' configures liblnk 20230716 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1756,15 +1756,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of liblnk 20230205:";;
+     short | recursive ) echo "Configuration of liblnk 20230716:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -2014,15 +2014,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-liblnk configure 20230205
+liblnk configure 20230716
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2735,15 +2735,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by liblnk $as_me 20230205, which was
+It was created by liblnk $as_me 20230716, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4224,15 +4224,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='liblnk'
- VERSION='20230205'
+ VERSION='20230716'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -33357,37 +33357,37 @@
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna" >&5
 printf %s "checking for libuna... " >&6; }
 
 if test -n "$libuna_CFLAGS"; then
     pkg_cv_libuna_CFLAGS="$libuna_CFLAGS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libuna >= 20210801\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libuna >= 20210801") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libuna >= 20230702\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libuna >= 20230702") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libuna_CFLAGS=`$PKG_CONFIG --cflags "libuna >= 20210801" 2>/dev/null`
+  pkg_cv_libuna_CFLAGS=`$PKG_CONFIG --cflags "libuna >= 20230702" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
 if test -n "$libuna_LIBS"; then
     pkg_cv_libuna_LIBS="$libuna_LIBS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libuna >= 20210801\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libuna >= 20210801") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libuna >= 20230702\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libuna >= 20230702") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libuna_LIBS=`$PKG_CONFIG --libs "libuna >= 20210801" 2>/dev/null`
+  pkg_cv_libuna_LIBS=`$PKG_CONFIG --libs "libuna >= 20230702" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
@@ -33400,17 +33400,17 @@
 
 if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
         _pkg_short_errors_supported=yes
 else
         _pkg_short_errors_supported=no
 fi
         if test $_pkg_short_errors_supported = yes; then
-	        libuna_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libuna >= 20210801" 2>&1`
+	        libuna_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libuna >= 20230702" 2>&1`
         else
-	        libuna_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libuna >= 20210801" 2>&1`
+	        libuna_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libuna >= 20230702" 2>&1`
         fi
 	# Put the nasty error message in config.log where it belongs
 	echo "$libuna_PKG_ERRORS" >&5
 
 	ac_cv_libuna=check
 elif test $pkg_failed = untried; then
      	{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
@@ -34712,14 +34712,1107 @@
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
 
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_byte_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_byte_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_byte_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_byte_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_byte_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_byte_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_ucs2 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_ucs2 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_ucs2 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_ucs2 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs2" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_ucs4 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_ucs4 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_ucs4 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_ucs4 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_ucs4" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf7_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf7_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf7_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf7_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_utf8 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_utf8 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf8 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf8 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf8 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf8 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_utf8_rfc2279 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_utf8_rfc2279 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_utf8_rfc2279 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_utf8_rfc2279 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_utf8_rfc2279" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf8_rfc2279 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf8_rfc2279 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf8_rfc2279 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf8_rfc2279 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf8_rfc2279" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf8_rfc2279 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf8_rfc2279 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf8_rfc2279 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf8_rfc2279 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf8_rfc2279" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_size_to_utf16 in -luna" >&5
+printf %s "checking for libuna_unicode_character_size_to_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_size_to_utf16+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_size_to_utf16 ();
+int
+main (void)
+{
+return libuna_unicode_character_size_to_utf16 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf16=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_size_to_utf16=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_size_to_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_size_to_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_size_to_utf16" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf16+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf16 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf16 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf16=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf16=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf16" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf16 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf16+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf16 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf16 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf16=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf16=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf16" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf16_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf16_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf16_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf16_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf16_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf16_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf16_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf32 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf32+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf32 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf32 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf32=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf32=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf32" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf32 in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf32+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf32 ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf32 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf32=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf32=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf32" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_from_utf32_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_from_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_from_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_unicode_character_copy_to_utf32_stream in -luna" >&5
+printf %s "checking for libuna_unicode_character_copy_to_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_unicode_character_copy_to_utf32_stream ();
+int
+main (void)
+{
+return libuna_unicode_character_copy_to_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_unicode_character_copy_to_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+
                 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_stream_size_from_utf8 in -luna" >&5
 printf %s "checking for libuna_utf8_stream_size_from_utf8 in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf8_stream_size_from_utf8+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -35597,14 +36690,56 @@
 if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_byte_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_byte_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_compare_with_byte_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_compare_with_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf7_stream in -luna" >&5
 printf %s "checking for libuna_utf8_string_size_from_utf7_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf7_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -35723,14 +36858,56 @@
 if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf7_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf7_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_compare_with_utf7_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_compare_with_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf8_stream in -luna" >&5
 printf %s "checking for libuna_utf8_string_size_from_utf8_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -35849,386 +37026,386 @@
 if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_size_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf8_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf8_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_size_from_utf16_stream ();
+char libuna_utf8_string_compare_with_utf8_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_size_from_utf16_stream ();
+return libuna_utf8_string_compare_with_utf8_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_copy_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf8_string_size_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_copy_from_utf16_stream ();
+char libuna_utf8_string_size_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf8_string_copy_from_utf16_stream ();
+return libuna_utf8_string_size_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_with_index_copy_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf8_string_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_with_index_copy_from_utf16_stream ();
+char libuna_utf8_string_copy_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf8_string_with_index_copy_from_utf16_stream ();
+return libuna_utf8_string_copy_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_size_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf8_string_with_index_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_size_from_utf32_stream ();
+char libuna_utf8_string_with_index_copy_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf8_string_size_from_utf32_stream ();
+return libuna_utf8_string_with_index_copy_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf16 in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_copy_from_utf32_stream ();
+char libuna_utf8_string_compare_with_utf16 ();
 int
 main (void)
 {
-return libuna_utf8_string_copy_from_utf32_stream ();
+return libuna_utf8_string_compare_with_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf8_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_size_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_with_index_copy_from_utf32_stream ();
+char libuna_utf8_string_size_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_with_index_copy_from_utf32_stream ();
+return libuna_utf8_string_size_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf8_string_size_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_size_from_utf16 ();
+char libuna_utf8_string_copy_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_size_from_utf16 ();
+return libuna_utf8_string_copy_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf16=yes
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_size_from_utf16=no
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf8_string_copy_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_with_index_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_copy_from_utf16 ();
+char libuna_utf8_string_with_index_copy_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_copy_from_utf16 ();
+return libuna_utf8_string_with_index_copy_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16=yes
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_copy_from_utf16=no
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf8_string_with_index_copy_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf8_string_with_index_copy_from_utf16 ();
+char libuna_utf8_string_compare_with_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf8_string_with_index_copy_from_utf16 ();
+return libuna_utf8_string_compare_with_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16=yes
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16=no
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf32 in -luna" >&5
@@ -36353,14 +37530,224 @@
 if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf32 in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf32+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_compare_with_utf32 ();
+int
+main (void)
+{
+return libuna_utf8_string_compare_with_utf32 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf32=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf32=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf32" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_size_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_size_from_utf32_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_size_from_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_size_from_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_copy_from_utf32_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_copy_from_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_copy_from_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_with_index_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_with_index_copy_from_utf32_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_with_index_copy_from_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_with_index_copy_from_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_compare_with_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf8_string_compare_with_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf8_string_compare_with_utf32_stream ();
+int
+main (void)
+{
+return libuna_utf8_string_compare_with_utf32_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf8_string_compare_with_utf32_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf8_string_size_from_scsu_stream in -luna" >&5
 printf %s "checking for libuna_utf8_string_size_from_scsu_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf8_string_size_from_scsu_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -36606,14 +37993,56 @@
 if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_byte_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_byte_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_compare_with_byte_stream ();
+int
+main (void)
+{
+return libuna_utf16_string_compare_with_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf7_stream in -luna" >&5
 printf %s "checking for libuna_utf16_string_size_from_utf7_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf7_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -36732,15 +38161,183 @@
 if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf7_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf8_stream in -luna" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf7_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_compare_with_utf7_stream ();
+int
+main (void)
+{
+return libuna_utf16_string_compare_with_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf16_string_size_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_size_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf16_string_size_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf16_string_copy_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_copy_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf16_string_copy_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf16_string_with_index_copy_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_with_index_copy_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf16_string_with_index_copy_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf8_stream in -luna" >&5
 printf %s "checking for libuna_utf16_string_size_from_utf8_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
@@ -36858,14 +38455,56 @@
 if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf8_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf8_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf16_string_compare_with_utf8_stream ();
+int
+main (void)
+{
+return libuna_utf16_string_compare_with_utf8_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf8_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf16_stream in -luna" >&5
 printf %s "checking for libuna_utf16_string_size_from_utf16_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -36984,386 +38623,386 @@
 if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf16_string_size_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_size_from_utf32_stream ();
+char libuna_utf16_string_compare_with_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_size_from_utf32_stream ();
+return libuna_utf16_string_compare_with_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf16_string_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf32 in -luna" >&5
+printf %s "checking for libuna_utf16_string_size_from_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf32+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_copy_from_utf32_stream ();
+char libuna_utf16_string_size_from_utf32 ();
 int
 main (void)
 {
-return libuna_utf16_string_copy_from_utf32_stream ();
+return libuna_utf16_string_size_from_utf32 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf32=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf32=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf16_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf32 in -luna" >&5
+printf %s "checking for libuna_utf16_string_copy_from_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf32+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_with_index_copy_from_utf32_stream ();
+char libuna_utf16_string_copy_from_utf32 ();
 int
 main (void)
 {
-return libuna_utf16_string_with_index_copy_from_utf32_stream ();
+return libuna_utf16_string_copy_from_utf32 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf16_string_size_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf32 in -luna" >&5
+printf %s "checking for libuna_utf16_string_with_index_copy_from_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_size_from_utf8 ();
+char libuna_utf16_string_with_index_copy_from_utf32 ();
 int
 main (void)
 {
-return libuna_utf16_string_size_from_utf8 ();
+return libuna_utf16_string_with_index_copy_from_utf32 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf8=yes
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf8=no
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf16_string_copy_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf32 in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf32 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf32+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_copy_from_utf8 ();
+char libuna_utf16_string_compare_with_utf32 ();
 int
 main (void)
 {
-return libuna_utf16_string_copy_from_utf8 ();
+return libuna_utf16_string_compare_with_utf32 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf8=yes
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf32=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf8=no
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf32=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf32" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf32" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf32" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf16_string_with_index_copy_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_size_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_with_index_copy_from_utf8 ();
+char libuna_utf16_string_size_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_with_index_copy_from_utf8 ();
+return libuna_utf16_string_size_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8=yes
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8=no
+  ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_utf32 in -luna" >&5
-printf %s "checking for libuna_utf16_string_size_from_utf32 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_size_from_utf32+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_size_from_utf32 ();
+char libuna_utf16_string_copy_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_size_from_utf32 ();
+return libuna_utf16_string_copy_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf32=yes
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_size_from_utf32=no
+  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_size_from_utf32" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_size_from_utf32" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_size_from_utf32" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_copy_from_utf32 in -luna" >&5
-printf %s "checking for libuna_utf16_string_copy_from_utf32 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_copy_from_utf32+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_copy_from_utf32 ();
+char libuna_utf16_string_with_index_copy_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_copy_from_utf32 ();
+return libuna_utf16_string_with_index_copy_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32=yes
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_copy_from_utf32=no
+  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_copy_from_utf32" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_with_index_copy_from_utf32 in -luna" >&5
-printf %s "checking for libuna_utf16_string_with_index_copy_from_utf32 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_compare_with_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf16_string_compare_with_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf16_string_with_index_copy_from_utf32 ();
+char libuna_utf16_string_compare_with_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf16_string_with_index_copy_from_utf32 ();
+return libuna_utf16_string_compare_with_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32=yes
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32=no
+  ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf16_string_with_index_copy_from_utf32" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf16_string_compare_with_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf16_string_size_from_scsu_stream in -luna" >&5
@@ -37615,14 +39254,56 @@
 if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_byte_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_byte_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_byte_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf32_string_compare_with_byte_stream ();
+int
+main (void)
+{
+return libuna_utf32_string_compare_with_byte_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_byte_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf7_stream in -luna" >&5
 printf %s "checking for libuna_utf32_string_size_from_utf7_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf7_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -37741,14 +39422,56 @@
 if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf7_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_utf7_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_utf7_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf32_string_compare_with_utf7_stream ();
+int
+main (void)
+{
+return libuna_utf32_string_compare_with_utf7_stream ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_utf7_stream" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf8_stream in -luna" >&5
 printf %s "checking for libuna_utf32_string_size_from_utf8_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -37783,15 +39506,139 @@
 if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf8_stream in -luna" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf32_string_size_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf32_string_size_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf32_string_size_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf8 in -luna" >&5
+printf %s "checking for libuna_utf32_string_copy_from_utf8 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf8+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-luna  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libuna_utf32_string_copy_from_utf8 ();
+int
+main (void)
+{
+return libuna_utf32_string_copy_from_utf8 ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf8=yes
+else $as_nop
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf8=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" = xyes
+then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
+  ac_cv_libuna=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for ac_cv_libuna_dummy=yes in -llibuna_utf32_string_with_index_copy_from_utf8" >&5
+printf %s "checking for ac_cv_libuna_dummy=yes in -llibuna_utf32_string_with_index_copy_from_utf8... " >&6; }
+if test ${ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-llibuna_utf32_string_with_index_copy_from_utf8  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char ac_cv_libuna_dummy=yes ();
+int
+main (void)
+{
+return ac_cv_libuna_dummy=yes ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes=yes
+else $as_nop
+  ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" >&5
+printf "%s\n" "$ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" >&6; }
+if test "x$ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" = xyes
+then :
+  ac_cv_libuna=no
+fi
+
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf8_stream in -luna" >&5
 printf %s "checking for libuna_utf32_string_copy_from_utf8_stream in -luna... " >&6; }
 if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
@@ -37867,510 +39714,512 @@
 if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_size_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_utf8_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_utf8_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_size_from_utf16_stream ();
+char libuna_utf32_string_compare_with_utf8_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_size_from_utf16_stream ();
+return libuna_utf32_string_compare_with_utf8_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_utf8_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_copy_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf32_string_size_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_copy_from_utf16_stream ();
+char libuna_utf32_string_size_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf32_string_copy_from_utf16_stream ();
+return libuna_utf32_string_size_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf16_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_with_index_copy_from_utf16_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf32_string_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_with_index_copy_from_utf16_stream ();
+char libuna_utf32_string_copy_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf32_string_with_index_copy_from_utf16_stream ();
+return libuna_utf32_string_copy_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream=no
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_size_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf16 in -luna" >&5
+printf %s "checking for libuna_utf32_string_with_index_copy_from_utf16 in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_size_from_utf32_stream ();
+char libuna_utf32_string_with_index_copy_from_utf16 ();
 int
 main (void)
 {
-return libuna_utf32_string_size_from_utf32_stream ();
+return libuna_utf32_string_with_index_copy_from_utf16 ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream+y}
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_size_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_copy_from_utf32_stream ();
+char libuna_utf32_string_size_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_copy_from_utf32_stream ();
+return libuna_utf32_string_size_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf32_stream in -luna" >&5
-printf %s "checking for libuna_utf32_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_with_index_copy_from_utf32_stream ();
+char libuna_utf32_string_copy_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_with_index_copy_from_utf32_stream ();
+return libuna_utf32_string_copy_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream=yes
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream=no
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf32_string_size_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_with_index_copy_from_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_size_from_utf8 ();
+char libuna_utf32_string_with_index_copy_from_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_size_from_utf8 ();
+return libuna_utf32_string_with_index_copy_from_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf8=yes
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf8=no
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf8 in -luna" >&5
-printf %s "checking for libuna_utf32_string_copy_from_utf8 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf8+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_utf16_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_utf16_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_copy_from_utf8 ();
+char libuna_utf32_string_compare_with_utf16_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_copy_from_utf8 ();
+return libuna_utf32_string_compare_with_utf16_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf8=yes
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf8=no
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf8" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_utf16_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for ac_cv_libuna_dummy=yes in -llibuna_utf32_string_with_index_copy_from_utf8" >&5
-printf %s "checking for ac_cv_libuna_dummy=yes in -llibuna_utf32_string_with_index_copy_from_utf8... " >&6; }
-if test ${ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_size_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
-LIBS="-llibuna_utf32_string_with_index_copy_from_utf8  $LIBS"
+LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char ac_cv_libuna_dummy=yes ();
+char libuna_utf32_string_size_from_utf32_stream ();
 int
 main (void)
 {
-return ac_cv_libuna_dummy=yes ();
+return libuna_utf32_string_size_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes=yes
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes=no
+  ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" >&5
-printf "%s\n" "$ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" >&6; }
-if test "x$ac_cv_lib_libuna_utf32_string_with_index_copy_from_utf8_ac_cv_libuna_dummy_yes" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf32_stream" = xyes
 then :
+  ac_cv_libuna_dummy=yes
+else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf32_string_size_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_size_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_size_from_utf16 ();
+char libuna_utf32_string_copy_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_size_from_utf16 ();
+return libuna_utf32_string_copy_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf16=yes
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_size_from_utf16=no
+  ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_size_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_size_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_size_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_copy_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf32_string_copy_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_copy_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_with_index_copy_from_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_copy_from_utf16 ();
+char libuna_utf32_string_with_index_copy_from_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_copy_from_utf16 ();
+return libuna_utf32_string_with_index_copy_from_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16=yes
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_copy_from_utf16=no
+  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_copy_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
-        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_with_index_copy_from_utf16 in -luna" >&5
-printf %s "checking for libuna_utf32_string_with_index_copy_from_utf16 in -luna... " >&6; }
-if test ${ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16+y}
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_compare_with_utf32_stream in -luna" >&5
+printf %s "checking for libuna_utf32_string_compare_with_utf32_stream in -luna... " >&6; }
+if test ${ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-luna  $LIBS"
 cat confdefs.h - <<_ACEOF >conftest.$ac_ext
 /* end confdefs.h.  */
 
 /* Override any GCC internal prototype to avoid an error.
    Use char because int might match the return type of a GCC
    builtin and then its argument prototype would still apply.  */
-char libuna_utf32_string_with_index_copy_from_utf16 ();
+char libuna_utf32_string_compare_with_utf32_stream ();
 int
 main (void)
 {
-return libuna_utf32_string_with_index_copy_from_utf16 ();
+return libuna_utf32_string_compare_with_utf32_stream ();
   ;
   return 0;
 }
 _ACEOF
 if ac_fn_c_try_link "$LINENO"
 then :
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16=yes
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream=yes
 else $as_nop
-  ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16=no
+  ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream=no
 fi
 rm -f core conftest.err conftest.$ac_objext conftest.beam \
     conftest$ac_exeext conftest.$ac_ext
 LIBS=$ac_check_lib_save_LIBS
 fi
-{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" >&5
-printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" >&6; }
-if test "x$ac_cv_lib_una_libuna_utf32_string_with_index_copy_from_utf16" = xyes
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream" >&5
+printf "%s\n" "$ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream" >&6; }
+if test "x$ac_cv_lib_una_libuna_utf32_string_compare_with_utf32_stream" = xyes
 then :
   ac_cv_libuna_dummy=yes
 else $as_nop
   ac_cv_libuna=no
 fi
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libuna_utf32_string_size_from_scsu_stream in -luna" >&5
@@ -38640,14 +40489,62 @@
 printf "%s\n" "$ac_cv_libuna_defines_compare_greater" >&6; }
 
         if test "x$ac_cv_libuna_defines_compare_less" != xyes
 then :
   ac_cv_libuna=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking if \`LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE' is defined" >&5
+printf %s "checking if \`LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE' is defined... " >&6; }
+if test ${ac_cv_libuna_defines_compare_greater+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_ext=c
+ac_cpp='$CPP $CPPFLAGS'
+ac_compile='$CC -c $CFLAGS $CPPFLAGS conftest.$ac_ext >&5'
+ac_link='$CC -o conftest$ac_exeext $CFLAGS $CPPFLAGS $LDFLAGS conftest.$ac_ext $LIBS >&5'
+ac_compiler_gnu=$ac_cv_c_compiler_gnu
+
+    cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+#include <libuna.h>
+int
+main (void)
+{
+int test = LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE;
+
+return( 0 );
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_libuna_defines_compare_greater=yes
+else $as_nop
+  ac_cv_libuna_defines_compare_greater=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+    ac_ext=c
+ac_cpp='$CPP $CPPFLAGS'
+ac_compile='$CC -c $CFLAGS $CPPFLAGS conftest.$ac_ext >&5'
+ac_link='$CC -o conftest$ac_exeext $CFLAGS $CPPFLAGS $LDFLAGS conftest.$ac_ext $LIBS >&5'
+ac_compiler_gnu=$ac_cv_c_compiler_gnu
+
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_libuna_defines_compare_greater" >&5
+printf "%s\n" "$ac_cv_libuna_defines_compare_greater" >&6; }
+
+        if test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes
+then :
+  ac_cv_libuna=no
+fi
+
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
     if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -48201,37 +50098,37 @@
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps" >&5
 printf %s "checking for libfwps... " >&6; }
 
 if test -n "$libfwps_CFLAGS"; then
     pkg_cv_libfwps_CFLAGS="$libfwps_CFLAGS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libfwps >= 20230130\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libfwps >= 20230130") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libfwps >= 20230711\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libfwps >= 20230711") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libfwps_CFLAGS=`$PKG_CONFIG --cflags "libfwps >= 20230130" 2>/dev/null`
+  pkg_cv_libfwps_CFLAGS=`$PKG_CONFIG --cflags "libfwps >= 20230711" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
 if test -n "$libfwps_LIBS"; then
     pkg_cv_libfwps_LIBS="$libfwps_LIBS"
  elif test -n "$PKG_CONFIG"; then
     if test -n "$PKG_CONFIG" && \
-    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libfwps >= 20230130\""; } >&5
-  ($PKG_CONFIG --exists --print-errors "libfwps >= 20230130") 2>&5
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"libfwps >= 20230711\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "libfwps >= 20230711") 2>&5
   ac_status=$?
   printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
   test $ac_status = 0; }; then
-  pkg_cv_libfwps_LIBS=`$PKG_CONFIG --libs "libfwps >= 20230130" 2>/dev/null`
+  pkg_cv_libfwps_LIBS=`$PKG_CONFIG --libs "libfwps >= 20230711" 2>/dev/null`
 		      test "x$?" != "x0" && pkg_failed=yes
 else
   pkg_failed=yes
 fi
  else
     pkg_failed=untried
 fi
@@ -48244,17 +50141,17 @@
 
 if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
         _pkg_short_errors_supported=yes
 else
         _pkg_short_errors_supported=no
 fi
         if test $_pkg_short_errors_supported = yes; then
-	        libfwps_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libfwps >= 20230130" 2>&1`
+	        libfwps_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "libfwps >= 20230711" 2>&1`
         else
-	        libfwps_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libfwps >= 20230130" 2>&1`
+	        libfwps_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "libfwps >= 20230711" 2>&1`
         fi
 	# Put the nasty error message in config.log where it belongs
 	echo "$libfwps_PKG_ERRORS" >&5
 
 	ac_cv_libfwps=check
 elif test $pkg_failed = untried; then
      	{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
@@ -49261,14 +51158,182 @@
 if test "x$ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_string" = xyes
 then :
   ac_cv_libfwps_dummy=yes
 else $as_nop
   ac_cv_libfwps=no
 fi
 
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_data_as_utf8_path_string_size in -lfwps" >&5
+printf %s "checking for libfwps_record_get_data_as_utf8_path_string_size in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string_size+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_data_as_utf8_path_string_size ();
+int
+main (void)
+{
+return libfwps_record_get_data_as_utf8_path_string_size ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string_size=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string_size=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string_size" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string_size" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string_size" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_data_as_utf8_path_string in -lfwps" >&5
+printf %s "checking for libfwps_record_get_data_as_utf8_path_string in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_data_as_utf8_path_string ();
+int
+main (void)
+{
+return libfwps_record_get_data_as_utf8_path_string ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_data_as_utf8_path_string" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_data_as_utf16_path_string_size in -lfwps" >&5
+printf %s "checking for libfwps_record_get_data_as_utf16_path_string_size in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string_size+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_data_as_utf16_path_string_size ();
+int
+main (void)
+{
+return libfwps_record_get_data_as_utf16_path_string_size ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string_size=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string_size=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string_size" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string_size" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string_size" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_data_as_utf16_path_string in -lfwps" >&5
+printf %s "checking for libfwps_record_get_data_as_utf16_path_string in -lfwps... " >&6; }
+if test ${ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfwps  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char libfwps_record_get_data_as_utf16_path_string ();
+int
+main (void)
+{
+return libfwps_record_get_data_as_utf16_path_string ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string=yes
+else $as_nop
+  ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string" >&5
+printf "%s\n" "$ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string" >&6; }
+if test "x$ac_cv_lib_fwps_libfwps_record_get_data_as_utf16_path_string" = xyes
+then :
+  ac_cv_libfwps_dummy=yes
+else $as_nop
+  ac_cv_libfwps=no
+fi
+
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for libfwps_record_get_data_as_guid in -lfwps" >&5
 printf %s "checking for libfwps_record_get_data_as_guid in -lfwps... " >&6; }
 if test ${ac_cv_lib_fwps_libfwps_record_get_data_as_guid+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
@@ -51919,15 +53984,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by liblnk $as_me 20230205, which was
+This file was extended by liblnk $as_me 20230716, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -51987,15 +54052,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-liblnk config.status 20230205
+liblnk config.status 20230716
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `liblnk-20230205/libuna/libuna_url_stream.c` & `liblnk-20230716/libuna/libuna_url_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_symbol.h` & `liblnk-20230716/libuna/libuna_codepage_mac_symbol.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_support.c` & `liblnk-20230716/libuna/libuna_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_scsu.h` & `liblnk-20230716/libuna/libuna_scsu.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_5.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_5.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-5 codepage (Cyrillic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_2.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_2.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1253.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1253.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_koi8_u.h` & `liblnk-20230716/libuna/libuna_codepage_koi8_u.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1252.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1252.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf32_stream.c` & `liblnk-20230716/libuna/libuna_utf32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -122,14 +122,15 @@
      const libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf32_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_stream_size_from_utf8";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf32_stream_size                = 0;
 	size_t utf8_string_index                     = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -159,15 +160,15 @@
 		 "%s: invalid UTF-32 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf32_stream_size = 1;
+	safe_utf32_stream_size = 1;
 
 	while( utf8_string_index < utf8_string_size )
 	{
 		/* Convert the UTF-8 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf8(
 		     &unicode_character,
@@ -185,15 +186,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-32 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf32(
 		     unicode_character,
-		     utf32_stream_size,
+		     &safe_utf32_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-32.",
@@ -204,15 +205,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf32_stream_size *= 4;
+	*utf32_stream_size = safe_utf32_stream_size * 4;
 
 	return( 1 );
 }
 
 /* Copies an UTF-32 stream from an UTF-8 string
  * Returns 1 if successful or -1 on error
  */
@@ -355,14 +356,15 @@
      const libuna_utf16_character_t *utf16_string,
      size_t utf16_string_size,
      size_t *utf32_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_stream_size_from_utf16";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf32_stream_size                = 0;
 	size_t utf16_string_index                    = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -392,15 +394,15 @@
 		 "%s: invalid UTF-32 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf32_stream_size = 1;
+	safe_utf32_stream_size = 1;
 
 	while( utf16_string_index < utf16_string_size )
 	{
 		/* Convert the UTF-16 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16(
 		     &unicode_character,
@@ -418,15 +420,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-32 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf32(
 		     unicode_character,
-		     utf32_stream_size,
+		     &safe_utf32_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-32.",
@@ -437,15 +439,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf32_stream_size *= 4;
+	*utf32_stream_size = safe_utf32_stream_size * 4;
 
 	return( 1 );
 }
 
 /* Copies an UTF-32 stream from an UTF-16 string
  * Returns 1 if successful or -1 on error
  */
@@ -588,14 +590,15 @@
      const libuna_utf32_character_t *utf32_string,
      size_t utf32_string_size,
      size_t *utf32_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_stream_size_from_utf32";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf32_stream_size                = 0;
 	size_t utf32_string_index                    = 0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -625,15 +628,15 @@
 		 "%s: invalid UTF-32 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf32_stream_size = 1;
+	safe_utf32_stream_size = 1;
 
 	while( utf32_string_index < utf32_string_size )
 	{
 		/* Convert the UTF-32 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32(
 		     &unicode_character,
@@ -651,15 +654,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-32 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf32(
 		     unicode_character,
-		     utf32_stream_size,
+		     &safe_utf32_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-32.",
@@ -670,15 +673,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf32_stream_size *= 4;
+	*utf32_stream_size = safe_utf32_stream_size * 4;
 
 	return( 1 );
 }
 
 /* Copies an UTF-32 stream from an UTF-32 string
  * Returns 1 if successful or -1 on error
  */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1257.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1257.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_cyrillic.c` & `liblnk-20230716/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_thai.c` & `liblnk-20230716/libuna/libuna_codepage_mac_thai.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf32_string.c` & `liblnk-20230716/libuna/libuna_utf32_string.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1920,17 +1920,18 @@
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      size_t *utf32_string_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_string_size_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf16_stream == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1995,26 +1996,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -2030,18 +2019,29 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Determine how many UTF-8 character bytes are required
 		 */
-		if( libuna_unicode_character_size_to_utf32(
-		     unicode_character,
-		     utf32_string_size,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_size_to_utf32(
+			          unicode_character,
+			          utf32_string_size,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_size_to_ucs4(
+			          unicode_character,
+			          utf32_string_size,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_INPUT_FAILED,
 			 "%s: unable to unable to determine size of Unicode character in UTF-32.",
 			 function );
@@ -2106,17 +2106,18 @@
      size_t *utf32_string_index,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf32_string_with_index_copy_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2198,26 +2199,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -2233,20 +2222,33 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Convert the Unicode character into UTF-32 character bytes
 		 */
-		if( libuna_unicode_character_copy_to_utf32(
-		     unicode_character,
-		     utf32_string,
-		     utf32_string_size,
-		     utf32_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_to_utf32(
+			          unicode_character,
+			          utf32_string,
+			          utf32_string_size,
+			          utf32_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_to_ucs4(
+			          unicode_character,
+			          utf32_string,
+			          utf32_string_size,
+			          utf32_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character to UTF-32.",
 			 function );
@@ -2288,19 +2290,20 @@
      size_t utf32_string_size,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                                     = "libuna_utf32_string_compare_with_utf16_stream";
+	libuna_unicode_character_t utf16_stream_unicode_character = 0;
+	libuna_unicode_character_t utf32_unicode_character        = 0;
 	size_t utf16_stream_index                                 = 0;
 	size_t utf32_string_index                                 = 0;
-	libuna_unicode_character_t utf32_unicode_character        = 0;
-	libuna_unicode_character_t utf16_stream_unicode_character = 0;
 	int read_byte_order                                       = 0;
+	int result                                                = 0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2371,26 +2374,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf32_string_size >= 1 )
 	 && ( utf32_string[ utf32_string_size - 1 ] == 0 ) )
 	{
 		utf32_string_size -= 1;
 	}
 	/* Check if the UTF-16 stream is terminated with zero bytes
 	 */
@@ -2401,20 +2392,33 @@
 		utf16_stream_size -= 2;
 	}
 	while( ( utf32_string_index < utf32_string_size )
 	    && ( utf16_stream_index < utf16_stream_size ) )
 	{
 		/* Convert the UTF-32 character bytes into an Unicode character
 		 */
-		if( libuna_unicode_character_copy_from_utf32(
-		     &utf32_unicode_character,
-		     utf32_string,
-		     utf32_string_size,
-		     &utf32_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_from_utf32(
+			          &utf32_unicode_character,
+			          utf32_string,
+			          utf32_string_size,
+			          &utf32_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_from_ucs4(
+			          &utf32_unicode_character,
+			          utf32_string,
+			          utf32_string_size,
+			          &utf32_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character from UTF-32.",
 			 function );
@@ -2548,26 +2552,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 1 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -2755,26 +2747,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 1 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -2932,26 +2912,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf32_string_size >= 1 )
 	 && ( utf32_string[ utf32_string_size - 1 ] == 0 ) )
 	{
 		utf32_string_size -= 1;
 	}
 	/* Check if the UTF-32 stream is terminated with zero bytes
 	 */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_thai.h` & `liblnk-20230716/libuna/libuna_codepage_mac_thai.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_874.c` & `liblnk-20230716/libuna/libuna_codepage_windows_874.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1251.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1251.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_libcerror.h` & `liblnk-20230716/libuna/libuna_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_949.c` & `liblnk-20230716/libuna/libuna_codepage_windows_949.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_6.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_5.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-6 codepage (Arabic) functions
+ * ISO 8859-5 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_6_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_6_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_5_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_6_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_6_unicode_to_byte_stream_base_0x0618[ 64 ];
+const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_6_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1256.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1256.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_greek.h` & `liblnk-20230716/libuna/libuna_codepage_mac_greek.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_russian.h` & `liblnk-20230716/libuna/libuna_codepage_mac_russian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_ukrainian.h` & `liblnk-20230716/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_6.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_6.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_874.h` & `liblnk-20230716/libuna/libuna_codepage_windows_874.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1251.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1251.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1256.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_base16_stream.h` & `liblnk-20230716/libuna/libuna_base16_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_2.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_2.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/Makefile.am` & `liblnk-20230716/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1257.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1257.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1254.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1252.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1254 codepage (Turkish) functions
+ * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1254_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1252_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1252_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1254_copy_from_byte_stream(
+int libuna_codepage_windows_1252_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1254_copy_to_byte_stream(
+int libuna_codepage_windows_1252_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1252_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1255.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1255.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_unused.h` & `liblnk-20230716/libuna/libuna_unused.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1253.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1253.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_unicode_character.h` & `liblnk-20230716/libuna/libuna_unicode_character.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -56,14 +56,58 @@
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      int codepage,
      libcerror_error_t **error );
 
 LIBUNA_EXTERN \
+int libuna_unicode_character_size_to_ucs2(
+     libuna_unicode_character_t unicode_character,
+     size_t *ucs2_character_size,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_from_ucs2(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf16_character_t *ucs2_string,
+     size_t ucs2_string_size,
+     size_t *ucs2_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_to_ucs2(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf16_character_t *ucs2_string,
+     size_t ucs2_string_size,
+     size_t *ucs2_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_size_to_ucs4(
+     libuna_unicode_character_t unicode_character,
+     size_t *ucs4_character_size,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_from_ucs4(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf32_character_t *ucs4_string,
+     size_t ucs4_string_size,
+     size_t *ucs4_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_to_ucs4(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf32_character_t *ucs4_string,
+     size_t ucs4_string_size,
+     size_t *ucs4_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
 int libuna_unicode_character_size_to_utf7_stream(
      libuna_unicode_character_t unicode_character,
      size_t *utf7_stream_character_size,
      uint32_t *utf7_stream_base64_data,
      libcerror_error_t **error );
 
 LIBUNA_EXTERN \
@@ -103,14 +147,36 @@
      libuna_unicode_character_t unicode_character,
      libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf8_string_index,
      libcerror_error_t **error );
 
 LIBUNA_EXTERN \
+int libuna_unicode_character_size_to_utf8_rfc2279(
+     libuna_unicode_character_t unicode_character,
+     size_t *utf8_character_size,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_from_utf8_rfc2279(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf8_character_t *utf8_string,
+     size_t utf8_string_size,
+     size_t *utf8_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
+int libuna_unicode_character_copy_to_utf8_rfc2279(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf8_character_t *utf8_string,
+     size_t utf8_string_size,
+     size_t *utf8_string_index,
+     libcerror_error_t **error );
+
+LIBUNA_EXTERN \
 int libuna_unicode_character_size_to_utf16(
      libuna_unicode_character_t unicode_character,
      size_t *utf16_character_size,
      libcerror_error_t **error );
 
 LIBUNA_EXTERN \
 int libuna_unicode_character_copy_from_utf16(
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_dingbats.h` & `liblnk-20230716/libuna/libuna_codepage_mac_dingbats.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_scsu.c` & `liblnk-20230716/libuna/libuna_scsu.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_byte_stream.c` & `liblnk-20230716/libuna/libuna_byte_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_celtic.h` & `liblnk-20230716/libuna/libuna_codepage_mac_celtic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_croatian.c` & `liblnk-20230716/libuna/libuna_codepage_mac_croatian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_3.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_3.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_15.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_15.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_roman.c` & `liblnk-20230716/libuna/libuna_codepage_mac_roman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf32_string.h` & `liblnk-20230716/libuna/libuna_utf32_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_koi8_r.c` & `liblnk-20230716/libuna/libuna_codepage_koi8_r.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_icelandic.c` & `liblnk-20230716/libuna/libuna_codepage_mac_icelandic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_936.h` & `liblnk-20230716/libuna/libuna_codepage_windows_936.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_base64_stream.h` & `liblnk-20230716/libuna/libuna_base64_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_celtic.c` & `liblnk-20230716/libuna/libuna_codepage_mac_celtic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_950.c` & `liblnk-20230716/libuna/libuna_codepage_windows_950.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf8_string.h` & `liblnk-20230716/libuna/libuna_utf8_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_936.c` & `liblnk-20230716/libuna/libuna_codepage_windows_936.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_unicode_character.c` & `liblnk-20230716/libuna/libuna_unicode_character.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -2142,14 +2142,497 @@
 		return( -1 );
 	}
 	*byte_stream_index = safe_byte_stream_index;
 
 	return( result );
 }
 
+/* Determines the size of an UCS-2 character from an Unicode character
+ * Adds the size to the UCS-2 character size value
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_size_to_ucs2(
+     libuna_unicode_character_t unicode_character,
+     size_t *ucs2_character_size,
+     libcerror_error_t **error )
+{
+	static char *function = "libuna_unicode_character_size_to_ucs2";
+
+	if( ucs2_character_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 character size.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine if the Unicode character is valid
+	 * UCS-2 with surrogate pairs supports upto 0x10ffff characters
+	 */
+	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character > LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
+	{
+		*ucs2_character_size += 2;
+	}
+	else
+	{
+		*ucs2_character_size += 1;
+	}
+	return( 1 );
+}
+
+/* Copies an Unicode character from an UCS-2 string
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_from_ucs2(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf16_character_t *ucs2_string,
+     size_t ucs2_string_size,
+     size_t *ucs2_string_index,
+     libcerror_error_t **error )
+{
+	static char *function                             = "libuna_unicode_character_copy_from_ucs2";
+	libuna_utf16_character_t ucs2_surrogate           = 0;
+	libuna_unicode_character_t safe_unicode_character = 0;
+	size_t safe_ucs2_string_index                     = 0;
+
+	if( unicode_character == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UCS-2 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_ucs2_string_index = *ucs2_string_index;
+
+	if( safe_ucs2_string_index >= ucs2_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UCS-2 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	safe_unicode_character  = ucs2_string[ safe_ucs2_string_index ];
+	safe_ucs2_string_index += 1;
+
+	/* Determine if the UCS-2 character is within the high surrogate range
+	 */
+	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_END ) )
+	{
+		if( safe_ucs2_string_index >= ucs2_string_size )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+			 "%s: missing surrogate UCS-2 character bytes.",
+			 function );
+
+			return( -1 );
+		}
+		ucs2_surrogate = ucs2_string[ safe_ucs2_string_index ];
+
+		/* Determine if the UCS-2 character is within the low surrogate range
+		 */
+		if( ( ucs2_surrogate >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
+		 && ( ucs2_surrogate <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+		{
+			safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
+			safe_unicode_character <<= 10;
+			safe_unicode_character  += ucs2_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
+			safe_unicode_character  += 0x010000;
+
+			safe_ucs2_string_index += 1;
+		}
+	}
+	/* Determine if the Unicode character is valid
+	 * UCS-2 with surrogate pairs supports upto 0x10ffff characters
+	 */
+	if( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	*unicode_character = safe_unicode_character;
+	*ucs2_string_index = safe_ucs2_string_index;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character into a UCS-2 string
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_to_ucs2(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf16_character_t *ucs2_string,
+     size_t ucs2_string_size,
+     size_t *ucs2_string_index,
+     libcerror_error_t **error )
+{
+	static char *function         = "libuna_unicode_character_copy_to_ucs2";
+	size_t safe_ucs2_string_index = 0;
+
+	if( ucs2_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UCS-2 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs2_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-2 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_ucs2_string_index = *ucs2_string_index;
+
+	if( safe_ucs2_string_index >= ucs2_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UCS-2 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character <= LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
+	{
+		ucs2_string[ safe_ucs2_string_index++ ] = (libuna_utf16_character_t) unicode_character;
+	}
+	else
+	{
+		if( ( ucs2_string_size < 2 )
+		 || ( safe_ucs2_string_index > ( ucs2_string_size - 2 ) ) )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+			 "%s: UCS-2 string too small.",
+			 function );
+
+			return( -1 );
+		}
+		unicode_character                      -= 0x010000;
+		ucs2_string[ safe_ucs2_string_index++ ] = (libuna_utf16_character_t) ( ( unicode_character >> 10 ) + LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START );
+		ucs2_string[ safe_ucs2_string_index++ ] = (libuna_utf16_character_t) ( ( unicode_character & 0x03ff ) + LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START );
+	}
+	*ucs2_string_index = safe_ucs2_string_index;
+
+	return( 1 );
+}
+
+/* Determines the size of an UCS-4 character from an Unicode character
+ * Adds the size to the UCS-4 character size value
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_size_to_ucs4(
+     libuna_unicode_character_t unicode_character,
+     size_t *ucs4_character_size,
+     libcerror_error_t **error )
+{
+	static char *function = "libuna_unicode_character_size_to_ucs4";
+
+	LIBUNA_UNREFERENCED_PARAMETER( unicode_character )
+
+	if( ucs4_character_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 character size.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	*ucs4_character_size += 1;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character from an UCS-4 string
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_from_ucs4(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf32_character_t *ucs4_string,
+     size_t ucs4_string_size,
+     size_t *ucs4_string_index,
+     libcerror_error_t **error )
+{
+	static char *function                             = "libuna_unicode_character_copy_from_ucs4";
+	libuna_unicode_character_t safe_unicode_character = 0;
+	size_t safe_ucs4_string_index                     = 0;
+
+	if( unicode_character == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UCS-4 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_ucs4_string_index = *ucs4_string_index;
+
+	if( safe_ucs4_string_index >= ucs4_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UCS-4 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	safe_unicode_character = ucs4_string[ safe_ucs4_string_index ];
+
+	/* Determine if the Unicode character is valid
+	 */
+	if( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	*unicode_character = safe_unicode_character;
+	*ucs4_string_index = safe_ucs4_string_index + 1;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character into a UCS-4 string
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_to_ucs4(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf32_character_t *ucs4_string,
+     size_t ucs4_string_size,
+     size_t *ucs4_string_index,
+     libcerror_error_t **error )
+{
+	static char *function         = "libuna_unicode_character_copy_to_ucs4";
+	size_t safe_ucs4_string_index = 0;
+
+	if( ucs4_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UCS-4 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( ucs4_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UCS-4 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_ucs4_string_index = *ucs4_string_index;
+
+	if( safe_ucs4_string_index >= ucs4_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UCS-4 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	ucs4_string[ safe_ucs4_string_index ] = (libuna_utf32_character_t) unicode_character;
+
+	*ucs4_string_index = safe_ucs4_string_index + 1;
+
+	return( 1 );
+}
+
 /* Determines the size of an UTF-7 stream character from an Unicode character
  * Adds the size to the UTF-7 stream character size value
  * Returns 1 if successful or -1 on error
  */
 int libuna_unicode_character_size_to_utf7_stream(
      libuna_unicode_character_t unicode_character,
      size_t *utf7_stream_character_size,
@@ -2189,17 +2672,26 @@
 		return( -1 );
 	}
 	safe_utf7_stream_character_size = *utf7_stream_character_size;
 	safe_utf7_stream_base64_data    = *utf7_stream_base64_data;
 
 	/* Determine if the Unicode character is valid
 	 */
-	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	/* The + character must be escaped
 	 */
 	if( unicode_character == (libuna_unicode_character_t) '+' )
 	{
 	}
 	/* Allow for the end of string character
@@ -2715,15 +3207,22 @@
 				safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
 				safe_unicode_character <<= 10;
 				safe_unicode_character  += utf16_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
 				safe_unicode_character  += 0x010000;
 			}
 			else
 			{
-				safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+				 "%s: unsupported low surrogate UTF-16 character.",
+				 function );
+
+				return( -1 );
 			}
 		}
 		if( safe_utf7_stream_index >= utf7_stream_size )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -2829,17 +3328,26 @@
 		return( -1 );
 	}
 	safe_utf7_stream_index       = *utf7_stream_index;
 	safe_utf7_stream_base64_data = *utf7_stream_base64_data;
 
 	/* Determine if the Unicode character is valid
 	 */
-	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	/* A-Z is not a continous range on an EBCDIC based system
 	 * it consists of the ranges: A-I, J-R, S-Z
 	 */
 	if( ( unicode_character >= 0x41 )
 	 && ( unicode_character <= 0x49 ) )
 	{
@@ -3143,14 +3651,15 @@
 	*utf7_stream_index       = safe_utf7_stream_index;
 	*utf7_stream_base64_data = safe_utf7_stream_base64_data;
 
 	return( 1 );
 }
 
 /* Determines the size of an UTF-8 character from an Unicode character
+ * This function supports upto U+10FFFF (4 byte UTF-8 characters)
  * Adds the size to the UTF-8 character size value
  * Returns 1 if successful or -1 on error
  */
 int libuna_unicode_character_size_to_utf8(
      libuna_unicode_character_t unicode_character,
      size_t *utf8_character_size,
      libcerror_error_t **error )
@@ -3165,65 +3674,55 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-8 character size.",
 		 function );
 
 		return( -1 );
 	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	/* RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
 	if( unicode_character < 0x00000080UL )
 	{
 		safe_utf8_character_size += 1;
 	}
 	else if( unicode_character < 0x00000800UL )
 	{
 		safe_utf8_character_size += 2;
 	}
 	else if( unicode_character < 0x00010000UL )
 	{
 		safe_utf8_character_size += 3;
 	}
-	else if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
-	{
-		safe_utf8_character_size += 3;
-	}
 	else
 	{
 		safe_utf8_character_size += 4;
 	}
-
-/* If UTF-8 USC support is needed it should be implemented in
- * utf8_usc or something, but for now leave this here as a reminder
-
-	else if( unicode_character < 0x010000 )
-	{
-		safe_utf8_character_size += 3;
-	}
-	else if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
-	{
-		safe_utf8_character_size += 2;
-	}
-	else if( unicode_character < 0x0200000 )
-	{
-		safe_utf8_character_size += 4;
-	}
-	else if( unicode_character < 0x0400000 )
-	{
-		safe_utf8_character_size += 5;
-	}
-	else
-	{
-		safe_utf8_character_size += 6;
-	}
-*/
 	*utf8_character_size += safe_utf8_character_size;
 
 	return( 1 );
 }
 
 /* Copies an Unicode character from an UTF-8 string
+ * This function supports upto U+10FFFF (4 byte UTF-8 characters)
  * Returns 1 if successful or -1 on error
  */
 int libuna_unicode_character_copy_from_utf8(
      libuna_unicode_character_t *unicode_character,
      const libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf8_string_index,
@@ -3232,16 +3731,16 @@
 	static char *function                             = "libuna_unicode_character_copy_from_utf8";
 	libuna_unicode_character_t safe_unicode_character = 0;
 	size_t safe_utf8_string_index                     = 0;
 	uint8_t byte_value1                               = 0;
 	uint8_t byte_value2                               = 0;
 	uint8_t byte_value3                               = 0;
 	uint8_t byte_value4                               = 0;
-	uint8_t byte_value5                               = 0;
 	uint8_t utf8_character_additional_bytes           = 0;
+	int result                                        = 0;
 
 	if( unicode_character == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -3296,72 +3795,63 @@
 
 		return( -1 );
 	}
 	/* Determine the number of additional bytes of the UTF-8 character
 	 */
 	byte_value1 = utf8_string[ safe_utf8_string_index ];
 
+	/* Determine the UTF-8 character and make sure it is valid
+	 * RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
+	if( byte_value1 > 0xf4 )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
+		 function,
+		 byte_value1 );
+
+		return( -1 );
+	}
 	if( byte_value1 < 0xc0 )
 	{
 		utf8_character_additional_bytes = 0;
 	}
 	else if( byte_value1 < 0xe0 )
 	{
 		utf8_character_additional_bytes = 1;
 	}
 	else if( byte_value1 < 0xf0 )
 	{
 		utf8_character_additional_bytes = 2;
 	}
-	else if( byte_value1 < 0xf8 )
-	{
-		utf8_character_additional_bytes = 3;
-	}
-	else if( byte_value1 < 0xfc )
-	{
-		utf8_character_additional_bytes = 4;
-	}
 	else
 	{
-		utf8_character_additional_bytes = 5;
+		utf8_character_additional_bytes = 3;
 	}
 	if( ( ( (size_t) utf8_character_additional_bytes + 1 ) > utf8_string_size )
 	 || ( safe_utf8_string_index > ( utf8_string_size - ( utf8_character_additional_bytes + 1 ) ) ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
 		 "%s: missing UTF-8 character bytes.",
 		 function );
 
 		return( -1 );
 	}
-	/* Determine the UTF-8 character and make sure it is valid
-	 * Unicode limits the UTF-8 character to consist of a maximum of 4 bytes
-	 * while ISO 10646 Universal Character Set (UCS) allows up to 6 bytes
-	 */
-	if( byte_value1 > 0xf4 )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
-		 function,
-		 byte_value1 );
-
-		return( -1 );
-	}
 	safe_unicode_character = byte_value1;
 
 	if( utf8_character_additional_bytes == 0 )
 	{
-		if( ( byte_value1 >= 0x80 )
-		 && ( byte_value1 < 0xc2 ) )
+		if( byte_value1 >= 0x80 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 			 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
@@ -3370,79 +3860,552 @@
 			return( -1 );
 		}
 	}
 	if( utf8_character_additional_bytes >= 1 )
 	{
 		byte_value2 = utf8_string[ safe_utf8_string_index + 1 ];
 
-		if( byte_value2 > 0xbf )
+		if( ( byte_value2 < 0x80 )
+		 || ( byte_value2 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
 			 byte_value2 );
 
 			return( -1 );
 		}
-		if( ( byte_value1 == 0xe0 )
-		 && ( byte_value2 < 0xa0 ) )
+		result = 1;
+
+		switch( byte_value1 )
+		{
+			case 0xe0:
+				if( ( byte_value2 < 0xa0 )
+				 || ( byte_value2 > 0xbf ) )
+				{
+					result = 0;
+				}
+				break;
+
+			case 0xed:
+				if( ( byte_value2 < 0x80 )
+				 || ( byte_value2 > 0x9f ) )
+				{
+					result = 0;
+				}
+				break;
+
+			case 0xf0:
+				if( ( byte_value2 < 0x90 )
+				 || ( byte_value2 > 0xbf ) )
+				{
+					result = 0;
+				}
+				break;
+
+			case 0xf4:
+				if( ( byte_value2 < 0x80 )
+				 || ( byte_value2 > 0xbf ) )
+				{
+					result = 0;
+				}
+				break;
+
+			default:
+				break;
+		}
+		if( result == 0 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
+			 "%s: invalid 1st and 2nd UTF-8 character byte pair: 0x%02" PRIx8 " 0x%02" PRIx8 ".",
 			 function,
+			 byte_value1,
 			 byte_value2 );
 
 			return( -1 );
 		}
-		else if( ( byte_value1 == 0xed )
-		      && ( byte_value2 > 0x9f ) )
+		safe_unicode_character <<= 6;
+		safe_unicode_character += byte_value2;
+
+		if( utf8_character_additional_bytes == 1 )
+		{
+			safe_unicode_character -= 0x03080;
+		}
+	}
+	if( utf8_character_additional_bytes >= 2 )
+	{
+		byte_value3 = utf8_string[ safe_utf8_string_index + 2 ];
+
+		if( ( byte_value3 < 0x80 )
+		 || ( byte_value3 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
+			 "%s: invalid 3rd UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
-			 byte_value2 );
+			 byte_value3 );
 
 			return( -1 );
 		}
-		else if( ( byte_value1 == 0xf0 )
-		      && ( byte_value2 < 0x90 ) )
+		result = 1;
+
+		switch( byte_value2 )
+		{
+			case 0xe0:
+				if( ( byte_value2 < 0xa0 )
+				 || ( byte_value2 > 0xbf ) )
+				{
+					result = 0;
+				}
+				break;
+
+			case 0xed:
+				if( ( byte_value2 < 0x80 )
+				 || ( byte_value2 > 0x9f ) )
+				{
+					result = 0;
+				}
+				break;
+
+			default:
+				break;
+		}
+		if( result == 0 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
+			 "%s: invalid 2nd and 3rd UTF-8 character byte pair: 0x%02" PRIx8 " 0x%02" PRIx8 ".",
 			 function,
-			 byte_value2 );
+			 byte_value2,
+			 byte_value3 );
 
 			return( -1 );
 		}
-		else if( ( byte_value1 == 0xf4 )
-		      && ( byte_value2 > 0x8f ) )
+		safe_unicode_character <<= 6;
+		safe_unicode_character += byte_value3;
+
+		if( utf8_character_additional_bytes == 2 )
+		{
+			safe_unicode_character -= 0x0e2080;
+		}
+	}
+	if( utf8_character_additional_bytes >= 3 )
+	{
+		byte_value4 = utf8_string[ safe_utf8_string_index + 3 ];
+
+		if( ( byte_value4 < 0x80 )
+		 || ( byte_value4 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
+			 "%s: invalid 4th UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
-			 byte_value2 );
+			 byte_value4 );
 
 			return( -1 );
 		}
-		else if( byte_value2 < 0x80 )
+		safe_unicode_character <<= 6;
+		safe_unicode_character += byte_value4;
+
+		if( utf8_character_additional_bytes == 3 )
+		{
+			safe_unicode_character -= 0x03c82080;
+		}
+	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( ( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	*unicode_character = safe_unicode_character;
+	*utf8_string_index = safe_utf8_string_index + 1 + utf8_character_additional_bytes;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character into a UTF-8 string
+ * This function supports upto U+10FFFF (4 byte UTF-8 characters)
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_to_utf8(
+     libuna_unicode_character_t unicode_character,
+     libuna_utf8_character_t *utf8_string,
+     size_t utf8_string_size,
+     size_t *utf8_string_index,
+     libcerror_error_t **error )
+{
+	static char *function                   = "libuna_unicode_character_copy_to_utf8";
+	size_t safe_utf8_string_index           = 0;
+	size_t utf8_character_iterator          = 0;
+	uint8_t utf8_character_additional_bytes = 0;
+	uint8_t utf8_first_character_mark       = 0;
+
+	if( utf8_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UTF-8 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_utf8_string_index = *utf8_string_index;
+
+	if( safe_utf8_string_index >= utf8_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UTF-8 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine if the Unicode character is valid
+	 */
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine how many UTF-8 character bytes are required
+	 */
+	if( unicode_character < 0x080 )
+	{
+		utf8_character_additional_bytes = 0;
+		utf8_first_character_mark       = 0;
+	}
+	else if( unicode_character < 0x0800 )
+	{
+		utf8_character_additional_bytes = 1;
+		utf8_first_character_mark       = 0x0c0;
+	}
+	else if( unicode_character < 0x010000 )
+	{
+		utf8_character_additional_bytes = 2;
+		utf8_first_character_mark       = 0x0e0;
+	}
+	else
+	{
+		utf8_character_additional_bytes = 3;
+		utf8_first_character_mark       = 0x0f0;
+	}
+	/* Convert Unicode character into UTF-8 character bytes
+	 */
+	if( ( utf8_character_additional_bytes > utf8_string_size )
+	 || ( safe_utf8_string_index >= ( utf8_string_size - utf8_character_additional_bytes ) ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UTF-8 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	for( utf8_character_iterator = safe_utf8_string_index + utf8_character_additional_bytes;
+	     utf8_character_iterator > safe_utf8_string_index;
+	     utf8_character_iterator-- )
+	{
+		utf8_string[ utf8_character_iterator ] = (libuna_utf8_character_t) ( ( unicode_character & 0x0bf ) | 0x080 );
+
+		unicode_character >>= 6;
+	}
+	utf8_string[ safe_utf8_string_index ] = (libuna_utf8_character_t) ( unicode_character | utf8_first_character_mark );
+
+	*utf8_string_index = safe_utf8_string_index + 1 + utf8_character_additional_bytes;
+
+	return( 1 );
+}
+
+/* Determines the size of an UTF-8 character from an Unicode character
+ * This function supports upto U+7FFFFFF (6 byte UTF-8 characters)
+ * Adds the size to the UTF-8 character size value
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_size_to_utf8_rfc2279(
+     libuna_unicode_character_t unicode_character,
+     size_t *utf8_character_size,
+     libcerror_error_t **error )
+{
+	static char *function           = "libuna_unicode_character_size_to_utf8_rfc2279";
+	size_t safe_utf8_character_size = 0;
+
+	if( utf8_character_size == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 character size.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	/* RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
+	if( unicode_character < 0x00000080UL )
+	{
+		safe_utf8_character_size += 1;
+	}
+	else if( unicode_character < 0x00000800UL )
+	{
+		safe_utf8_character_size += 2;
+	}
+	else if( unicode_character < 0x00010000UL )
+	{
+		safe_utf8_character_size += 3;
+	}
+	else if( unicode_character < 0x00200000UL )
+	{
+		safe_utf8_character_size += 4;
+	}
+	else if( unicode_character < 0x04000000UL )
+	{
+		safe_utf8_character_size += 5;
+	}
+	else
+	{
+		safe_utf8_character_size += 6;
+	}
+	*utf8_character_size += safe_utf8_character_size;
+
+	return( 1 );
+}
+
+/* Copies an Unicode character from an UTF-8 string
+ * This function supports upto U+7FFFFFF (6 byte UTF-8 characters)
+ * Returns 1 if successful or -1 on error
+ */
+int libuna_unicode_character_copy_from_utf8_rfc2279(
+     libuna_unicode_character_t *unicode_character,
+     const libuna_utf8_character_t *utf8_string,
+     size_t utf8_string_size,
+     size_t *utf8_string_index,
+     libcerror_error_t **error )
+{
+	static char *function                             = "libuna_unicode_character_copy_from_utf8_rfc2279";
+	libuna_unicode_character_t safe_unicode_character = 0;
+	size_t safe_utf8_string_index                     = 0;
+	uint8_t byte_value1                               = 0;
+	uint8_t byte_value2                               = 0;
+	uint8_t byte_value3                               = 0;
+	uint8_t byte_value4                               = 0;
+	uint8_t byte_value5                               = 0;
+	uint8_t byte_value6                               = 0;
+	uint8_t utf8_character_additional_bytes           = 0;
+
+	if( unicode_character == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_size > (size_t) SSIZE_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_EXCEEDS_MAXIMUM,
+		 "%s: invalid UTF-8 string size value exceeds maximum.",
+		 function );
+
+		return( -1 );
+	}
+	if( utf8_string_index == NULL )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
+		 "%s: invalid UTF-8 string index.",
+		 function );
+
+		return( -1 );
+	}
+	safe_utf8_string_index = *utf8_string_index;
+
+	if( safe_utf8_string_index >= utf8_string_size )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: UTF-8 string too small.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine the number of additional bytes of the UTF-8 character
+	 */
+	byte_value1 = utf8_string[ safe_utf8_string_index ];
+
+	/* Determine the UTF-8 character and make sure it is valid
+	 * RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
+	if( byte_value1 > 0xfd )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+		 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
+		 function,
+		 byte_value1 );
+
+		return( -1 );
+	}
+	if( byte_value1 < 0xc0 )
+	{
+		utf8_character_additional_bytes = 0;
+	}
+	else if( byte_value1 < 0xe0 )
+	{
+		utf8_character_additional_bytes = 1;
+	}
+	else if( byte_value1 < 0xf0 )
+	{
+		utf8_character_additional_bytes = 2;
+	}
+	else if( byte_value1 < 0xf8 )
+	{
+		utf8_character_additional_bytes = 3;
+	}
+	else if( byte_value1 < 0xfc )
+	{
+		utf8_character_additional_bytes = 4;
+	}
+	else
+	{
+		utf8_character_additional_bytes = 5;
+	}
+	if( ( ( (size_t) utf8_character_additional_bytes + 1 ) > utf8_string_size )
+	 || ( safe_utf8_string_index > ( utf8_string_size - ( utf8_character_additional_bytes + 1 ) ) ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
+		 "%s: missing UTF-8 character bytes.",
+		 function );
+
+		return( -1 );
+	}
+	/* Determine the UTF-8 character and make sure it is valid
+	 * RFC 3629 limits the UTF-8 character to consist of a maximum of 4 bytes
+	 * while its predecessor RFC 2279 allowed up to 6 bytes
+	 */
+	safe_unicode_character = byte_value1;
+
+	if( utf8_character_additional_bytes == 0 )
+	{
+		if( byte_value1 >= 0x80 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
+			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
+			 "%s: invalid 1st UTF-8 character byte: 0x%02" PRIx8 ".",
+			 function,
+			 byte_value1 );
+
+			return( -1 );
+		}
+	}
+	if( utf8_character_additional_bytes >= 1 )
+	{
+		byte_value2 = utf8_string[ safe_utf8_string_index + 1 ];
+
+		if( ( byte_value2 < 0x80 )
+		 || ( byte_value2 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 			 "%s: invalid 2nd UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
@@ -3531,54 +4494,64 @@
 		if( utf8_character_additional_bytes == 4 )
 		{
 			safe_unicode_character -= 0x0fa082080;
 		}
 	}
 	if( utf8_character_additional_bytes == 5 )
 	{
-		if( ( utf8_string[ safe_utf8_string_index + 5 ] < 0x80 )
-		  || ( utf8_string[ safe_utf8_string_index + 5 ] > 0xbf ) )
+		byte_value6 = utf8_string[ safe_utf8_string_index + 5 ];
+
+		if( ( byte_value6 < 0x80 )
+		  || ( byte_value6 > 0xbf ) )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 			 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 			 "%s: invalid 6th UTF-8 character byte: 0x%02" PRIx8 ".",
 			 function,
-			 utf8_string[ safe_utf8_string_index + 5 ] );
+			 byte_value6 );
 
 			return( -1 );
 		}
 		safe_unicode_character <<= 6;
-		safe_unicode_character += utf8_string[ safe_utf8_string_index + 5 ];
+		safe_unicode_character += byte_value6;
 		safe_unicode_character -= 0x082082080;
 	}
 	/* Determine if the Unicode character is valid
 	 */
-	if( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	if( safe_unicode_character > LIBUNA_UCS_CHARACTER_MAX )
 	{
-		safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character = safe_unicode_character;
 	*utf8_string_index = safe_utf8_string_index + 1 + utf8_character_additional_bytes;
 
 	return( 1 );
 }
 
 /* Copies an Unicode character into a UTF-8 string
+ * This function supports upto U+7FFFFFF (6 byte UTF-8 characters)
  * Returns 1 if successful or -1 on error
  */
-int libuna_unicode_character_copy_to_utf8(
+int libuna_unicode_character_copy_to_utf8_rfc2279(
      libuna_unicode_character_t unicode_character,
      libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf8_string_index,
      libcerror_error_t **error )
 {
-	static char *function                   = "libuna_unicode_character_copy_to_utf8";
+	static char *function                   = "libuna_unicode_character_copy_to_utf8_rfc2279";
 	size_t safe_utf8_string_index           = 0;
 	size_t utf8_character_iterator          = 0;
 	uint8_t utf8_character_additional_bytes = 0;
 	uint8_t utf8_first_character_mark       = 0;
 
 	if( utf8_string == NULL )
 	{
@@ -3624,17 +4597,24 @@
 		 "%s: UTF-8 string too small.",
 		 function );
 
 		return( -1 );
 	}
 	/* Determine if the Unicode character is valid
 	 */
-	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	if( unicode_character > LIBUNA_UCS_CHARACTER_MAX )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	/* Determine how many UTF-8 character bytes are required
 	 */
 	if( unicode_character < 0x080 )
 	{
 		utf8_character_additional_bytes = 0;
 		utf8_first_character_mark       = 0;
@@ -3711,16 +4691,28 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-16 character size.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( unicode_character > LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
-         && ( unicode_character <= LIBUNA_UTF16_CHARACTER_MAX ) )
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
+	if( unicode_character > LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
 	{
 		*utf16_character_size += 2;
 	}
 	else
 	{
 		*utf16_character_size += 1;
 	}
@@ -3829,23 +4821,38 @@
 			safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
 			safe_unicode_character <<= 10;
 			safe_unicode_character  += utf16_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
 			safe_unicode_character  += 0x010000;
 		}
 		else
 		{
-			safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+			 "%s: unsupported low surrogate UTF-16 character.",
+			 function );
+
+			return( -1 );
 		}
 	}
 	/* Determine if the Unicode character is valid
 	 */
-	else if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
-	      && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	if( ( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character  = safe_unicode_character;
 	*utf16_string_index = safe_utf16_string_index;
 
 	return( 1 );
 }
 
@@ -3907,18 +4914,25 @@
 		 function );
 
 		return( -1 );
 	}
 	/* Determine if the Unicode character is valid
 	 */
 	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	  && ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-	 || ( unicode_character > LIBUNA_UTF16_CHARACTER_MAX ) )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	if( unicode_character <= LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
 	{
 		utf16_string[ safe_utf16_string_index++ ] = (libuna_utf16_character_t) unicode_character;
 	}
 	else
 	{
@@ -3954,14 +4968,15 @@
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                             = "libuna_unicode_character_copy_from_utf16_stream";
 	libuna_unicode_character_t safe_unicode_character = 0;
 	libuna_utf16_character_t utf16_surrogate          = 0;
 	size_t safe_utf16_stream_index                    = 0;
+	int byte_order_without_flags                      = 0;
 
 	if( unicode_character == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -3999,16 +5014,18 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-16 stream index.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
+	byte_order_without_flags = byte_order & 0xff;
+
+	if( ( byte_order_without_flags != LIBUNA_ENDIAN_BIG )
+	 && ( byte_order_without_flags != LIBUNA_ENDIAN_LITTLE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 		 "%s: unsupported byte order.",
 		 function );
@@ -4025,90 +5042,113 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
 		 "%s: UTF-16 stream too small.",
 		 function );
 
 		return( -1 );
 	}
-	if( byte_order == LIBUNA_ENDIAN_BIG )
+	if( byte_order_without_flags == LIBUNA_ENDIAN_BIG )
 	{
 		safe_unicode_character   = utf16_stream[ safe_utf16_stream_index ];
 		safe_unicode_character <<= 8;
 		safe_unicode_character  += utf16_stream[ safe_utf16_stream_index + 1 ];
 	}
-	else if( byte_order == LIBUNA_ENDIAN_LITTLE )
+	else if( byte_order_without_flags == LIBUNA_ENDIAN_LITTLE )
 	{
 		safe_unicode_character   = utf16_stream[ safe_utf16_stream_index + 1 ];
 		safe_unicode_character <<= 8;
 		safe_unicode_character  += utf16_stream[ safe_utf16_stream_index ];
 	}
 	safe_utf16_stream_index += 2;
 
 	/* Determine if the Unicode character is valid
 	 */
 	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
 	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
 	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported UTF-16 character.",
-		 function );
-
-		return( -1 );
-	}
-	/* Determine if the UTF-16 character is within the high surrogate range
-	 */
-	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_END ) )
-	{
-		if( safe_utf16_stream_index > ( utf16_stream_size - 2 ) )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: missing surrogate UTF-16 character bytes.",
+			 "%s: unsupported UTF-16 character.",
 			 function );
 
 			return( -1 );
 		}
-		if( byte_order == LIBUNA_ENDIAN_BIG )
+	}
+	/* Determine if the UTF-16 character is within the high surrogate range
+	 */
+	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_END ) )
+	{
+		if( safe_utf16_stream_index > ( utf16_stream_size - 2 ) )
 		{
-			utf16_surrogate   = utf16_stream[ safe_utf16_stream_index ];
-			utf16_surrogate <<= 8;
-			utf16_surrogate  += utf16_stream[ safe_utf16_stream_index + 1 ];
+			if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+				 "%s: missing surrogate UTF-16 character bytes.",
+				 function );
+
+				return( -1 );
+			}
 		}
-		else if( byte_order == LIBUNA_ENDIAN_LITTLE )
+		else
 		{
-			utf16_surrogate   = utf16_stream[ safe_utf16_stream_index + 1 ];
-			utf16_surrogate <<= 8;
-			utf16_surrogate  += utf16_stream[ safe_utf16_stream_index ];
-		}
-		safe_utf16_stream_index += 2;
+			if( byte_order_without_flags == LIBUNA_ENDIAN_BIG )
+			{
+				utf16_surrogate   = utf16_stream[ safe_utf16_stream_index ];
+				utf16_surrogate <<= 8;
+				utf16_surrogate  += utf16_stream[ safe_utf16_stream_index + 1 ];
+			}
+			else if( byte_order_without_flags == LIBUNA_ENDIAN_LITTLE )
+			{
+				utf16_surrogate   = utf16_stream[ safe_utf16_stream_index + 1 ];
+				utf16_surrogate <<= 8;
+				utf16_surrogate  += utf16_stream[ safe_utf16_stream_index ];
+			}
+			/* Determine if the UTF-16 character is within the low surrogate range
+			 */
+			if( ( utf16_surrogate >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
+			 && ( utf16_surrogate <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+			{
+				safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
+				safe_unicode_character <<= 10;
+				safe_unicode_character  += utf16_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
+				safe_unicode_character  += 0x010000;
 
-		/* Determine if the UTF-16 character is within the low surrogate range
-		 */
-		if( ( utf16_surrogate < LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
-		 || ( utf16_surrogate > LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-		{
-			libcerror_error_set(
-			 error,
-			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
-			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
-			 "%s: unsupported low surrogate UTF-16 character.",
-			 function );
+				safe_utf16_stream_index += 2;
+			}
+			else if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+			{
+				libcerror_error_set(
+				 error,
+				 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+				 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+				 "%s: unsupported low surrogate UTF-16 character.",
+				 function );
 
-			return( -1 );
+				return( -1 );
+			}
 		}
-		safe_unicode_character  -= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START;
-		safe_unicode_character <<= 10;
-		safe_unicode_character  += utf16_surrogate - LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START;
-		safe_unicode_character  += 0x010000;
+	}
+	if( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character  = safe_unicode_character;
 	*utf16_stream_index = safe_utf16_stream_index;
 
 	return( 1 );
 }
 
@@ -4122,14 +5162,15 @@
      size_t *utf16_stream_index,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                    = "libuna_unicode_character_copy_to_utf16_stream";
 	libuna_utf16_character_t utf16_surrogate = 0;
 	size_t safe_utf16_stream_index           = 0;
+	int byte_order_without_flags             = 0;
 
 	if( utf16_stream == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -4156,43 +5197,58 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-16 stream index.",
 		 function );
 
 		return( -1 );
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
+	byte_order_without_flags = byte_order & 0xff;
+
+	if( ( byte_order_without_flags != LIBUNA_ENDIAN_BIG )
+	 && ( byte_order_without_flags != LIBUNA_ENDIAN_LITTLE ) )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
 		 "%s: unsupported byte order.",
 		 function );
 
 		return( -1 );
 	}
 	safe_utf16_stream_index = *utf16_stream_index;
 
 	/* Determine if the Unicode character is valid
 	 */
-	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-	 || ( unicode_character > LIBUNA_UTF16_CHARACTER_MAX ) )
+	if( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 		 "%s: unsupported Unicode character.",
 		 function );
 
 		return( -1 );
 	}
+	if( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	 && ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	{
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			libcerror_error_set(
+			 error,
+			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+			 "%s: unsupported Unicode character.",
+			 function );
+
+			return( -1 );
+		}
+	}
 	if( unicode_character <= LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX )
 	{
 		if( ( utf16_stream_size < 2 )
 		 || ( safe_utf16_stream_index > ( utf16_stream_size - 2 ) ) )
 		{
 			libcerror_error_set(
 			 error,
@@ -4271,15 +5327,15 @@
 }
 
 /* Determines the size of an UTF-32 character from an Unicode character
  * Adds the size to the UTF-32 character size value
  * Returns 1 if successful or -1 on error
  */
 int libuna_unicode_character_size_to_utf32(
-     libuna_unicode_character_t unicode_character LIBUNA_ATTRIBUTE_UNUSED,
+     libuna_unicode_character_t unicode_character,
      size_t *utf32_character_size,
      libcerror_error_t **error )
 {
 	static char *function = "libuna_unicode_character_size_to_utf32";
 
 	LIBUNA_UNREFERENCED_PARAMETER( unicode_character )
 
@@ -4290,14 +5346,27 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid UTF-32 character size.",
 		 function );
 
 		return( -1 );
 	}
+	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
+	{
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
+	}
 	*utf32_character_size += 1;
 
 	return( 1 );
 }
 
 /* Copies an Unicode character from an UTF-32 string
  * Returns 1 if successful or -1 on error
@@ -4366,24 +5435,30 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_VALUE_TOO_SMALL,
 		 "%s: UTF-32 string too small.",
 		 function );
 
 		return( -1 );
 	}
+	safe_unicode_character = utf32_string[ safe_utf32_string_index ];
+
 	/* Determine if the Unicode character is valid
 	 */
-	if( ( utf32_string[ safe_utf32_string_index ] >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
-	 && ( utf32_string[ safe_utf32_string_index ] <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	if( ( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
-	}
-	else
-	{
-		safe_unicode_character = utf32_string[ safe_utf32_string_index ];
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character  = safe_unicode_character;
 	*utf32_string_index = safe_utf32_string_index + 1;
 
 	return( 1 );
 }
 
@@ -4445,23 +5520,28 @@
 		 function );
 
 		return( -1 );
 	}
 	/* Determine if the Unicode character is valid
 	 */
 	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	  && ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-	 || ( unicode_character > LIBUNA_UTF32_CHARACTER_MAX ) )
-	{
-		utf32_string[ safe_utf32_string_index ] = (libuna_utf32_character_t) LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
-	}
-	else
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		utf32_string[ safe_utf32_string_index ] = (libuna_utf32_character_t) unicode_character;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
+	utf32_string[ safe_utf32_string_index ] = (libuna_utf32_character_t) unicode_character;
+
 	*utf32_string_index = safe_utf32_string_index + 1;
 
 	return( 1 );
 }
 
 /* Copies an Unicode character from an UTF-32 stream
  * Returns 1 if successful or -1 on error
@@ -4566,18 +5646,26 @@
 		safe_unicode_character <<= 8;
 		safe_unicode_character  += utf32_stream[ safe_utf32_stream_index + 1 ];
 		safe_unicode_character <<= 8;
 		safe_unicode_character  += utf32_stream[ safe_utf32_stream_index ];
 	}
 	/* Determine if the Unicode character is valid
 	 */
-	if( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START )
-	 && ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	if( ( ( safe_unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
+	  &&  ( safe_unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( safe_unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		safe_unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	*unicode_character  = safe_unicode_character;
 	*utf32_stream_index = safe_utf32_stream_index + 4;
 
 	return( 1 );
 }
 
@@ -4653,18 +5741,25 @@
 		 function );
 
 		return( -1 );
 	}
 	/* Determine if the Unicode character is valid
 	 */
 	if( ( ( unicode_character >= LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START )
-	  && ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
-	 || ( unicode_character > LIBUNA_UTF32_CHARACTER_MAX ) )
+	  &&  ( unicode_character <= LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END ) )
+	 || ( unicode_character > LIBUNA_UNICODE_CHARACTER_MAX ) )
 	{
-		unicode_character = LIBUNA_UNICODE_REPLACEMENT_CHARACTER;
+		libcerror_error_set(
+		 error,
+		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
+		 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
+		 "%s: unsupported Unicode character.",
+		 function );
+
+		return( -1 );
 	}
 	if( byte_order == LIBUNA_ENDIAN_BIG )
 	{
 		utf32_stream[ safe_utf32_stream_index + 3 ] = (uint8_t) ( unicode_character & 0xff );
 		unicode_character                         >>= 8;
 		utf32_stream[ safe_utf32_stream_index + 2 ] = (uint8_t) ( unicode_character & 0xff );
 		unicode_character                         >>= 8;
```

### Comparing `liblnk-20230205/libuna/libuna_utf8_string.c` & `liblnk-20230716/libuna/libuna_utf8_string.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1781,17 +1781,18 @@
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf8_string_size_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf16_stream == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1856,26 +1857,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -1891,18 +1880,29 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Determine how many UTF-8 character bytes are required
 		 */
-		if( libuna_unicode_character_size_to_utf8(
-		     unicode_character,
-		     utf8_string_size,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_size_to_utf8(
+			          unicode_character,
+			          utf8_string_size,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_size_to_utf8_rfc2279(
+			          unicode_character,
+			          utf8_string_size,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_INPUT_FAILED,
 			 "%s: unable to unable to determine size of Unicode character in UTF-8.",
 			 function );
@@ -1967,17 +1967,18 @@
      size_t *utf8_string_index,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf8_string_with_index_copy_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2059,26 +2060,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -2094,20 +2083,33 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Convert the Unicode character into UTF-8 character bytes
 		 */
-		if( libuna_unicode_character_copy_to_utf8(
-		     unicode_character,
-		     utf8_string,
-		     utf8_string_size,
-		     utf8_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_to_utf8(
+			          unicode_character,
+			          utf8_string,
+			          utf8_string_size,
+			          utf8_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_to_utf8_rfc2279(
+			          unicode_character,
+			          utf8_string,
+			          utf8_string_size,
+			          utf8_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character to UTF-8.",
 			 function );
@@ -2149,19 +2151,20 @@
      size_t utf8_string_size,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                                     = "libuna_utf8_string_compare_with_utf16_stream";
+	libuna_unicode_character_t utf16_stream_unicode_character = 0;
+	libuna_unicode_character_t utf8_unicode_character         = 0;
 	size_t utf16_stream_index                                 = 0;
 	size_t utf8_string_index                                  = 0;
-	libuna_unicode_character_t utf8_unicode_character         = 0;
-	libuna_unicode_character_t utf16_stream_unicode_character = 0;
 	int read_byte_order                                       = 0;
+	int result                                                = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2232,26 +2235,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf8_string_size >= 1 )
 	 && ( utf8_string[ utf8_string_size - 1 ] == 0 ) )
 	{
 		utf8_string_size -= 1;
 	}
 	/* Check if the UTF-16 stream is terminated with zero bytes
 	 */
@@ -2262,20 +2253,33 @@
 		utf16_stream_size -= 2;
 	}
 	while( ( utf8_string_index < utf8_string_size )
 	    && ( utf16_stream_index < utf16_stream_size ) )
 	{
 		/* Convert the UTF-8 character bytes into an Unicode character
 		 */
-		if( libuna_unicode_character_copy_from_utf8(
-		     &utf8_unicode_character,
-		     utf8_string,
-		     utf8_string_size,
-		     &utf8_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_from_utf8(
+			          &utf8_unicode_character,
+			          utf8_string,
+			          utf8_string_size,
+			          &utf8_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_from_utf8_rfc2279(
+			          &utf8_unicode_character,
+			          utf8_string,
+			          utf8_string_size,
+			          &utf8_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character from UTF-8.",
 			 function );
@@ -2832,26 +2836,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 3 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -3039,26 +3031,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 3 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -3216,26 +3196,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf8_string_size >= 1 )
 	 && ( utf8_string[ utf8_string_size - 1 ] == 0 ) )
 	{
 		utf8_string_size -= 1;
 	}
 	/* Check if the UTF-32 stream is terminated with zero bytes
 	 */
```

### Comparing `liblnk-20230205/libuna/libuna_base32_stream.c` & `liblnk-20230716/libuna/libuna_base32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_950.h` & `liblnk-20230716/libuna/libuna_codepage_windows_950.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_error.h` & `liblnk-20230716/libuna/libuna_error.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_932.h` & `liblnk-20230716/libuna/libuna_codepage_windows_932.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_turkish.h` & `liblnk-20230716/libuna/libuna_codepage_mac_turkish.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf8_stream.c` & `liblnk-20230716/libuna/libuna_utf8_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_ukrainian.c` & `liblnk-20230716/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_koi8_r.h` & `liblnk-20230716/libuna/libuna_codepage_koi8_r.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_base16_stream.c` & `liblnk-20230716/libuna/libuna_base16_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1250.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1250.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_16.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_16.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_croatian.h` & `liblnk-20230716/libuna/libuna_codepage_mac_croatian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_gaelic.c` & `liblnk-20230716/libuna/libuna_codepage_mac_gaelic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf16_stream.h` & `liblnk-20230716/libuna/libuna_utf16_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_10.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_7.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-10 codepage (Nordic) functions
+ * ISO 8859-7 codepage (Greek) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,34 +15,34 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_10_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_10_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_7_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_7_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_10_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_7_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_10_unicode_to_byte_stream_base_0x00c0[ 144 ];
+const uint8_t libuna_codepage_iso_8859_7_unicode_to_byte_stream_base_0x00a0[ 24 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_10_unicode_to_byte_stream_base_0x0160[ 16 ];
+const uint8_t libuna_codepage_iso_8859_7_unicode_to_byte_stream_base_0x0380[ 80 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_10_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_7_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_centraleurroman.c` & `liblnk-20230716/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_932.c` & `liblnk-20230716/libuna/libuna_codepage_windows_932.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf8_stream.h` & `liblnk-20230716/libuna/libuna_utf8_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_url_stream.h` & `liblnk-20230716/libuna/libuna_url_stream.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_farsi.c` & `liblnk-20230716/libuna/libuna_codepage_mac_farsi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_949.h` & `liblnk-20230716/libuna/libuna_codepage_windows_949.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_romanian.h` & `liblnk-20230716/libuna/libuna_codepage_mac_roman.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRomanian codepage functions
+ * MacRoman codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_romanian_copy_from_byte_stream(
+int libuna_codepage_mac_roman_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_romanian_copy_to_byte_stream(
+int libuna_codepage_mac_roman_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_gaelic.h` & `liblnk-20230716/libuna/libuna_codepage_mac_gaelic.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_8.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_8.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_types.h` & `liblnk-20230716/libuna/libuna_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_arabic.c` & `liblnk-20230716/libuna/libuna_codepage_mac_arabic.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1252.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1258.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1252 codepage (Western European/Latin 1) functions
+ * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1252_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1252_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1258_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1252_copy_from_byte_stream(
+int libuna_codepage_windows_1258_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1252_copy_to_byte_stream(
+int libuna_codepage_windows_1258_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1252_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1250.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1250.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_russian.c` & `liblnk-20230716/libuna/libuna_codepage_mac_russian.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf16_string.c` & `liblnk-20230716/libuna/libuna_utf16_string.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1639,17 +1639,18 @@
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_string_size_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf16_stream == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1714,26 +1715,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -1749,18 +1738,29 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Determine how many UTF-16 character bytes are required
 		 */
-		if( libuna_unicode_character_size_to_utf16(
-		     unicode_character,
-		     utf16_string_size,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_size_to_utf16(
+			          unicode_character,
+			          utf16_string_size,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_size_to_ucs2(
+			          unicode_character,
+			          utf16_string_size,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_INPUT_FAILED,
 			 "%s: unable to unable to determine size of Unicode character in UTF-16.",
 			 function );
@@ -1825,17 +1825,18 @@
      size_t *utf16_string_index,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_string_with_index_copy_from_utf16_stream";
-	size_t utf16_stream_index                    = 0;
 	libuna_unicode_character_t unicode_character = 0;
+	size_t utf16_stream_index                    = 0;
 	int read_byte_order                          = 0;
+	int result                                   = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -1917,26 +1918,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf16_stream_index + 1 ) < utf16_stream_size )
 	{
 		/* Convert the UTF-16 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16_stream(
 		     &unicode_character,
 		     utf16_stream,
@@ -1952,20 +1941,33 @@
 			 "%s: unable to copy Unicode character from UTF-16 stream.",
 			 function );
 
 			return( -1 );
 		}
 		/* Convert the Unicode character into UTF-16 character bytes
 		 */
-		if( libuna_unicode_character_copy_to_utf16(
-		     unicode_character,
-		     utf16_string,
-		     utf16_string_size,
-		     utf16_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_to_utf16(
+			          unicode_character,
+			          utf16_string,
+			          utf16_string_size,
+			          utf16_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_to_ucs2(
+			          unicode_character,
+			          utf16_string,
+			          utf16_string_size,
+			          utf16_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character to UTF-16.",
 			 function );
@@ -2007,19 +2009,20 @@
      size_t utf16_string_size,
      const uint8_t *utf16_stream,
      size_t utf16_stream_size,
      int byte_order,
      libcerror_error_t **error )
 {
 	static char *function                                     = "libuna_utf16_string_compare_with_utf16_stream";
+	libuna_unicode_character_t utf16_stream_unicode_character = 0;
+	libuna_unicode_character_t utf16_unicode_character        = 0;
 	size_t utf16_stream_index                                 = 0;
 	size_t utf16_string_index                                 = 0;
-	libuna_unicode_character_t utf16_unicode_character        = 0;
-	libuna_unicode_character_t utf16_stream_unicode_character = 0;
 	int read_byte_order                                       = 0;
+	int result                                                = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -2090,26 +2093,14 @@
 			utf16_stream_index = 2;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf16_string_size >= 1 )
 	 && ( utf16_string[ utf16_string_size - 1 ] == 0 ) )
 	{
 		utf16_string_size -= 1;
 	}
 	/* Check if the UTF-16 stream is terminated with zero bytes
 	 */
@@ -2120,20 +2111,33 @@
 		utf16_stream_size -= 2;
 	}
 	while( ( utf16_string_index < utf16_string_size )
 	    && ( utf16_stream_index < utf16_stream_size ) )
 	{
 		/* Convert the UTF-16 character bytes into an Unicode character
 		 */
-		if( libuna_unicode_character_copy_from_utf16(
-		     &utf16_unicode_character,
-		     utf16_string,
-		     utf16_string_size,
-		     &utf16_string_index,
-		     error ) != 1 )
+		if( ( byte_order & LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE ) == 0 )
+		{
+			result = libuna_unicode_character_copy_from_utf16(
+			          &utf16_unicode_character,
+			          utf16_string,
+			          utf16_string_size,
+			          &utf16_string_index,
+			          error );
+		}
+		else
+		{
+			result = libuna_unicode_character_copy_from_ucs2(
+			          &utf16_unicode_character,
+			          utf16_string,
+			          utf16_string_size,
+			          &utf16_string_index,
+			          error );
+		}
+		if( result != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to copy Unicode character from UTF-16.",
 			 function );
@@ -2690,26 +2694,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 3 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -2897,26 +2889,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	while( ( utf32_stream_index + 3 ) < utf32_stream_size )
 	{
 		/* Convert the UTF-32 stream bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32_stream(
 		     &unicode_character,
 		     utf32_stream,
@@ -3074,26 +3054,14 @@
 			utf32_stream_index = 4;
 		}
 		if( byte_order == 0 )
 		{
 			byte_order = read_byte_order;
 		}
 	}
-	if( ( byte_order != LIBUNA_ENDIAN_BIG )
-	 && ( byte_order != LIBUNA_ENDIAN_LITTLE ) )
-	{
-		libcerror_error_set(
-		 error,
-		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
-		 LIBCERROR_ARGUMENT_ERROR_UNSUPPORTED_VALUE,
-		 "%s: unsupported byte order.",
-		 function );
-
-		return( -1 );
-	}
 	if( ( utf16_string_size >= 1 )
 	 && ( utf16_string[ utf16_string_size - 1 ] == 0 ) )
 	{
 		utf16_string_size -= 1;
 	}
 	/* Check if the UTF-32 stream is terminated with zero bytes
 	 */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_5.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_9.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-5 codepage (Cyrillic) functions
+ * ISO 8859-9 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_5_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_9_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
+const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_extern.h` & `liblnk-20230716/libuna/libuna_extern.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_4.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_4.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_byte_stream.h` & `liblnk-20230716/libuna/libuna_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_roman.h` & `liblnk-20230716/libuna/libuna_codepage_mac_romanian.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRoman codepage functions
+ * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_roman_copy_from_byte_stream(
+int libuna_codepage_mac_romanian_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_roman_copy_to_byte_stream(
+int libuna_codepage_mac_romanian_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_utf16_string.h` & `liblnk-20230716/libuna/libuna_utf16_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_4.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_4.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_10.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_10.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_icelandic.h` & `liblnk-20230716/libuna/libuna_codepage_mac_icelandic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/Makefile.in` & `liblnk-20230716/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libuna/libuna_utf7_stream.h` & `liblnk-20230716/libuna/libuna_utf7_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_symbol.c` & `liblnk-20230716/libuna/libuna_codepage_mac_symbol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_base32_stream.h` & `liblnk-20230716/libuna/libuna_base32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_turkish.c` & `liblnk-20230716/libuna/libuna_codepage_mac_turkish.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_inuit.c` & `liblnk-20230716/libuna/libuna_codepage_mac_inuit.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacInuit codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf16_stream.c` & `liblnk-20230716/libuna/libuna_utf16_stream.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -118,14 +118,15 @@
      const libuna_utf8_character_t *utf8_string,
      size_t utf8_string_size,
      size_t *utf16_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_stream_size_from_utf8";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf16_stream_size                = 0;
 	size_t utf8_string_index                     = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -155,15 +156,15 @@
 		 "%s: invalid UTF-16 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf16_stream_size = 1;
+	safe_utf16_stream_size = 1;
 
 	while( utf8_string_index < utf8_string_size )
 	{
 		/* Convert the UTF-8 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf8(
 		     &unicode_character,
@@ -181,15 +182,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-16 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf16(
 		     unicode_character,
-		     utf16_stream_size,
+		     &safe_utf16_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-16.",
@@ -200,15 +201,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf16_stream_size *= 2;
+	*utf16_stream_size = safe_utf16_stream_size * 2;
 
 	return( 1 );
 }
 
 /* Copies an UTF-16 stream from an UTF-8 string
  * Returns 1 if successful or -1 on error
  */
@@ -351,14 +352,15 @@
      const libuna_utf16_character_t *utf16_string,
      size_t utf16_string_size,
      size_t *utf16_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_stream_size_from_utf16";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf16_stream_size                = 0;
 	size_t utf16_string_index                    = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -388,15 +390,15 @@
 		 "%s: invalid UTF-16 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf16_stream_size = 1;
+	safe_utf16_stream_size = 1;
 
 	while( utf16_string_index < utf16_string_size )
 	{
 		/* Convert the UTF-16 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf16(
 		     &unicode_character,
@@ -414,15 +416,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-16 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf16(
 		     unicode_character,
-		     utf16_stream_size,
+		     &safe_utf16_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-16.",
@@ -433,15 +435,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf16_stream_size *= 2;
+	*utf16_stream_size = safe_utf16_stream_size * 2;
 
 	return( 1 );
 }
 
 /* Copies an UTF-16 stream from an UTF-16 string
  * Returns 1 if successful or -1 on error
  */
@@ -584,14 +586,15 @@
      const libuna_utf32_character_t *utf32_string,
      size_t utf32_string_size,
      size_t *utf16_stream_size,
      libcerror_error_t **error )
 {
 	static char *function                        = "libuna_utf16_stream_size_from_utf32";
 	libuna_unicode_character_t unicode_character = 0;
+	size_t safe_utf16_stream_size                = 0;
 	size_t utf32_string_index                    = 0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
@@ -621,15 +624,15 @@
 		 "%s: invalid UTF-16 stream size.",
 		 function );
 
 		return( -1 );
 	}
 	/* Add the byte order mark
 	 */
-	*utf16_stream_size += 1;
+	safe_utf16_stream_size += 1;
 
 	while( utf32_string_index < utf32_string_size )
 	{
 		/* Convert the UTF-32 character bytes into an Unicode character
 		 */
 		if( libuna_unicode_character_copy_from_utf32(
 		     &unicode_character,
@@ -647,15 +650,15 @@
 
 			return( -1 );
 		}
 		/* Determine how many UTF-16 character bytes are required
 		 */
 		if( libuna_unicode_character_size_to_utf16(
 		     unicode_character,
-		     utf16_stream_size,
+		     &safe_utf16_stream_size,
 		     error ) != 1 )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_CONVERSION,
 			 LIBCERROR_CONVERSION_ERROR_OUTPUT_FAILED,
 			 "%s: unable to determine size of Unicode character in UTF-16.",
@@ -666,15 +669,15 @@
 		if( unicode_character == 0 )
 		{
 			break;
 		}
 	}
 	/* Convert the number of characters into bytes
 	 */
-	*utf16_stream_size *= 2;
+	*utf16_stream_size = safe_utf16_stream_size * 2;
 
 	return( 1 );
 }
 
 /* Copies an UTF-16 stream from an UTF-32 string
  * Returns 1 if successful or -1 on error
  */
```

### Comparing `liblnk-20230205/libuna/libuna_utf7_stream.c` & `liblnk-20230716/libuna/libuna_utf7_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_support.h` & `liblnk-20230716/libuna/libuna_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_utf32_stream.h` & `liblnk-20230716/libuna/libuna_utf32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_3.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_greek.c` & `liblnk-20230716/libuna/libuna_codepage_mac_greek.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_definitions.h` & `liblnk-20230716/libuna/libuna_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20220611
+#define LIBUNA_VERSION						20230710
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20220611"
+#define LIBUNA_VERSION_STRING					"20230710"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
@@ -384,14 +384,16 @@
 /* Base64 processing flags
  */
 enum LIBUNA_BASE64_FLAGS
 {
 	LIBUNA_BASE64_FLAG_STRIP_WHITESPACE			= 0x01
 };
 
+#define LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE		0x8000
+
 #endif /* !defined( HAVE_LOCAL_LIBUNA ) */
 
 #define LIBUNA_BASE32_VARIANT_ENCODING_BYTE_STREAM		0
 #define LIBUNA_BASE64_VARIANT_ENCODING_BYTE_STREAM		0
 
 /* Character case definitions
  */
@@ -418,16 +420,15 @@
 #define LIBUNA_UNICODE_BASIC_MULTILINGUAL_PLANE_MAX		0x0000ffffUL
 #define LIBUNA_UNICODE_SURROGATE_LOW_RANGE_START		0x0000dc00UL
 #define LIBUNA_UNICODE_SURROGATE_LOW_RANGE_END			0x0000dfffUL
 #define LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_START		0x0000d800UL
 #define LIBUNA_UNICODE_SURROGATE_HIGH_RANGE_END			0x0000dbffUL
 #define LIBUNA_UNICODE_CHARACTER_MAX				0x0010ffffUL
 
-#define LIBUNA_UTF16_CHARACTER_MAX				0x0010ffffUL
-#define LIBUNA_UTF32_CHARACTER_MAX				0x7fffffffUL
+#define LIBUNA_UCS_CHARACTER_MAX				0x7fffffffUL
 
 #define LIBUNA_ASCII_REPLACEMENT_CHARACTER			0x1a
 
 /* UTF-7 definitions
  */
 #define	LIBUNA_UTF7_IS_BASE64_ENCODED				0x80000000UL
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1255.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1255.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_14.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_14.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_13.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_13.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_centraleurroman.h` & `liblnk-20230716/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_8.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_8.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_9.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_9.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-9 codepage (Turkish) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1254.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1254.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_cyrillic.h` & `liblnk-20230716/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_arabic.h` & `liblnk-20230716/libuna/libuna_codepage_mac_arabic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1258.c` & `liblnk-20230716/libuna/libuna_codepage_windows_1258.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_farsi.h` & `liblnk-20230716/libuna/libuna_codepage_mac_farsi.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_15.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_15.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_7.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_7.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_dingbats.c` & `liblnk-20230716/libuna/libuna_codepage_mac_dingbats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_9.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_6.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-9 codepage (Turkish) functions
+ * ISO 8859-6 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_9_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_6_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_6_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
+const uint16_t libuna_codepage_iso_8859_6_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
+const uint8_t libuna_codepage_iso_8859_6_unicode_to_byte_stream_base_0x0618[ 64 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_6_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_windows_1258.h` & `liblnk-20230716/libuna/libuna_codepage_windows_1254.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1258 codepage (Vietnamese) functions
+ * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1258_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1254_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1258_copy_from_byte_stream(
+int libuna_codepage_windows_1254_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1258_copy_to_byte_stream(
+int libuna_codepage_windows_1254_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1258_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1254_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_base64_stream.c` & `liblnk-20230716/libuna/libuna_base64_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_romanian.c` & `liblnk-20230716/libuna/libuna_codepage_mac_romanian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_error.c` & `liblnk-20230716/libuna/libuna_error.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_koi8_u.c` & `liblnk-20230716/libuna/libuna_codepage_koi8_u.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_13.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_10.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-13 codepage (Baltic) functions
+ * ISO 8859-10 codepage (Nordic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,34 +15,34 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_13_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_13_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_10_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_10_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_13_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_10_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_13_unicode_to_byte_stream_base_0x00a0[ 224 ];
+const uint8_t libuna_codepage_iso_8859_10_unicode_to_byte_stream_base_0x00c0[ 144 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_13_unicode_to_byte_stream_base_0x2018[ 8 ];
+const uint8_t libuna_codepage_iso_8859_10_unicode_to_byte_stream_base_0x0160[ 16 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_13_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_10_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_7.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_14.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-7 codepage (Greek) functions
+ * ISO 8859-14 codepage (Celtic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,34 +15,37 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_7_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_7_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_14_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_14_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_7_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_14_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_7_unicode_to_byte_stream_base_0x00a0[ 24 ];
+const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x00c0[ 64 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_7_unicode_to_byte_stream_base_0x0380[ 80 ];
+const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x0170[ 8 ];
+
+LIBUNA_EXTERN_VARIABLE \
+const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x1e80[ 8 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_7_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_14_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_14.h` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_13.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-14 codepage (Celtic) functions
+ * ISO 8859-13 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,37 +15,34 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_14_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_14_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_13_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_13_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_14_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_13_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x00c0[ 64 ];
+const uint8_t libuna_codepage_iso_8859_13_unicode_to_byte_stream_base_0x00a0[ 224 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x0170[ 8 ];
-
-LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_14_unicode_to_byte_stream_base_0x1e80[ 8 ];
+const uint8_t libuna_codepage_iso_8859_13_unicode_to_byte_stream_base_0x2018[ 8 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_14_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_13_H ) */
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_mac_inuit.h` & `liblnk-20230716/libuna/libuna_codepage_mac_inuit.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacInuit codepage functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libuna/libuna_codepage_iso_8859_16.c` & `liblnk-20230716/libuna/libuna_codepage_iso_8859_16.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) function
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `liblnk-20230205/libfwsi/libfwsi_libfwps.h` & `liblnk-20230716/libfwsi/libfwsi_libfwps.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_entry_extension_values.c` & `liblnk-20230716/libfwsi/libfwsi_file_entry_extension_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0014_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0014_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_entry_extension_values.h` & `liblnk-20230716/libfwsi/libfwsi_file_entry_extension_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_support.c` & `liblnk-20230716/libfwsi/libfwsi_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0013_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0013_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_libcdata.h` & `liblnk-20230716/libfwsi/libfwsi_libcdata.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_libcerror.h` & `liblnk-20230716/libfwsi/libfwsi_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_control_panel_values.h` & `liblnk-20230716/libfwsi/libfwsi_control_panel_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0025_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0025_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0001_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0001_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_root_folder.h` & `liblnk-20230716/libfwsi/libfwsi_root_folder.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_delegate_values.h` & `liblnk-20230716/libfwsi/libfwsi_delegate_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_libfole.h` & `liblnk-20230716/libfwsi/libfwsi_libfole.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_root_folder_values.h` & `liblnk-20230716/libfwsi/libfwsi_root_folder_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_mtp_volume_values.h` & `liblnk-20230716/libfwsi/libfwsi_mtp_volume_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0006_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0006_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_libfdatetime.h` & `liblnk-20230716/libfwsi/libfwsi_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_users_property_view_values.h` & `liblnk-20230716/libfwsi/libfwsi_users_property_view_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/Makefile.am` & `liblnk-20230716/libfwsi/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_entry_values.c` & `liblnk-20230716/libfwsi/libfwsi_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_libuna.h` & `liblnk-20230716/libfwsi/libfwsi_libuna.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_volume_values.c` & `liblnk-20230716/libfwsi/libfwsi_volume_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_volume_values.h` & `liblnk-20230716/libfwsi/libfwsi_volume_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_attributes.c` & `liblnk-20230716/libfwsi/libfwsi_file_attributes.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_shell_folder_identifier.h` & `liblnk-20230716/libfwsi/libfwsi_shell_folder_identifier.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_types.h` & `liblnk-20230716/libfwsi/libfwsi_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_control_panel_identifier.c` & `liblnk-20230716/libfwsi/libfwsi_control_panel_identifier.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_codepage.h` & `liblnk-20230716/libfwsi/libfwsi_codepage.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef000a_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef000a_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0003_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0003_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_delegate_values.c` & `liblnk-20230716/libfwsi/libfwsi_delegate_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_entry_extension.h` & `liblnk-20230716/libfwsi/libfwsi_file_entry_extension.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_network_location_values.h` & `liblnk-20230716/libfwsi/libfwsi_network_location_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_item_list.h` & `liblnk-20230716/libfwsi/libfwsi_item_list.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_compressed_folder_values.c` & `liblnk-20230716/libfwsi/libfwsi_compressed_folder_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0000_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0000_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_notify.h` & `liblnk-20230716/libfwsi/libfwsi_notify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0014_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0014_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0013_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0013_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_game_folder_values.c` & `liblnk-20230716/libfwsi/libfwsi_game_folder_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0019_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0019_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_entry.c` & `liblnk-20230716/libfwsi/libfwsi_file_entry.c`

 * *Files 4% similar despite different names*

```diff
@@ -223,14 +223,16 @@
 	}
 	*file_attribute_flags = file_entry_values->file_attribute_flags;
 
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 formatted name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwsi_file_entry_get_utf8_name_size(
      libfwsi_item_t *file_entry,
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
@@ -277,15 +279,15 @@
 	file_entry_values = (libfwsi_file_entry_values_t *) internal_item->value;
 
 	if( file_entry_values->is_unicode != 0 )
 	{
 		result = libuna_utf8_string_size_from_utf16_stream(
 			  file_entry_values->name,
 			  file_entry_values->name_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  utf8_string_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_size_from_byte_stream(
 			  file_entry_values->name,
@@ -305,14 +307,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 formatted name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwsi_file_entry_get_utf8_name(
      libfwsi_item_t *file_entry,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libcerror_error_t **error )
@@ -362,15 +366,15 @@
 	if( file_entry_values->is_unicode != 0 )
 	{
 		result = libuna_utf8_string_copy_from_utf16_stream(
 		          utf8_string,
 		          utf8_string_size,
 			  file_entry_values->name,
 			  file_entry_values->name_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf8_string_copy_from_byte_stream(
 		          utf8_string,
 		          utf8_string_size,
@@ -390,14 +394,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 formatted name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwsi_file_entry_get_utf16_name_size(
      libfwsi_item_t *file_entry,
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
@@ -444,15 +450,15 @@
 	file_entry_values = (libfwsi_file_entry_values_t *) internal_item->value;
 
 	if( file_entry_values->is_unicode != 0 )
 	{
 		result = libuna_utf16_string_size_from_utf16_stream(
 			  file_entry_values->name,
 			  file_entry_values->name_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  utf16_string_size,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_size_from_byte_stream(
 			  file_entry_values->name,
@@ -472,14 +478,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 formatted name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful or -1 on error
  */
 int libfwsi_file_entry_get_utf16_name(
      libfwsi_item_t *file_entry,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error )
@@ -529,15 +537,15 @@
 	if( file_entry_values->is_unicode != 0 )
 	{
 		result = libuna_utf16_string_copy_from_utf16_stream(
 		          utf16_string,
 		          utf16_string_size,
 			  file_entry_values->name,
 			  file_entry_values->name_size,
-			  LIBUNA_ENDIAN_LITTLE,
+			  LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 			  error );
 	}
 	else
 	{
 		result = libuna_utf16_string_copy_from_byte_stream(
 		          utf16_string,
 		          utf16_string_size,
```

### Comparing `liblnk-20230205/libfwsi/libfwsi_cdburn_values.h` & `liblnk-20230716/libfwsi/libfwsi_cdburn_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_unknown_0x74_values.c` & `liblnk-20230716/libfwsi/libfwsi_unknown_0x74_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_uri_sub_values.h` & `liblnk-20230716/libfwsi/libfwsi_uri_sub_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_debug.c` & `liblnk-20230716/libfwsi/libfwsi_debug.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_shell_folder_identifier.c` & `liblnk-20230716/libfwsi/libfwsi_shell_folder_identifier.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_attributes.h` & `liblnk-20230716/libfwsi/libfwsi_file_attributes.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_volume.c` & `liblnk-20230716/libfwsi/libfwsi_volume.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_notify.c` & `liblnk-20230716/libfwsi/libfwsi_notify.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0025_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0025_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_uri_values.h` & `liblnk-20230716/libfwsi/libfwsi_uri_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_known_folder_identifier.c` & `liblnk-20230716/libfwsi/libfwsi_known_folder_identifier.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_unknown_0x74_values.h` & `liblnk-20230716/libfwsi/libfwsi_unknown_0x74_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0005_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0005_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_network_location.h` & `liblnk-20230716/libfwsi/libfwsi_network_location.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_mtp_volume_values.c` & `liblnk-20230716/libfwsi/libfwsi_mtp_volume_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_game_folder_values.h` & `liblnk-20230716/libfwsi/libfwsi_game_folder_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_support.h` & `liblnk-20230716/libfwsi/libfwsi_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_mtp_file_entry_values.c` & `liblnk-20230716/libfwsi/libfwsi_mtp_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_unused.h` & `liblnk-20230716/libfwsi/libfwsi_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_root_folder_values.c` & `liblnk-20230716/libfwsi/libfwsi_root_folder_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_uri_values.c` & `liblnk-20230716/libfwsi/libfwsi_uri_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_users_property_view_values.c` & `liblnk-20230716/libfwsi/libfwsi_users_property_view_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_item.h` & `liblnk-20230716/libfwsi/libfwsi_item.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_compressed_folder_values.h` & `liblnk-20230716/libfwsi/libfwsi_compressed_folder_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_libfguid.h` & `liblnk-20230716/libfwsi/libfwsi_libfguid.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_entry.h` & `liblnk-20230716/libfwsi/libfwsi_file_entry.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_volume.h` & `liblnk-20230716/lnktools/property_store.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Volume (shell item) functions
+ * Property store functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,67 +15,49 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWSI_VOLUME_H )
-#define _LIBFWSI_VOLUME_H
+#if !defined( _PROPERTY_STORE_H )
+#define _PROPERTY_STORE_H
 
 #include <common.h>
+#include <file_stream.h>
 #include <types.h>
 
-#include "libfwsi_extern.h"
-#include "libfwsi_libcerror.h"
-#include "libfwsi_types.h"
+#include "lnktools_libfwps.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-LIBFWSI_EXTERN \
-int libfwsi_volume_get_utf8_name_size(
-     libfwsi_item_t *volume,
-     size_t *utf8_string_size,
+int property_store_path_string_fprint(
+     const system_character_t *file_entry_path,
+     size_t file_entry_path_length,
+     FILE *notify_stream,
      libcerror_error_t **error );
 
-LIBFWSI_EXTERN \
-int libfwsi_volume_get_utf8_name(
-     libfwsi_item_t *volume,
-     uint8_t *utf8_string,
-     size_t utf8_string_size,
+int property_store_record_fprint(
+     const uint8_t *property_set_identifier,
+     const system_character_t *property_set_identifier_string,
+     libfwps_record_t *property_record,
+     FILE *notify_stream,
      libcerror_error_t **error );
 
-LIBFWSI_EXTERN \
-int libfwsi_volume_get_utf16_name_size(
-     libfwsi_item_t *volume,
-     size_t *utf16_string_size,
+int property_store_set_fprint(
+     libfwps_set_t *property_set,
+     FILE *notify_stream,
      libcerror_error_t **error );
 
-LIBFWSI_EXTERN \
-int libfwsi_volume_get_utf16_name(
-     libfwsi_item_t *volume,
-     uint16_t *utf16_string,
-     size_t utf16_string_size,
-     libcerror_error_t **error );
-
-LIBFWSI_EXTERN \
-int libfwsi_volume_get_identifier(
-     libfwsi_item_t *volume,
-     uint8_t *guid_data,
-     size_t guid_data_size,
-     libcerror_error_t **error );
-
-LIBFWSI_EXTERN \
-int libfwsi_volume_get_shell_folder_identifier(
-     libfwsi_item_t *volume,
-     uint8_t *guid_data,
-     size_t guid_data_size,
+int property_store_fprint(
+     libfwps_store_t *property_store,
+     FILE *notify_stream,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBFWSI_VOLUME_H ) */
+#endif /* !defined( _PROPERTY_STORE_H ) */
```

### Comparing `liblnk-20230205/libfwsi/libfwsi_control_panel_identifier.h` & `liblnk-20230716/libfwsi/libfwsi_control_panel_identifier.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef000a_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef000a_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_root_folder.c` & `liblnk-20230716/libfwsi/libfwsi_root_folder.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_control_panel_category_values.c` & `liblnk-20230716/libfwsi/libfwsi_control_panel_category_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_debug.h` & `liblnk-20230716/libfwsi/libfwsi_debug.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/Makefile.in` & `liblnk-20230716/libfwsi/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0000_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0000_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0001_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0001_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_control_panel_values.c` & `liblnk-20230716/libfwsi/libfwsi_control_panel_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_network_location_values.c` & `liblnk-20230716/libfwsi/libfwsi_network_location_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0003_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0003_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_cdburn_values.c` & `liblnk-20230716/libfwsi/libfwsi_cdburn_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_error.c` & `liblnk-20230716/libfwsi/libfwsi_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_error.h` & `liblnk-20230716/libfwsi/libfwsi_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0005_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0005_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_uri_sub_values.c` & `liblnk-20230716/libfwsi/libfwsi_uri_sub_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_control_panel_cpl_file_values.c` & `liblnk-20230716/libfwsi/libfwsi_control_panel_cpl_file_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extern.h` & `liblnk-20230716/libfwsi/libfwsi_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_known_folder_identifier.h` & `liblnk-20230716/libfwsi/libfwsi_known_folder_identifier.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_control_panel_category_values.h` & `liblnk-20230716/libfwsi/libfwsi_control_panel_category_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_control_panel_cpl_file_values.h` & `liblnk-20230716/libfwsi/libfwsi_control_panel_cpl_file_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_item_list.c` & `liblnk-20230716/libfwsi/libfwsi_item_list.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_definitions.h` & `liblnk-20230716/libfwsi/libfwsi_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwsi/definitions.h> are copied here
  * for local use of libfwsi
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWSI_VERSION					20230114
+#define LIBFWSI_VERSION					20230710
 
 /* The version string
  */
-#define LIBFWSI_VERSION_STRING				"20230114"
+#define LIBFWSI_VERSION_STRING				"20230710"
 
 /* The byte order definitions
  */
 #define LIBFWSI_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWSI_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The item type definitions
```

### Comparing `liblnk-20230205/libfwsi/libfwsi_libcnotify.h` & `liblnk-20230716/libfwsi/libfwsi_libcnotify.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_entry_extension.c` & `liblnk-20230716/libfwsi/libfwsi_file_entry_extension.c`

 * *Files 6% similar despite different names*

```diff
@@ -228,14 +228,16 @@
 	}
 	*file_reference = file_entry_extension_values->file_reference;
 
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-8 formatted long name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwsi_file_entry_extension_get_utf8_long_name_size(
      libfwsi_extension_block_t *file_entry_extension,
      size_t *utf8_string_size,
      libcerror_error_t **error )
 {
@@ -284,15 +286,15 @@
 	 || ( file_entry_extension_values->long_name_size == 0 ) )
 	{
 		return( 0 );
 	}
 	if( libuna_utf8_string_size_from_utf16_stream(
 	     file_entry_extension_values->long_name,
 	     file_entry_extension_values->long_name_size,
-	     LIBUNA_ENDIAN_LITTLE,
+	     LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 	     utf8_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
@@ -301,14 +303,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-8 formatted long name
+ * This function uses UTF-8 RFC 2279 (or 6-byte UTF-8) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwsi_file_entry_extension_get_utf8_long_name(
      libfwsi_extension_block_t *file_entry_extension,
      uint8_t *utf8_string,
      size_t utf8_string_size,
      libcerror_error_t **error )
@@ -360,15 +364,15 @@
 		return( 0 );
 	}
 	if( libuna_utf8_string_copy_from_utf16_stream(
 	     utf8_string,
 	     utf8_string_size,
 	     file_entry_extension_values->long_name,
 	     file_entry_extension_values->long_name_size,
-	     LIBUNA_ENDIAN_LITTLE,
+	     LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set UTF-8 string.",
@@ -376,14 +380,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the size of the UTF-16 formatted long name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size includes the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwsi_file_entry_extension_get_utf16_long_name_size(
      libfwsi_extension_block_t *file_entry_extension,
      size_t *utf16_string_size,
      libcerror_error_t **error )
 {
@@ -432,15 +438,15 @@
 	 || ( file_entry_extension_values->long_name_size == 0 ) )
 	{
 		return( 0 );
 	}
 	if( libuna_utf16_string_size_from_utf16_stream(
 	     file_entry_extension_values->long_name,
 	     file_entry_extension_values->long_name_size,
-	     LIBUNA_ENDIAN_LITTLE,
+	     LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 	     utf16_string_size,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_GET_FAILED,
@@ -449,14 +455,16 @@
 
 		return( -1 );
 	}
 	return( 1 );
 }
 
 /* Retrieves the UTF-16 formatted long name
+ * This function uses UCS-2 (with surrogates) to support characters outside Unicode
+ * The size should include the end of string character
  * Returns 1 if successful, 0 if not available or -1 on error
  */
 int libfwsi_file_entry_extension_get_utf16_long_name(
      libfwsi_extension_block_t *file_entry_extension,
      uint16_t *utf16_string,
      size_t utf16_string_size,
      libcerror_error_t **error )
@@ -508,15 +516,15 @@
 		return( 0 );
 	}
 	if( libuna_utf16_string_copy_from_utf16_stream(
 	     utf16_string,
 	     utf16_string_size,
 	     file_entry_extension_values->long_name,
 	     file_entry_extension_values->long_name_size,
-	     LIBUNA_ENDIAN_LITTLE,
+	     LIBUNA_ENDIAN_LITTLE | LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set UTF-16 string.",
```

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0019_values.c` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0019_values.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_extension_block_0xbeef0006_values.h` & `liblnk-20230716/libfwsi/libfwsi_extension_block_0xbeef0006_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_network_location.c` & `liblnk-20230716/libfwsi/libfwsi_network_location.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_file_entry_values.h` & `liblnk-20230716/libfwsi/libfwsi_file_entry_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_mtp_file_entry_values.h` & `liblnk-20230716/libfwsi/libfwsi_mtp_file_entry_values.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libfwsi/libfwsi_item.c` & `liblnk-20230716/libfwsi/libfwsi_item.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/Makefile.in` & `liblnk-20230716/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/ChangeLog` & `liblnk-20230716/ChangeLog`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libuna.m4` & `liblnk-20230716/m4/libuna.m4`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20210801
+dnl Version: 20230702
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -39,15 +39,15 @@
         ])
       ],
       [dnl Check for a pkg-config file
       AS_IF(
         [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
         [PKG_CHECK_MODULES(
           [libuna],
-          [libuna >= 20210801],
+          [libuna >= 20230702],
           [ac_cv_libuna=yes],
           [ac_cv_libuna=check])
         ])
       AS_IF(
         [test "x$ac_cv_libuna" = xyes],
         [ac_cv_libuna_CPPFLAGS="$pkg_cv_libuna_CFLAGS"
         ac_cv_libuna_LIBADD="$pkg_cv_libuna_LIBS"])
@@ -221,14 +221,146 @@
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_byte_stream_copy_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
 
+        dnl Unicode character functions
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_ucs2,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_ucs4,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_utf8_rfc2279,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf8_rfc2279,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf8_rfc2279,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_size_to_utf16,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf16,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf16,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf16_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf16_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf32,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf32,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_from_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_unicode_character_copy_to_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+
         dnl UTF-8 stream functions
         AC_CHECK_LIB(
           una,
           libuna_utf8_stream_size_from_utf8,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
@@ -335,14 +467,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_with_index_copy_from_byte_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf8_string_compare_with_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf8_string_size_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
@@ -350,14 +487,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_with_index_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf8_string_compare_with_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf8_string_size_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
@@ -365,55 +507,55 @@
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_with_index_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_size_from_utf16_stream,
+          libuna_utf8_string_compare_with_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_copy_from_utf16_stream,
+          libuna_utf8_string_size_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_with_index_copy_from_utf16_stream,
+          libuna_utf8_string_copy_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_size_from_utf32_stream,
+          libuna_utf8_string_with_index_copy_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_copy_from_utf32_stream,
+          libuna_utf8_string_compare_with_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_with_index_copy_from_utf32_stream,
+          libuna_utf8_string_size_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_size_from_utf16,
+          libuna_utf8_string_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_copy_from_utf16,
+          libuna_utf8_string_with_index_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf8_string_with_index_copy_from_utf16,
+          libuna_utf8_string_compare_with_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_size_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
@@ -425,14 +567,39 @@
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_with_index_copy_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf8_string_compare_with_utf32,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf8_string_size_from_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf8_string_copy_from_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf8_string_with_index_copy_from_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf8_string_compare_with_utf32_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf8_string_size_from_scsu_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf8_string_copy_from_scsu_stream,
           [ac_cv_libuna_dummy=yes],
@@ -457,14 +624,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_with_index_copy_from_byte_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf16_string_compare_with_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf16_string_size_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
@@ -472,14 +644,35 @@
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_with_index_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf16_string_compare_with_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf16_string_size_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf16_string_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf16_string_with_index_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        dnl libuna_utf16_string_compare_with_utf8 is implemented by libuna_utf8_string_compare_with_utf16
+        AC_CHECK_LIB(
+          una,
           libuna_utf16_string_size_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
@@ -487,14 +680,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_with_index_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf16_string_compare_with_utf8_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf16_string_size_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
@@ -502,55 +700,55 @@
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_with_index_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_size_from_utf32_stream,
+          libuna_utf16_string_compare_with_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_copy_from_utf32_stream,
+          libuna_utf16_string_size_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_with_index_copy_from_utf32_stream,
+          libuna_utf16_string_copy_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_size_from_utf8,
+          libuna_utf16_string_with_index_copy_from_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_copy_from_utf8,
+          libuna_utf16_string_compare_with_utf32,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_with_index_copy_from_utf8,
+          libuna_utf16_string_size_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_size_from_utf32,
+          libuna_utf16_string_copy_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_copy_from_utf32,
+          libuna_utf16_string_with_index_copy_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf16_string_with_index_copy_from_utf32,
+          libuna_utf16_string_compare_with_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf16_string_size_from_scsu_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
@@ -579,14 +777,19 @@
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_with_index_copy_from_byte_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf32_string_compare_with_byte_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf32_string_size_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
@@ -594,84 +797,106 @@
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_with_index_copy_from_utf7_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf32_string_compare_with_utf7_stream,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
           libuna_utf32_string_size_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
+          libuna_utf32_string_size_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          una,
+          libuna_utf32_string_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        AC_CHECK_LIB(
+          libuna_utf32_string_with_index_copy_from_utf8,
+          [ac_cv_libuna_dummy=yes],
+          [ac_cv_libuna=no])
+        dnl libuna_utf32_string_compare_with_utf8 is implemented by libuna_utf8_string_compare_with_utf32
+        AC_CHECK_LIB(
+          una,
           libuna_utf32_string_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_with_index_copy_from_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_size_from_utf16_stream,
+          libuna_utf32_string_compare_with_utf8_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_copy_from_utf16_stream,
+          libuna_utf32_string_size_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_with_index_copy_from_utf16_stream,
+          libuna_utf32_string_copy_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_size_from_utf32_stream,
+          libuna_utf32_string_with_index_copy_from_utf16,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
+        dnl libuna_utf32_string_compare_with_utf16 is implemented by libuna_utf16_string_compare_with_utf32
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_copy_from_utf32_stream,
+          libuna_utf32_string_size_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_with_index_copy_from_utf32_stream,
+          libuna_utf32_string_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_size_from_utf8,
+          libuna_utf32_string_with_index_copy_from_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_copy_from_utf8,
+          libuna_utf32_string_compare_with_utf16_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
-          libuna_utf32_string_with_index_copy_from_utf8,
+          una,
+          libuna_utf32_string_size_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_size_from_utf16,
+          libuna_utf32_string_copy_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_copy_from_utf16,
+          libuna_utf32_string_with_index_copy_from_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
-          libuna_utf32_string_with_index_copy_from_utf16,
+          libuna_utf32_string_compare_with_utf32_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
         AC_CHECK_LIB(
           una,
           libuna_utf32_string_size_from_scsu_stream,
           [ac_cv_libuna_dummy=yes],
           [ac_cv_libuna=no])
@@ -704,14 +929,21 @@
         AX_LIBUNA_CHECK_DEFINITION(
           LIBUNA_COMPARE_GREATER,
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_compare_less" != xyes],
           [ac_cv_libuna=no])
 
+        AX_LIBUNA_CHECK_DEFINITION(
+          LIBUNA_UTF16_STREAM_ALLOW_UNPAIRED_SURROGATE,
+          [ac_cv_libuna_defines_compare_greater])
+        AS_IF(
+          [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
+          [ac_cv_libuna=no])
+
         ac_cv_libuna_LIBADD="-luna"])
       ])
     AS_IF(
       [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
```

### Comparing `liblnk-20230205/m4/libfwps.m4` & `liblnk-20230716/m4/libfwps.m4`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libfwps required headers and functions
 dnl
-dnl Version: 20230130
+dnl Version: 20230711
 
 dnl Function to detect if libfwps is available
 dnl ac_libfwps_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWPS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwps" = xno],
     [ac_cv_libfwps=no],
@@ -22,15 +22,15 @@
         ])
       ],
       [dnl Check for a pkg-config file
       AS_IF(
         [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
         [PKG_CHECK_MODULES(
           [libfwps],
-          [libfwps >= 20230130],
+          [libfwps >= 20230711],
           [ac_cv_libfwps=yes],
           [ac_cv_libfwps=check])
         ])
       AS_IF(
         [test "x$ac_cv_libfwps" = xyes],
         [ac_cv_libfwps_CPPFLAGS="$pkg_cv_libfwps_CFLAGS"
         ac_cv_libfwps_LIBADD="$pkg_cv_libfwps_LIBS"])
@@ -169,14 +169,34 @@
         AC_CHECK_LIB(
           fwps,
           libfwps_record_get_data_as_utf16_string,
           [ac_cv_libfwps_dummy=yes],
           [ac_cv_libfwps=no])
         AC_CHECK_LIB(
           fwps,
+          libfwps_record_get_data_as_utf8_path_string_size,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_data_as_utf8_path_string,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_data_as_utf16_path_string_size,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
+          libfwps_record_get_data_as_utf16_path_string,
+          [ac_cv_libfwps_dummy=yes],
+          [ac_cv_libfwps=no])
+        AC_CHECK_LIB(
+          fwps,
           libfwps_record_get_data_as_guid,
           [ac_cv_libfwps_dummy=yes],
           [ac_cv_libfwps=no])
 
         ac_cv_libfwps_LIBADD="-lfwps"])
       ])
     AS_IF(
```

### Comparing `liblnk-20230205/m4/gettext.m4` & `liblnk-20230716/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/tests.m4` & `liblnk-20230716/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/lib-prefix.m4` & `liblnk-20230716/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/ltoptions.m4` & `liblnk-20230716/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libcpath.m4` & `liblnk-20230716/m4/libcpath.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/lib-ld.m4` & `liblnk-20230716/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libcthreads.m4` & `liblnk-20230716/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/lib-link.m4` & `liblnk-20230716/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/python.m4` & `liblnk-20230716/m4/python.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libtool.m4` & `liblnk-20230716/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/nls.m4` & `liblnk-20230716/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libclocale.m4` & `liblnk-20230716/m4/libclocale.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libfdatetime.m4` & `liblnk-20230716/m4/libfdatetime.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/host-cpu-c-abi.m4` & `liblnk-20230716/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libcnotify.m4` & `liblnk-20230716/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/ltversion.m4` & `liblnk-20230716/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libcdata.m4` & `liblnk-20230716/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/progtest.m4` & `liblnk-20230716/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/lt~obsolete.m4` & `liblnk-20230716/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libcfile.m4` & `liblnk-20230716/m4/libcfile.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/po.m4` & `liblnk-20230716/m4/po.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/pthread.m4` & `liblnk-20230716/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/common.m4` & `liblnk-20230716/m4/common.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libcerror.m4` & `liblnk-20230716/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libfguid.m4` & `liblnk-20230716/m4/libfguid.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/iconv.m4` & `liblnk-20230716/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/ltsugar.m4` & `liblnk-20230716/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libcsplit.m4` & `liblnk-20230716/m4/libcsplit.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libfole.m4` & `liblnk-20230716/m4/libfole.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/intlmacosx.m4` & `liblnk-20230716/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/types.m4` & `liblnk-20230716/m4/types.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libfwsi.m4` & `liblnk-20230716/m4/libfwsi.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/m4/libbfio.m4` & `liblnk-20230716/m4/libbfio.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/COPYING.LESSER` & `liblnk-20230716/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_system.c` & `liblnk-20230716/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_error.c` & `liblnk-20230716/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_extern.h` & `liblnk-20230716/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/Makefile.am` & `liblnk-20230716/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_error.h` & `liblnk-20230716/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_support.h` & `liblnk-20230716/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_types.h` & `liblnk-20230716/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_definitions.h` & `liblnk-20230716/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_unused.h` & `liblnk-20230716/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/Makefile.in` & `liblnk-20230716/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_support.c` & `liblnk-20230716/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcerror/libcerror_system.h` & `liblnk-20230716/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_libcerror.h` & `liblnk-20230716/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_unused.h` & `liblnk-20230716/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_support.h` & `liblnk-20230716/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_support.c` & `liblnk-20230716/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/Makefile.am` & `liblnk-20230716/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_print.c` & `liblnk-20230716/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_verbose.c` & `liblnk-20230716/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_stream.h` & `liblnk-20230716/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_extern.h` & `liblnk-20230716/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_stream.c` & `liblnk-20230716/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/Makefile.in` & `liblnk-20230716/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_print.h` & `liblnk-20230716/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_verbose.h` & `liblnk-20230716/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcnotify/libcnotify_definitions.h` & `liblnk-20230716/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/ltmain.sh` & `liblnk-20230716/ltmain.sh`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/compile` & `liblnk-20230716/compile`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/config.rpath` & `liblnk-20230716/config.rpath`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/depcomp` & `liblnk-20230716/depcomp`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/po/en@quot.header` & `liblnk-20230716/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/po/Rules-quot` & `liblnk-20230716/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/po/remove-potcdate.sin` & `liblnk-20230716/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/po/Makevars.in` & `liblnk-20230716/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/po/en@boldquot.header` & `liblnk-20230716/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/po/Makevars` & `liblnk-20230716/po/Makevars`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/po/insert-header.sin` & `liblnk-20230716/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/po/Makefile.in.in` & `liblnk-20230716/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_array.c` & `liblnk-20230716/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_btree_node.c` & `liblnk-20230716/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_tree_node.c` & `liblnk-20230716/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_libcthreads.h` & `liblnk-20230716/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_range_list_value.h` & `liblnk-20230716/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_unused.h` & `liblnk-20230716/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_range_list.h` & `liblnk-20230716/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/Makefile.am` & `liblnk-20230716/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_range_list.c` & `liblnk-20230716/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_extern.h` & `liblnk-20230716/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_support.c` & `liblnk-20230716/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_list_element.h` & `liblnk-20230716/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_btree_values_list.c` & `liblnk-20230716/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_range_list_value.c` & `liblnk-20230716/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_libcerror.h` & `liblnk-20230716/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_error.c` & `liblnk-20230716/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_error.h` & `liblnk-20230716/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_support.h` & `liblnk-20230716/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_btree_node.h` & `liblnk-20230716/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_list.c` & `liblnk-20230716/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_tree_node.h` & `liblnk-20230716/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_list.h` & `liblnk-20230716/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_types.h` & `liblnk-20230716/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_list_element.c` & `liblnk-20230716/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/Makefile.in` & `liblnk-20230716/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_btree_values_list.h` & `liblnk-20230716/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_array.h` & `liblnk-20230716/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_btree.h` & `liblnk-20230716/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_definitions.h` & `liblnk-20230716/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcdata/libcdata_btree.c` & `liblnk-20230716/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/acinclude.m4` & `liblnk-20230716/acinclude.m4`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_types.h` & `liblnk-20230716/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_wide_string.h` & `liblnk-20230716/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_error.h` & `liblnk-20230716/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_support.h` & `liblnk-20230716/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_narrow_split_string.c` & `liblnk-20230716/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_narrow_split_string.h` & `liblnk-20230716/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/Makefile.am` & `liblnk-20230716/libcsplit/Makefile.am`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_wide_split_string.c` & `liblnk-20230716/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_narrow_string.h` & `liblnk-20230716/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_unused.h` & `liblnk-20230716/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_wide_string.c` & `liblnk-20230716/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_narrow_string.c` & `liblnk-20230716/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/Makefile.in` & `liblnk-20230716/libcsplit/Makefile.in`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_wide_split_string.h` & `liblnk-20230716/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_definitions.h` & `liblnk-20230716/libcsplit/libcsplit_definitions.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_error.c` & `liblnk-20230716/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_support.c` & `liblnk-20230716/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_libcerror.h` & `liblnk-20230716/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/libcsplit/libcsplit_extern.h` & `liblnk-20230716/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `liblnk-20230205/configure.ac` & `liblnk-20230716/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [liblnk],
- [20230205],
+ [20230716],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/liblnk.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
```

