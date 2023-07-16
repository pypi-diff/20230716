# Comparing `tmp/HibiAPI-0.7.7.tar.gz` & `tmp/HibiAPI-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HibiAPI-0.7.7.tar", max compression
+gzip compressed data, was "HibiAPI-0.8.0.tar", last modified: Sun Jul 16 02:24:39 2023, max compression
```

## Comparing `HibiAPI-0.7.7.tar` & `HibiAPI-0.8.0.tar`

### file list

```diff
@@ -1,67 +1,85 @@
--rw-r--r--   0        0        0    11349 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/LICENSE
--rw-r--r--   0        0        0     9748 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/README.md
--rw-r--r--   0        0        0      480 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/__init__.py
--rw-r--r--   0        0        0     2607 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/__main__.py
--rw-r--r--   0        0        0       66 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/__init__.py
--rw-r--r--   0        0        0      107 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/bilibili/__init__.py
--rw-r--r--   0        0        0      346 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/bilibili/api/__init__.py
--rw-r--r--   0        0        0    11317 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/bilibili/api/base.py
--rw-r--r--   0        0        0     5514 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/bilibili/api/v2.py
--rw-r--r--   0        0        0     4321 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/bilibili/api/v3.py
--rw-r--r--   0        0        0     1117 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/bilibili/constants.py
--rw-r--r--   0        0        0      363 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/bilibili/net.py
--rw-r--r--   0        0        0      203 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/netease/__init__.py
--rw-r--r--   0        0        0     7880 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/netease/api.py
--rw-r--r--   0        0        0     1090 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/netease/constants.py
--rw-r--r--   0        0        0      349 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/netease/net.py
--rw-r--r--   0        0        0      313 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/pixiv/__init__.py
--rw-r--r--   0        0        0    10179 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/pixiv/api.py
--rw-r--r--   0        0        0      809 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/pixiv/constants.py
--rw-r--r--   0        0        0     2170 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/pixiv/net.py
--rw-r--r--   0        0        0     4119 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/qrcode.py
--rw-r--r--   0        0        0      156 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/sauce/__init__.py
--rw-r--r--   0        0        0     4112 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/sauce/api.py
--rw-r--r--   0        0        0      642 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/sauce/constants.py
--rw-r--r--   0        0        0      300 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/sauce/net.py
--rw-r--r--   0        0        0      101 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/tieba/__init__.py
--rw-r--r--   0        0        0     4157 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/tieba/api.py
--rw-r--r--   0        0        0       88 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/tieba/net.py
--rw-r--r--   0        0        0      173 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/wallpaper/__init__.py
--rw-r--r--   0        0        0     3452 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/wallpaper/api.py
--rw-r--r--   0        0        0      197 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/wallpaper/constants.py
--rw-r--r--   0        0        0      226 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/api/wallpaper/net.py
--rw-r--r--   0        0        0       91 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/__init__.py
--rw-r--r--   0        0        0     4778 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/application.py
--rw-r--r--   0        0        0     2019 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/handlers.py
--rw-r--r--   0        0        0     3605 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/middlewares.py
--rw-r--r--   0        0        0     1056 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/__init__.py
--rw-r--r--   0        0        0      345 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/bilibili/__init__.py
--rw-r--r--   0        0        0     4262 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/bilibili/v2.py
--rw-r--r--   0        0        0     5131 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/bilibili/v3.py
--rw-r--r--   0        0        0     7397 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/netease.py
--rw-r--r--   0        0        0    11606 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/pixiv.py
--rw-r--r--   0        0        0     2006 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/qrcode.py
--rw-r--r--   0        0        0     3254 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/sauce.py
--rw-r--r--   0        0        0     1950 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/tieba.py
--rw-r--r--   0        0        0     2843 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/app/routes/wallpaper.py
--rw-r--r--   0        0        0      264 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/configs/bilibili.yml
--rw-r--r--   0        0        0     1914 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/configs/general.yml
--rw-r--r--   0        0        0      396 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/configs/netease.yml
--rw-r--r--   0        0        0      462 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/configs/pixiv.yml
--rw-r--r--   0        0        0      279 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/configs/qrcode.yml
--rw-r--r--   0        0        0      810 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/configs/sauce.yml
--rw-r--r--   0        0        0      209 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/configs/tieba.yml
--rw-r--r--   0        0        0      127 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/configs/wallpaper.yml
--rw-r--r--   0        0        0        0 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/__init__.py
--rw-r--r--   0        0        0     4250 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/cache.py
--rw-r--r--   0        0        0     3586 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/config.py
--rw-r--r--   0        0        0     3655 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/decorators/__init__.py
--rw-r--r--   0        0        0     2840 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/decorators/timer.py
--rw-r--r--   0        0        0     3168 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/exceptions.py
--rw-r--r--   0        0        0     2308 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/log.py
--rw-r--r--   0        0        0     3791 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/net.py
--rw-r--r--   0        0        0     2705 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/routing.py
--rw-r--r--   0        0        0     1766 2022-02-24 15:14:59.137930 HibiAPI-0.7.7/hibiapi/utils/temp.py
--rw-r--r--   0        0        0     1310 2022-02-24 15:14:59.141930 HibiAPI-0.7.7/pyproject.toml
--rw-r--r--   0        0        0    11387 2022-02-24 15:15:55.614302 HibiAPI-0.7.7/setup.py
--rw-r--r--   0        0        0    11003 2022-02-24 15:15:55.615292 HibiAPI-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/LICENSE
+-rw-r--r--   0        0        0    10989 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/README.md
+-rw-r--r--   0        0        0      480 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/__init__.py
+-rw-r--r--   0        0        0     3273 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/__init__.py
+-rw-r--r--   0        0        0      175 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bika/__init__.py
+-rw-r--r--   0        0        0     5724 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bika/api.py
+-rw-r--r--   0        0        0      662 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bika/constants.py
+-rw-r--r--   0        0        0     2047 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bika/net.py
+-rw-r--r--   0        0        0      107 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bilibili/__init__.py
+-rw-r--r--   0        0        0      312 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bilibili/api/__init__.py
+-rw-r--r--   0        0        0    10550 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bilibili/api/base.py
+-rw-r--r--   0        0        0     5363 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bilibili/api/v2.py
+-rw-r--r--   0        0        0     3707 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bilibili/api/v3.py
+-rw-r--r--   0        0        0     1117 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bilibili/constants.py
+-rw-r--r--   0        0        0      363 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/bilibili/net.py
+-rw-r--r--   0        0        0      163 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/netease/__init__.py
+-rw-r--r--   0        0        0     8226 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/netease/api.py
+-rw-r--r--   0        0        0     1090 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/netease/constants.py
+-rw-r--r--   0        0        0      349 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/netease/net.py
+-rw-r--r--   0        0        0      280 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/pixiv/__init__.py
+-rw-r--r--   0        0        0    14622 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/pixiv/api.py
+-rw-r--r--   0        0        0      643 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/pixiv/constants.py
+-rw-r--r--   0        0        0     2725 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/pixiv/net.py
+-rw-r--r--   0        0        0     4506 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/qrcode.py
+-rw-r--r--   0        0        0      156 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/sauce/__init__.py
+-rw-r--r--   0        0        0     4110 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/sauce/api.py
+-rw-r--r--   0        0        0      642 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/sauce/constants.py
+-rw-r--r--   0        0        0      285 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/sauce/net.py
+-rw-r--r--   0        0        0       86 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/tieba/__init__.py
+-rw-r--r--   0        0        0     3914 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/tieba/api.py
+-rw-r--r--   0        0        0       88 2023-07-16 02:24:08.015597 HibiAPI-0.8.0/hibiapi/api/tieba/net.py
+-rw-r--r--   0        0        0      133 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/api/wallpaper/__init__.py
+-rw-r--r--   0        0        0     3388 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/api/wallpaper/api.py
+-rw-r--r--   0        0        0      197 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/api/wallpaper/constants.py
+-rw-r--r--   0        0        0      226 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/api/wallpaper/net.py
+-rw-r--r--   0        0        0       91 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/__init__.py
+-rw-r--r--   0        0        0     5870 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/application.py
+-rw-r--r--   0        0        0     1908 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/handlers.py
+-rw-r--r--   0        0        0     3312 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/middlewares.py
+-rw-r--r--   0        0        0     1128 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/__init__.py
+-rw-r--r--   0        0        0      862 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/bika.py
+-rw-r--r--   0        0        0      399 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/bilibili/__init__.py
+-rw-r--r--   0        0        0      258 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/bilibili/v2.py
+-rw-r--r--   0        0        0      218 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/bilibili/v3.py
+-rw-r--r--   0        0        0      285 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/netease.py
+-rw-r--r--   0        0        0      843 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/pixiv.py
+-rw-r--r--   0        0        0     2011 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/qrcode.py
+-rw-r--r--   0        0        0     3254 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/sauce.py
+-rw-r--r--   0        0        0      248 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/tieba.py
+-rw-r--r--   0        0        0      268 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/app/routes/wallpaper.py
+-rw-r--r--   0        0        0      103 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/bika.yml
+-rw-r--r--   0        0        0      264 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/bilibili.yml
+-rw-r--r--   0        0        0     2180 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/general.yml
+-rw-r--r--   0        0        0      396 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/netease.yml
+-rw-r--r--   0        0        0      374 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/pixiv.yml
+-rw-r--r--   0        0        0      279 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/qrcode.yml
+-rw-r--r--   0        0        0      810 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/sauce.yml
+-rw-r--r--   0        0        0      209 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/tieba.yml
+-rw-r--r--   0        0        0      127 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/configs/wallpaper.yml
+-rw-r--r--   0        0        0        0 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/__init__.py
+-rw-r--r--   0        0        0     3733 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/cache.py
+-rw-r--r--   0        0        0     3020 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/config.py
+-rw-r--r--   0        0        0     3777 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/decorators/__init__.py
+-rw-r--r--   0        0        0     1473 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/decorators/enum.py
+-rw-r--r--   0        0        0     2956 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/decorators/timer.py
+-rw-r--r--   0        0        0     1779 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/exceptions.py
+-rw-r--r--   0        0        0     1864 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/log.py
+-rw-r--r--   0        0        0     3791 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/net.py
+-rw-r--r--   0        0        0     5989 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/routing.py
+-rw-r--r--   0        0        0      782 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/hibiapi/utils/temp.py
+-rw-r--r--   0        0        0     2309 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/__init__.py
+-rw-r--r--   0        0        0     3553 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_base.py
+-rw-r--r--   0        0        0     3311 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_bika.py
+-rw-r--r--   0        0        0     4255 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_bilibili_v2.py
+-rw-r--r--   0        0        0     3431 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_bilibili_v3.py
+-rw-r--r--   0        0        0     4041 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_netease.py
+-rw-r--r--   0        0        0     7732 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_pixiv.py
+-rw-r--r--   0        0        0     1839 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_qrcode.py
+-rw-r--r--   0        0        0   180127 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_sauce.jpg
+-rw-r--r--   0        0        0     1202 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_sauce.py
+-rw-r--r--   0        0        0     1547 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_tieba.py
+-rw-r--r--   0        0        0     2273 2023-07-16 02:24:08.019597 HibiAPI-0.8.0/test/test_wallpaper.py
+-rw-r--r--   0        0        0    11451 1970-01-01 00:00:00.000000 HibiAPI-0.8.0/PKG-INFO
```

### Comparing `HibiAPI-0.7.7/LICENSE` & `HibiAPI-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HibiAPI-0.7.7/README.md` & `HibiAPI-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,30 @@
+Metadata-Version: 2.1
+Name: HibiAPI
+Version: 0.8.0
+Summary: A program that implements easy-to-use APIs for a variety of commonly used sites
+License: Apache-2.0
+Author-email: mixmoe <admin@obfs.dev>
+Requires-Python: >=3.8,<4.0
+Provides-Extra: scripts
+Project-URL: documentation, https://github.com/mixmoe/HibiAPI/wiki
+Project-URL: homepage, https://api.obfs.dev
+Project-URL: repository, https://github.com/mixmoe/HibiAPI
+Description-Content-Type: text/markdown
+
 <!-- spell-checker: disable -->
 <!-- markdownlint-disable MD033 MD041 -->
 
 <img src=".github/logo.svg" align="right">
 
 <div align="left">
 
 # HibiAPI
 
-**_一个实现了多种常用站点的易用化API的程序._**
+**_一个实现了多种常用站点的易用化 API 的程序._**
 
 **_A program that implements easy-to-use APIs for a variety of commonly used sites._**
 
 [![Demo Version](https://img.shields.io/badge/dynamic/json?label=demo%20status&query=%24.info.version&url=https%3A%2F%2Fapi.obfs.dev%2Fopenapi.json&style=for-the-badge&color=lightblue)](https://api.obfs.dev)
 
 ![Lint](https://github.com/mixmoe/HibiAPI/workflows/Lint/badge.svg)
 ![Test](https://github.com/mixmoe/HibiAPI/workflows/Test/badge.svg)
@@ -31,59 +44,64 @@
 
 </div>
 
 ---
 
 ## 前言
 
-- `HibiAPI`提供多种网站公开内容的API集合, 它们包括:
-  - Pixiv的图片和小说相关信息获取和搜索
-  - Bilibili的视频/番剧等信息获取和搜索
-  - 网易云音乐的音乐/MV等信息获取和搜索
+- `HibiAPI`提供多种网站公开内容的 API 集合, 它们包括:
+
+  - Pixiv 的图片和小说相关信息获取和搜索
+  - Bilibili 的视频/番剧等信息获取和搜索
+  - 网易云音乐的音乐/MV 等信息获取和搜索
   - 百度贴吧的帖子内容的获取
   - [爱壁纸](https://adesk.com/)的横版和竖版壁纸获取
-  - and more…
+  - 哔咔漫画的漫画信息获取和搜索
+  - …
 
 - 该项目的前身是 Imjad API[^1]
   - 由于它的使用人数过多, 致使调用超出限制, 所以本人希望提供一个开源替代来供社区进行自由地部署和使用, 从而减轻一部分该 API 的使用压力
 
-[^1]: [什么是Imjad API](https://github.com/mixmoe/HibiAPI/wiki/FAQ#%E4%BB%80%E4%B9%88%E6%98%AFimjad-api)
+[^1]: [什么是 Imjad API](https://github.com/mixmoe/HibiAPI/wiki/FAQ#%E4%BB%80%E4%B9%88%E6%98%AFimjad-api)
 
 ## 优势
 
 ### 开源
 
-- 本项目以[Apache-2.0](./LICENSE)许可开源, 即:
-  - 你可以直接使用该项目提供的功能, 无需任何授权
-  - 你可以在**注明来源版权信息**的情况下对源代码进行任意分发和修改以及衍生
+- 本项目以[Apache-2.0](./LICENSE)许可开源, 请看[开源许可](#开源许可)一节
 
 ### 高效
 
 - 使用 Python 的[异步机制](https://docs.python.org/zh-cn/3/library/asyncio.html), 由[FastAPI](https://fastapi.tiangolo.com/)驱动, 带来高效的使用体验 ~~虽然性能瓶颈压根不在这~~
 
 ### 稳定
 
-- 在代码中广泛使用了Python的[类型提示支持](https://docs.python.org/zh-cn/3/library/typing.html), 使代码可读性更高且更加易于维护和调试
+- 在代码中广泛使用了 Python 的[类型提示支持](https://docs.python.org/zh-cn/3/library/typing.html), 使代码可读性更高且更加易于维护和调试
 
-- 在开发初期起就一直使用[PyLance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance), [Flake8](https://flake8.pycqa.org/en/latest/)以及[MyPy](https://mypy.readthedocs.io/)来对代码进行类型推断和纠错
+- 在开发初期起就一直使用多种现代 Python 开发工具辅助开发, 包括:
+
+  - 使用 [PyLance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) 进行静态类型推断
+  - 使用 [Flake8](https://flake8.pycqa.org/en/latest/) 对代码格式进行检查
+  - 使用 [Black](https://black.readthedocs.io/en/stable/) 格式化代码以提升代码可读性
 
 - 不直接使用第三方开发的 API 调用库, 而是全部用更加适合 Web 应用的逻辑重写第三方 API 请求, 更加可控 ~~疯狂造轮子~~
 
-## 已实现API[^2]
+## 已实现 API[^2]
 
 [^2]: 请查看 [#1](https://github.com/mixmoe/HibiAPI/issues/1)
 
 - [x] Pixiv
 - [x] 网易云音乐
 - [ ] ~~一言~~ (其代替方案<https://hitokoto.cn>提供的方案已足够好, 暂不考虑支持)
 - [x] Bilibili
 - [x] 二维码
-- [ ] ~~企鹅FM~~ (似乎用的人不是很多)
+- [ ] ~~企鹅 FM~~ (似乎用的人不是很多)
 - [x] 百度贴吧
 - [x] 爱壁纸
+- [x] 哔咔漫画
 
 ## 部署指南
 
 [![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
 
 - 手动部署指南: **[点击此处查看](https://github.com/mixmoe/HibiAPI/wiki/Deployment)**
 
@@ -92,80 +110,82 @@
 **我有更多的应用实例?** [立即 PR!](https://github.com/mixmoe/HibiAPI/pulls)
 
 - [`journey-ad/pixiv-viewer`](https://github.com/journey-ad/pixiv-viewer)
 
   - **又一个 Pixiv 阅览工具**
 
 - 公开搭建实例
-  |         **站点名称**         |            **网址**             |        **状态**         |
+  | **站点名称** | **网址** | **状态** |
   | :--------------------------: | :-----------------------------: | :---------------------: |
-  |      **官方 Demo[^3]**       |     <https://api.obfs.dev>      |  ![official][official]  |
-  |           轻零 API           |   <https://hibiapi.lite0.com>   |     ![lite0][lite0]     |
-  |     Kyomotoi の菜几服务      |   <https://api.kyomotoi.moe>    |       ![kyo][kyo]       |
-  |          老狐狸 API          | <https://hibiapi.aliserver.net> | ![older-fox][older-fox] |
-  | [MyCard](https://mycard.moe) |   <https://hibi.moecube.com>    |    ![mycard][mycard]    |
+  | **官方 Demo[^3]** | <https://api.obfs.dev> | [![official][official]][official-stats] |
+  | 轻零 API | <https://hibiapi.lite0.com> | ![lite0][lite0] |
+  | Kyomotoi の菜几服务 | <https://api.kyomotoi.moe> | ![kyo][kyo] |
+  | 老狐狸 API | <https://hibiapi.aliserver.net> | ![older-fox][older-fox] |
+  | [MyCard](https://mycard.moe) | <https://hibi.moecube.com> | ![mycard][mycard] |
 
-[^3]: 为了减轻服务器负担, Demo服务器已开启了Cloudflare全站缓存, 如果有实时获取更新的需求, 请自行搭建或使用其他部署实例
+[^3]: 为了减轻服务器负担, Demo 服务器已开启了 Cloudflare 全站缓存, 如果有实时获取更新的需求, 请自行搭建或使用其他部署实例
 
 [official]: https://img.shields.io/website?url=https%3A%2F%2Fapi.obfs.dev%2Fopenapi.json
+[official-stats]: https://metrics.librato.com/s/public/g1hepph3j
 [lite0]: https://img.shields.io/website?url=https%3A%2F%2Fhibiapi.lite0.com%2Fopenapi.json
 [kyo]: https://img.shields.io/website?url=https%3A%2F%2Fapi.kyomotoi.moe%2Fopenapi.json
 [older-fox]: https://img.shields.io/website?url=https%3A%2F%2Fhibiapi.aliserver.net%2Fopenapi.json
 [mycard]: https://img.shields.io/website?url=https%3A%2F%2Fhibi.moecube.com%2Fopenapi.json
 
 ## 特别鸣谢
 
-[**@journey-ad**](https://github.com/journey-ad) 大佬的 [Imjad API](https://api.imjad.cn/)
+[**@journey-ad**](https://github.com/journey-ad) 大佬的 **Imjad API**, 它是本项目的起源
 
 ### 参考项目
 
 > **正是因为有了你们, 这个项目才得以存在**
 
 - Pixiv: [`Mikubill/pixivpy-async`](https://github.com/Mikubill/pixivpy-async) [`upbit/pixivpy`](https://github.com/upbit/pixivpy)
 
 - Bilibili: [`SocialSisterYi/bilibili-API-collect`](https://github.com/SocialSisterYi/bilibili-API-collect) [`soimort/you-get`](https://github.com/soimort/you-get)
 
 - 网易云音乐: [`metowolf/NeteaseCloudMusicApi`](https://github.com/metowolf/NeteaseCloudMusicApi) [`greats3an/pyncm`](https://github.com/greats3an/pyncm) [`Binaryify/NeteaseCloudMusicApi`](https://github.com/Binaryify/NeteaseCloudMusicApi)
 
 - 百度贴吧: [`libsgh/tieba-api`](https://github.com/libsgh/tieba-api)
 
-### 贡献者们
+- 哔咔漫画：[`niuhuan/pica-rust`](https://github.com/niuhuan/pica-rust) [`abbeyokgo/PicaComic-Api`](https://github.com/abbeyokgo/PicaComic-Api)
 
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)
-<!-- ALL-CONTRIBUTORS-BADGE:END -->
+### 贡献者们
 
 感谢这些为这个项目作出贡献的各位大佬:
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
-  <tr>
-    <td align="center"><a href="http://kyomotoi.moe"><img src="https://avatars.githubusercontent.com/u/37587870?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kyomotoi</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=Kyomotoi" title="Documentation">📖</a> <a href="https://github.com/mixmoe/HibiAPI/commits?author=Kyomotoi" title="Tests">⚠️</a></td>
-    <td align="center"><a href="http://thdog.moe"><img src="https://avatars.githubusercontent.com/u/46120251?v=4?s=100" width="100px;" alt=""/><br /><sub><b>城倉奏</b></sub></a><br /><a href="#example-shirokurakana" title="Examples">💡</a></td>
-    <td align="center"><a href="http://skipm4.com"><img src="https://avatars.githubusercontent.com/u/40311581?v=4?s=100" width="100px;" alt=""/><br /><sub><b>SkipM4</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=SkipM4" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://github.com/leaf7th"><img src="https://avatars.githubusercontent.com/u/38352552?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nook</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=leaf7th" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/jiangzhuochi"><img src="https://avatars.githubusercontent.com/u/50538375?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jocky Chiang</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=jiangzhuochi" title="Code">💻</a></td>
-    <td align="center"><a href="https://github.com/cleoold"><img src="https://avatars.githubusercontent.com/u/13920903?v=4?s=100" width="100px;" alt=""/><br /><sub><b>midori</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=cleoold" title="Documentation">📖</a></td>
-    <td align="center"><a href="https://www.2yo.cc"><img src="https://avatars.githubusercontent.com/u/41198038?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pretty9</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=Pretty9" title="Code">💻</a></td>
-  </tr>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://kyomotoi.moe"><img src="https://avatars.githubusercontent.com/u/37587870?v=4?s=100" width="100px;" alt="Kyomotoi"/><br /><sub><b>Kyomotoi</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=Kyomotoi" title="Documentation">📖</a> <a href="https://github.com/mixmoe/HibiAPI/commits?author=Kyomotoi" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://thdog.moe"><img src="https://avatars.githubusercontent.com/u/46120251?v=4?s=100" width="100px;" alt="城倉奏"/><br /><sub><b>城倉奏</b></sub></a><br /><a href="#example-shirokurakana" title="Examples">💡</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://skipm4.com"><img src="https://avatars.githubusercontent.com/u/40311581?v=4?s=100" width="100px;" alt="SkipM4"/><br /><sub><b>SkipM4</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=SkipM4" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/leaf7th"><img src="https://avatars.githubusercontent.com/u/38352552?v=4?s=100" width="100px;" alt="Nook"/><br /><sub><b>Nook</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=leaf7th" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jiangzhuochi"><img src="https://avatars.githubusercontent.com/u/50538375?v=4?s=100" width="100px;" alt="Jocky Chiang"/><br /><sub><b>Jocky Chiang</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=jiangzhuochi" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cleoold"><img src="https://avatars.githubusercontent.com/u/13920903?v=4?s=100" width="100px;" alt="midori"/><br /><sub><b>midori</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=cleoold" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.2yo.cc"><img src="https://avatars.githubusercontent.com/u/41198038?v=4?s=100" width="100px;" alt="Pretty9"/><br /><sub><b>Pretty9</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=Pretty9" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://nocilol.me/"><img src="https://avatars.githubusercontent.com/u/16256221?v=4?s=100" width="100px;" alt="Jad"/><br /><sub><b>Jad</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/issues?q=author%3Ajourney-ad" title="Bug reports">🐛</a> <a href="#ideas-journey-ad" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://nanoka.top"><img src="https://avatars.githubusercontent.com/u/31837214?v=4?s=100" width="100px;" alt="Yumine Sakura"/><br /><sub><b>Yumine Sakura</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=asadahimeka" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/yeyang52"><img src="https://avatars.githubusercontent.com/u/107110851?v=4?s=100" width="100px;" alt="yeyang"/><br /><sub><b>yeyang</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=yeyang52" title="Code">💻</a></td>
+    </tr>
+  </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 _本段符合 [all-contributors](https://github.com/all-contributors/all-contributors) 规范_
 
-## 联系方式
-
-- 邮箱: <admin@obfs.dev>
-
 ## 开源许可
 
     Copyright 2020-2021 Mix Technology
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
@@ -173,7 +193,8 @@
         http://www.apache.org/licenses/LICENSE-2.0
 
     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
+
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/bilibili/api/base.py` & `HibiAPI-0.8.0/hibiapi/api/bilibili/api/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,185 +2,140 @@
 import json
 from enum import Enum, IntEnum
 from time import time
 from typing import Any, Dict, Optional, overload
 
 from httpx import URL
 
-from hibiapi.utils.cache import disable_cache
+from hibiapi.api.bilibili.constants import BilibiliConstants
+from hibiapi.utils.decorators import enum_auto_doc
 from hibiapi.utils.net import catch_network_error
-from hibiapi.utils.routing import BaseEndpoint
-
-from ..constants import BilibiliConstants
+from hibiapi.utils.routing import BaseEndpoint, dont_route
 
 
+@enum_auto_doc
 class TimelineType(str, Enum):
-    """
-    番剧时间线类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | global  | 番剧 |
-    | cn  | 国产动画 |
-    """
+    """番剧时间线类型"""
 
     CN = "cn"
+    """国产动画"""
     GLOBAL = "global"
+    """番剧"""
 
 
+@enum_auto_doc
 class CommentSortType(IntEnum):
-    """
-    评论排序类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | 0 | 按时间 |
-    | 1 | 按热评 |
-    | 2 | 按点赞 |
-    """
+    """评论排序类型"""
 
     LIKES = 2
+    """按点赞"""
     HOT = 1
+    """按热评"""
     TIME = 0
+    """按时间"""
 
 
+@enum_auto_doc
 class CommentType(IntEnum):
-    """
-    评论来源类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | 1 | 视频 |
-    | 12 | 文章 |
-    | 11 | 含图片的动态 |
-    | 17 | 不含图片的动态 |
-    | 14 | 音乐 |
-    | 19 | 歌单 |
-    """
+    """评论来源类型"""
 
     VIDEO = 1
+    """视频"""
     ARTICLE = 12
+    """文章"""
     DYNAMIC_PICTURE = 11
+    """含图片的动态"""
     DYNAMIC_TEXT = 17
+    """不含图片的动态"""
     AUDIO = 14
+    """音乐"""
     AUDIO_LIST = 19
+    """歌单"""
 
 
+@enum_auto_doc
 class VideoQualityType(IntEnum):
-    """
-    视频质量类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | 6 | 240P |
-    | 16 | 360P |
-    | 32 | 480P |
-    | 64 | 720P |
-    | 74 | 720P 60FPS |
-    | 80 | 1080P |
-    | 112 | 1080P+ |
-    | 116 | 1080P 60FPS |
-    | 120 | 4K |
-    """
+    """视频质量类型"""
 
     VIDEO_240P = 6
     VIDEO_360P = 16
     VIDEO_480P = 32
     VIDEO_720P = 64
     VIDEO_720P_60FPS = 74
     VIDEO_1080P = 80
     VIDEO_1080P_PLUS = 112
     VIDEO_1080P_60FPS = 116
     VIDEO_4K = 120
 
 
+@enum_auto_doc
 class VideoFormatType(IntEnum):
-    """
-    视频格式类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | 0 | FLV |
-    | 2 | MP4 |
-    | 16 | DASH |
-    """
+    """视频格式类型"""
 
     FLV = 0
     MP4 = 2
     DASH = 16
 
 
+@enum_auto_doc
 class RankBangumiType(str, Enum):
-    """
-    番剧排行榜类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | global  | 番剧 |
-    | cn  | 国产动画 |
-    """
+    """番剧排行榜类型"""
 
     CN = "cn"
+    """国产动画"""
     GLOBAL = "global"
+    """番剧"""
 
 
+@enum_auto_doc
 class RankContentType(IntEnum):
-    """
-    视频排行榜内容类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | 0  | 全站 |
-    | 1  | 动画 |
-    | 168  | 国创相关 |
-    | 3  | 音乐 |
-    | 129  | 舞蹈 |
-    | 4  | 游戏 |
-    | 36  | 科技 |
-    | 160  | 生活 |
-    | 119  | 鬼畜 |
-    | 155  | 时尚 |
-    | 165  | 广告 |
-    | 5  | 娱乐 |
-    | 23  | 电影 |
-    | 11  | 电视剧 |
-    """
+    """视频排行榜内容类型"""
 
     FULL_SITE = 0
+    """全站"""
     DOUGA = 1
+    """动画"""
     GUOCHUANG = 168
+    """国创相关"""
     MUSIC = 3
+    """音乐"""
     DANCE = 129
+    """舞蹈"""
     GAME = 4
+    """游戏"""
     TECHNOLOGY = 36
+    """科技"""
     LIFE = 160
+    """生活"""
     KICHIKU = 119
+    """鬼畜"""
     FASHION = 155
+    """时尚"""
     INFORMATION = 165
+    """广告"""
     ENT = 5
+    """娱乐"""
     MOVIE = 23
+    """电影"""
     TV = 11
+    """电视剧"""
 
 
+@enum_auto_doc
 class RankDurationType(IntEnum):
-    """
-    排行榜时间段类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | 1  | 日排行 |
-    | 3  | 三日排行 |
-    | 7  | 周排行 |
-    | 30  | 月排行 |
-    """
+    """排行榜时间段类型"""
 
     DAILY = 1
+    """日排行"""
     THREE_DAY = 3
+    """三日排行"""
     WEEKLY = 7
+    """周排行"""
     MONTHLY = 30
+    """月排行"""
 
 
 class BaseBilibiliEndpoint(BaseEndpoint):
     def _sign(self, base: str, endpoint: str, params: Dict[str, Any]) -> URL:
         params.update(
             {
                 **BilibiliConstants.DEFAULT_PARAMS,
@@ -192,15 +147,14 @@
         params = {k: params[k] for k in sorted(params.keys())}
         url = self._join(base=base, endpoint=endpoint, params=params)
         params["sign"] = hashlib.md5(url.query + BilibiliConstants.SECRET).hexdigest()
         return URL(url, params=params)
 
     @staticmethod
     def _parse_json(content: str) -> Dict[str, Any]:
-        content = content.replace("http:", "https:")
         try:
             return json.loads(content)
         except json.JSONDecodeError:
             # NOTE: this is used to parse jsonp response
             right, left = content.find("("), content.rfind(")")
             return json.loads(content[right + 1 : left].strip())
 
@@ -221,29 +175,27 @@
         source: str,
         *,
         sign: bool = True,
         params: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
         ...
 
-    @disable_cache
+    @dont_route
     @catch_network_error
     async def request(
         self,
         endpoint: str,
         source: Optional[str] = None,
         *,
         sign: bool = True,
         params: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
         host = BilibiliConstants.SERVER_HOST[source or "app"]
-        url = (
-            self._join(base=host, endpoint=endpoint, params=params or {})
-            if not sign
-            else self._sign(base=host, endpoint=endpoint, params=params or {})
+        url = (self._sign if sign else self._join)(
+            base=host, endpoint=endpoint, params=params or {}
         )
         response = await self.client.get(url)
         response.raise_for_status()
         return self._parse_json(response.text)
 
     async def playurl(
         self,
@@ -321,14 +273,15 @@
                 "ps": pagesize,
                 "pn": page,
             },
         )
 
     async def favorite_video(
         self,
+        *,
         fid: int,
         vmid: int,
         page: int = 1,
         pagesize: int = 20,
     ):
         return await self.request(
             "x/v2/fav/video",
@@ -451,15 +404,15 @@
             "api",
             sign=False,
             params={
                 "type": "json",
             },
         )
 
-    async def timeline(self, type: TimelineType = TimelineType.GLOBAL):
+    async def timeline(self, *, type: TimelineType = TimelineType.GLOBAL):
         return await self.request(
             "web_api/timeline_{type}",
             "bgm",
             sign=False,
             params={
                 "type": type,
             },
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/bilibili/api/v2.py` & `HibiAPI-0.8.0/hibiapi/api/bilibili/api/v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from enum import Enum
 from functools import wraps
 from typing import Callable, Coroutine, Optional, TypeVar, Union
 
-from hibiapi.utils.exceptions import ClientSideException
-from hibiapi.utils.net import AsyncHTTPClient
-from hibiapi.utils.routing import BaseEndpoint
-
-from .base import (
+from hibiapi.api.bilibili.api.base import (
     BaseBilibiliEndpoint,
     CommentSortType,
     CommentType,
     RankBangumiType,
     RankContentType,
     RankDurationType,
     TimelineType,
     VideoFormatType,
     VideoQualityType,
 )
+from hibiapi.utils.decorators import enum_auto_doc
+from hibiapi.utils.exceptions import ClientSideException
+from hibiapi.utils.net import AsyncHTTPClient
+from hibiapi.utils.routing import BaseEndpoint
 
 _AnyCallable = TypeVar("_AnyCallable", bound=Callable[..., Coroutine])
 
 
 def process_keyerror(function: _AnyCallable) -> _AnyCallable:
     @wraps(function)
     async def wrapper(*args, **kwargs):
@@ -28,44 +28,37 @@
             return await function(*args, **kwargs)
         except (KeyError, IndexError) as e:
             raise ClientSideException(detail=str(e)) from None
 
     return wrapper  # type:ignore
 
 
-class V2EndpointsType(str, Enum):
-    playurl = "playurl"
-    seasoninfo = "seasoninfo"
-    source = "source"
-    seasonrecommend = "seasonrecommend"
-    comments = "comments"
-    search = "search"
-    rank = "rank"
-    typedynamic = "typedynamic"
-    recommend = "recommend"
-    timeline = "timeline"
-    space = "space"
-    archive = "archive"
-    favlist = "favlist"
-
-
+@enum_auto_doc
 class SearchType(str, Enum):
+    """搜索类型"""
+
     search = "search"
+    """综合搜索"""
+
     suggest = "suggest"
+    """搜索建议"""
+
     hot = "hot"
+    """热门"""
 
 
-class BilibiliEndpointV2(BaseEndpoint):
+class BilibiliEndpointV2(BaseEndpoint, cache_endpoints=False):
     def __init__(self, client: AsyncHTTPClient):
         super().__init__(client)
         self.base = BaseBilibiliEndpoint(client)
 
     @process_keyerror
     async def playurl(
         self,
+        *,
         aid: int,
         page: Optional[int] = None,
         quality: VideoQualityType = VideoQualityType.VIDEO_480P,
         type: VideoFormatType = VideoFormatType.MP4,
     ):  # NOTE: not completely same with origin
         video_view = await self.base.view(aid=aid)
         if page is None:
@@ -92,15 +85,15 @@
         self,
         *,
         aid: Optional[int] = None,
         season_id: Optional[int] = None,
         index: Optional[int] = None,
         sort: CommentSortType = CommentSortType.TIME,
         page: int = 1,
-        pagesize: int = 20
+        pagesize: int = 20,
     ):  # NOTE: not same with origin
         if season_id is not None:
             assert index is not None, "parameter 'index' is required"
             season_info = await self.base.season_info(season_id=season_id)
             oid = season_info["result"]["episodes"][index - 1]["av_id"]
         elif aid is not None:
             oid = aid
@@ -117,15 +110,15 @@
     async def search(
         self,
         *,
         keyword: str = "",
         type: SearchType = SearchType.search,
         page: int = 1,
         pagesize: int = 20,
-        limit: int = 50
+        limit: int = 50,
     ):
         if type == SearchType.suggest:
             return await self.base.search_suggest(keyword=keyword)
         elif type == SearchType.hot:
             return await self.base.search_hot(limit=limit)
         else:
             return await self.base.search(
@@ -135,15 +128,15 @@
             )
 
     async def rank(
         self,
         *,
         content: Union[RankContentType, RankBangumiType] = RankContentType.FULL_SITE,
         duration: RankDurationType = RankDurationType.THREE_DAY,
-        new: bool = True
+        new: bool = True,
     ):
         if isinstance(content, int):
             return await self.base.rank_list(
                 content=content,
                 duration=duration,
                 new=new,
             )
@@ -167,21 +160,21 @@
     async def space(self, *, vmid: int, page: int = 1, pagesize: int = 10):
         return await self.base.space(
             vmid=vmid,
             page=page,
             pagesize=pagesize,
         )
 
-    async def archive(self, vmid: int, page: int = 1, pagesize: int = 10):
+    async def archive(self, *, vmid: int, page: int = 1, pagesize: int = 10):
         return await self.base.space_archive(
             vmid=vmid,
             page=page,
             pagesize=pagesize,
         )
 
-    async def favlist(self, fid: int, vmid: int, page: int = 1, pagesize: int = 20):
+    async def favlist(self, *, fid: int, vmid: int, page: int = 1, pagesize: int = 20):
         return await self.base.favorite_video(
             fid=fid,
             vmid=vmid,
             page=page,
             pagesize=pagesize,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/bilibili/constants.py` & `HibiAPI-0.8.0/hibiapi/api/bilibili/constants.py`

 * *Files identical despite different names*

### Comparing `HibiAPI-0.7.7/hibiapi/api/netease/api.py` & `HibiAPI-0.8.0/hibiapi/api/netease/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,86 @@
 import base64
 import json
-from enum import Enum, IntEnum
+import secrets
+import string
+from datetime import timedelta
+from enum import IntEnum
 from ipaddress import IPv4Address
 from random import randint
-from secrets import token_urlsafe
 from typing import Any, Dict, List, Optional
 
 from Cryptodome.Cipher import AES
 from Cryptodome.Util.Padding import pad
+from fastapi import Query
 
-from hibiapi.utils.cache import disable_cache
+from hibiapi.api.netease.constants import NeteaseConstants
+from hibiapi.utils.cache import cache_config
+from hibiapi.utils.decorators import enum_auto_doc
 from hibiapi.utils.exceptions import UpstreamAPIException
 from hibiapi.utils.net import catch_network_error
-from hibiapi.utils.routing import BaseEndpoint
-
-from .constants import NeteaseConstants
-
-
-class EndpointsType(str, Enum):
-    search = "search"
-    artist = "artist"
-    album = "album"
-    detail = "detail"
-    song = "song"
-    playlist = "playlist"
-    lyric = "lyric"
-    mv = "mv"
-    comments = "comments"
-    record = "record"
-    djradio = "djradio"
-    dj = "dj"
-    detail_dj = "detail_dj"
-    user = "user"
-    user_playlist = "user_playlist"
+from hibiapi.utils.routing import BaseEndpoint, dont_route
 
 
+@enum_auto_doc
 class SearchType(IntEnum):
-    """
-    搜索内容类型
-
-    | **数值** | **含义** |
-    |---|---|
-    | 1  | 单曲 |
-    | 10  | 专辑 |
-    | 100  | 歌手 |
-    | 1000  | 歌单 |
-    | 1002  | 用户 |
-    | 1004  | mv |
-    | 1006  | 歌词 |
-    | 1009  | 主播电台 |
-    """
+    """搜索内容类型"""
 
     SONG = 1
+    """单曲"""
     ALBUM = 10
+    """专辑"""
     ARTIST = 100
+    """歌手"""
     PLAYLIST = 1000
+    """歌单"""
     USER = 1002
+    """用户"""
     MV = 1004
+    """MV"""
     LYRICS = 1006
+    """歌词"""
     DJ = 1009
+    """主播电台"""
     VIDEO = 1014
+    """视频"""
 
 
+@enum_auto_doc
 class BitRateType(IntEnum):
-    """
-    歌曲码率
-    """
+    """歌曲码率"""
 
     LOW = 64000
     MEDIUM = 128000
     STANDARD = 198000
     HIGH = 320000
 
 
-class RecordPeriodType(IntEnum):
-    """
-    听歌记录时段类型
+@enum_auto_doc
+class MVResolutionType(IntEnum):
+    """MV分辨率"""
+
+    QVGA = 240
+    VGA = 480
+    HD = 720
+    FHD = 1080
+
 
-    | **数值** | **含义** |
-    |---|---|
-    | 0 | 所有时段 |
-    | 1 | 本周 |
-    """
+@enum_auto_doc
+class RecordPeriodType(IntEnum):
+    """听歌记录时段类型"""
 
     WEEKLY = 1
+    """本周"""
     ALL = 0
+    """所有时段"""
 
 
 class _EncryptUtil:
+    alphabets = bytearray(ord(char) for char in string.ascii_letters + string.digits)
+
     @staticmethod
     def _aes(data: bytes, key: bytes) -> bytes:
         data = pad(data, 16) if len(data) % 16 else data
         return base64.encodebytes(
             AES.new(
                 key=key,
                 mode=AES.MODE_CBC,
@@ -106,53 +95,57 @@
             exp=NeteaseConstants.RSA_PUBKEY,
             mod=NeteaseConstants.RSA_MODULUS,
         )
         return f"{result:0>256x}"
 
     @classmethod
     def encrypt(cls, data: Dict[str, Any]) -> Dict[str, str]:
-        secret = token_urlsafe(12).encode()
+        secret = bytes(secrets.choice(cls.alphabets) for _ in range(16))
         secure_key = cls._rsa(bytes(reversed(secret)))
         return {
             "params": cls._aes(
                 data=cls._aes(
                     data=json.dumps(data).encode(),
                     key=NeteaseConstants.AES_KEY,
                 ),
                 key=secret,
             ).decode("ascii"),
             "encSecKey": secure_key,
         }
 
 
 class NeteaseEndpoint(BaseEndpoint):
-    @disable_cache
+    def _construct_headers(self):
+        headers = self.client.headers.copy()
+        headers["X-Real-IP"] = str(
+            IPv4Address(
+                randint(
+                    int(NeteaseConstants.SOURCE_IP_SEGMENT.network_address),
+                    int(NeteaseConstants.SOURCE_IP_SEGMENT.broadcast_address),
+                )
+            )
+        )
+        return headers
+
+    @dont_route
     @catch_network_error
     async def request(
         self, endpoint: str, *, params: Optional[Dict[str, Any]] = None
     ) -> Dict[str, Any]:
-        params = {**(params or {}), "csrf_token": ""}
-        headers = {
-            "x-real-ip": str(  # random a ip address from a specificed network segment
-                IPv4Address(
-                    randint(
-                        int(NeteaseConstants.SOURCE_IP_SEGMENT.network_address),
-                        int(NeteaseConstants.SOURCE_IP_SEGMENT.broadcast_address),
-                    )
-                )
-            ),
-            **NeteaseConstants.DEFAULT_HEADERS,
+        params = {
+            **(params or {}),
+            "csrf_token": self.client.cookies.get("__csrf", ""),
         }
         response = await self.client.post(
             self._join(
                 NeteaseConstants.HOST,
                 endpoint=endpoint,
                 params=params,
             ),
-            headers=headers,
+            headers=self._construct_headers(),
             data=_EncryptUtil.encrypt(params),
         )
         response.raise_for_status()
         if not response.text.strip():
             raise UpstreamAPIException(
                 f"Upstream API {endpoint=} returns blank content"
             )
@@ -163,15 +156,15 @@
         *,
         s: str,
         search_type: SearchType = SearchType.SONG,
         limit: int = 20,
         offset: int = 0,
     ):
         return await self.request(
-            "weapi/cloudsearch/get/web",
+            "api/cloudsearch/pc",
             params={
                 "s": s,
                 "type": search_type,
                 "limit": limit,
                 "offset": offset,
                 "total": True,
             },
@@ -189,29 +182,35 @@
         return await self.request(
             "weapi/v1/album/{album_id}",
             params={
                 "album_id": id,
             },
         )
 
-    async def detail(self, *, id: List[int]):
+    async def detail(self, *, id: List[int] = Query()):
         return await self.request(
-            "weapi/v3/song/detail",
+            "api/v3/song/detail",
             params={
                 "c": json.dumps(
                     [{"id": str(i)} for i in id],
                 ),
             },
         )
 
-    async def song(self, *, id: List[int], br: BitRateType = BitRateType.STANDARD):
+    @cache_config(ttl=timedelta(minutes=20))
+    async def song(
+        self,
+        *,
+        id: List[int] = Query(),
+        br: BitRateType = BitRateType.STANDARD,
+    ):
         return await self.request(
             "weapi/song/enhance/player/url",
             params={
-                "ids": id,
+                "ids": [str(i) for i in id],
                 "br": br,
             },
         )
 
     async def playlist(self, *, id: int):
         return await self.request(
             "weapi/v6/playlist/detail",
@@ -240,14 +239,28 @@
         return await self.request(
             "api/v1/mv/detail",
             params={
                 "id": id,
             },
         )
 
+    async def mv_url(
+        self,
+        *,
+        id: int,
+        res: MVResolutionType = MVResolutionType.FHD,
+    ):
+        return await self.request(
+            "weapi/song/enhance/play/mv/url",
+            params={
+                "id": id,
+                "r": res,
+            },
+        )
+
     async def comments(self, *, id: int, offset: int = 0, limit: int = 1):
         return await self.request(
             "weapi/v1/resource/comments/R_SO_4_{song_id}",
             params={
                 "song_id": id,
                 "offset": offset,
                 "total": True,
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/netease/constants.py` & `HibiAPI-0.8.0/hibiapi/api/netease/constants.py`

 * *Files identical despite different names*

### Comparing `HibiAPI-0.7.7/hibiapi/api/pixiv/constants.py` & `HibiAPI-0.8.0/hibiapi/api/pixiv/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 
 from hibiapi.utils.config import APIConfig
 
 
 class PixivConstants:
     DEFAULT_HEADERS: Dict[str, Any] = {
         "App-OS": "ios",
-        "App-OS-Version": "12.2",
-        "App-Version": "7.6.2",
-        "User-Agent": "PixivIOSApp/7.6.2 (iOS 12.2; iPhone9,1)",
+        "App-OS-Version": "14.6",
+        "User-Agent": "PixivIOSApp/7.13.3 (iOS 14.6; iPhone13,2)",
     }
     CLIENT_ID: str = "MOBrBDS8blbauoSck0ZfDbtuzpyT"
     CLIENT_SECRET: str = "lsACyCD94FhDUtGTXi3QzcFE2uU1hqtDaKeqrdwj"
     HASH_SECRET: bytes = (
         b"28c1fdd170a5204386cb1313c7077b34f83e4aaf4aa829ce78c231e05b0bae2c"
     )
     CONFIG: APIConfig = APIConfig("pixiv")
-    REFRESH_INTERVAL: int = CONFIG["account"]["refresh-interval"].as_number()
     APP_HOST: str = "https://app-api.pixiv.net"
-    PUB_HOST: str = "https://public-api.secure.pixiv.net"
     AUTH_HOST: str = "https://oauth.secure.pixiv.net"
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/pixiv/net.py` & `HibiAPI-0.8.0/hibiapi/api/pixiv/net.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import asyncio
 import hashlib
-from datetime import datetime
-from typing import Dict
+from datetime import datetime, timedelta, timezone
+from itertools import cycle
+from typing import Dict, List
 
 from httpx import URL
 from pydantic import BaseModel, Extra, Field
 
-from hibiapi.utils.net import AsyncHTTPClient, BaseNetClient
+from hibiapi.utils.log import logger
+from hibiapi.utils.net import BaseNetClient
 
 from .constants import PixivConstants
 
 
 class AccountDataModel(BaseModel):
     class Config:
         extra = Extra.allow
@@ -26,46 +29,58 @@
 class PixivAuthData(AccountDataModel):
     time: datetime = Field(default_factory=datetime.now)
     expires_in: int
     access_token: str
     refresh_token: str
     user: PixivUserData
 
-    @classmethod
-    async def login(cls, *, refresh_token: str):
+
+class NetRequest(BaseNetClient):
+    def __init__(self, tokens: List[str]):
+        super().__init__(
+            headers=PixivConstants.DEFAULT_HEADERS.copy(),
+            proxies=PixivConstants.CONFIG["proxy"].as_dict(),
+        )
+        self.user_tokens = cycle(tokens)
+        self.auth_lock = asyncio.Lock()
+        self.user_tokens_dict: Dict[str, PixivAuthData] = {}
+        self.headers["accept-language"] = PixivConstants.CONFIG["language"].as_str()
+
+    def get_available_user(self):
+        token = next(self.user_tokens)
+        if (auth_data := self.user_tokens_dict.get(token)) and (
+            auth_data.time + timedelta(minutes=1, seconds=auth_data.expires_in)
+            > datetime.now()
+        ):
+            return auth_data, token
+        return None, token
+
+    async def auth(self, refresh_token: str):
         url = URL(PixivConstants.AUTH_HOST).join("/auth/token")
-        time = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S+00:00")
+        time = datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%S+00:00")
         headers = {
-            **PixivConstants.DEFAULT_HEADERS,
+            **self.headers,
             "X-Client-Time": time,
             "X-Client-Hash": hashlib.md5(
                 time.encode() + PixivConstants.HASH_SECRET
             ).hexdigest(),
         }
-        data = {
+        payload = {
             "get_secure_url": 1,
             "client_id": PixivConstants.CLIENT_ID,
             "client_secret": PixivConstants.CLIENT_SECRET,
             "grant_type": "refresh_token",
             "refresh_token": refresh_token,
         }
 
-        async with AsyncHTTPClient(
-            proxies=PixivConstants.CONFIG["proxy"].get(Dict[str, str])  # type:ignore
-        ) as client:
-            response = await client.post(url, data=data, headers=headers)
+        async with self as client:
+            response = await client.post(url, data=payload, headers=headers)
             response.raise_for_status()
-        return cls.parse_obj(response.json())
 
-    async def renew(self) -> "PixivAuthData":
-        return await self.login(refresh_token=self.refresh_token)
-
-
-class NetRequest(BaseNetClient):
-    def __init__(self, user: PixivAuthData):
-        super().__init__(
-            headers=PixivConstants.DEFAULT_HEADERS.copy(),
-            proxies=PixivConstants.CONFIG["proxy"].as_dict(),
+        self.user_tokens_dict[refresh_token] = PixivAuthData.parse_obj(response.json())
+        user_data = self.user_tokens_dict[refresh_token].user
+        logger.opt(colors=True).info(
+            f"Pixiv account <m>{user_data.id}</m> info <b>Updated</b>: "
+            f"<b><e>{user_data.name}</e>({user_data.account})</b>."
         )
-        self.user = user
-        self.headers["accept-language"] = PixivConstants.CONFIG["language"].as_str()
-        self.headers["authorization"] = f"Bearer {self.user.access_token}"
+
+        return self.user_tokens_dict[refresh_token]
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/qrcode.py` & `HibiAPI-0.8.0/hibiapi/api/qrcode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,84 @@
 from datetime import datetime
 from enum import Enum
 from io import BytesIO
+from os import fdopen
 from pathlib import Path
-from typing import List, Literal, Optional
+from typing import List, Literal, Optional, cast
 
-from PIL import Image  # type:ignore
-from pydantic import AnyHttpUrl, BaseModel, Field, conint, validate_arguments
+from PIL import Image
+from pydantic import AnyHttpUrl, BaseModel, Field, validate_arguments
 from pydantic.color import Color
-from qrcode import QRCode, constants  # type:ignore
-from qrcode.image.pil import PilImage  # type:ignore
+from qrcode import QRCode, constants
+from qrcode.image.pil import PilImage
 
 from hibiapi.utils.config import APIConfig
-from hibiapi.utils.decorators import ToAsync
+from hibiapi.utils.decorators import ToAsync, enum_auto_doc
 from hibiapi.utils.exceptions import ClientSideException
 from hibiapi.utils.net import BaseNetClient
 from hibiapi.utils.routing import BaseHostUrl
 from hibiapi.utils.temp import TempFile
 
 Config = APIConfig("qrcode")
 
 
 class HostUrl(BaseHostUrl):
     allowed_hosts = Config["qrcode"]["icon-site"].get(List[str])
 
 
+@enum_auto_doc
 class QRCodeLevel(str, Enum):
-    L = "L"
-    M = "M"
-    Q = "Q"
-    H = "H"
+    """二维码容错率"""
 
+    LOW = "L"
+    """最低容错率"""
+    MEDIUM = "M"
+    """中等容错率"""
+    QUARTILE = "Q"
+    """高容错率"""
+    HIGH = "H"
+    """最高容错率"""
 
+
+@enum_auto_doc
 class ReturnEncode(str, Enum):
+    """二维码返回的编码方式"""
+
     raw = "raw"
+    """直接重定向到二维码图片"""
     json = "json"
+    """返回JSON格式的二维码信息"""
     js = "js"
     jsc = "jsc"
 
 
 class QRInfo(BaseModel):
     url: Optional[AnyHttpUrl] = None
     path: Path
     time: datetime = Field(default_factory=datetime.now)
     data: str
     logo: Optional[HostUrl] = None
-    level: QRCodeLevel = QRCodeLevel.M
-    size: int = 200  # type:ignore
+    level: QRCodeLevel = QRCodeLevel.MEDIUM
+    size: int = 200
     code: Literal[0] = 0
     status: Literal["success"] = "success"
 
     @classmethod
     @validate_arguments
     async def new(
         cls,
         text: str,
         *,
-        size: conint(  # type:ignore
-            strict=True,
-            gt=Config["qrcode"]["min-size"].as_number(),  # noqa:F821
-            lt=Config["qrcode"]["max-size"].as_number(),  # noqa:F821
-        ) = 200,
+        size: int = Field(
+            200,
+            gt=Config["qrcode"]["min-size"].as_number(),
+            lt=Config["qrcode"]["max-size"].as_number(),
+        ),
         logo: Optional[HostUrl] = None,
-        level: QRCodeLevel = QRCodeLevel.M,
+        level: QRCodeLevel = QRCodeLevel.MEDIUM,
         bgcolor: Color = Color("FFFFFF"),
         fgcolor: Color = Color("000000"),
     ):
         icon_stream = None
         if logo is not None:
             async with BaseNetClient() as client:
                 response = await client.get(
@@ -91,35 +104,38 @@
     @classmethod
     @ToAsync
     def _generate(
         cls,
         text: str,
         *,
         size: int = 200,
-        level: QRCodeLevel = QRCodeLevel.M,
+        level: QRCodeLevel = QRCodeLevel.MEDIUM,
         icon_stream: Optional[BytesIO] = None,
         bgcolor: str = "#FFFFFF",
         fgcolor: str = "#000000",
     ) -> Path:
         qr = QRCode(
             error_correction={
-                QRCodeLevel.L: constants.ERROR_CORRECT_L,
-                QRCodeLevel.M: constants.ERROR_CORRECT_M,
-                QRCodeLevel.Q: constants.ERROR_CORRECT_Q,
-                QRCodeLevel.H: constants.ERROR_CORRECT_H,
+                QRCodeLevel.LOW: constants.ERROR_CORRECT_L,
+                QRCodeLevel.MEDIUM: constants.ERROR_CORRECT_M,
+                QRCodeLevel.QUARTILE: constants.ERROR_CORRECT_Q,
+                QRCodeLevel.HIGH: constants.ERROR_CORRECT_H,
             }[level],
             border=2,
             box_size=8,
         )
         qr.add_data(text)
-        image: Image.Image = qr.make_image(
-            PilImage,
-            back_color=bgcolor,
-            fill_color=fgcolor,
-        ).get_image()  # type:ignore
+        image = cast(
+            Image.Image,
+            qr.make_image(
+                PilImage,
+                back_color=bgcolor,
+                fill_color=fgcolor,
+            ).get_image(),
+        )
         image = image.resize((size, size))
         if icon_stream is not None:
             try:
                 icon = Image.open(icon_stream)
             except ValueError as e:
                 raise ClientSideException("Invalid image format.") from e
             icon_width, icon_height = icon.size
@@ -129,9 +145,11 @@
                     int(size / 2 - icon_width / 2),
                     int(size / 2 - icon_height / 2),
                     int(size / 2 + icon_width / 2),
                     int(size / 2 + icon_height / 2),
                 ),
                 mask=icon if icon.mode == "RGBA" else None,
             )
-        image.save(file := TempFile.create(ext=".png"))
-        return file
+        descriptor, path = TempFile.create(".png")
+        with fdopen(descriptor, "wb") as f:
+            image.save(f, format="PNG")
+        return path
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/sauce/api.py` & `HibiAPI-0.8.0/hibiapi/api/sauce/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import random
 from enum import IntEnum
 from io import BytesIO
 from typing import Any, Dict, Optional, overload
 
 from httpx import HTTPError
 
-from hibiapi.utils.cache import disable_cache
+from hibiapi.api.sauce.constants import SauceConstants
+from hibiapi.utils.decorators import enum_auto_doc
 from hibiapi.utils.exceptions import ClientSideException
 from hibiapi.utils.net import catch_network_error
 from hibiapi.utils.routing import BaseEndpoint, BaseHostUrl
 
-from .constants import SauceConstants
-
 
 class UnavailableSourceException(ClientSideException):
     code = 422
     detail = "given image is not avaliable to fetch"
 
 
 class ImageSourceOversizedException(UnavailableSourceException):
@@ -38,28 +37,25 @@
     @classmethod
     def validate(cls, v: Any) -> BytesIO:
         if not isinstance(v, BytesIO):
             raise ValueError(f"Expected UploadFile, received: {type(v)}")
         return v
 
 
+@enum_auto_doc
 class DeduplicateType(IntEnum):
-    """
-    0=no result deduping
-    1=consolidate booru results and dedupe by item identifier
-    2=all implemented dedupe methods such as by series name.
-    Default is 2, more levels may be added in future.
-    """
-
     DISABLED = 0
+    """no result deduplicating"""
     IDENTIFIER = 1
+    """consolidate search results and deduplicate by item identifier"""
     ALL = 2
+    """all implemented deduplicate methods such as by series name"""
 
 
-class SauceEndpoint(BaseEndpoint):
+class SauceEndpoint(BaseEndpoint, cache_endpoints=False):
     base = "https://saucenao.com"
 
     async def fetch(self, host: HostUrl) -> UploadFileIO:
         try:
             response = await self.client.get(
                 url=host,
                 headers=SauceConstants.IMAGE_HEADERS,
@@ -68,15 +64,14 @@
             response.raise_for_status()
             if len(response.content) > SauceConstants.IMAGE_MAXIMUM_SIZE:
                 raise ImageSourceOversizedException
             return UploadFileIO(response.content)
         except HTTPError as e:
             raise UnavailableSourceException(detail=str(e)) from e
 
-    @disable_cache
     @catch_network_error
     async def request(
         self, *, file: UploadFileIO, params: Dict[str, Any]
     ) -> Dict[str, Any]:
         response = await self.client.post(
             url=self._join(
                 self.base,
@@ -99,32 +94,31 @@
         *,
         url: HostUrl,
         size: int = 30,
         deduplicate: DeduplicateType = DeduplicateType.ALL,
         database: Optional[int] = None,
         enabled_mask: Optional[int] = None,
         disabled_mask: Optional[int] = None,
-    ):
+    ) -> Dict[str, Any]:
         ...
 
     @overload
     async def search(
         self,
         *,
         file: UploadFileIO,
         size: int = 30,
         deduplicate: DeduplicateType = DeduplicateType.ALL,
         database: Optional[int] = None,
         enabled_mask: Optional[int] = None,
         disabled_mask: Optional[int] = None,
-    ):
+    ) -> Dict[str, Any]:
         ...
 
-    @disable_cache
-    async def search(  # type:ignore
+    async def search(
         self,
         *,
         url: Optional[HostUrl] = None,
         file: Optional[UploadFileIO] = None,
         size: int = 30,
         deduplicate: DeduplicateType = DeduplicateType.ALL,
         database: Optional[int] = None,
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/sauce/constants.py` & `HibiAPI-0.8.0/hibiapi/api/sauce/constants.py`

 * *Files identical despite different names*

### Comparing `HibiAPI-0.7.7/hibiapi/api/tieba/api.py` & `HibiAPI-0.8.0/hibiapi/api/tieba/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 import hashlib
 from enum import Enum
 from random import randint
 from typing import Any, Dict, Optional
 
-from hibiapi.utils.cache import disable_cache
 from hibiapi.utils.config import APIConfig
 from hibiapi.utils.net import catch_network_error
-from hibiapi.utils.routing import BaseEndpoint
+from hibiapi.utils.routing import BaseEndpoint, dont_route
 
 Config = APIConfig("tieba")
 
 
-class EndpointsType(str, Enum):
-    post_list = "post_list"
-    post_detail = "post_detail"
-    subpost_detail = "subpost_detail"
-    user_profile = "user_profile"
-    user_subscribed = "user_subscribed"
-
-
 class TiebaSignUtils:
     salt = b"tiebaclient!!!"
 
     @staticmethod
     def random_digit(length: int) -> str:
         return "".join(map(str, [randint(0, 9) for _ in range(length)]))
 
@@ -66,15 +57,15 @@
         )
         return cls.construct_content(params)
 
 
 class TiebaEndpoint(BaseEndpoint):
     base = "http://c.tieba.baidu.com"
 
-    @disable_cache
+    @dont_route
     @catch_network_error
     async def request(
         self, endpoint: str, *, params: Optional[Dict[str, Any]] = None
     ) -> Dict[str, Any]:
         response = await self.client.post(
             url=self._join(self.base, endpoint, {}),
             content=TiebaSignUtils.sign(params or {}),
```

### Comparing `HibiAPI-0.7.7/hibiapi/api/wallpaper/api.py` & `HibiAPI-0.8.0/hibiapi/api/wallpaper/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 from datetime import timedelta
 from enum import Enum
 from typing import Any, Dict, Optional
 
-from hibiapi.utils.cache import cache_config, disable_cache
+from hibiapi.utils.cache import cache_config
 from hibiapi.utils.config import APIConfig
+from hibiapi.utils.decorators import enum_auto_doc
 from hibiapi.utils.net import catch_network_error
-from hibiapi.utils.routing import BaseEndpoint
+from hibiapi.utils.routing import BaseEndpoint, dont_route
 
 Config = APIConfig("wallpaper")
 
 
-class EndpointsType(str, Enum):
-    wallpaper = "wallpaper"
-    vertical = "vertical"
-
-
+@enum_auto_doc
 class WallpaperCategoryType(str, Enum):
-    """
-    壁纸分类
-
-    | **数值** | **含义** |
-    |---|---|
-    | girl | 女生 |
-    | animal | 动物 |
-    | landscape | 自然 |
-    | anime | 二次元 |
-    | drawn | 手绘 |
-    | mechanics | 机械 |
-    | boy | 男生 |
-    | game | 游戏 |
-    | text | 文字 |
-    """
+    """壁纸分类"""
 
     girl = "girl"
+    """女生"""
     animal = "animal"
+    """动物"""
     landscape = "landscape"
+    """自然"""
     anime = "anime"
+    """二次元"""
     drawn = "drawn"
+    """手绘"""
     mechanics = "mechanics"
+    """机械"""
     boy = "boy"
+    """男生"""
     game = "game"
+    """游戏"""
     text = "text"
+    """文字"""
 
 
 CATEGORY: Dict[WallpaperCategoryType, str] = {
     WallpaperCategoryType.girl: "4e4d610cdf714d2966000000",
     WallpaperCategoryType.animal: "4e4d610cdf714d2966000001",
     WallpaperCategoryType.landscape: "4e4d610cdf714d2966000002",
     WallpaperCategoryType.anime: "4e4d610cdf714d2966000003",
@@ -52,23 +44,28 @@
     WallpaperCategoryType.mechanics: "4e4d610cdf714d2966000005",
     WallpaperCategoryType.boy: "4e4d610cdf714d2966000006",
     WallpaperCategoryType.game: "4e4d610cdf714d2966000007",
     WallpaperCategoryType.text: "5109e04e48d5b9364ae9ac45",
 }
 
 
+@enum_auto_doc
 class WallpaperOrderType(str, Enum):
+    """壁纸排序方式"""
+
     hot = "hot"
+    """热门"""
     new = "new"
+    """最新"""
 
 
 class WallpaperEndpoint(BaseEndpoint):
     base = "http://service.aibizhi.adesk.com"
 
-    @disable_cache
+    @dont_route
     @catch_network_error
     async def request(
         self, endpoint: str, *, params: Optional[Dict[str, Any]] = None
     ) -> Dict[str, Any]:
 
         response = await self.client.get(
             self._join(
```

### Comparing `HibiAPI-0.7.7/hibiapi/app/application.py` & `HibiAPI-0.8.0/hibiapi/app/application.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import asyncio
+from ipaddress import ip_address
 from secrets import compare_digest
-from typing import List, NoReturn
+from typing import List
 from urllib.parse import ParseResult
 
 import sentry_sdk
 from fastapi import Depends, FastAPI, Request, Response
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from fastapi.staticfiles import StaticFiles
 from pydantic import BaseModel
 from sentry_sdk.integrations.logging import LoggingIntegration
 
 from hibiapi import __version__
+from hibiapi.app.routes import router as ImplRouter
+from hibiapi.utils.cache import cache
 from hibiapi.utils.config import Config
-from hibiapi.utils.exceptions import ClientSideException
+from hibiapi.utils.exceptions import ClientSideException, RateLimitReachedException
 from hibiapi.utils.log import logger
+from hibiapi.utils.net import BaseNetClient
 from hibiapi.utils.temp import TempFile
 
-from .routes import router as ImplRouter
-
 DESCRIPTION = (
     """
 **A program that implements easy-to-use APIs for a variety of commonly used sites**
 
 - *Documents*:
     - [Redoc](/docs) (Easier to read and more beautiful)
     - [Swagger UI](/docs/test) (Integrated interactive testing function)
@@ -48,15 +50,14 @@
     username: str
     password: str
 
 
 AUTHORIZATION_ENABLED = Config["authorization"]["enabled"].as_bool()
 AUTHORIZATION_ALLOWED = Config["authorization"]["allowed"].get(List[AuthorizationModel])
 
-
 security = HTTPBasic()
 
 
 async def basic_authorization_depend(
     credentials: HTTPBasicCredentials = Depends(security),
 ):
     # NOTE: We use `compare_digest` to avoid timing attacks.
@@ -69,86 +70,108 @@
     raise ClientSideException(
         f"Invalid credentials for user {credentials.username!r}",
         status_code=401,
         headers={"WWW-Authenticate": "Basic"},
     )
 
 
+RATE_LIMIT_ENABLED = Config["limit"]["enabled"].as_bool()
+RATE_LIMIT_MAX = Config["limit"]["max"].as_number()
+RATE_LIMIT_INTERVAL = Config["limit"]["interval"].as_number()
+
+
+async def rate_limit_depend(request: Request):
+    if not request.client:
+        return
+
+    try:
+        client_ip = ip_address(request.client.host)
+        client_ip_hex = client_ip.packed.hex()
+        limit_key = f"rate_limit:IPv{client_ip.version}-{client_ip_hex:x}"
+    except ValueError:
+        limit_key = f"rate_limit:fallback-{request.client.host}"
+
+    request_count: int = await cache.incr(limit_key)  # type:ignore
+    if request_count <= 1:
+        await cache.expire(limit_key, timeout=RATE_LIMIT_INTERVAL)
+    elif request_count > RATE_LIMIT_MAX:
+        limit_remain: int = await cache.get_expire(limit_key)
+        raise RateLimitReachedException(headers={"Retry-After": limit_remain})
+
+    return
+
+
 app = FastAPI(
-    debug=Config["debug"].as_bool(),
     title="HibiAPI",
     version=__version__,
     description=DESCRIPTION,
     docs_url="/docs/test",
     redoc_url="/docs",
 )
 app.include_router(
     ImplRouter,
     prefix="/api",
     dependencies=(
-        [Depends(basic_authorization_depend)] if AUTHORIZATION_ENABLED else []
+        ([Depends(basic_authorization_depend)] if AUTHORIZATION_ENABLED else [])
+        + ([Depends(rate_limit_depend)] if RATE_LIMIT_ENABLED else [])
     ),
 )
-app.mount(
-    "/temp",
-    StaticFiles(directory=str(TempFile.path), check_dir=False),
-    "Temporary file directory",
-)
+app.mount("/temp", StaticFiles(directory=TempFile.path, check_dir=False))
 
 
 @app.get("/", include_in_schema=False)
 async def redirect():
     return Response(status_code=302, headers={"Location": "/docs"})
 
 
 @app.get("/robots.txt", include_in_schema=False)
 async def robots():
     content = Config["content"]["robots"].as_str().strip()
     return Response(content, status_code=200)
 
 
-@app.on_event("startup")
-async def cleaner():
-    async def clean() -> NoReturn:
-        while True:
-            try:
-                await TempFile.clean()
-            except Exception:
-                logger.exception("Exception occurred during executing cleaning task:")
-            await asyncio.sleep(3600)
-
-    asyncio.ensure_future(clean())
-
-
 @app.on_event("shutdown")
 def flush_sentry():
     client = sentry_sdk.Hub.current.client
     if client is not None:
         client.close()
     sentry_sdk.flush()
-    logger.info("Sentry client has been closed")
+    logger.debug("Sentry client has been closed")
+
+
+@app.on_event("shutdown")
+async def cleanup_clients():
+    opened_clients = [
+        client for client in BaseNetClient.clients if not client.is_closed
+    ]
+    if opened_clients:
+        await asyncio.gather(
+            *map(lambda client: client.aclose(), opened_clients),
+            return_exceptions=True,
+        )
+    logger.debug(f"Cleaned <r>{len(opened_clients)}</r> unclosed HTTP clients")
 
 
 """
 Temporary redirection solution below for #12
 """
 
 
 def _redirect(request: Request, path: str, to: str) -> Response:
     return Response(
         status_code=301,
         headers={
             "Location": ParseResult(
                 scheme="",
                 netloc="",
-                path=path + to,
+                path=to + path,
                 params="",
                 query=str(request.query_params),
                 fragment="",
-            )
+            ).geturl()
         },
     )
 
 
 @app.get("/qrcode/{path:path}", include_in_schema=False)
 async def _qr_redirect(path: str, request: Request):
     return _redirect(request, path, "/api/qrcode/")
@@ -162,8 +185,8 @@
 @app.get("/netease/{path:path}", include_in_schema=False)
 async def _netease_redirect(path: str, request: Request):
     return _redirect(request, path, "/api/netease/")
 
 
 @app.get("/bilibili/{path:path}", include_in_schema=False)
 async def _bilibili_redirect(path: str, request: Request):
-    return _redirect(request, path, "/api/bilibili/")
+    return _redirect(request, path, "/api/bilibili/v2/")
```

### Comparing `HibiAPI-0.7.7/hibiapi/app/handlers.py` & `HibiAPI-0.8.0/hibiapi/app/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 
 @app.exception_handler(exceptions.BaseServerException)
 async def exception_handler(
     request: Request,
     exc: exceptions.BaseServerException,
 ) -> Response:
     if isinstance(exc, exceptions.UncaughtException):
-        cause = exc.exc
-        exc.data.trace = exceptions.ExceptionInfo.new(cause.__traceback__).persist().id
         logger.opt(exception=exc).exception(f"Uncaught exception raised {exc.data=}:")
+
     exc.data.url = str(request.url)  # type:ignore
     return Response(
         content=exc.data.json(),
         status_code=exc.data.code,
         headers=exc.data.headers,
         media_type="application/json",
     )
```

### Comparing `HibiAPI-0.7.7/hibiapi/app/middlewares.py` & `HibiAPI-0.8.0/hibiapi/app/middlewares.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,51 @@
 from datetime import datetime
-from typing import Any, Callable, Coroutine, List, Optional, Set
+from typing import Awaitable, Callable, List
 
 from fastapi import Request, Response
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.middleware.gzip import GZipMiddleware
+from fastapi.middleware.trustedhost import TrustedHostMiddleware
 from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
 from sentry_sdk.integrations.httpx import HttpxIntegration
 from starlette.datastructures import MutableHeaders
 
 from hibiapi.utils.config import Config
-from hibiapi.utils.exceptions import (
-    BaseServerException,
-    ClientSideException,
-    UncaughtException,
-)
+from hibiapi.utils.exceptions import BaseServerException, UncaughtException
 from hibiapi.utils.log import LoguruHandler, logger
 from hibiapi.utils.routing import request_headers, response_headers
 
 from .application import app
 from .handlers import exception_handler
 
-HttpxIntegration.setup_once()
+RequestHandler = Callable[[Request], Awaitable[Response]]
+
 
 if Config["server"]["gzip"].as_bool():
     app.add_middleware(GZipMiddleware)
 app.add_middleware(
     CORSMiddleware,
     allow_origins=Config["server"]["cors"]["origins"].get(List[str]),
     allow_credentials=Config["server"]["cors"]["credentials"].as_bool(),
     allow_methods=Config["server"]["cors"]["methods"].get(List[str]),
     allow_headers=Config["server"]["cors"]["headers"].get(List[str]),
 )
+app.add_middleware(
+    TrustedHostMiddleware,
+    allowed_hosts=Config["server"]["allowed"].get(List[str]),
+)
 app.add_middleware(SentryAsgiMiddleware)
 
-RequestHandler = Callable[[Request], Coroutine[Any, Any, Response]]
-
-ALLOWED_DOMAINS = Config["server"]["domains"].get(Optional[Set[str]])  # type: ignore
-
-
-@app.middleware("http")
-async def domain_limiter(request: Request, call_next: RequestHandler) -> Response:
-    if (ALLOWED_DOMAINS is not None) and (
-        (domain := request.url.netloc) not in ALLOWED_DOMAINS
-    ):
-        raise ClientSideException(f"{domain=} is not allowed.", code=403)
-    return await call_next(request)
+HttpxIntegration.setup_once()
 
 
 @app.middleware("http")
 async def request_logger(request: Request, call_next: RequestHandler) -> Response:
     start_time = datetime.now()
-    host, port = request.client
+    host, port = request.client or (None, None)
     response = await call_next(request)
     process_time = (datetime.now() - start_time).total_seconds() * 1000
     response_headers.get().setdefault("X-Process-Time", f"{process_time:.3f}")
     bg, fg = (
         ("green", "red")
         if response.status_code < 400
         else ("yellow", "blue")
```

### Comparing `HibiAPI-0.7.7/hibiapi/app/routes/__init__.py` & `HibiAPI-0.8.0/hibiapi/app/routes/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from typing import List, Protocol, cast
 
+from hibiapi.app.routes import (
+    bika,
+    bilibili,
+    netease,
+    pixiv,
+    qrcode,
+    sauce,
+    tieba,
+    wallpaper,
+)
 from hibiapi.utils.config import APIConfig
 from hibiapi.utils.exceptions import ExceptionReturn
 from hibiapi.utils.log import logger
 from hibiapi.utils.routing import SlashRouter
 
-from . import bilibili, netease, pixiv, qrcode, sauce, tieba, wallpaper
-
 router = SlashRouter(
     responses={
         code: {
             "model": ExceptionReturn,
         }
         for code in (400, 422, 500, 502)
     }
@@ -20,22 +28,24 @@
 class RouteInterface(Protocol):
     router: SlashRouter
     __mount__: str
     __config__: APIConfig
 
 
 modules = cast(
-    List[RouteInterface], [bilibili, netease, pixiv, qrcode, sauce, tieba, wallpaper]
+    List[RouteInterface],
+    [bilibili, netease, pixiv, qrcode, sauce, tieba, wallpaper, bika],
 )
 
 for module in modules:
     mount = (
-        mountpoint
-        if (mountpoint := module.__mount__).startswith("/")
-        else ("/" + mountpoint)
+        mount_point
+        if (mount_point := module.__mount__).startswith("/")
+        else f"/{mount_point}"
     )
+
     if not module.__config__["enabled"].as_bool():
         logger.warning(
             f"API Route <y><b>{mount}</b></y> has been <r><b>disabled</b></r> in config."
         )
         continue
     router.include_router(module.router, prefix=mount)
```

### Comparing `HibiAPI-0.7.7/hibiapi/app/routes/qrcode.py` & `HibiAPI-0.8.0/hibiapi/app/routes/qrcode.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 async def qrcode_api(
     request: Request,
     *,
     text: str,
     size: int = 200,
     logo: Optional[HostUrl] = None,
     encode: ReturnEncode = ReturnEncode.raw,
-    level: QRCodeLevel = QRCodeLevel.M,
+    level: QRCodeLevel = QRCodeLevel.MEDIUM,
     bgcolor: Color = Color("FFFFFF"),
     fgcolor: Color = Color("000000"),
     fun: str = "qrcode",
 ):
     qr = await QRInfo.new(
         text, size=size, logo=logo, level=level, bgcolor=bgcolor, fgcolor=fgcolor
     )
```

### Comparing `HibiAPI-0.7.7/hibiapi/app/routes/sauce.py` & `HibiAPI-0.8.0/hibiapi/app/routes/sauce.py`

 * *Files identical despite different names*

### Comparing `HibiAPI-0.7.7/hibiapi/configs/general.yml` & `HibiAPI-0.8.0/hibiapi/configs/general.yml`

 * *Files 18% similar despite different names*

```diff
@@ -3,43 +3,49 @@
 #  | |__| |_| |__  _   /  \  | |__) || |
 #  |  __  | | '_ \| | / /\ \ |  ___/ | |
 #  | |  | | | |_) | |/ ____ \| |    _| |_
 #  |_|  |_|_|_.__/|_/_/    \_\_|   |_____|
 #
 # An alternative implement of Imjad API
 
-debug: false # 是否开启Debug模式
-
 data:
   temp-expiry: 7 # 临时文件目录文件过期时间, 单位为天
   path: ./data # data目录所在位置
 
 server:
   host: 127.0.0.1 # 监听主机
   port: 8080 # 端口
   gzip: true
 
-  domains: null # 限定来源域名, 设置为null为不限制
+  # 限定来源域名, 支持通配符, 参考:
+  # https://fastapi.tiangolo.com/advanced/middleware/#trustedhostmiddleware
+  allowed: ["*"]
 
   cors:
     origins:
       - "http://localhost.tiangolo.com"
       - "https://localhost.tiangolo.com"
       - "http://localhost"
       - "http://localhost:8080"
     credentials: true
     methods: ["*"]
     headers: ["*"]
 
   allowed-forward: null # Reference: https://stackoverflow.com/questions/63511413
 
+limit: # 单IP速率限制策略
+  enabled: true
+  max: 60 # 每个单位时间内最大请求数
+  interval: 60 # 单位时间长度, 单位为秒
+
 cache:
   enabled: true # 设置是否启用缓存
   ttl: 3600 # 缓存默认生存时间, 单位为秒
-  uri: "memory://" # 缓存URI
+  uri: "mem://" # 缓存URI
+  controllable: true # 配置是否可以通过Cache-Control请求头刷新缓存
 
 log:
   level: INFO # 日志等级, 可选 [TRACE,DEBUG,INFO,WARNING,ERROR]
   format: > # 输出日志格式, 如果没有必要请不要修改
     <level>
     <v>{level:<8}</v>
     [{time:YYYY/MM/DD} {time:HH:mm:ss.SSS} <d>{module}:{name}:{line}</d>]</level>
```

### Comparing `HibiAPI-0.7.7/hibiapi/configs/sauce.yml` & `HibiAPI-0.8.0/hibiapi/configs/sauce.yml`

 * *Files identical despite different names*

### Comparing `HibiAPI-0.7.7/hibiapi/utils/cache.py` & `HibiAPI-0.8.0/hibiapi/utils/cache.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,136 +1,129 @@
-import base64
 import hashlib
-import pickle
-import pickletools
-import time
-import zlib
 from datetime import timedelta
 from functools import wraps
-from typing import Any, Callable, Coroutine, Dict, Optional, Tuple, TypeVar
+from typing import Any, Awaitable, Callable, Dict, Optional, Tuple, TypeVar, cast
 
-from aiocache import Cache as AioCache  # type:ignore
-from aiocache.base import BaseCache  # type:ignore
-from aiocache.serializers import BaseSerializer  # type:ignore
+from cashews import Cache
 from pydantic import BaseModel
 from pydantic.decorator import ValidatedFunction
 
 from .config import Config
 from .log import logger
 
+CACHE_CONFIG_KEY = "_cache_config"
+
+AsyncFunc = Callable[..., Awaitable[Any]]
+T_AsyncFunc = TypeVar("T_AsyncFunc", bound=AsyncFunc)
+
+
 CACHE_ENABLED = Config["cache"]["enabled"].as_bool()
 CACHE_DELTA = timedelta(seconds=Config["cache"]["ttl"].as_number())
 CACHE_URI = Config["cache"]["uri"].as_str()
+CACHE_CONTROLLABLE = Config["cache"]["controllable"].as_bool()
 
-T_AsyncFunc = TypeVar("T_AsyncFunc", bound=Callable[..., Coroutine])
-
-
-class GZippedBase85Serializer(BaseSerializer):
-    def dumps(self, value: Any) -> str:
-        return base64.b85encode(
-            zlib.compress(
-                pickletools.optimize(
-                    pickle.dumps(value, protocol=pickle.HIGHEST_PROTOCOL)
-                ),
-                level=zlib.Z_BEST_COMPRESSION,
-            ),
-        ).decode()
-
-    def loads(self, value: Optional[str]) -> Any:
-        return (
-            pickle.loads(
-                zlib.decompress(base64.b85decode(value)),
-            )
-            if value
-            else None
-        )
+cache = Cache(name="hibiapi")
+try:
+    cache.setup(CACHE_URI)
+except Exception as e:
+    logger.warning(
+        f"Cache URI <y>{CACHE_URI!r}</y> setup <r><b>failed</b></r>: "
+        f"<r>{e!r}</r>, use memory backend instead."
+    )
 
 
 class CacheConfig(BaseModel):
-    endpoint: Callable[..., Coroutine]
+    endpoint: AsyncFunc
     namespace: str
     enabled: bool = True
     ttl: timedelta = CACHE_DELTA
 
     @staticmethod
-    def new(function: Callable[..., Coroutine]):
-        return CacheConfig(endpoint=function, namespace=function.__qualname__)
+    def new(
+        function: AsyncFunc,
+        *,
+        enabled: bool = True,
+        ttl: timedelta = CACHE_DELTA,
+        namespace: Optional[str] = None,
+    ):
+        return CacheConfig(
+            endpoint=function,
+            enabled=enabled,
+            ttl=ttl,
+            namespace=namespace or function.__qualname__,
+        )
 
 
 def cache_config(
     enabled: bool = True,
     ttl: timedelta = CACHE_DELTA,
     namespace: Optional[str] = None,
 ):
-    def decorator(endpoint: T_AsyncFunc) -> T_AsyncFunc:
+    def decorator(function: T_AsyncFunc) -> T_AsyncFunc:
         setattr(
-            endpoint,
-            "cache_config",
-            CacheConfig(
-                endpoint=endpoint,
-                namespace=namespace or endpoint.__qualname__,
-                enabled=enabled,
-                ttl=ttl,
-            ),
+            function,
+            CACHE_CONFIG_KEY,
+            CacheConfig.new(function, enabled=enabled, ttl=ttl, namespace=namespace),
         )
-        return endpoint
+        return function
 
     return decorator
 
 
 disable_cache = cache_config(enabled=False)
 
 
 class CachedValidatedFunction(ValidatedFunction):
     def serialize(self, args: Tuple[Any, ...], kwargs: Dict[str, Any]) -> BaseModel:
         values = self.build_values(args=args, kwargs=kwargs)
-        return self.model(**values)  # type:ignore
+        return self.model(**values)
 
 
 def endpoint_cache(function: T_AsyncFunc) -> T_AsyncFunc:
     from .routing import request_headers, response_headers
 
     vf = CachedValidatedFunction(function, config={})
-    cache: BaseCache = AioCache.from_url(CACHE_URI)  # type:ignore
-    config: CacheConfig = getattr(function, "cache_config", CacheConfig.new(function))
+    config = cast(
+        CacheConfig,
+        getattr(function, CACHE_CONFIG_KEY, None) or CacheConfig.new(function),
+    )
 
-    cache.namespace, cache.ttl = config.namespace, config.ttl.total_seconds()
-    cache.serializer = GZippedBase85Serializer(encoding="utf-8")
-
-    if not CACHE_ENABLED:
-        config.enabled = False
+    config.enabled = CACHE_ENABLED and config.enabled
 
     @wraps(function)
     async def wrapper(*args, **kwargs):
-        cache_policy: str = request_headers.get().get("cache-control", "public")
+        cache_policy = "public"
+
+        if CACHE_CONTROLLABLE:
+            cache_policy = request_headers.get().get("cache-control", cache_policy)
 
-        if (not config.enabled) or (cache_policy.casefold() == "no-store"):
+        if not config.enabled or cache_policy.casefold() == "no-store":
             return await vf.call(*args, **kwargs)
 
-        key = hashlib.md5(
-            (model := vf.serialize(args=args, kwargs=kwargs))
-            .json(exclude={"self"}, sort_keys=True, ensure_ascii=False)
-            .encode()
-        ).hexdigest()
+        key = (
+            f"{config.namespace}:"
+            + hashlib.md5(
+                (model := vf.serialize(args=args, kwargs=kwargs))
+                .json(exclude={"self"}, sort_keys=True, ensure_ascii=False)
+                .encode()
+            ).hexdigest()
+        )
+
+        response_header = response_headers.get()
+        result: Optional[Any] = None
 
         if cache_policy.casefold() == "no-cache":
             await cache.delete(key)
+        elif result := await cache.get(key):
+            logger.debug(f"Request hit cache <b><e>{key}</e></b>")
+            response_header.setdefault("X-Cache-Hit", key)
+
+        if result is None:
+            result = await vf.execute(model)
+            await cache.set(key, result, expire=config.ttl)
 
-        resp_header = response_headers.get()
-
-        if await cache.exists(key):
-            logger.debug(
-                f"Request to endpoint <g>{function.__qualname__}</g> "
-                f"restoring from <e>{key=}</e> in cache data."
-            )
-            resp_header.setdefault("X-Cache-Hit", key)
-            result, cache_date = await cache.get(key)  # type:ignore
-        else:
-            result, cache_date = await vf.execute(model), time.time()
-            await cache.set(key, (result, cache_date))
-
-        if (cache_remain := int(cache_date + cache.ttl - time.time())) > 0:
-            resp_header.setdefault("Cache-Control", f"max-age={cache_remain}")
+        if (cache_remain := await cache.get_expire(key)) > 0:
+            response_header.setdefault("Cache-Control", f"max-age={cache_remain}")
 
         return result
 
     return wrapper  # type:ignore
```

### Comparing `HibiAPI-0.7.7/hibiapi/utils/config.py` & `HibiAPI-0.8.0/hibiapi/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,45 @@
 import json
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Type, TypeVar, overload
 
-import confuse  # type:ignore
+import confuse
 import dotenv
 from pydantic import parse_obj_as
 
 from hibiapi import __file__ as root_file
 
 CONFIG_DIR = Path(".") / "configs"
 DEFAULT_DIR = Path(root_file).parent / "configs"
 
 _T = TypeVar("_T")
 
 
-def _generate_default() -> int:
-    CONFIG_DIR.mkdir(parents=True, exist_ok=True)
-    generated = 0
-    for file in os.listdir(DEFAULT_DIR):
-        default_path = DEFAULT_DIR / file
-        config_path = CONFIG_DIR / file
-        if config_path.is_file():
-            continue
-        generated += config_path.write_text(
-            default_path.read_text(encoding="utf-8"),
-            encoding="utf-8",
-        )
-    return generated
-
-
-if dotenv.find_dotenv():
-    assert dotenv.load_dotenv(), "Failed to load .env"
-else:
-    assert _generate_default() <= 0, "Please complete config file!"
-
-
 class ConfigSubView(confuse.Subview):
     @overload
     def get(self) -> Any:
         ...
 
     @overload
     def get(self, template: Type[_T]) -> _T:
         ...
 
-    def get(self, template: Type[_T] = Any) -> _T:  # type: ignore
+    def get(self, template: Type[_T] = Any) -> _T:
         return parse_obj_as(template, super().get())
 
     def as_str(self) -> str:
         return self.get(str)
 
     def as_str_seq(self, split: str = "\n") -> List[str]:
-        return self.as_str().strip().split(split)
+        return [
+            stripped
+            for line in self.as_str().strip().split(split)
+            if (stripped := line.strip())
+        ]
 
     def as_number(self) -> int:
         return self.get(int)
 
     def as_bool(self) -> bool:
         return self.get(bool)
 
@@ -69,27 +52,29 @@
     def __getitem__(self, key: str) -> "ConfigSubView":
         return self.__class__(self, key)
 
 
 class AppConfig(confuse.Configuration):
     def __init__(self, name: str):
         self._config_name = name
-        self._config = CONFIG_DIR / (filename := name + ".yml")
+        self._config = CONFIG_DIR / (filename := f"{name}.yml")
         self._default = DEFAULT_DIR / filename
         super().__init__(name)
         self._add_env_source()
 
     def config_dir(self) -> str:
         return str(CONFIG_DIR)
 
     def user_config_path(self) -> str:
         return str(self._config)
 
     def _add_env_source(self):
-        config_name = self._config_name.lower() + "_"
+        if dotenv.find_dotenv():
+            dotenv.load_dotenv()
+        config_name = f"{self._config_name.lower()}_"
         env_configs = {
             k[len(config_name) :].lower(): str(v)
             for k, v in os.environ.items()
             if k.lower().startswith(config_name)
         }
         # Convert `AAA_BBB_CCC=DDD` to `{'aaa':{'bbb':{'ccc':'ddd'}}}`
         source_tree: Dict[str, Any] = {}
@@ -123,10 +108,7 @@
 
 
 class APIConfig(GeneralConfig):
     pass
 
 
 Config = GeneralConfig("general")
-
-DATA_PATH = Config["data"]["path"].as_path().expanduser().absolute()
-DEBUG = Config["debug"].as_bool()
```

### Comparing `HibiAPI-0.7.7/hibiapi/utils/decorators/__init__.py` & `HibiAPI-0.8.0/hibiapi/utils/decorators/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,41 +2,39 @@
 
 import asyncio
 from asyncio import sleep as async_sleep
 from functools import partial, wraps
 from inspect import iscoroutinefunction
 from time import sleep as sync_sleep
 from typing import (
-    Any,
+    Awaitable,
     Callable,
-    Coroutine,
     Iterable,
     Optional,
     Protocol,
     Tuple,
     Type,
     TypeVar,
     Union,
     overload,
 )
 
 from typing_extensions import ParamSpec
 
-from ..log import logger
-from .timer import TimeIt
-
-_T = TypeVar("_T")
+from hibiapi.utils.decorators.enum import enum_auto_doc as enum_auto_doc  # noqa: F401
+from hibiapi.utils.decorators.timer import Callable_T, TimeIt
+from hibiapi.utils.log import logger
 
 Argument_T = ParamSpec("Argument_T")
 Return_T = TypeVar("Return_T")
 
 
 class RetryT(Protocol):
     @overload
-    def __call__(self, function: Callable) -> Callable:
+    def __call__(self, function: Callable_T) -> Callable_T:
         ...
 
     @overload
     def __call__(
         self,
         *,
         retries: int = ...,
@@ -53,15 +51,15 @@
         delay: float = ...,
         exceptions: Optional[Iterable[Type[Exception]]] = ...,
     ) -> Union[Callable, RetryT]:
         ...
 
 
 @overload
-def Retry(function: Callable) -> Callable:
+def Retry(function: Callable_T) -> Callable_T:
     ...
 
 
 @overload
 def Retry(
     *,
     retries: int = ...,
@@ -126,17 +124,17 @@
         assert isinstance(error, Exception)
         raise error
 
     return async_wrapper if iscoroutinefunction(function) else sync_wrapper
 
 
 def ToAsync(
-    function: Callable[Argument_T, Return_T]  # type:ignore
-) -> Callable[Argument_T, Coroutine[Any, Any, Return_T]]:  # type:ignore
+    function: Callable[Argument_T, Return_T]
+) -> Callable[Argument_T, Awaitable[Return_T]]:
     @TimeIt
     @wraps(function)
-    async def wrapper(*args, **kwargs):
+    async def wrapper(*args: Argument_T.args, **kwargs: Argument_T.kwargs) -> Return_T:
         return await asyncio.get_running_loop().run_in_executor(
             None, lambda: function(*args, **kwargs)
         )
 
     return wrapper
```

### Comparing `HibiAPI-0.7.7/hibiapi/utils/decorators/timer.py` & `HibiAPI-0.8.0/hibiapi/utils/decorators/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 import time
 from dataclasses import dataclass, field
 from functools import wraps
 from inspect import iscoroutinefunction
-from typing import Any, Callable, ClassVar, Dict, Optional
+from typing import Any, Callable, ClassVar, Dict, Optional, TypeVar
 
-from ..log import logger
+from hibiapi.utils.log import logger
+
+Callable_T = TypeVar("Callable_T", bound=Callable)
 
 
 class TimerError(Exception):
     """A custom exception used to report errors in use of Timer class"""
 
 
 @dataclass
@@ -60,15 +62,15 @@
     def __exit__(self, *exc_info: Any) -> None:
         """Stop the context manager timer"""
         self.stop()
 
     def _recreate_cm(self) -> Timer:
         return self.__class__(self.name, self.text, self.logger_func)
 
-    def __call__(self, function: Callable) -> Callable:
+    def __call__(self, function: Callable_T) -> Callable_T:
         @wraps(function)
         async def async_wrapper(*args: Any, **kwargs: Any):
             self.text = (
                 f"<g>Async</g> function <y>{function.__qualname__}</y> "
                 "cost <e>{:.3f}ms</e>"
             )
 
@@ -81,11 +83,13 @@
                 f"<g>sync</g> function <y>{function.__qualname__}</y> "
                 "cost <e>{:.3f}ms</e>"
             )
 
             with self._recreate_cm():
                 return function(*args, **kwargs)
 
-        return async_wrapper if iscoroutinefunction(function) else sync_wrapper
+        return (
+            async_wrapper if iscoroutinefunction(function) else sync_wrapper
+        )  # type:ignore
 
 
 TimeIt = Timer(logger_func=logger.trace)
```

### Comparing `HibiAPI-0.7.7/setup.py` & `HibiAPI-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,186 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+<!-- spell-checker: disable -->
+<!-- markdownlint-disable MD033 MD041 -->
 
-packages = \
-['hibiapi',
- 'hibiapi.api',
- 'hibiapi.api.bilibili',
- 'hibiapi.api.bilibili.api',
- 'hibiapi.api.netease',
- 'hibiapi.api.pixiv',
- 'hibiapi.api.sauce',
- 'hibiapi.api.tieba',
- 'hibiapi.api.wallpaper',
- 'hibiapi.app',
- 'hibiapi.app.routes',
- 'hibiapi.app.routes.bilibili',
- 'hibiapi.utils',
- 'hibiapi.utils.decorators']
-
-package_data = \
-{'': ['*'], 'hibiapi': ['configs/*']}
-
-install_requires = \
-['aiocache>=0.11.1,<0.12.0',
- 'click>=8.0.1,<9.0.0',
- 'confuse>=1.4.0,<2.0.0',
- 'fastapi>=0.71.0,<0.72.0',
- 'httpx[http2]>=0.21.3,<0.23.0',
- 'loguru>=0.5.3,<0.7.0',
- 'pycryptodomex>=3.10.1,<4.0.0',
- 'pydantic>=1.9.0,<2.0.0',
- 'python-dotenv>=0.17,<0.20',
- 'python-multipart>=0.0.5,<0.0.6',
- 'qrcode[pil]>=6.1,<8.0',
- 'sentry-sdk>=1.5.0,<2.0.0',
- 'uvicorn[standard]>=0.14,<0.18']
-
-entry_points = \
-{'console_scripts': ['hibiapi = hibiapi.__main__:main']}
-
-setup_kwargs = {
-    'name': 'hibiapi',
-    'version': '0.7.7',
-    'description': 'A program that implements easy-to-use APIs for a variety of commonly used sites',
-    'long_description': '<!-- spell-checker: disable -->\n<!-- markdownlint-disable MD033 MD041 -->\n\n<img src=".github/logo.svg" align="right">\n\n<div align="left">\n\n# HibiAPI\n\n**_一个实现了多种常用站点的易用化API的程序._**\n\n**_A program that implements easy-to-use APIs for a variety of commonly used sites._**\n\n[![Demo Version](https://img.shields.io/badge/dynamic/json?label=demo%20status&query=%24.info.version&url=https%3A%2F%2Fapi.obfs.dev%2Fopenapi.json&style=for-the-badge&color=lightblue)](https://api.obfs.dev)\n\n![Lint](https://github.com/mixmoe/HibiAPI/workflows/Lint/badge.svg)\n![Test](https://github.com/mixmoe/HibiAPI/workflows/Test/badge.svg)\n[![Coverage](https://codecov.io/gh/mixmoe/HibiAPI/branch/main/graph/badge.svg)](https://codecov.io/gh/mixmoe/HibiAPI)\n\n[![PyPI](https://img.shields.io/pypi/v/hibiapi)](https://pypi.org/project/hibiapi/)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/hibiapi)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hibiapi)\n![PyPI - License](https://img.shields.io/pypi/l/hibiapi)\n\n![GitHub last commit](https://img.shields.io/github/last-commit/mixmoe/HibiAPI)\n![GitHub commit activity](https://img.shields.io/github/commit-activity/m/mixmoe/hibiapi)\n![Lines of code](https://img.shields.io/tokei/lines/github/mixmoe/hibiapi)\n[![GitHub stars](https://img.shields.io/github/stars/mixmoe/HibiAPI)](https://github.com/mixmoe/HibiAPI/stargazers)\n[![GitHub forks](https://img.shields.io/github/forks/mixmoe/HibiAPI)](https://github.com/mixmoe/HibiAPI/network)\n[![GitHub issues](https://img.shields.io/github/issues/mixmoe/HibiAPI)](https://github.com/mixmoe/HibiAPI/issues)\n\n</div>\n\n---\n\n## 前言\n\n- `HibiAPI`提供多种网站公开内容的API集合, 它们包括:\n  - Pixiv的图片和小说相关信息获取和搜索\n  - Bilibili的视频/番剧等信息获取和搜索\n  - 网易云音乐的音乐/MV等信息获取和搜索\n  - 百度贴吧的帖子内容的获取\n  - [爱壁纸](https://adesk.com/)的横版和竖版壁纸获取\n  - and more…\n\n- 该项目的前身是 Imjad API[^1]\n  - 由于它的使用人数过多, 致使调用超出限制, 所以本人希望提供一个开源替代来供社区进行自由地部署和使用, 从而减轻一部分该 API 的使用压力\n\n[^1]: [什么是Imjad API](https://github.com/mixmoe/HibiAPI/wiki/FAQ#%E4%BB%80%E4%B9%88%E6%98%AFimjad-api)\n\n## 优势\n\n### 开源\n\n- 本项目以[Apache-2.0](./LICENSE)许可开源, 即:\n  - 你可以直接使用该项目提供的功能, 无需任何授权\n  - 你可以在**注明来源版权信息**的情况下对源代码进行任意分发和修改以及衍生\n\n### 高效\n\n- 使用 Python 的[异步机制](https://docs.python.org/zh-cn/3/library/asyncio.html), 由[FastAPI](https://fastapi.tiangolo.com/)驱动, 带来高效的使用体验 ~~虽然性能瓶颈压根不在这~~\n\n### 稳定\n\n- 在代码中广泛使用了Python的[类型提示支持](https://docs.python.org/zh-cn/3/library/typing.html), 使代码可读性更高且更加易于维护和调试\n\n- 在开发初期起就一直使用[PyLance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance), [Flake8](https://flake8.pycqa.org/en/latest/)以及[MyPy](https://mypy.readthedocs.io/)来对代码进行类型推断和纠错\n\n- 不直接使用第三方开发的 API 调用库, 而是全部用更加适合 Web 应用的逻辑重写第三方 API 请求, 更加可控 ~~疯狂造轮子~~\n\n## 已实现API[^2]\n\n[^2]: 请查看 [#1](https://github.com/mixmoe/HibiAPI/issues/1)\n\n- [x] Pixiv\n- [x] 网易云音乐\n- [ ] ~~一言~~ (其代替方案<https://hitokoto.cn>提供的方案已足够好, 暂不考虑支持)\n- [x] Bilibili\n- [x] 二维码\n- [ ] ~~企鹅FM~~ (似乎用的人不是很多)\n- [x] 百度贴吧\n- [x] 爱壁纸\n\n## 部署指南\n\n[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)\n\n- 手动部署指南: **[点击此处查看](https://github.com/mixmoe/HibiAPI/wiki/Deployment)**\n\n## 应用实例\n\n**我有更多的应用实例?** [立即 PR!](https://github.com/mixmoe/HibiAPI/pulls)\n\n- [`journey-ad/pixiv-viewer`](https://github.com/journey-ad/pixiv-viewer)\n\n  - **又一个 Pixiv 阅览工具**\n\n- 公开搭建实例\n  |         **站点名称**         |            **网址**             |        **状态**         |\n  | :--------------------------: | :-----------------------------: | :---------------------: |\n  |      **官方 Demo[^3]**       |     <https://api.obfs.dev>      |  ![official][official]  |\n  |           轻零 API           |   <https://hibiapi.lite0.com>   |     ![lite0][lite0]     |\n  |     Kyomotoi の菜几服务      |   <https://api.kyomotoi.moe>    |       ![kyo][kyo]       |\n  |          老狐狸 API          | <https://hibiapi.aliserver.net> | ![older-fox][older-fox] |\n  | [MyCard](https://mycard.moe) |   <https://hibi.moecube.com>    |    ![mycard][mycard]    |\n\n[^3]: 为了减轻服务器负担, Demo服务器已开启了Cloudflare全站缓存, 如果有实时获取更新的需求, 请自行搭建或使用其他部署实例\n\n[official]: https://img.shields.io/website?url=https%3A%2F%2Fapi.obfs.dev%2Fopenapi.json\n[lite0]: https://img.shields.io/website?url=https%3A%2F%2Fhibiapi.lite0.com%2Fopenapi.json\n[kyo]: https://img.shields.io/website?url=https%3A%2F%2Fapi.kyomotoi.moe%2Fopenapi.json\n[older-fox]: https://img.shields.io/website?url=https%3A%2F%2Fhibiapi.aliserver.net%2Fopenapi.json\n[mycard]: https://img.shields.io/website?url=https%3A%2F%2Fhibi.moecube.com%2Fopenapi.json\n\n## 特别鸣谢\n\n[**@journey-ad**](https://github.com/journey-ad) 大佬的 [Imjad API](https://api.imjad.cn/)\n\n### 参考项目\n\n> **正是因为有了你们, 这个项目才得以存在**\n\n- Pixiv: [`Mikubill/pixivpy-async`](https://github.com/Mikubill/pixivpy-async) [`upbit/pixivpy`](https://github.com/upbit/pixivpy)\n\n- Bilibili: [`SocialSisterYi/bilibili-API-collect`](https://github.com/SocialSisterYi/bilibili-API-collect) [`soimort/you-get`](https://github.com/soimort/you-get)\n\n- 网易云音乐: [`metowolf/NeteaseCloudMusicApi`](https://github.com/metowolf/NeteaseCloudMusicApi) [`greats3an/pyncm`](https://github.com/greats3an/pyncm) [`Binaryify/NeteaseCloudMusicApi`](https://github.com/Binaryify/NeteaseCloudMusicApi)\n\n- 百度贴吧: [`libsgh/tieba-api`](https://github.com/libsgh/tieba-api)\n\n### 贡献者们\n\n<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->\n[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors-)\n<!-- ALL-CONTRIBUTORS-BADGE:END -->\n\n感谢这些为这个项目作出贡献的各位大佬:\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tr>\n    <td align="center"><a href="http://kyomotoi.moe"><img src="https://avatars.githubusercontent.com/u/37587870?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kyomotoi</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=Kyomotoi" title="Documentation">📖</a> <a href="https://github.com/mixmoe/HibiAPI/commits?author=Kyomotoi" title="Tests">⚠️</a></td>\n    <td align="center"><a href="http://thdog.moe"><img src="https://avatars.githubusercontent.com/u/46120251?v=4?s=100" width="100px;" alt=""/><br /><sub><b>城倉奏</b></sub></a><br /><a href="#example-shirokurakana" title="Examples">💡</a></td>\n    <td align="center"><a href="http://skipm4.com"><img src="https://avatars.githubusercontent.com/u/40311581?v=4?s=100" width="100px;" alt=""/><br /><sub><b>SkipM4</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=SkipM4" title="Documentation">📖</a></td>\n    <td align="center"><a href="https://github.com/leaf7th"><img src="https://avatars.githubusercontent.com/u/38352552?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nook</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=leaf7th" title="Code">💻</a></td>\n    <td align="center"><a href="https://github.com/jiangzhuochi"><img src="https://avatars.githubusercontent.com/u/50538375?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jocky Chiang</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=jiangzhuochi" title="Code">💻</a></td>\n    <td align="center"><a href="https://github.com/cleoold"><img src="https://avatars.githubusercontent.com/u/13920903?v=4?s=100" width="100px;" alt=""/><br /><sub><b>midori</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=cleoold" title="Documentation">📖</a></td>\n    <td align="center"><a href="https://www.2yo.cc"><img src="https://avatars.githubusercontent.com/u/41198038?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Pretty9</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=Pretty9" title="Code">💻</a></td>\n  </tr>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\n_本段符合 [all-contributors](https://github.com/all-contributors/all-contributors) 规范_\n\n## 联系方式\n\n- 邮箱: <admin@obfs.dev>\n\n## 开源许可\n\n    Copyright 2020-2021 Mix Technology\n\n    Licensed under the Apache License, Version 2.0 (the "License");\n    you may not use this file except in compliance with the License.\n    You may obtain a copy of the License at\n\n        http://www.apache.org/licenses/LICENSE-2.0\n\n    Unless required by applicable law or agreed to in writing, software\n    distributed under the License is distributed on an "AS IS" BASIS,\n    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n    See the License for the specific language governing permissions and\n    limitations under the License.\n',
-    'author': 'mixmoe',
-    'author_email': 'admin@obfs.dev',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://api.obfs.dev',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+<img src=".github/logo.svg" align="right">
 
+<div align="left">
 
-setup(**setup_kwargs)
+# HibiAPI
+
+**_一个实现了多种常用站点的易用化 API 的程序._**
+
+**_A program that implements easy-to-use APIs for a variety of commonly used sites._**
+
+[![Demo Version](https://img.shields.io/badge/dynamic/json?label=demo%20status&query=%24.info.version&url=https%3A%2F%2Fapi.obfs.dev%2Fopenapi.json&style=for-the-badge&color=lightblue)](https://api.obfs.dev)
+
+![Lint](https://github.com/mixmoe/HibiAPI/workflows/Lint/badge.svg)
+![Test](https://github.com/mixmoe/HibiAPI/workflows/Test/badge.svg)
+[![Coverage](https://codecov.io/gh/mixmoe/HibiAPI/branch/main/graph/badge.svg)](https://codecov.io/gh/mixmoe/HibiAPI)
+
+[![PyPI](https://img.shields.io/pypi/v/hibiapi)](https://pypi.org/project/hibiapi/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/hibiapi)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hibiapi)
+![PyPI - License](https://img.shields.io/pypi/l/hibiapi)
+
+![GitHub last commit](https://img.shields.io/github/last-commit/mixmoe/HibiAPI)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/m/mixmoe/hibiapi)
+![Lines of code](https://img.shields.io/tokei/lines/github/mixmoe/hibiapi)
+[![GitHub stars](https://img.shields.io/github/stars/mixmoe/HibiAPI)](https://github.com/mixmoe/HibiAPI/stargazers)
+[![GitHub forks](https://img.shields.io/github/forks/mixmoe/HibiAPI)](https://github.com/mixmoe/HibiAPI/network)
+[![GitHub issues](https://img.shields.io/github/issues/mixmoe/HibiAPI)](https://github.com/mixmoe/HibiAPI/issues)
+
+</div>
+
+---
+
+## 前言
+
+- `HibiAPI`提供多种网站公开内容的 API 集合, 它们包括:
+
+  - Pixiv 的图片和小说相关信息获取和搜索
+  - Bilibili 的视频/番剧等信息获取和搜索
+  - 网易云音乐的音乐/MV 等信息获取和搜索
+  - 百度贴吧的帖子内容的获取
+  - [爱壁纸](https://adesk.com/)的横版和竖版壁纸获取
+  - 哔咔漫画的漫画信息获取和搜索
+  - …
+
+- 该项目的前身是 Imjad API[^1]
+  - 由于它的使用人数过多, 致使调用超出限制, 所以本人希望提供一个开源替代来供社区进行自由地部署和使用, 从而减轻一部分该 API 的使用压力
+
+[^1]: [什么是 Imjad API](https://github.com/mixmoe/HibiAPI/wiki/FAQ#%E4%BB%80%E4%B9%88%E6%98%AFimjad-api)
+
+## 优势
+
+### 开源
+
+- 本项目以[Apache-2.0](./LICENSE)许可开源, 请看[开源许可](#开源许可)一节
+
+### 高效
+
+- 使用 Python 的[异步机制](https://docs.python.org/zh-cn/3/library/asyncio.html), 由[FastAPI](https://fastapi.tiangolo.com/)驱动, 带来高效的使用体验 ~~虽然性能瓶颈压根不在这~~
+
+### 稳定
+
+- 在代码中广泛使用了 Python 的[类型提示支持](https://docs.python.org/zh-cn/3/library/typing.html), 使代码可读性更高且更加易于维护和调试
+
+- 在开发初期起就一直使用多种现代 Python 开发工具辅助开发, 包括:
+
+  - 使用 [PyLance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) 进行静态类型推断
+  - 使用 [Flake8](https://flake8.pycqa.org/en/latest/) 对代码格式进行检查
+  - 使用 [Black](https://black.readthedocs.io/en/stable/) 格式化代码以提升代码可读性
+
+- 不直接使用第三方开发的 API 调用库, 而是全部用更加适合 Web 应用的逻辑重写第三方 API 请求, 更加可控 ~~疯狂造轮子~~
+
+## 已实现 API[^2]
+
+[^2]: 请查看 [#1](https://github.com/mixmoe/HibiAPI/issues/1)
+
+- [x] Pixiv
+- [x] 网易云音乐
+- [ ] ~~一言~~ (其代替方案<https://hitokoto.cn>提供的方案已足够好, 暂不考虑支持)
+- [x] Bilibili
+- [x] 二维码
+- [ ] ~~企鹅 FM~~ (似乎用的人不是很多)
+- [x] 百度贴吧
+- [x] 爱壁纸
+- [x] 哔咔漫画
+
+## 部署指南
+
+[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
+
+- 手动部署指南: **[点击此处查看](https://github.com/mixmoe/HibiAPI/wiki/Deployment)**
+
+## 应用实例
+
+**我有更多的应用实例?** [立即 PR!](https://github.com/mixmoe/HibiAPI/pulls)
+
+- [`journey-ad/pixiv-viewer`](https://github.com/journey-ad/pixiv-viewer)
+
+  - **又一个 Pixiv 阅览工具**
+
+- 公开搭建实例
+  | **站点名称** | **网址** | **状态** |
+  | :--------------------------: | :-----------------------------: | :---------------------: |
+  | **官方 Demo[^3]** | <https://api.obfs.dev> | [![official][official]][official-stats] |
+  | 轻零 API | <https://hibiapi.lite0.com> | ![lite0][lite0] |
+  | Kyomotoi の菜几服务 | <https://api.kyomotoi.moe> | ![kyo][kyo] |
+  | 老狐狸 API | <https://hibiapi.aliserver.net> | ![older-fox][older-fox] |
+  | [MyCard](https://mycard.moe) | <https://hibi.moecube.com> | ![mycard][mycard] |
+
+[^3]: 为了减轻服务器负担, Demo 服务器已开启了 Cloudflare 全站缓存, 如果有实时获取更新的需求, 请自行搭建或使用其他部署实例
+
+[official]: https://img.shields.io/website?url=https%3A%2F%2Fapi.obfs.dev%2Fopenapi.json
+[official-stats]: https://metrics.librato.com/s/public/g1hepph3j
+[lite0]: https://img.shields.io/website?url=https%3A%2F%2Fhibiapi.lite0.com%2Fopenapi.json
+[kyo]: https://img.shields.io/website?url=https%3A%2F%2Fapi.kyomotoi.moe%2Fopenapi.json
+[older-fox]: https://img.shields.io/website?url=https%3A%2F%2Fhibiapi.aliserver.net%2Fopenapi.json
+[mycard]: https://img.shields.io/website?url=https%3A%2F%2Fhibi.moecube.com%2Fopenapi.json
+
+## 特别鸣谢
+
+[**@journey-ad**](https://github.com/journey-ad) 大佬的 **Imjad API**, 它是本项目的起源
+
+### 参考项目
+
+> **正是因为有了你们, 这个项目才得以存在**
+
+- Pixiv: [`Mikubill/pixivpy-async`](https://github.com/Mikubill/pixivpy-async) [`upbit/pixivpy`](https://github.com/upbit/pixivpy)
+
+- Bilibili: [`SocialSisterYi/bilibili-API-collect`](https://github.com/SocialSisterYi/bilibili-API-collect) [`soimort/you-get`](https://github.com/soimort/you-get)
+
+- 网易云音乐: [`metowolf/NeteaseCloudMusicApi`](https://github.com/metowolf/NeteaseCloudMusicApi) [`greats3an/pyncm`](https://github.com/greats3an/pyncm) [`Binaryify/NeteaseCloudMusicApi`](https://github.com/Binaryify/NeteaseCloudMusicApi)
+
+- 百度贴吧: [`libsgh/tieba-api`](https://github.com/libsgh/tieba-api)
+
+- 哔咔漫画：[`niuhuan/pica-rust`](https://github.com/niuhuan/pica-rust) [`abbeyokgo/PicaComic-Api`](https://github.com/abbeyokgo/PicaComic-Api)
+
+### 贡献者们
+
+感谢这些为这个项目作出贡献的各位大佬:
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://kyomotoi.moe"><img src="https://avatars.githubusercontent.com/u/37587870?v=4?s=100" width="100px;" alt="Kyomotoi"/><br /><sub><b>Kyomotoi</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=Kyomotoi" title="Documentation">📖</a> <a href="https://github.com/mixmoe/HibiAPI/commits?author=Kyomotoi" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://thdog.moe"><img src="https://avatars.githubusercontent.com/u/46120251?v=4?s=100" width="100px;" alt="城倉奏"/><br /><sub><b>城倉奏</b></sub></a><br /><a href="#example-shirokurakana" title="Examples">💡</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://skipm4.com"><img src="https://avatars.githubusercontent.com/u/40311581?v=4?s=100" width="100px;" alt="SkipM4"/><br /><sub><b>SkipM4</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=SkipM4" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/leaf7th"><img src="https://avatars.githubusercontent.com/u/38352552?v=4?s=100" width="100px;" alt="Nook"/><br /><sub><b>Nook</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=leaf7th" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jiangzhuochi"><img src="https://avatars.githubusercontent.com/u/50538375?v=4?s=100" width="100px;" alt="Jocky Chiang"/><br /><sub><b>Jocky Chiang</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=jiangzhuochi" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cleoold"><img src="https://avatars.githubusercontent.com/u/13920903?v=4?s=100" width="100px;" alt="midori"/><br /><sub><b>midori</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=cleoold" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.2yo.cc"><img src="https://avatars.githubusercontent.com/u/41198038?v=4?s=100" width="100px;" alt="Pretty9"/><br /><sub><b>Pretty9</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=Pretty9" title="Code">💻</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://nocilol.me/"><img src="https://avatars.githubusercontent.com/u/16256221?v=4?s=100" width="100px;" alt="Jad"/><br /><sub><b>Jad</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/issues?q=author%3Ajourney-ad" title="Bug reports">🐛</a> <a href="#ideas-journey-ad" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://nanoka.top"><img src="https://avatars.githubusercontent.com/u/31837214?v=4?s=100" width="100px;" alt="Yumine Sakura"/><br /><sub><b>Yumine Sakura</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=asadahimeka" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/yeyang52"><img src="https://avatars.githubusercontent.com/u/107110851?v=4?s=100" width="100px;" alt="yeyang"/><br /><sub><b>yeyang</b></sub></a><br /><a href="https://github.com/mixmoe/HibiAPI/commits?author=yeyang52" title="Code">💻</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+_本段符合 [all-contributors](https://github.com/all-contributors/all-contributors) 规范_
+
+## 开源许可
+
+    Copyright 2020-2021 Mix Technology
+
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
+
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
```

