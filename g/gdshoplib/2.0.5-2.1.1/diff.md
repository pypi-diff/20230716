# Comparing `tmp/gdshoplib-2.0.5.tar.gz` & `tmp/gdshoplib-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdshoplib-2.0.5.tar", max compression
+gzip compressed data, was "gdshoplib-2.1.1.tar", max compression
```

## Comparing `gdshoplib-2.0.5.tar` & `gdshoplib-2.1.1.tar`

### file list

```diff
@@ -1,89 +1,87 @@
--rw-r--r--   0        0        0     2004 2023-05-24 11:47:55.174891 gdshoplib-2.0.5/README.md
--rw-r--r--   0        0        0      210 2023-05-24 11:47:55.177560 gdshoplib-2.0.5/gdshoplib/__init__.py
--rw-r--r--   0        0        0       80 2023-01-03 20:04:30.238472 gdshoplib-2.0.5/gdshoplib/__main__.py
--rw-r--r--   0        0        0      117 2023-05-30 14:34:35.058893 gdshoplib-2.0.5/gdshoplib/activities/notion.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.507364 gdshoplib-2.0.5/gdshoplib/apps/__init__.py
--rw-r--r--   0        0        0      292 2023-05-24 11:47:55.179848 gdshoplib-2.0.5/gdshoplib/apps/crm/dialog.py
--rw-r--r--   0        0        0     3476 2023-05-24 11:47:55.182121 gdshoplib-2.0.5/gdshoplib/apps/crm/on_request.py
--rw-r--r--   0        0        0    10971 2023-07-13 21:17:32.023970 gdshoplib-2.0.5/gdshoplib/apps/crm/orders.py
--rw-r--r--   0        0        0      674 2023-05-24 11:47:55.186839 gdshoplib-2.0.5/gdshoplib/apps/crm/stats.py
--rw-r--r--   0        0        0      315 2023-05-24 11:47:55.189032 gdshoplib-2.0.5/gdshoplib/apps/delivery/delivery.py
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003805 gdshoplib-2.0.5/gdshoplib/apps/finance/__init__.py
--rw-r--r--   0        0        0      206 2023-05-24 11:47:55.191346 gdshoplib-2.0.5/gdshoplib/apps/finance/storage.py
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003925 gdshoplib-2.0.5/gdshoplib/apps/marketing/__init__.py
--rw-r--r--   0        0        0      163 2023-05-24 11:47:55.193504 gdshoplib-2.0.5/gdshoplib/apps/payments/payments.py
--rw-r--r--   0        0        0      378 2023-01-01 19:36:37.510481 gdshoplib-2.0.5/gdshoplib/apps/platforms/README.md
--rw-r--r--   0        0        0      665 2023-05-24 11:47:55.195540 gdshoplib-2.0.5/gdshoplib/apps/platforms/__init__.py
--rw-r--r--   0        0        0     1742 2023-05-24 11:47:55.197783 gdshoplib-2.0.5/gdshoplib/apps/platforms/avito.py
--rw-r--r--   0        0        0      113 2023-02-02 20:37:00.702563 gdshoplib-2.0.5/gdshoplib/apps/platforms/base.py
--rw-r--r--   0        0        0      152 2023-01-12 22:25:31.627980 gdshoplib-2.0.5/gdshoplib/apps/platforms/instagram.py
--rw-r--r--   0        0        0       95 2023-01-12 22:25:09.142423 gdshoplib-2.0.5/gdshoplib/apps/platforms/ok.py
--rw-r--r--   0        0        0      467 2023-05-24 11:47:55.199621 gdshoplib-2.0.5/gdshoplib/apps/platforms/sm.py
--rw-r--r--   0        0        0       95 2023-01-12 22:26:15.528644 gdshoplib-2.0.5/gdshoplib/apps/platforms/tg.py
--rw-r--r--   0        0        0      908 2023-05-24 11:47:55.201920 gdshoplib-2.0.5/gdshoplib/apps/platforms/ula.py
--rw-r--r--   0        0        0      512 2023-05-24 11:47:55.204568 gdshoplib-2.0.5/gdshoplib/apps/platforms/vk.py
--rw-r--r--   0        0        0     3373 2023-05-24 11:47:58.629272 gdshoplib-2.0.5/gdshoplib/apps/platforms/yam.py
--rw-r--r--   0        0        0      187 2023-01-01 19:36:37.519008 gdshoplib-2.0.5/gdshoplib/apps/products/README.md
--rw-r--r--   0        0        0        0 2022-11-29 21:45:29.004030 gdshoplib-2.0.5/gdshoplib/apps/products/__init__.py
--rw-r--r--   0        0        0     1931 2023-02-02 20:29:22.002155 gdshoplib-2.0.5/gdshoplib/apps/products/description.py
--rw-r--r--   0        0        0     5779 2023-07-12 22:35:57.507949 gdshoplib-2.0.5/gdshoplib/apps/products/media.py
--rw-r--r--   0        0        0     5173 2023-07-13 21:07:48.093813 gdshoplib-2.0.5/gdshoplib/apps/products/price.py
--rw-r--r--   0        0        0     5687 2023-05-30 20:06:07.280114 gdshoplib-2.0.5/gdshoplib/apps/products/product.py
--rw-r--r--   0        0        0     5947 2023-06-18 20:41:49.001382 gdshoplib-2.0.5/gdshoplib/apps/uploader/uploader.py
--rw-r--r--   0        0        0      562 2023-06-02 20:28:20.558582 gdshoplib-2.0.5/gdshoplib/cli/application.py
--rw-r--r--   0        0        0      243 2023-05-24 11:47:55.215449 gdshoplib-2.0.5/gdshoplib/cli/crm/application.py
--rw-r--r--   0        0        0     1098 2023-07-12 23:37:55.448098 gdshoplib-2.0.5/gdshoplib/cli/crm/order.py
--rw-r--r--   0        0        0      357 2023-05-24 11:47:55.219994 gdshoplib-2.0.5/gdshoplib/cli/crm/stats.py
--rw-r--r--   0        0        0      162 2023-05-24 11:47:55.222526 gdshoplib-2.0.5/gdshoplib/cli/finance/application.py
--rw-r--r--   0        0        0      383 2023-05-24 11:47:55.224775 gdshoplib-2.0.5/gdshoplib/cli/finance/store.py
--rw-r--r--   0        0        0      734 2023-05-30 20:06:07.282477 gdshoplib-2.0.5/gdshoplib/cli/product/application.py
--rw-r--r--   0        0        0     2239 2023-05-30 20:06:07.284766 gdshoplib-2.0.5/gdshoplib/cli/product/barcode_cli.py
--rw-r--r--   0        0        0     5334 2023-06-18 20:26:13.335384 gdshoplib-2.0.5/gdshoplib/cli/product/cache.py
--rw-r--r--   0        0        0     1963 2023-06-06 10:07:12.790146 gdshoplib-2.0.5/gdshoplib/cli/product/controle.py
--rw-r--r--   0        0        0     1797 2023-05-24 11:47:55.235444 gdshoplib-2.0.5/gdshoplib/cli/product/description.py
--rw-r--r--   0        0        0      672 2023-05-24 11:47:55.237453 gdshoplib-2.0.5/gdshoplib/cli/product/feed.py
--rw-r--r--   0        0        0     3091 2023-05-24 11:47:55.239401 gdshoplib-2.0.5/gdshoplib/cli/product/media.py
--rw-r--r--   0        0        0     1801 2023-07-13 20:46:37.938402 gdshoplib-2.0.5/gdshoplib/cli/product/price.py
--rw-r--r--   0        0        0      238 2023-05-24 11:47:55.243363 gdshoplib-2.0.5/gdshoplib/cli/service/application.py
--rw-r--r--   0        0        0      458 2023-06-02 20:27:44.870766 gdshoplib-2.0.5/gdshoplib/cli/service/avito.py
--rw-r--r--   0        0        0     1070 2023-06-02 22:30:11.800230 gdshoplib-2.0.5/gdshoplib/cli/service/vk.py
--rw-r--r--   0        0        0      962 2023-05-30 22:43:31.841649 gdshoplib-2.0.5/gdshoplib/cli/temporal/application.py
--rw-r--r--   0        0        0     1404 2023-06-13 21:49:15.384565 gdshoplib-2.0.5/gdshoplib/core/ecosystem.py
--rw-r--r--   0        0        0     3744 2023-07-13 20:47:53.451699 gdshoplib-2.0.5/gdshoplib/core/settings.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.525746 gdshoplib-2.0.5/gdshoplib/packages/__init__.py
--rw-r--r--   0        0        0     1320 2023-05-30 20:06:07.289858 gdshoplib-2.0.5/gdshoplib/packages/barcode_pack.py
--rw-r--r--   0        0        0     3829 2023-05-24 11:47:55.253311 gdshoplib-2.0.5/gdshoplib/packages/cache.py
--rw-r--r--   0        0        0     4177 2023-05-24 11:47:55.255216 gdshoplib-2.0.5/gdshoplib/packages/feed.py
--rw-r--r--   0        0        0      774 2023-01-01 19:36:37.530383 gdshoplib-2.0.5/gdshoplib/packages/lang.py
--rw-r--r--   0        0        0      148 2023-05-24 11:47:55.257504 gdshoplib-2.0.5/gdshoplib/packages/marker.py
--rw-r--r--   0        0        0     2362 2023-07-12 22:35:57.003635 gdshoplib-2.0.5/gdshoplib/packages/renderer.py
--rw-r--r--   0        0        0     3869 2023-06-15 19:46:00.483976 gdshoplib-2.0.5/gdshoplib/packages/s3.py
--rw-r--r--   0        0        0     1986 2023-06-18 20:25:34.332713 gdshoplib-2.0.5/gdshoplib/packages/s3v2.py
--rw-r--r--   0        0        0        0 2023-01-01 19:36:37.533334 gdshoplib-2.0.5/gdshoplib/services/__init__.py
--rw-r--r--   0        0        0     3746 2023-07-12 22:35:57.908452 gdshoplib-2.0.5/gdshoplib/services/avito/avito.py
--rw-r--r--   0        0        0        0 2023-07-04 21:57:07.519433 gdshoplib-2.0.5/gdshoplib/services/cdek/cdek.py
--rw-r--r--   0        0        0      106 2023-07-09 23:40:49.717481 gdshoplib-2.0.5/gdshoplib/services/gdshop/gdshop.py
--rw-r--r--   0        0        0     2821 2022-11-29 21:45:29.006810 gdshoplib-2.0.5/gdshoplib/services/notion/README.md
--rw-r--r--   0        0        0       50 2023-01-01 19:36:37.534464 gdshoplib-2.0.5/gdshoplib/services/notion/__init__.py
--rw-r--r--   0        0        0     1931 2023-07-12 21:53:17.811158 gdshoplib-2.0.5/gdshoplib/services/notion/base.py
--rw-r--r--   0        0        0      655 2023-06-11 10:01:55.572121 gdshoplib-2.0.5/gdshoplib/services/notion/block.py
--rw-r--r--   0        0        0     1174 2023-01-08 13:59:30.362864 gdshoplib-2.0.5/gdshoplib/services/notion/database.py
--rw-r--r--   0        0        0     1908 2023-07-12 22:35:57.809104 gdshoplib-2.0.5/gdshoplib/services/notion/manager.py
--rw-r--r--   0        0        0     2531 2023-05-24 11:47:55.273029 gdshoplib-2.0.5/gdshoplib/services/notion/models/props.py
--rw-r--r--   0        0        0     4027 2023-07-12 22:49:22.825924 gdshoplib-2.0.5/gdshoplib/services/notion/notion.py
--rw-r--r--   0        0        0    10195 2023-07-13 20:51:36.374381 gdshoplib-2.0.5/gdshoplib/services/notion/page.py
--rw-r--r--   0        0        0     2893 2023-05-24 11:47:55.277301 gdshoplib-2.0.5/gdshoplib/services/vk/market.py
--rw-r--r--   0        0        0     1825 2023-05-24 11:47:55.278048 gdshoplib-2.0.5/gdshoplib/services/vk/media.py
--rw-r--r--   0        0        0      986 2023-05-24 11:47:55.282128 gdshoplib-2.0.5/gdshoplib/services/vk/page.py
--rw-r--r--   0        0        0     2596 2023-05-24 11:47:55.285739 gdshoplib-2.0.5/gdshoplib/services/vk/stats.py
--rw-r--r--   0        0        0     2880 2023-05-24 11:47:58.644858 gdshoplib-2.0.5/gdshoplib/services/vk/stories.py
--rw-r--r--   0        0        0     2433 2023-07-12 22:35:57.881523 gdshoplib-2.0.5/gdshoplib/services/vk/vk.py
--rw-r--r--   0        0        0      104 2023-05-24 11:47:55.290271 gdshoplib-2.0.5/gdshoplib/services/ym/ym.py
--rw-r--r--   0        0        0      990 2023-07-09 23:40:49.720503 gdshoplib-2.0.5/gdshoplib/templates/basic.txt
--rw-r--r--   0        0        0      447 2023-05-24 11:47:55.298840 gdshoplib-2.0.5/gdshoplib/templates/instagram.txt
--rw-r--r--   0        0        0      990 2023-05-24 11:47:55.301319 gdshoplib-2.0.5/gdshoplib/templates/order_info.txt
--rw-r--r--   0        0        0      989 2023-05-24 11:47:55.305236 gdshoplib-2.0.5/gdshoplib/templates/ula.txt
--rw-r--r--   0        0        0     1052 2023-05-24 11:47:55.308271 gdshoplib-2.0.5/gdshoplib/templates/vk.txt
--rw-r--r--   0        0        0      470 2023-05-30 21:41:48.464779 gdshoplib-2.0.5/gdshoplib/workflows/notion.py
--rw-r--r--   0        0        0     1625 2023-07-13 21:07:57.428436 gdshoplib-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     3812 1970-01-01 00:00:00.000000 gdshoplib-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2004 2023-05-24 11:47:55.174891 gdshoplib-2.1.1/README.md
+-rw-r--r--   0        0        0      210 2023-05-24 11:47:55.177560 gdshoplib-2.1.1/gdshoplib/__init__.py
+-rw-r--r--   0        0        0       80 2023-01-03 20:04:30.238472 gdshoplib-2.1.1/gdshoplib/__main__.py
+-rw-r--r--   0        0        0      117 2023-05-30 14:34:35.058893 gdshoplib-2.1.1/gdshoplib/activities/notion.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.507364 gdshoplib-2.1.1/gdshoplib/apps/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-24 11:47:55.179848 gdshoplib-2.1.1/gdshoplib/apps/crm/dialog.py
+-rw-r--r--   0        0        0     3637 2023-07-16 21:55:55.675033 gdshoplib-2.1.1/gdshoplib/apps/crm/on_request.py
+-rw-r--r--   0        0        0    11093 2023-07-16 21:55:58.447408 gdshoplib-2.1.1/gdshoplib/apps/crm/orders.py
+-rw-r--r--   0        0        0      674 2023-05-24 11:47:55.186839 gdshoplib-2.1.1/gdshoplib/apps/crm/stats.py
+-rw-r--r--   0        0        0      315 2023-05-24 11:47:55.189032 gdshoplib-2.1.1/gdshoplib/apps/delivery/delivery.py
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003805 gdshoplib-2.1.1/gdshoplib/apps/finance/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-24 11:47:55.191346 gdshoplib-2.1.1/gdshoplib/apps/finance/storage.py
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.003925 gdshoplib-2.1.1/gdshoplib/apps/marketing/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-24 11:47:55.193504 gdshoplib-2.1.1/gdshoplib/apps/payments/payments.py
+-rw-r--r--   0        0        0      378 2023-01-01 19:36:37.510481 gdshoplib-2.1.1/gdshoplib/apps/platforms/README.md
+-rw-r--r--   0        0        0      665 2023-05-24 11:47:55.195540 gdshoplib-2.1.1/gdshoplib/apps/platforms/__init__.py
+-rw-r--r--   0        0        0     1742 2023-05-24 11:47:55.197783 gdshoplib-2.1.1/gdshoplib/apps/platforms/avito.py
+-rw-r--r--   0        0        0      113 2023-02-02 20:37:00.702563 gdshoplib-2.1.1/gdshoplib/apps/platforms/base.py
+-rw-r--r--   0        0        0      152 2023-01-12 22:25:31.627980 gdshoplib-2.1.1/gdshoplib/apps/platforms/instagram.py
+-rw-r--r--   0        0        0       95 2023-01-12 22:25:09.142423 gdshoplib-2.1.1/gdshoplib/apps/platforms/ok.py
+-rw-r--r--   0        0        0      467 2023-05-24 11:47:55.199621 gdshoplib-2.1.1/gdshoplib/apps/platforms/sm.py
+-rw-r--r--   0        0        0       95 2023-01-12 22:26:15.528644 gdshoplib-2.1.1/gdshoplib/apps/platforms/tg.py
+-rw-r--r--   0        0        0      908 2023-05-24 11:47:55.201920 gdshoplib-2.1.1/gdshoplib/apps/platforms/ula.py
+-rw-r--r--   0        0        0      512 2023-05-24 11:47:55.204568 gdshoplib-2.1.1/gdshoplib/apps/platforms/vk.py
+-rw-r--r--   0        0        0     3373 2023-05-24 11:47:58.629272 gdshoplib-2.1.1/gdshoplib/apps/platforms/yam.py
+-rw-r--r--   0        0        0      187 2023-01-01 19:36:37.519008 gdshoplib-2.1.1/gdshoplib/apps/products/README.md
+-rw-r--r--   0        0        0        0 2022-11-29 21:45:29.004030 gdshoplib-2.1.1/gdshoplib/apps/products/__init__.py
+-rw-r--r--   0        0        0     1931 2023-02-02 20:29:22.002155 gdshoplib-2.1.1/gdshoplib/apps/products/description.py
+-rw-r--r--   0        0        0     5779 2023-07-12 22:35:57.507949 gdshoplib-2.1.1/gdshoplib/apps/products/media.py
+-rw-r--r--   0        0        0     1716 2023-07-16 21:55:55.591343 gdshoplib-2.1.1/gdshoplib/apps/products/price.py
+-rw-r--r--   0        0        0     5687 2023-07-16 20:26:10.882089 gdshoplib-2.1.1/gdshoplib/apps/products/product.py
+-rw-r--r--   0        0        0     5947 2023-06-18 20:41:49.001382 gdshoplib-2.1.1/gdshoplib/apps/uploader/uploader.py
+-rw-r--r--   0        0        0      562 2023-06-02 20:28:20.558582 gdshoplib-2.1.1/gdshoplib/cli/application.py
+-rw-r--r--   0        0        0      243 2023-05-24 11:47:55.215449 gdshoplib-2.1.1/gdshoplib/cli/crm/application.py
+-rw-r--r--   0        0        0     1098 2023-07-12 23:37:55.448098 gdshoplib-2.1.1/gdshoplib/cli/crm/order.py
+-rw-r--r--   0        0        0      357 2023-05-24 11:47:55.219994 gdshoplib-2.1.1/gdshoplib/cli/crm/stats.py
+-rw-r--r--   0        0        0      162 2023-05-24 11:47:55.222526 gdshoplib-2.1.1/gdshoplib/cli/finance/application.py
+-rw-r--r--   0        0        0      383 2023-05-24 11:47:55.224775 gdshoplib-2.1.1/gdshoplib/cli/finance/store.py
+-rw-r--r--   0        0        0      734 2023-05-30 20:06:07.282477 gdshoplib-2.1.1/gdshoplib/cli/product/application.py
+-rw-r--r--   0        0        0     2239 2023-05-30 20:06:07.284766 gdshoplib-2.1.1/gdshoplib/cli/product/barcode_cli.py
+-rw-r--r--   0        0        0     5334 2023-06-18 20:26:13.335384 gdshoplib-2.1.1/gdshoplib/cli/product/cache.py
+-rw-r--r--   0        0        0     1963 2023-06-06 10:07:12.790146 gdshoplib-2.1.1/gdshoplib/cli/product/controle.py
+-rw-r--r--   0        0        0     1797 2023-05-24 11:47:55.235444 gdshoplib-2.1.1/gdshoplib/cli/product/description.py
+-rw-r--r--   0        0        0      672 2023-05-24 11:47:55.237453 gdshoplib-2.1.1/gdshoplib/cli/product/feed.py
+-rw-r--r--   0        0        0     3091 2023-05-24 11:47:55.239401 gdshoplib-2.1.1/gdshoplib/cli/product/media.py
+-rw-r--r--   0        0        0     1832 2023-07-16 21:55:55.625303 gdshoplib-2.1.1/gdshoplib/cli/product/price.py
+-rw-r--r--   0        0        0      238 2023-05-24 11:47:55.243363 gdshoplib-2.1.1/gdshoplib/cli/service/application.py
+-rw-r--r--   0        0        0      458 2023-06-02 20:27:44.870766 gdshoplib-2.1.1/gdshoplib/cli/service/avito.py
+-rw-r--r--   0        0        0     1070 2023-06-02 22:30:11.800230 gdshoplib-2.1.1/gdshoplib/cli/service/vk.py
+-rw-r--r--   0        0        0      962 2023-05-30 22:43:31.841649 gdshoplib-2.1.1/gdshoplib/cli/temporal/application.py
+-rw-r--r--   0        0        0     1404 2023-06-13 21:49:15.384565 gdshoplib-2.1.1/gdshoplib/core/ecosystem.py
+-rw-r--r--   0        0        0     3794 2023-07-16 20:23:56.588877 gdshoplib-2.1.1/gdshoplib/core/settings.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.525746 gdshoplib-2.1.1/gdshoplib/packages/__init__.py
+-rw-r--r--   0        0        0     1320 2023-05-30 20:06:07.289858 gdshoplib-2.1.1/gdshoplib/packages/barcode_pack.py
+-rw-r--r--   0        0        0     3829 2023-05-24 11:47:55.253311 gdshoplib-2.1.1/gdshoplib/packages/cache.py
+-rw-r--r--   0        0        0     4177 2023-05-24 11:47:55.255216 gdshoplib-2.1.1/gdshoplib/packages/feed.py
+-rw-r--r--   0        0        0      774 2023-01-01 19:36:37.530383 gdshoplib-2.1.1/gdshoplib/packages/lang.py
+-rw-r--r--   0        0        0      148 2023-05-24 11:47:55.257504 gdshoplib-2.1.1/gdshoplib/packages/marker.py
+-rw-r--r--   0        0        0     2362 2023-07-12 22:35:57.003635 gdshoplib-2.1.1/gdshoplib/packages/renderer.py
+-rw-r--r--   0        0        0     3869 2023-06-15 19:46:00.483976 gdshoplib-2.1.1/gdshoplib/packages/s3.py
+-rw-r--r--   0        0        0     1986 2023-06-18 20:25:34.332713 gdshoplib-2.1.1/gdshoplib/packages/s3v2.py
+-rw-r--r--   0        0        0        0 2023-01-01 19:36:37.533334 gdshoplib-2.1.1/gdshoplib/services/__init__.py
+-rw-r--r--   0        0        0     3746 2023-07-12 22:35:57.908452 gdshoplib-2.1.1/gdshoplib/services/avito/avito.py
+-rw-r--r--   0        0        0        0 2023-07-04 21:57:07.519433 gdshoplib-2.1.1/gdshoplib/services/cdek/cdek.py
+-rw-r--r--   0        0        0     1062 2023-07-16 21:55:58.603395 gdshoplib-2.1.1/gdshoplib/services/gdshop/gdshop.py
+-rw-r--r--   0        0        0     2821 2022-11-29 21:45:29.006810 gdshoplib-2.1.1/gdshoplib/services/notion/README.md
+-rw-r--r--   0        0        0       50 2023-01-01 19:36:37.534464 gdshoplib-2.1.1/gdshoplib/services/notion/__init__.py
+-rw-r--r--   0        0        0     1931 2023-07-12 21:53:17.811158 gdshoplib-2.1.1/gdshoplib/services/notion/base.py
+-rw-r--r--   0        0        0      655 2023-06-11 10:01:55.572121 gdshoplib-2.1.1/gdshoplib/services/notion/block.py
+-rw-r--r--   0        0        0     1174 2023-01-08 13:59:30.362864 gdshoplib-2.1.1/gdshoplib/services/notion/database.py
+-rw-r--r--   0        0        0     1908 2023-07-12 22:35:57.809104 gdshoplib-2.1.1/gdshoplib/services/notion/manager.py
+-rw-r--r--   0        0        0     2531 2023-05-24 11:47:55.273029 gdshoplib-2.1.1/gdshoplib/services/notion/models/props.py
+-rw-r--r--   0        0        0     4027 2023-07-12 22:49:22.825924 gdshoplib-2.1.1/gdshoplib/services/notion/notion.py
+-rw-r--r--   0        0        0    10195 2023-07-16 20:24:05.490318 gdshoplib-2.1.1/gdshoplib/services/notion/page.py
+-rw-r--r--   0        0        0     2893 2023-05-24 11:47:55.277301 gdshoplib-2.1.1/gdshoplib/services/vk/market.py
+-rw-r--r--   0        0        0     1825 2023-05-24 11:47:55.278048 gdshoplib-2.1.1/gdshoplib/services/vk/media.py
+-rw-r--r--   0        0        0      986 2023-05-24 11:47:55.282128 gdshoplib-2.1.1/gdshoplib/services/vk/page.py
+-rw-r--r--   0        0        0     2596 2023-05-24 11:47:55.285739 gdshoplib-2.1.1/gdshoplib/services/vk/stats.py
+-rw-r--r--   0        0        0     2880 2023-05-24 11:47:58.644858 gdshoplib-2.1.1/gdshoplib/services/vk/stories.py
+-rw-r--r--   0        0        0     2433 2023-07-12 22:35:57.881523 gdshoplib-2.1.1/gdshoplib/services/vk/vk.py
+-rw-r--r--   0        0        0      104 2023-05-24 11:47:55.290271 gdshoplib-2.1.1/gdshoplib/services/ym/ym.py
+-rw-r--r--   0        0        0      978 2023-07-16 20:21:54.946692 gdshoplib-2.1.1/gdshoplib/templates/basic.txt
+-rw-r--r--   0        0        0      447 2023-05-24 11:47:55.298840 gdshoplib-2.1.1/gdshoplib/templates/instagram.txt
+-rw-r--r--   0        0        0     1040 2023-07-16 20:24:48.251152 gdshoplib-2.1.1/gdshoplib/templates/vk.txt
+-rw-r--r--   0        0        0      470 2023-05-30 21:41:48.464779 gdshoplib-2.1.1/gdshoplib/workflows/notion.py
+-rw-r--r--   0        0        0     1652 2023-07-16 21:38:08.780664 gdshoplib-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 gdshoplib-2.1.1/PKG-INFO
```

### Comparing `gdshoplib-2.0.5/README.md` & `gdshoplib-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/crm/on_request.py` & `gdshoplib-2.1.1/gdshoplib/apps/crm/on_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Optional
 
 from pydantic import BaseModel, ValidationError
 
-from gdshoplib.apps.products.price import Price
 from gdshoplib.services.notion.models.props import PropModel
 
 
 class OnRequestTable:
     def __init__(self, blocks, /, notion, parent):
         self.notion = notion
         self.parent = parent
@@ -49,15 +48,15 @@
             self._rows = self._parse_rows()
         return self._rows
 
     def price(self, base_price="neitral"):
         return (
             sum(
                 [
-                    Price(r)[base_price] * r.quantity
+                    r.profit if base_price == "profit" else r.now * r.quantity
                     for r in filter(
                         lambda x: isinstance(x, OnRequestTableRow), self.rows
                     )
                 ]
             )
             or 0
         )
@@ -114,14 +113,22 @@
     quantity: int
     error: Optional[str]
 
     @property
     def price_eur(self):
         return self.price
 
+    @property
+    def now(self):
+        return round(self.price * 102 * 1.28 * 1.10 * 1.08)
+
+    @property
+    def profit(self):
+        return round(self.price * 102 * 1.28 * 0.10)
+
 
 class OnRequestTableInvalidRow(BaseModel):
     block_id: str
     name: Optional[str]
     link: Optional[str]
     price: Optional[str]
     quantity: Optional[str]
```

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/crm/orders.py` & `gdshoplib-2.1.1/gdshoplib/apps/crm/orders.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,14 +165,18 @@
         self.promocodes.sort(key=lambda x: x.discount)
         return self.promocodes[0]
 
     @property
     def price(self):
         result = self.on_request.price()
         for product in self.products:
+            result += product.price.now
+        return result
+        result = self.on_request.price()
+        for product in self.products:
             if self.order_type == "Агент":
                 result += product.price.neitral
             else:
                 promocode = self.get_promocode()
                 if promocode and product.price.current_discount < promocode.discount:
                     _price = (
                         product.price.profit
@@ -195,18 +199,18 @@
                 else product.price.now
             )
 
         return result
 
     @property
     def profit(self):
-        base_price = self.on_request.price("gross")
+        profit = self.on_request.price("profit")
         for product in self.products:
-            base_price += product.price.gross
-        return self.price - base_price
+            profit += product.price.profit
+        return profit
 
     def generate_id(self):
         return f"{self.platform.key.lower()}.{int(time.time())}"
 
     def description_on_request_product(self, row):
         quantity = f"({row.quantity} шт.)"
         return f"{row.name} {quantity if row.quantity > 1 else ''}: {Price(row)['neitral'] * row.quantity} ₽"
@@ -307,18 +311,18 @@
         ...
 
     @classmethod
     def update(cls):
         # Обновление карточки Order
         for order in cls.query(notion=Notion(caching=True), params=cls.list_filter()):
             order.on_request.update()
-            order.set_price_description()
+            # order.set_price_description()
             order.set_profit()
             order.set_price()
-            order.set_max_discount()
+            # order.set_max_discount()
             order.update_status("Комплектация")
             if not order.pk:
                 order.set_id()
 
     @classmethod
     def update_decline(cls):
         date = datetime.date.today() - datetime.timedelta(days=7)
```

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/crm/stats.py` & `gdshoplib-2.1.1/gdshoplib/apps/crm/stats.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/platforms/__init__.py` & `gdshoplib-2.1.1/gdshoplib/apps/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/platforms/avito.py` & `gdshoplib-2.1.1/gdshoplib/apps/platforms/avito.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/platforms/ula.py` & `gdshoplib-2.1.1/gdshoplib/apps/platforms/ula.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/platforms/vk.py` & `gdshoplib-2.1.1/gdshoplib/apps/platforms/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/platforms/yam.py` & `gdshoplib-2.1.1/gdshoplib/apps/platforms/yam.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/products/description.py` & `gdshoplib-2.1.1/gdshoplib/apps/products/description.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/products/media.py` & `gdshoplib-2.1.1/gdshoplib/apps/products/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/products/product.py` & `gdshoplib-2.1.1/gdshoplib/apps/products/product.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/apps/uploader/uploader.py` & `gdshoplib-2.1.1/gdshoplib/apps/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/application.py` & `gdshoplib-2.1.1/gdshoplib/cli/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/crm/order.py` & `gdshoplib-2.1.1/gdshoplib/cli/crm/order.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/product/application.py` & `gdshoplib-2.1.1/gdshoplib/cli/product/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/product/barcode_cli.py` & `gdshoplib-2.1.1/gdshoplib/cli/product/barcode_cli.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/product/cache.py` & `gdshoplib-2.1.1/gdshoplib/cli/product/cache.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/product/controle.py` & `gdshoplib-2.1.1/gdshoplib/cli/product/controle.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/product/description.py` & `gdshoplib-2.1.1/gdshoplib/cli/product/description.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/product/feed.py` & `gdshoplib-2.1.1/gdshoplib/cli/product/feed.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/product/media.py` & `gdshoplib-2.1.1/gdshoplib/cli/product/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/product/price.py` & `gdshoplib-2.1.1/gdshoplib/cli/product/price.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,26 +33,35 @@
 
         if loop_iteration:
             time.sleep(loop_iteration)
         else:
             break
 
 
+@app.command()
+def get(sku: str):
+    product = Product.get(sku)
+    print(
+        dict(
+            sku=sku,
+            discount=product.price.current_discount,
+            now=product.price.now,
+            profit=product.price.profit,
+        )
+    )
+
+
 ###
 
 
 def price_update_action(id):
     product = Product(id)
     props_map = {
         "price_now": dict(name="Текущая Цена", value=product.price.now),
         "price_neitral": dict(name="Безубыточность", value=product.price.neitral),
-        "price_current_discount": dict(
-            name="Текущая Скидка", value=product.price.current_discount
-        ),
-        "price_gross": dict(name="Себестоимость", value=product.price.gross),
     }
 
     for k, v in props_map.items():
         if not product[k] and not v["value"] or product[k] == v["value"]:
             continue
 
         product.notion.update_prop(
```

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/service/vk.py` & `gdshoplib-2.1.1/gdshoplib/cli/service/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/cli/temporal/application.py` & `gdshoplib-2.1.1/gdshoplib/cli/temporal/application.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/core/ecosystem.py` & `gdshoplib-2.1.1/gdshoplib/core/ecosystem.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/core/settings.py` & `gdshoplib-2.1.1/gdshoplib/core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 class GeneralSettings(BaseSettings):
     TEMPLATES_PATH: DirectoryPath = (BASEPATH / "templates").resolve()
     MONTH_SALE_RATE: int = 9
     TURNOVER_RATE: int = 5
 
 
+class DBSettings(BaseSettings):
+    DB_DSB: str
+
+
 class NotionSettings(BaseSettings):
     NOTION_SECRET_TOKEN: str
     CACHE_ENABLED: bool = True
     KAFKA_BROKER: Optional[str]
     KAFKA_TOPIC: Optional[str] = "notion"
```

### Comparing `gdshoplib-2.0.5/gdshoplib/packages/barcode_pack.py` & `gdshoplib-2.1.1/gdshoplib/packages/barcode_pack.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/packages/cache.py` & `gdshoplib-2.1.1/gdshoplib/packages/cache.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/packages/feed.py` & `gdshoplib-2.1.1/gdshoplib/packages/feed.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/packages/lang.py` & `gdshoplib-2.1.1/gdshoplib/packages/lang.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/packages/renderer.py` & `gdshoplib-2.1.1/gdshoplib/packages/renderer.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/packages/s3.py` & `gdshoplib-2.1.1/gdshoplib/packages/s3.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/packages/s3v2.py` & `gdshoplib-2.1.1/gdshoplib/packages/s3v2.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/avito/avito.py` & `gdshoplib-2.1.1/gdshoplib/services/avito/avito.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/notion/README.md` & `gdshoplib-2.1.1/gdshoplib/services/notion/README.md`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/notion/base.py` & `gdshoplib-2.1.1/gdshoplib/services/notion/base.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/notion/block.py` & `gdshoplib-2.1.1/gdshoplib/services/notion/block.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/notion/database.py` & `gdshoplib-2.1.1/gdshoplib/services/notion/database.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/notion/manager.py` & `gdshoplib-2.1.1/gdshoplib/services/notion/manager.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/notion/models/props.py` & `gdshoplib-2.1.1/gdshoplib/services/notion/models/props.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/notion/notion.py` & `gdshoplib-2.1.1/gdshoplib/services/notion/notion.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/notion/page.py` & `gdshoplib-2.1.1/gdshoplib/services/notion/page.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/vk/market.py` & `gdshoplib-2.1.1/gdshoplib/services/vk/market.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/vk/media.py` & `gdshoplib-2.1.1/gdshoplib/services/vk/media.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/vk/page.py` & `gdshoplib-2.1.1/gdshoplib/services/vk/page.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/vk/stats.py` & `gdshoplib-2.1.1/gdshoplib/services/vk/stats.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/vk/stories.py` & `gdshoplib-2.1.1/gdshoplib/services/vk/stories.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/services/vk/vk.py` & `gdshoplib-2.1.1/gdshoplib/services/vk/vk.py`

 * *Files identical despite different names*

### Comparing `gdshoplib-2.0.5/gdshoplib/templates/basic.txt` & `gdshoplib-2.1.1/gdshoplib/templates/vk.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% if product.quantity == 0 %}📦 Под заказ 📦
-
 {% endif %}{{ product.name }}{% if product.price.current_discount and product.quantity > 0 and product.price.current_discount > 4 %}
-Цена указана со скидкой: {{ product.price.current_discount }}% {% endif %}
+Текущая скидка: -{{ product.price.current_discount }} ₽ {% endif %}
 
 {% if product.brand %}Бренд: {{product.brand.title}}{% endif %}{% if product.collection %}
 Коллекция: {{product.collection}}{% endif %}{% if product.size %}
 Размер: {{product.size}}{% endif %}{% if product.color %}
 Цвет: {{product.color}}{% endif %}
 
 {% if product.short_description %}{{product.short_description}}{% endif %}
 {% if product.specifications %}{% for material in product.specifications %}
 - {{material}}{% endfor %}{% endif %}{% if product.notes %}{% for note in product.notes %}
 - {{note}}{% endfor %}{% endif %}
 
 Доставка в любой город России
 Местонахождение магазина, Москва
 
-Артикул: {{product.sku}}
+{% if product.short_description %}
+{% for tag in product.tags %}#{{tag}} {% endfor %}{%endif%}
```

### Comparing `gdshoplib-2.0.5/gdshoplib/templates/order_info.txt` & `gdshoplib-2.1.1/gdshoplib/templates/basic.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% if product.quantity == 0 %}📦 Под заказ 📦
 
 {% endif %}{{ product.name }}{% if product.price.current_discount and product.quantity > 0 and product.price.current_discount > 4 %}
-Цена указана со скидкой: {{ product.price.current_discount }}% {% endif %}
+Текущая скидка: -{{ product.price.current_discount }} ₽ {% endif %}
 
 {% if product.brand %}Бренд: {{product.brand.title}}{% endif %}{% if product.collection %}
 Коллекция: {{product.collection}}{% endif %}{% if product.size %}
 Размер: {{product.size}}{% endif %}{% if product.color %}
 Цвет: {{product.color}}{% endif %}
 
 {% if product.short_description %}{{product.short_description}}{% endif %}
```

### Comparing `gdshoplib-2.0.5/pyproject.toml` & `gdshoplib-2.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gdshoplib"
-version = "2.0.5"
+version = "2.1.1"
 description = ""
 authors = ["Nikolay Baryshnikov <root@k0d.ru>"]
 packages=[
     { include = "gdshoplib" },
 ]
 license="MIT"
 readme="README.md"
@@ -47,14 +47,15 @@
 python-barcode = "^0.14.0"
 pyzbar = "^0.1.9"
 opencv-python = "^4.7.0.72"
 kafka-python = "^2.0.2"
 msgpack = "^1.0.5"
 ujson = "^5.7.0"
 temporalio = "^1.2.0"
+psycopg2-binary = "^2.9.6"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0.4"
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
```

### Comparing `gdshoplib-2.0.5/PKG-INFO` & `gdshoplib-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdshoplib
-Version: 2.0.5
+Version: 2.1.1
 Summary: 
 Home-page: https://github.com/p141592
 License: MIT
 Author: Nikolay Baryshnikov
 Author-email: root@k0d.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,15 @@
 Requires-Dist: kafka-python (>=2.0.2,<3.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: msgpack (>=1.0.5,<2.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-barcode (>=0.14.0,<0.15.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: pyzbar (>=0.1.9,<0.2.0)
 Requires-Dist: qrcode[pil] (>=7.4.2,<8.0.0)
 Requires-Dist: redis (>=4.3.5,<5.0.0)
```

