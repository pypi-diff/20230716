# Comparing `tmp/forecastmanager-0.0.7.tar.gz` & `tmp/forecastmanager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.0.7.tar", last modified: Thu Jul  6 09:27:09 2023, max compression
+gzip compressed data, was "forecastmanager-0.0.8.tar", last modified: Sun Jul 16 17:39:04 2023, max compression
```

## Comparing `forecastmanager-0.0.7.tar` & `forecastmanager-0.0.8.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.484578 forecastmanager-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 09:27:09.484578 forecastmanager-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.472577 forecastmanager-0.0.7/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.476578 forecastmanager-0.0.7/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.476578 forecastmanager-0.0.7/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.476578 forecastmanager-0.0.7/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/site_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.472577 forecastmanager-0.0.7/forecastmanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.472577 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.480578 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/clearsky.png
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/cloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/fair.png
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/fog.png
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavyrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/partlycloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/rain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/rainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/rainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/sleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/sleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/sleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/snow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/snowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/snowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.484578 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/js/
--rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/js/forecast_basemap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/static/forecastmanager/js/helpers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.472577 forecastmanager-0.0.7/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.484578 forecastmanager-0.0.7/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/templates/forecastmanager/forecast_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/templates/forecastmanager/load_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/templates/forecastmanager/query_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/forecastmanager/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:27:09.476578 forecastmanager-0.0.7/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 09:27:09.000000 forecastmanager-0.0.7/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-06 09:27:09.000000 forecastmanager-0.0.7/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:27:09.000000 forecastmanager-0.0.7/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 09:27:09.000000 forecastmanager-0.0.7/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 09:27:09.000000 forecastmanager-0.0.7/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 09:26:45.000000 forecastmanager-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-06 09:27:09.484578 forecastmanager-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/0003_alter_forecast_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/site_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.772605 forecastmanager-0.0.8/forecastmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.772605 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.780605 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/clearsky.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/cloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/fair.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/fog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/partlycloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/forecast_basemap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/helpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.772605 forecastmanager-0.0.8/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/forecast_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/view_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/setup.cfg
```

### Comparing `forecastmanager-0.0.7/PKG-INFO` & `forecastmanager-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.7/forecastmanager/blocks.py` & `forecastmanager-0.0.8/forecastmanager/blocks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.0.8/forecastmanager/management/commands/generate_forecast.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 from django.core.management.base import BaseCommand
 
 import pandas as pd
-import json
 import requests
 
 from wagtailgeowidget.helpers import geosgeometry_str_to_struct
 from forecastmanager.models import City,Forecast
+from forecastmanager.site_settings import ForecastSetting,ForecastPeriod
 
 
 # Define the base URL for the Met Norway API
-BASE_URL = "https://api.met.no/weatherapi/locationforecast/2.0/compact"
+BASE_URL = "https://api.met.no/weatherapi/locationforecast/2.0/complete"
 headers = {
   'User-Agent':'Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Mobile Safari/537.36'
 }
 
 logger = logging.getLogger(__name__)
 
 default_options = () if not hasattr(BaseCommand, 'option_list') \
@@ -29,14 +29,17 @@
 
         # forecast_mode = list(IntegrationSettings.objects.all().values())
         # print("ATTEMPTING TO GENERATE 7 DAY FORECAST")
         # if forecast_mode[0]['enable_auto_forecast']:
            
         cities_ls = list(City.objects.all().values())
 
+        forecast_setting = ForecastSetting.objects.all().first()
+        parameters = forecast_setting.data_parameter_values
+
         for city in cities_ls:
 
             location = geosgeometry_str_to_struct(str(city['location']))
             lat = location['y']
             lon = location['x']
 
             # Construct the API URL for this location
@@ -53,65 +56,63 @@
 
                 df = pd.json_normalize(data)
 
                 # convert the 'time' column to a datetime object and set it as the index
                 df['time'] = pd.to_datetime(df['time'])
                 df.set_index('time', inplace=True)
 
+
                 # Define a function to extract the required values from a group
-                def extract_values(group):
+                def extract_values(group, params):
                     # Extract the minimum and maximum values of air temperature, wind speed, and wind direction
-                    min_temp = group['data.instant.details.air_temperature'].min()
-                    max_temp = group['data.instant.details.air_temperature'].max()
-                    # Extract the value of next_12_hours summary
-                    next_12_hours = group['data.next_12_hours.summary.symbol_code'].iloc[0]
-                    # Create a dictionary of the extracted values
-                    values = {'min_temp': min_temp, 'max_temp': max_temp, 
-                            'next_12_hours': next_12_hours}
-                    return pd.Series(values, index=['min_temp', 'max_temp', 
-                                                    'next_12_hours'])
+    
+                    param_val = {}
+                    for param in params:
+                    
+                        if param["parameter"] == 'air_temperature_max' or param["parameter"] =='air_temperature_min' or param["parameter"]  =='precipitation_amount':
+                            param_val[f'{param["parameter"]}'] =round(group[f'data.next_6_hours.details.{param["parameter"]}'].mean(),1)
+                              
+                        else:
+                            if f'data.instant.details.{param["parameter"]}' in group.columns:
+                                param_val[f'{param["parameter"]}'] = round(group[f'data.instant.details.{param["parameter"]}'].mean(),1)
+
+                            else:
+                                param_val[f'{param["parameter"]}'] = None
+
+                    param_val['condition'] = group['data.next_6_hours.summary.symbol_code'].iloc[0]
+
+                    
+                    return pd.Series(param_val)
 
                 # Group the DataFrame by date and apply the extract_values() function to each group
-                grouped = df.groupby(pd.Grouper(freq='D')).apply(extract_values)
-                grouped = grouped.dropna()
+                grouped = df.groupby(pd.Grouper(freq='D')).apply(extract_values, parameters)
+                grouped = grouped.dropna(how="all")
+                grouped = grouped.replace({np.nan: None})
 
                 # Get the name of the parent from the first column
                 parent_name = city['name']
                 # Try to get an existing parent with the same name, or create a new one
                 city = City.objects.get(name=parent_name)
-                
+                print("City:", parent_name )
+
                 for index, row in grouped.iterrows():
                     time = index.to_pydatetime()
-                    min_temp = row['min_temp']
-                    max_temp = row['max_temp']
-
-                    # Create or update the child object with the parent and the name from the second column
-                    # prioritize condition for the next 1 hour 
-                    if 'next_1_hours' in row:
-                        condition = row['next_1_hours'].split("_")[0]
-                    elif 'next_6_hours' in row:
-                        condition = row['next_6_hours'].split("_")[0]
-                    else:
-                        condition = row['next_12_hours'].split("_")[0]
-
+                    
                     # use update_or_create to update existing data
                     # and create new ones if the data does not exist
                     obj, created = Forecast.objects.update_or_create(
                         forecast_date=time,
                         city=city, 
                         defaults={
-                            'min_temp': min_temp,
-                            'max_temp': max_temp,
-                            'condition': condition
-                        }
+                            'condition':row['condition'].split('_')[0] if row['condition'] else row['condition'],
+                            'effective_period':ForecastPeriod.objects.get(pk=1),
+                            'data_value':row.to_dict()
+                            }
                     )
 
-            else:
-                # Handle errors
-                print(f"Error fetching weather data for ({lat}, {lon}): {response.status_code}")
 
 
         # else:
         #     print("AUTOMATED FORECASTING DISABLED. Will try again in 3 hours")
```

### Comparing `forecastmanager-0.0.7/forecastmanager/migrations/0001_initial.py` & `forecastmanager-0.0.8/forecastmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/models.py` & `forecastmanager-0.0.8/forecastmanager/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import uuid
+
 from django.contrib.gis.db import models
 from django.utils.translation import gettext_lazy as _
-from wagtailgeowidget.panels import LeafletPanel
-from wagtailgeowidget.helpers import geosgeometry_str_to_struct
 from wagtail.admin.panels import FieldPanel, MultiFieldPanel
 from wagtail.fields import RichTextField, StreamField
-from wagtail.snippets.models import register_snippet
+from wagtailgeowidget.helpers import geosgeometry_str_to_struct
+from wagtailgeowidget.panels import LeafletPanel
 
 from .blocks import ExtremeBlock
+from .site_settings import ForecastPeriod
+
 
-# @register_snippet
 class DailyWeather(models.Model):
     issued_on = models.DateField(auto_now_add=True, null=True)
     forecast_date = models.DateField(_("Forecast Date"), auto_now=False, auto_now_add=False)
     forecast_desc = RichTextField(verbose_name=_('Weather Forecast Description'))
     summary_date = models.DateField(_("Summary Date"), auto_now=False, auto_now_add=False)
     summary_desc = RichTextField(verbose_name=_('Weather Summary Description'))
     extreme_date = models.DateField(_("Extreme Date"), auto_now=False, auto_now_add=False, null=True, blank=True)
@@ -31,31 +32,29 @@
             FieldPanel('forecast_desc'),
         ], heading="Weather Forecast"),
         MultiFieldPanel([
             FieldPanel('extreme_date'),
             FieldPanel('extremes')
         ], heading="Extremes")
 
-        
     ]
 
     def __str__(self) -> str:
         return f'Daily Weather - Issued on {self.issued_on.strftime("%Y-%m-%d")}'
 
 
-
 # Create your models here.
 class City(models.Model):
     id = models.UUIDField(
         primary_key=True,
         default=uuid.uuid4,
         editable=False,
         help_text=_("Unique UUID. Auto generated on creation."),
     )
-    name = models.CharField(verbose_name=_("City Name"), max_length=255, null=True, blank=False,unique=True)
+    name = models.CharField(verbose_name=_("City Name"), max_length=255, null=True, blank=False, unique=True)
     location = models.PointField(verbose_name=_("City Location (Lat, Lng)"))
 
     panels = [
         FieldPanel("name"),
         LeafletPanel("location"),
     ]
 
@@ -65,79 +64,64 @@
 
     def __str__(self) -> str:
         return self.name
 
     @property
     def coordinates(self):
         location = geosgeometry_str_to_struct(str(self.location))
-        return [location['x'],location['y'] ]
+        return [location['x'], location['y']]
+
 
 class Forecast(models.Model):
     CONDITION_CHOICES = (
-        ('clearsky', 'Clear sky'),
-        ('cloudy','Cloudy'),
-        ('fair','Fair'),
-        ('fog','Fog'),
-        ('heavyrain','Heavy Rain'),
-        ('heavyrainandthunder','Heavy Rain and Thunder'),
-        ('heavyrainshowers','Heavy Rain Showers'),
-        ('heavyrainshowersandthunder','Heavy Rain Showers and Thunder'),
-        ('heavysleet','Heavy Sleet'),
-        ('heavysleetandthunder','Heavy Sleet and Thunder'),
-        ('heavysleetshowers','Heavy Sleet Showers'),
-        ('heavysleetshowersandthunder','Heavy Sleet Showers and Thunder'),
-        ('heavysnow','Heavy Snow'),
-        ('heavysnowandthunder','Heavy Snow and Thunder'),
-        ('heavysnowshowers','Heavy Snow Showers'),
-        ('heavysnowshowersandthunder','Heavy Snow Showers and Thunder'),
-        ('lightrain','Light Rain'),
-        ('lightrainandthunder','Light Rain and Thunder'),
-        ('lightrainshowers','Light Rain Showers'),
-        ('lightrainshowersandthunder','Light Rain Showers and Thunder'),
-        ('lightsleet','Light Sleet'),
-        ('lightsleetandthunder','Light Sleet and Thunder'),
-        ('lightsleetshowers','Light Sleet Showers'),
-        ('lightsleetshowersandthunder','Light Sleet Showers and Thunder'),
-        ('lightsnowshowersandthunder','Light Snow Showers and Thunder'),
-        ('partlycloudy','Partly Cloudy'),
-        ('rain','Rain'),
-        ('rainandthunder','Rain and Thunder'),
-        ('rainshowers','Rain showers'),
-        ('rainshowersandthunder','Rain Showes and Thunder'),
-        ('sleet','Sleet'),
-        ('sleetandthunder','Sleet and Thunder'),
-        ('sleetshowers','Sleet Showers'),
-        ('sleetshowersandthunder','Sleet Showes and Thunder'),
-        ('snow','Snow'),
-        ('snowandthunder','Snow and Thunder'),
-        ('snowshowers','Snow Showers'),
-        ('snowshowersandthunder','Snow Showers and Thunder'),
+        ('clearsky', _('Clear sky')),
+        ('cloudy', _('Cloudy')),
+        ('fair', _('Fair')),
+        ('fog', _('Fog')),
+        ('heavyrain', _('Heavy Rain')),
+        ('heavyrainandthunder', _('Heavy Rain and Thunder')),
+        ('heavyrainshowers', _('Heavy Rain Showers')),
+        ('heavyrainshowersandthunder', _('Heavy Rain Showers and Thunder')),
+        ('heavysleet', _('Heavy Sleet')),
+        ('heavysleetandthunder', _('Heavy Sleet and Thunder')),
+        ('heavysleetshowers', _('Heavy Sleet Showers')),
+        ('heavysleetshowersandthunder', _('Heavy Sleet Showers and Thunder')),
+        ('heavysnow', _('Heavy Snow')),
+        ('heavysnowandthunder', _('Heavy Snow and Thunder')),
+        ('heavysnowshowers', _('Heavy Snow Showers')),
+        ('heavysnowshowersandthunder', _('Heavy Snow Showers and Thunder')),
+        ('lightrain', _('Light Rain')),
+        ('lightrainandthunder', _('Light Rain and Thunder')),
+        ('lightrainshowers', _('Light Rain Showers')),
+        ('lightrainshowersandthunder',_('Light Rain Showers and Thunder')),
+        ('lightsleet', _('Light Sleet')),
+        ('lightsleetandthunder', _('Light Sleet and Thunder')),
+        ('lightsleetshowers',_('Light Sleet Showers')),
+        ('lightsleetshowersandthunder', _('Light Sleet Showers and Thunder')),
+        ('lightsnowshowersandthunder',_('Light Snow Showers and Thunder')),
+        ('partlycloudy', _('Partly Cloudy')),
+        ('rain', _('Rain')),
+        ('rainandthunder', _('Rain and Thunder')),
+        ('rainshowers', _('Rain showers')),
+        ('rainshowersandthunder', _('Rain Showes and Thunder')),
+        ('sleet', _('Sleet')),
+        ('sleetandthunder', _('Sleet and Thunder')),
+        ('sleetshowers', _('Sleet Showers')),
+        ('sleetshowersandthunder', _('Sleet Showes and Thunder')),
+        ('snow', _('Snow')),
+        ('snowandthunder', _('Snow and Thunder')),
+        ('snowshowers', _('Snow Showers')),
+        ('snowshowersandthunder', _('Snow Showers and Thunder')),
 
     )
 
     city = models.ForeignKey(City, on_delete=models.CASCADE, verbose_name=_("City"))
-    forecast_date = models.DateField( auto_now=False, auto_now_add=False, verbose_name=_("Forecasts Date"))
-    max_temp = models.IntegerField(verbose_name=_("Maximum Temperature"), blank=True)
-    min_temp = models.IntegerField(verbose_name=_("Minimum Temperaure"), blank=True)
-    wind_direction = models.IntegerField(verbose_name=_("Wind Direction"), blank=True, null=True)
-    wind_speed = models.IntegerField(verbose_name=_("Wind Speed"), blank=True, null=True)
-    condition = models.CharField(choices=CONDITION_CHOICES, verbose_name=_("General Weather Condition"), help_text=_("E.g Light Showers"), null=True, max_length=255)
+    forecast_date = models.DateField(auto_now=False, auto_now_add=False, verbose_name=_("Forecasts Date"))
+    effective_period = models.ForeignKey(ForecastPeriod, on_delete=models.PROTECT, null=True)
+    condition = models.CharField(choices=CONDITION_CHOICES, verbose_name=_("General Weather Condition"),
+                                 help_text=_("E.g Light Showers"), null=True, max_length=255)
+    data_value = models.JSONField(null=True)
 
     class Meta:
+        unique_together = ("city", "forecast_date", "effective_period")
         verbose_name = _("Forecast")
         verbose_name_plural = _("Forecasts")
-        # unique_together = (('city', 'forecast_date'))
-
-    panels = [
-        FieldPanel("city"),
-        FieldPanel("forecast_date"),
-        FieldPanel("min_temp"),
-        FieldPanel("max_temp"),
-        FieldPanel("wind_direction"),
-        FieldPanel("wind_speed"),
-        FieldPanel("condition"),
-    ]
-
-    # def __str__(self):
-    #     return f"{self.city} - {self.forecast_date}" 
-
-
```

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/clearsky.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/clearsky.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/cloudy.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/cloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/fair.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/fair.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/fog.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/fog.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavyrain.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavyrainshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysleet.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysleetshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysnow.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysnowshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightrain.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightrainandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightrainshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsleet.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsleetshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsnow.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightsnowshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/partlycloudy.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/partlycloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/rain.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/rainandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/rainshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/sleet.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/sleetandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/sleetshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/snow.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/snowandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/snowshowers.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/js/forecast_basemap.js` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/forecast_basemap.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/static/forecastmanager/js/helpers.js` & `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/helpers.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.7/forecastmanager/templates/forecastmanager/create_forecast.html` & `forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/view_forecast.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,822 +1,708 @@
 00000000: 7b25 2065 7874 656e 6473 2027 666f 7265  {% extends 'fore
 00000010: 6361 7374 6d61 6e61 6765 722f 666f 7265  castmanager/fore
 00000020: 6361 7374 5f62 6173 652e 6874 6d6c 2720  cast_base.html' 
-00000030: 257d 0a0a 7b25 206c 6f61 6420 7761 6774  %}..{% load wagt
-00000040: 6169 6c73 6574 7469 6e67 735f 7461 6773  ailsettings_tags
-00000050: 2025 7d0a 7b25 2067 6574 5f73 6574 7469   %}.{% get_setti
-00000060: 6e67 7320 7573 655f 6465 6661 756c 745f  ngs use_default_
-00000070: 7369 7465 3d54 7275 6520 257d 0a7b 2520  site=True %}.{% 
-00000080: 6c6f 6164 2077 6167 7461 696c 6164 6d69  load wagtailadmi
-00000090: 6e5f 7461 6773 2069 3138 6e20 7374 6174  n_tags i18n stat
-000000a0: 6963 2025 7d0a 0a7b 2520 626c 6f63 6b20  ic %}..{% block 
-000000b0: 6578 7472 615f 6373 7320 257d 0a7b 7b62  extra_css %}.{{b
-000000c0: 6c6f 636b 2e73 7570 6572 7d7d 0a3c 7374  lock.super}}.<st
-000000d0: 796c 653e 0a20 202e 666f 7265 6361 7374  yle>.  .forecast
-000000e0: 2c0a 2020 7365 6c65 6374 207b 0a20 2020  ,.  select {.   
-000000f0: 2066 6f6e 742d 7369 7a65 3a20 3134 7078   font-size: 14px
-00000100: 0a20 207d 0a3c 2f73 7479 6c65 3e0a 0a7b  .  }.</style>..{
-00000110: 2520 656e 6462 6c6f 636b 2065 7874 7261  % endblock extra
-00000120: 5f63 7373 2025 7d0a 0a7b 2520 626c 6f63  _css %}..{% bloc
-00000130: 6b20 666f 7265 6361 7374 2025 7d0a 0a3c  k forecast %}..<
-00000140: 6832 2063 6c61 7373 3d22 772d 7061 6e65  h2 class="w-pane
-00000150: 6c5f 5f68 6561 6469 6e67 223e 4164 6420  l__heading">Add 
-00000160: 666f 7265 6361 7374 3c2f 6832 3e0a 0a3c  forecast</h2>..<
-00000170: 6469 7620 636c 6173 733d 2272 6f77 2072  div class="row r
-00000180: 6f77 2d66 6c75 7368 2220 7374 796c 653d  ow-flush" style=
-00000190: 2270 6164 6469 6e67 2d74 6f70 3a31 7265  "padding-top:1re
-000001a0: 6d22 3e0a 0a20 203c 6469 7620 636c 6173  m">..  <div clas
-000001b0: 733d 2263 6f6c 3522 3e0a 2020 2020 3c66  s="col5">.    <f
-000001c0: 6f72 6d20 656e 6374 7970 653d 226d 756c  orm enctype="mul
-000001d0: 7469 7061 7274 2f66 6f72 6d2d 6461 7461  tipart/form-data
-000001e0: 2220 6964 3d22 666f 7265 6361 7374 5f66  " id="forecast_f
-000001f0: 6f72 6d22 206d 6574 686f 643d 2770 6f73  orm" method='pos
-00000200: 7427 3e0a 2020 2020 2020 7b25 2063 7372  t'>.      {% csr
-00000210: 665f 746f 6b65 6e20 257d 0a20 2020 2020  f_token %}.     
-00000220: 203c 6469 7620 636c 6173 733d 2268 656c   <div class="hel
-00000230: 702d 626c 6f63 6b20 6865 6c70 2d69 6e66  p-block help-inf
-00000240: 6f22 3e0a 2020 2020 2020 2020 3c73 7667  o">.        <svg
-00000250: 2063 6c61 7373 3d22 6963 6f6e 2069 636f   class="icon ico
-00000260: 6e2d 7761 726e 696e 6720 6963 6f6e 2220  n-warning icon" 
-00000270: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
-00000280: 6522 3e0a 2020 2020 2020 2020 2020 3c75  e">.          <u
-00000290: 7365 2068 7265 663d 2223 6963 6f6e 2d69  se href="#icon-i
-000002a0: 6e66 6f2d 6369 7263 6c65 223e 3c2f 7573  nfo-circle"></us
-000002b0: 653e 0a20 2020 2020 2020 203c 2f73 7667  e>.        </svg
-000002c0: 3e0a 2020 2020 2020 2020 3c64 6976 3e0a  >.        <div>.
-000002d0: 2020 2020 2020 2020 2020 596f 7520 6361            You ca
-000002e0: 6e20 3c61 2073 7479 6c65 3d22 6375 7273  n <a style="curs
-000002f0: 6f72 3a70 6f69 6e74 6572 223e 3c62 2069  or:pointer"><b i
-00000300: 643d 2265 7870 6f72 7454 6162 6c65 223e  d="exportTable">
-00000310: 646f 776e 6c6f 6164 2061 2074 656d 706c  download a templ
-00000320: 6174 653c 2f62 3e3c 2f61 3e20 6f66 2074  ate</b></a> of t
-00000330: 6865 2043 5356 2066 6f72 206f 6666 6c69  he CSV for offli
-00000340: 6e65 0a20 2020 2020 2020 2020 2065 6469  ne.          edi
-00000350: 7469 6e67 2061 6e64 2075 706c 6f61 6420  ting and upload 
-00000360: 6974 2068 6572 652e 2054 6865 2074 656d  it here. The tem
-00000370: 706c 6174 6520 636f 6d65 7320 7072 6570  plate comes prep
-00000380: 6f70 756c 6174 6564 0a20 2020 2020 2020  opulated.       
-00000390: 2020 2077 6974 6820 616c 6c20 7072 652d     with all pre-
-000003a0: 6578 6973 6974 696e 6720 6369 7469 6573  exisiting cities
-000003b0: 2e0a 0a20 2020 2020 2020 203c 2f64 6976  ...        </div
-000003c0: 3e0a 2020 2020 2020 3c2f 6469 763e 0a0a  >.      </div>..
-000003d0: 2020 2020 2020 3c75 6c20 636c 6173 733d        <ul class=
-000003e0: 2266 6965 6c64 7320 666f 7265 6361 7374  "fields forecast
-000003f0: 223e 0a20 2020 2020 2020 203c 6c69 3e0a  ">.        <li>.
-00000400: 2020 2020 2020 2020 2020 0a0a 2020 2020            ..    
-00000410: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000420: 3d22 772d 6669 656c 645f 5f77 7261 7070  ="w-field__wrapp
-00000430: 6572 2220 6461 7461 2d66 6965 6c64 2d77  er" data-field-w
-00000440: 7261 7070 6572 3d22 223e 0a0a 2020 2020  rapper="">..    
-00000450: 2020 2020 2020 2020 3c6c 6162 656c 2063          <label c
-00000460: 6c61 7373 3d22 772d 6669 656c 645f 5f6c  lass="w-field__l
-00000470: 6162 656c 2220 666f 723d 2269 645f 6373  abel" for="id_cs
-00000480: 7622 2069 643d 2269 645f 6373 762d 6c61  v" id="id_csv-la
-00000490: 6265 6c22 3e0a 2020 2020 2020 2020 2020  bel">.          
-000004a0: 2020 2020 466f 7265 6361 7374 2055 706c      Forecast Upl
-000004b0: 6f61 640a 2020 2020 2020 2020 2020 2020  oad.            
-000004c0: 3c2f 6c61 6265 6c3e 0a20 2020 2020 2020  </label>.       
-000004d0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000004e0: 2277 2d66 6965 6c64 2077 2d66 6965 6c64  "w-field w-field
-000004f0: 2d2d 6669 6c65 5f66 6965 6c64 2077 2d66  --file_field w-f
-00000500: 6965 6c64 2d2d 6669 6c65 5f69 6e70 7574  ield--file_input
-00000510: 2220 6461 7461 2d66 6965 6c64 3d22 2220  " data-field="" 
-00000520: 6461 7461 2d63 6f6e 7465 6e74 7061 7468  data-contentpath
-00000530: 3d22 6373 7622 3e0a 0a20 2020 2020 2020  ="csv">..       
-00000540: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000550: 733d 2277 2d66 6965 6c64 5f5f 6572 726f  s="w-field__erro
-00000560: 7273 2220 6461 7461 2d66 6965 6c64 2d65  rs" data-field-e
-00000570: 7272 6f72 733d 2222 3e0a 2020 2020 2020  rrors="">.      
-00000580: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
-00000590: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000005a0: 6976 2063 6c61 7373 3d22 772d 6669 656c  iv class="w-fiel
-000005b0: 645f 5f68 656c 7022 2064 6174 612d 6669  d__help" data-fi
-000005c0: 656c 642d 6865 6c70 3d22 223e 0a0a 2020  eld-help="">..  
-000005d0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000005e0: 6976 2063 6c61 7373 3d22 6865 6c70 223e  iv class="help">
-000005f0: 5468 6520 7570 6c6f 6164 6564 2066 696c  The uploaded fil
-00000600: 6520 7368 6f75 6c64 2062 6520 6120 4353  e should be a CS
-00000610: 562c 2073 696d 696c 6172 2074 6f20 7468  V, similar to th
-00000620: 6520 7461 626c 6520 6f6e 2074 6865 2072  e table on the r
-00000630: 6967 6874 3c2f 6469 763e 0a0a 2020 2020  ight</div>..    
-00000640: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000650: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000660: 3c64 6976 2063 6c61 7373 3d22 772d 6669  <div class="w-fi
-00000670: 656c 645f 5f69 6e70 7574 2220 6461 7461  eld__input" data
-00000680: 2d66 6965 6c64 2d69 6e70 7574 3d22 223e  -field-input="">
-00000690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000006a0: 203c 696e 7075 7420 7479 7065 3d22 6669   <input type="fi
-000006b0: 6c65 2220 6e61 6d65 3d22 6373 7622 2061  le" name="csv" a
-000006c0: 6363 6570 743d 222e 6373 7622 2069 643d  ccept=".csv" id=
-000006d0: 2269 645f 6373 7622 3e0a 2020 2020 2020  "id_csv">.      
-000006e0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-000006f0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-00000700: 3e0a 2020 2020 2020 2020 2020 3c2f 6469  >.          </di
-00000710: 763e 0a20 2020 2020 2020 203c 2f6c 693e  v>.        </li>
-00000720: 0a0a 2020 2020 2020 2020 3c6c 693e 0a20  ..        <li>. 
-00000730: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00000740: 6173 733d 2277 2d66 6965 6c64 5f5f 7772  ass="w-field__wr
-00000750: 6170 7065 7222 2064 6174 612d 6669 656c  apper" data-fiel
-00000760: 642d 7772 6170 7065 723d 2222 3e0a 2020  d-wrapper="">.  
-00000770: 2020 2020 2020 2020 2020 3c6c 6162 656c            <label
-00000780: 2063 6c61 7373 3d22 772d 6669 656c 645f   class="w-field_
-00000790: 5f6c 6162 656c 2220 666f 723d 2269 645f  _label" for="id_
-000007a0: 7374 6172 745f 6461 7465 2220 6964 3d22  start_date" id="
-000007b0: 6964 5f73 7461 7274 5f64 6174 652d 6c61  id_start_date-la
-000007c0: 6265 6c22 3e0a 2020 2020 2020 2020 2020  bel">.          
-000007d0: 2020 2020 2020 466f 7265 6361 7374 2044        Forecast D
-000007e0: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
-000007f0: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-00000800: 2277 2d72 6571 7569 7265 642d 6d61 726b  "w-required-mark
-00000810: 223e 2a3c 2f73 7061 6e3e 0a20 2020 2020  ">*</span>.     
-00000820: 2020 2020 2020 203c 2f6c 6162 656c 3e0a         </label>.
-00000830: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-00000840: 7620 636c 6173 733d 2277 2d66 6965 6c64  v class="w-field
-00000850: 5f5f 6865 6c70 2220 6461 7461 2d66 6965  __help" data-fie
-00000860: 6c64 2d68 656c 703d 2222 3e0a 0a20 2020  ld-help="">..   
-00000870: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000880: 636c 6173 733d 2268 656c 7022 3e44 6174  class="help">Dat
-00000890: 6520 6f66 2066 6f72 6563 6173 743c 2f64  e of forecast</d
-000008a0: 6976 3e0a 0a20 2020 2020 2020 2020 2020  iv>..           
-000008b0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-000008c0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000008d0: 772d 6669 656c 6420 772d 6669 656c 642d  w-field w-field-
-000008e0: 2d64 6174 655f 6669 656c 6420 772d 6669  -date_field w-fi
-000008f0: 656c 642d 2d61 646d 696e 5f64 6174 655f  eld--admin_date_
-00000900: 696e 7075 7422 2064 6174 612d 6669 656c  input" data-fiel
-00000910: 643d 2222 2064 6174 612d 636f 6e74 656e  d="" data-conten
-00000920: 7470 6174 683d 2264 6174 6522 3e0a 2020  tpath="date">.  
-00000930: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000940: 6976 2063 6c61 7373 3d22 772d 6669 656c  iv class="w-fiel
-00000950: 645f 5f65 7272 6f72 7322 2064 6174 612d  d__errors" data-
-00000960: 6669 656c 642d 6572 726f 7273 3d22 223e  field-errors="">
-00000970: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000980: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000990: 733d 2277 2d66 6965 6c64 5f5f 696e 7075  s="w-field__inpu
-000009a0: 7422 2064 6174 612d 6669 656c 642d 696e  t" data-field-in
-000009b0: 7075 743d 2222 3e0a 2020 2020 2020 2020  put="">.        
-000009c0: 2020 2020 2020 2020 2020 2020 3c69 6e70              <inp
-000009d0: 7574 2074 7970 653d 2274 6578 7422 206e  ut type="text" n
-000009e0: 616d 653d 2273 7461 7274 5f64 6174 6522  ame="start_date"
-000009f0: 2061 7574 6f63 6f6d 706c 6574 653d 226f   autocomplete="o
-00000a00: 6666 2220 7265 7175 6972 6564 3d22 2220  ff" required="" 
-00000a10: 6964 3d22 6964 5f64 6174 6522 202f 3e0a  id="id_date" />.
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 2020 2020 3c73 6372 6970 743e 696e 6974      <script>init
-00000a40: 4461 7465 4368 6f6f 7365 7228 2269 645f  DateChooser("id_
-00000a50: 6461 7465 222c 207b 2022 6461 794f 6657  date", { "dayOfW
-00000a60: 6565 6b53 7461 7274 223a 2030 2c20 2266  eekStart": 0, "f
-00000a70: 6f72 6d61 7422 3a20 2259 2d6d 2d64 2220  ormat": "Y-m-d" 
-00000a80: 7d29 3b3c 2f73 6372 6970 743e 0a20 2020  });</script>.   
-00000a90: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00000aa0: 6976 3e0a 2020 2020 0a20 2020 2020 2020  iv>.    .       
-00000ab0: 2020 2020 2020 2020 203c 6469 7620 6461           <div da
-00000ac0: 7461 2d66 6965 6c64 2d68 656c 703d 2222  ta-field-help=""
-00000ad0: 3e3c 2f64 6976 3e0a 2020 2020 2020 2020  ></div>.        
-00000ae0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000af0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000b00: 2020 2020 3c2f 6c69 3e0a 0a20 2020 2020      </li>..     
-00000b10: 2020 203c 6469 7620 7374 796c 653d 2264     <div style="d
-00000b20: 6973 706c 6179 3a6e 6f6e 6522 2069 643d  isplay:none" id=
-00000b30: 2268 6561 6465 725f 7365 6374 696f 6e22  "header_section"
-00000b40: 3e0a 0a20 2020 2020 2020 203c 6872 3e0a  >..        <hr>.
-00000b50: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
-00000b60: 6173 733d 2268 656c 702d 626c 6f63 6b20  ass="help-block 
-00000b70: 6865 6c70 2d69 6e66 6f22 3e0a 2020 2020  help-info">.    
-00000b80: 2020 2020 2020 3c73 7667 2063 6c61 7373        <svg class
-00000b90: 3d22 6963 6f6e 2069 636f 6e2d 7761 726e  ="icon icon-warn
-00000ba0: 696e 6720 6963 6f6e 2220 6172 6961 2d68  ing icon" aria-h
-00000bb0: 6964 6465 6e3d 2274 7275 6522 3e0a 2020  idden="true">.  
-00000bc0: 2020 2020 2020 2020 2020 3c75 7365 2068            <use h
-00000bd0: 7265 663d 2223 6963 6f6e 2d69 6e66 6f2d  ref="#icon-info-
-00000be0: 6369 7263 6c65 223e 3c2f 7573 653e 0a20  circle"></use>. 
-00000bf0: 2020 2020 2020 2020 203c 2f73 7667 3e0a           </svg>.
-00000c00: 2020 2020 2020 2020 2020 3c64 6976 3e0a            <div>.
-00000c10: 2020 2020 2020 2020 2020 2020 5665 7269              Veri
-00000c20: 6679 2074 6861 7420 616c 6c20 636f 6c75  fy that all colu
-00000c30: 6d6e 7320 6d61 7463 6820 636f 7272 6563  mns match correc
-00000c40: 746c 790a 2020 2020 2020 2020 2020 3c2f  tly.          </
-00000c50: 6469 763e 0a20 2020 2020 2020 203c 2f64  div>.        </d
-00000c60: 6976 3e0a 0a20 2020 2020 2020 203c 6c69  iv>..        <li
-00000c70: 3e0a 2020 2020 2020 2020 2020 3c64 6976  >.          <div
-00000c80: 2063 6c61 7373 3d22 726f 7720 726f 772d   class="row row-
-00000c90: 666c 7573 6822 2073 7479 6c65 3d22 7061  flush" style="pa
-00000ca0: 6464 696e 672d 746f 703a 3172 656d 223e  dding-top:1rem">
-00000cb0: 0a0a 2020 2020 2020 2020 2020 2020 3c64  ..            <d
-00000cc0: 6976 2063 6c61 7373 3d22 636f 6c36 223e  iv class="col6">
-00000cd0: 0a20 2020 2020 2020 2020 203c 6c61 6265  .          <labe
-00000ce0: 6c20 666f 723d 2263 6974 7922 2063 6c61  l for="city" cla
-00000cf0: 7373 3d22 772d 6669 656c 645f 5f6c 6162  ss="w-field__lab
-00000d00: 656c 223e 4369 7479 3a20 3c73 7061 6e20  el">City: <span 
-00000d10: 636c 6173 733d 2277 2d72 6571 7569 7265  class="w-require
-00000d20: 642d 6d61 726b 223e 2a3c 2f73 7061 6e3e  d-mark">*</span>
-00000d30: 3c2f 6c61 6265 6c3e 0a20 2020 2020 2020  </label>.       
-00000d40: 2020 203c 6469 7620 636c 6173 733d 2277     <div class="w
-00000d50: 2d66 6965 6c64 2077 2d66 6965 6c64 2d2d  -field w-field--
-00000d60: 6669 6c65 5f66 6965 6c64 2077 2d66 6965  file_field w-fie
-00000d70: 6c64 2d2d 6669 6c65 5f69 6e70 7574 223e  ld--file_input">
-00000d80: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-00000d90: 7620 636c 6173 733d 2277 2d66 6965 6c64  v class="w-field
-00000da0: 5f5f 696e 7075 7422 2064 6174 612d 6669  __input" data-fi
-00000db0: 656c 642d 696e 7075 743d 2222 3e0a 0a20  eld-input="">.. 
-00000dc0: 2020 2020 2020 2020 2020 2020 203c 7365               <se
-00000dd0: 6c65 6374 2069 643d 2263 6974 7922 3e0a  lect id="city">.
-00000de0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000df0: 7365 6c65 6374 3e0a 2020 2020 2020 2020  select>.        
-00000e00: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000e10: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000e20: 2020 2020 3c2f 6469 763e 0a0a 2020 2020      </div>..    
-00000e30: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000e40: 636f 6c36 223e 0a20 2020 2020 2020 2020  col6">.         
-00000e50: 203c 6c61 6265 6c20 666f 723d 226d 696e   <label for="min
-00000e60: 5465 6d70 2220 636c 6173 733d 2277 2d66  Temp" class="w-f
-00000e70: 6965 6c64 5f5f 6c61 6265 6c22 3e4d 696e  ield__label">Min
-00000e80: 2054 656d 703a 203c 7370 616e 2063 6c61   Temp: <span cla
-00000e90: 7373 3d22 772d 7265 7175 6972 6564 2d6d  ss="w-required-m
-00000ea0: 6172 6b22 3e2a 3c2f 7370 616e 3e3c 2f6c  ark">*</span></l
-00000eb0: 6162 656c 3e0a 0a20 2020 2020 2020 2020  abel>..         
-00000ec0: 203c 6469 7620 636c 6173 733d 2277 2d66   <div class="w-f
-00000ed0: 6965 6c64 2077 2d66 6965 6c64 2d2d 6669  ield w-field--fi
-00000ee0: 6c65 5f66 6965 6c64 2077 2d66 6965 6c64  le_field w-field
-00000ef0: 2d2d 6669 6c65 5f69 6e70 7574 223e 0a20  --file_input">. 
-00000f00: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000f10: 636c 6173 733d 2277 2d66 6965 6c64 5f5f  class="w-field__
-00000f20: 696e 7075 7422 2064 6174 612d 6669 656c  input" data-fiel
-00000f30: 642d 696e 7075 743d 2222 3e0a 0a20 2020  d-input="">..   
-00000f40: 2020 2020 2020 2020 2020 203c 7365 6c65             <sele
-00000f50: 6374 2069 643d 226d 696e 5465 6d70 223e  ct id="minTemp">
-00000f60: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00000f70: 2f73 656c 6563 743e 0a20 2020 2020 2020  /select>.       
-00000f80: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000f90: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000fa0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000fb0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000fc0: 2020 203c 2f6c 693e 0a0a 2020 2020 2020     </li>..      
-00000fd0: 2020 3c6c 693e 0a20 2020 2020 2020 2020    <li>.         
-00000fe0: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
-00000ff0: 2072 6f77 2d66 6c75 7368 2220 7374 796c   row-flush" styl
-00001000: 653d 2270 6164 6469 6e67 2d74 6f70 3a31  e="padding-top:1
-00001010: 7265 6d22 3e0a 0a20 2020 2020 2020 2020  rem">..         
-00001020: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00001030: 6f6c 3622 3e0a 2020 2020 2020 2020 2020  ol6">.          
-00001040: 2020 2020 3c6c 6162 656c 2066 6f72 3d22      <label for="
-00001050: 6d61 7854 656d 7022 2063 6c61 7373 3d22  maxTemp" class="
-00001060: 772d 6669 656c 645f 5f6c 6162 656c 223e  w-field__label">
-00001070: 4d61 7820 5465 6d70 3a20 3c73 7061 6e20  Max Temp: <span 
-00001080: 636c 6173 733d 2277 2d72 6571 7569 7265  class="w-require
-00001090: 642d 6d61 726b 223e 2a3c 2f73 7061 6e3e  d-mark">*</span>
-000010a0: 3c2f 6c61 6265 6c3e 0a0a 2020 2020 2020  </label>..      
-000010b0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000010c0: 7373 3d22 772d 6669 656c 6420 772d 6669  ss="w-field w-fi
-000010d0: 656c 642d 2d66 696c 655f 6669 656c 6420  eld--file_field 
-000010e0: 772d 6669 656c 642d 2d66 696c 655f 696e  w-field--file_in
-000010f0: 7075 7422 3e0a 2020 2020 2020 2020 2020  put">.          
-00001100: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00001110: 3d22 772d 6669 656c 645f 5f69 6e70 7574  ="w-field__input
-00001120: 2220 6461 7461 2d66 6965 6c64 2d69 6e70  " data-field-inp
-00001130: 7574 3d22 223e 0a20 2020 200a 2020 2020  ut="">.    .    
-00001140: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00001150: 656c 6563 7420 6964 3d22 6d61 7854 656d  elect id="maxTem
-00001160: 7022 3e0a 2020 2020 2020 2020 2020 2020  p">.            
-00001170: 2020 2020 2020 3c2f 7365 6c65 6374 3e0a        </select>.
-00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001190: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-000011a0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000011b0: 2020 2020 3c2f 6469 763e 0a0a 2020 2020      </div>..    
-000011c0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000011d0: 636f 6c36 223e 0a20 2020 2020 2020 2020  col6">.         
-000011e0: 203c 6c61 6265 6c20 666f 723d 2263 6f6e   <label for="con
-000011f0: 6469 7469 6f6e 2220 636c 6173 733d 2277  dition" class="w
-00001200: 2d66 6965 6c64 5f5f 6c61 6265 6c22 3e43  -field__label">C
-00001210: 6f6e 6469 7469 6f6e 3a20 3c73 7061 6e20  ondition: <span 
-00001220: 636c 6173 733d 2277 2d72 6571 7569 7265  class="w-require
-00001230: 642d 6d61 726b 223e 2a3c 2f73 7061 6e3e  d-mark">*</span>
-00001240: 3c2f 6c61 6265 6c3e 0a20 2020 2020 2020  </label>.       
-00001250: 2020 203c 6469 7620 636c 6173 733d 2277     <div class="w
-00001260: 2d66 6965 6c64 2077 2d66 6965 6c64 2d2d  -field w-field--
-00001270: 6669 6c65 5f66 6965 6c64 2077 2d66 6965  file_field w-fie
-00001280: 6c64 2d2d 6669 6c65 5f69 6e70 7574 223e  ld--file_input">
-00001290: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-000012a0: 7620 636c 6173 733d 2277 2d66 6965 6c64  v class="w-field
-000012b0: 5f5f 696e 7075 7422 2064 6174 612d 6669  __input" data-fi
-000012c0: 656c 642d 696e 7075 743d 2222 3e0a 0a20  eld-input="">.. 
-000012d0: 2020 2020 2020 2020 2020 2020 203c 7365               <se
-000012e0: 6c65 6374 2069 643d 2263 6f6e 6469 7469  lect id="conditi
-000012f0: 6f6e 223e 0a20 2020 2020 2020 2020 2020  on">.           
-00001300: 2020 203c 2f73 656c 6563 743e 0a20 2020     </select>.   
-00001310: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00001320: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00001330: 0a0a 2020 2020 2020 2020 3c2f 6469 763e  ..        </div>
-00001340: 0a20 2020 2020 2020 203c 2f6c 693e 0a20  .        </li>. 
-00001350: 2020 2020 203c 2f64 6976 3e0a 0a20 2020       </div>..   
-00001360: 2020 2020 203c 6c69 2020 7374 796c 653d       <li  style=
-00001370: 2270 6164 6469 6e67 2d74 6f70 3a31 656d  "padding-top:1em
-00001380: 223e 0a20 2020 2020 2020 2020 203c 6275  ">.          <bu
-00001390: 7474 6f6e 2074 7970 653d 2273 7562 6d69  tton type="submi
-000013a0: 7422 2069 643d 2273 7562 6d69 7446 6f72  t" id="submitFor
-000013b0: 6563 6173 7422 2063 6c61 7373 3d22 6275  ecast" class="bu
-000013c0: 7474 6f6e 223e 2050 7562 6c69 7368 3c2f  tton"> Publish</
-000013d0: 6275 7474 6f6e 3e0a 2020 2020 2020 2020  button>.        
-000013e0: 3c2f 6c69 3e0a 2020 2020 2020 3c2f 756c  </li>.      </ul
-000013f0: 3e0a 2020 2020 3c2f 666f 726d 3e0a 2020  >.    </form>.  
-00001400: 3c2f 6469 763e 0a20 203c 6469 7620 636c  </div>.  <div cl
-00001410: 6173 733d 2263 6f6c 3722 3e0a 2020 2020  ass="col7">.    
-00001420: 3c64 6976 2069 643d 2263 7265 6174 6554  <div id="createT
-00001430: 6162 6c65 2220 7374 796c 653d 7a2d 696e  able" style=z-in
-00001440: 6465 783a 313e 3c2f 6469 763e 0a20 2020  dex:1></div>.   
-00001450: 203c 6469 7620 6964 3d22 6578 706f 7274   <div id="export
-00001460: 5465 6d70 6c61 7465 2220 7374 796c 653d  Template" style=
-00001470: 2264 6973 706c 6179 3a20 6e6f 6e65 3b22  "display: none;"
-00001480: 3e3c 2f64 6976 3e0a 0a20 203c 2f64 6976  ></div>..  </div
-00001490: 3e0a 0a0a 3c2f 6469 763e 0a0a 0a7b 2520  >...</div>...{% 
-000014a0: 656e 6462 6c6f 636b 2025 7d0a 0a7b 2520  endblock %}..{% 
-000014b0: 626c 6f63 6b20 6578 7472 615f 6a73 2025  block extra_js %
-000014c0: 7d0a 7b7b 626c 6f63 6b2e 7375 7065 727d  }.{{block.super}
-000014d0: 7d0a 3c73 6372 6970 7420 7372 633d 227b  }.<script src="{
-000014e0: 2520 7665 7273 696f 6e65 645f 7374 6174  % versioned_stat
-000014f0: 6963 2027 7761 6774 6169 6c61 646d 696e  ic 'wagtailadmin
-00001500: 2f6a 732f 6461 7465 2d74 696d 652d 6368  /js/date-time-ch
-00001510: 6f6f 7365 722e 6a73 2720 257d 223e 3c2f  ooser.js' %}"></
-00001520: 7363 7269 7074 3e0a 3c73 6372 6970 7420  script>.<script 
-00001530: 7372 633d 227b 2520 7374 6174 6963 2027  src="{% static '
-00001540: 666f 7265 6361 7374 6d61 6e61 6765 722f  forecastmanager/
-00001550: 6a73 2f68 656c 7065 7273 2e6a 7327 2025  js/helpers.js' %
-00001560: 7d22 3e3c 2f73 6372 6970 743e 0a0a 7b25  }"></script>..{%
-00001570: 2069 6e63 6c75 6465 2022 7761 6774 6169   include "wagtai
-00001580: 6c61 646d 696e 2f70 6167 6573 2f5f 6564  ladmin/pages/_ed
-00001590: 6974 6f72 5f6a 732e 6874 6d6c 2220 257d  itor_js.html" %}
-000015a0: 207b 7b20 666f 726d 2e6d 6564 6961 2e6a   {{ form.media.j
-000015b0: 737d 7d0a 3c73 6372 6970 743e 0a20 2064  s}}.<script>.  d
-000015c0: 6f63 756d 656e 742e 6164 6445 7665 6e74  ocument.addEvent
-000015d0: 4c69 7374 656e 6572 2822 444f 4d43 6f6e  Listener("DOMCon
-000015e0: 7465 6e74 4c6f 6164 6564 222c 2066 756e  tentLoaded", fun
-000015f0: 6374 696f 6e20 2829 207b 0a0a 2020 2020  ction () {..    
-00001600: 7661 7220 7765 6174 6865 725f 636f 6e64  var weather_cond
-00001610: 6974 696f 6e5f 6c73 203d 204a 534f 4e2e  ition_ls = JSON.
-00001620: 7061 7273 6528 277b 7b77 6561 7468 6572  parse('{{weather
-00001630: 5f63 6f6e 6469 7469 6f6e 5f6c 737c 6573  _condition_ls|es
-00001640: 6361 7065 6a73 7d7d 2729 0a0a 2020 2020  capejs}}')..    
-00001650: 7661 7220 6369 7479 5f6c 7320 3d20 4a53  var city_ls = JS
-00001660: 4f4e 2e70 6172 7365 2827 7b7b 6369 7479  ON.parse('{{city
-00001670: 5f6c 737c 6573 6361 7065 6a73 7d7d 2729  _ls|escapejs}}')
-00001680: 0a0a 2020 2020 636f 6e73 7420 636f 6e74  ..    const cont
-00001690: 6169 6e65 7220 3d20 646f 6375 6d65 6e74  ainer = document
-000016a0: 2e71 7565 7279 5365 6c65 6374 6f72 2827  .querySelector('
-000016b0: 2363 7265 6174 6554 6162 6c65 2729 3b0a  #createTable');.
-000016c0: 2020 2020 636f 6e73 7420 7374 6174 6963      const static
-000016d0: 5f70 6174 6820 3d20 277b 2520 7374 6174  _path = '{% stat
-000016e0: 6963 2022 666f 7265 6361 7374 6d61 6e61  ic "forecastmana
-000016f0: 6765 722f 696d 672f 2220 257d 270a 0a20  ger/img/" %}'.. 
-00001700: 2020 200a 2020 2020 636f 6e73 7420 686f     .    const ho
-00001710: 7420 3d20 6e65 7720 4861 6e64 736f 6e74  t = new Handsont
-00001720: 6162 6c65 2863 6f6e 7461 696e 6572 2c20  able(container, 
-00001730: 7b0a 2020 2020 2020 7769 6474 683a 2027  {.      width: '
-00001740: 3130 3025 272c 0a20 2020 2020 2072 6f77  100%',.      row
-00001750: 4865 6164 6572 733a 2074 7275 652c 0a20  Headers: true,. 
-00001760: 2020 2020 2063 6f6c 4865 6164 6572 733a       colHeaders:
-00001770: 205b 0a20 2020 2020 2020 2027 4369 7479   [.        'City
-00001780: 272c 0a20 2020 2020 2020 2027 4d69 6e20  ',.        'Min 
-00001790: 5465 6d70 272c 0a20 2020 2020 2020 2027  Temp',.        '
-000017a0: 4d61 7820 5465 6d70 272c 0a20 2020 2020  Max Temp',.     
-000017b0: 2020 2027 436f 6e64 6974 696f 6e27 5d2c     'Condition'],
-000017c0: 0a20 2020 2020 2063 6f6c 756d 6e73 3a20  .      columns: 
-000017d0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
-000017e0: 2020 2020 2020 7479 7065 3a20 2764 726f        type: 'dro
-000017f0: 7064 6f77 6e27 2c0a 2020 2020 2020 2020  pdown',.        
-00001800: 2020 736f 7572 6365 3a20 6369 7479 5f6c    source: city_l
-00001810: 732e 6d61 7028 6369 7479 203d 3e20 6369  s.map(city => ci
-00001820: 7479 2e66 6965 6c64 732e 6e61 6d65 292c  ty.fields.name),
-00001830: 0a20 2020 2020 2020 2020 2061 6c6c 6f77  .          allow
-00001840: 456d 7074 793a 2066 616c 7365 2c0a 2020  Empty: false,.  
-00001850: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001860: 207b 0a20 2020 2020 2020 2020 2074 7970   {.          typ
-00001870: 653a 2027 6e75 6d65 7269 6327 2c0a 2020  e: 'numeric',.  
-00001880: 2020 2020 2020 2020 616c 6c6f 7745 6d70          allowEmp
-00001890: 7479 3a20 6661 6c73 652c 0a20 2020 2020  ty: false,.     
-000018a0: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
-000018b0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000018c0: 276e 756d 6572 6963 272c 0a20 2020 2020  'numeric',.     
-000018d0: 2020 2020 2061 6c6c 6f77 456d 7074 793a       allowEmpty:
-000018e0: 2066 616c 7365 2c0a 2020 2020 2020 2020   false,.        
-000018f0: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
-00001900: 2020 2020 2020 2074 7970 653a 2027 6472         type: 'dr
-00001910: 6f70 646f 776e 272c 0a20 2020 2020 2020  opdown',.       
-00001920: 2020 2073 6f75 7263 653a 2077 6561 7468     source: weath
-00001930: 6572 5f63 6f6e 6469 7469 6f6e 5f6c 732c  er_condition_ls,
-00001940: 0a20 2020 2020 2020 2020 2061 6c6c 6f77  .          allow
-00001950: 456d 7074 793a 2066 616c 7365 2c0a 2020  Empty: false,.  
-00001960: 2020 2020 2020 7d2c 0a20 2020 2020 205d        },.      ]
-00001970: 2c0a 2020 2020 2020 6461 7461 3a20 5b5d  ,.      data: []
-00001980: 2c0a 2020 2020 2020 2f2f 2064 726f 7064  ,.      // dropd
-00001990: 6f77 6e4d 656e 753a 2074 7275 652c 0a20  ownMenu: true,. 
-000019a0: 2020 2020 206d 756c 7469 436f 6c75 6d6e       multiColumn
-000019b0: 536f 7274 696e 673a 2074 7275 652c 0a20  Sorting: true,. 
-000019c0: 2020 2020 202f 2f20 6669 6c74 6572 733a       // filters:
-000019d0: 2074 7275 652c 0a20 2020 2020 2061 6c6c   true,.      all
-000019e0: 6f77 496e 7661 6c69 643a 2074 7275 652c  owInvalid: true,
-000019f0: 0a20 2020 2020 206d 696e 5370 6172 6552  .      minSpareR
-00001a00: 6f77 733a 2031 2c0a 2020 2020 2020 6865  ows: 1,.      he
-00001a10: 6967 6874 3a20 2761 7574 6f27 2c0a 2020  ight: 'auto',.  
-00001a20: 2020 2020 7374 7265 7463 6848 3a20 2261      stretchH: "a
-00001a30: 6c6c 222c 0a20 2020 2020 206c 6963 656e  ll",.      licen
-00001a40: 7365 4b65 793a 2027 6e6f 6e2d 636f 6d6d  seKey: 'non-comm
-00001a50: 6572 6369 616c 2d61 6e64 2d65 7661 6c75  ercial-and-evalu
-00001a60: 6174 696f 6e27 202f 2f20 666f 7220 6e6f  ation' // for no
-00001a70: 6e2d 636f 6d6d 6572 6369 616c 2075 7365  n-commercial use
-00001a80: 206f 6e6c 790a 2020 2020 7d29 3b0a 0a20   only.    });.. 
-00001a90: 2020 2063 6f6e 7374 2063 6f6c 756d 6e5f     const column_
-00001aa0: 7365 6c65 6374 6f72 7320 3d20 5b0a 2020  selectors = [.  
-00001ab0: 2020 2020 7b64 6f6d 5f69 643a 2763 6974      {dom_id:'cit
-00001ac0: 7927 2c20 696e 6465 783a 307d 2c0a 2020  y', index:0},.  
-00001ad0: 2020 2020 7b64 6f6d 5f69 643a 276d 696e      {dom_id:'min
-00001ae0: 5465 6d70 272c 2069 6e64 6578 3a31 7d2c  Temp', index:1},
-00001af0: 0a20 2020 2020 207b 646f 6d5f 6964 3a27  .      {dom_id:'
-00001b00: 6d61 7854 656d 7027 2c20 696e 6465 783a  maxTemp', index:
-00001b10: 327d 2c0a 2020 2020 2020 7b64 6f6d 5f69  2},.      {dom_i
-00001b20: 643a 2763 6f6e 6469 7469 6f6e 272c 2069  d:'condition', i
-00001b30: 6e64 6578 3a33 7d2c 0a20 2020 205d 0a0a  ndex:3},.    ]..
-00001b40: 2020 2020 646f 6375 6d65 6e74 2e67 6574      document.get
-00001b50: 456c 656d 656e 7442 7949 6428 2769 645f  ElementById('id_
-00001b60: 6373 7627 292e 6164 6445 7665 6e74 4c69  csv').addEventLi
-00001b70: 7374 656e 6572 2827 6368 616e 6765 272c  stener('change',
-00001b80: 2066 756e 6374 696f 6e20 2865 2920 7b0a   function (e) {.
-00001b90: 2020 2020 2020 7661 7220 6669 6c65 203d        var file =
-00001ba0: 2065 2e74 6172 6765 742e 6669 6c65 735b   e.target.files[
-00001bb0: 305d 3b0a 2020 2020 2020 7661 7220 7265  0];.      var re
-00001bc0: 6164 6572 203d 206e 6577 2046 696c 6552  ader = new FileR
-00001bd0: 6561 6465 7228 293b 0a0a 2020 2020 2020  eader();..      
-00001be0: 7265 6164 6572 2e6f 6e6c 6f61 6420 3d20  reader.onload = 
-00001bf0: 6675 6e63 7469 6f6e 2028 6576 656e 7429  function (event)
-00001c00: 207b 0a20 2020 2020 2020 2076 6172 2063   {.        var c
-00001c10: 7376 4461 7461 203d 2065 7665 6e74 2e74  svData = event.t
-00001c20: 6172 6765 742e 7265 7375 6c74 3b0a 2020  arget.result;.  
-00001c30: 2020 2020 2020 7661 7220 6c69 6e65 7320        var lines 
-00001c40: 3d20 6373 7644 6174 612e 7370 6c69 7428  = csvData.split(
-00001c50: 275c 6e27 293b 0a20 2020 2020 2020 2076  '\n');.        v
-00001c60: 6172 2063 6f6c 756d 6e48 6561 6465 7273  ar columnHeaders
-00001c70: 203d 206c 696e 6573 5b30 5d2e 7370 6c69   = lines[0].spli
-00001c80: 7428 272c 2729 3b0a 2020 2020 2020 2020  t(',');.        
-00001c90: 2428 2723 6865 6164 6572 5f73 6563 7469  $('#header_secti
-00001ca0: 6f6e 2729 2e73 686f 7728 290a 0a20 2020  on').show()..   
-00001cb0: 2020 2020 2076 6172 2063 6f6e 7465 6e74       var content
-00001cc0: 7320 3d20 6576 656e 742e 7461 7267 6574  s = event.target
-00001cd0: 2e72 6573 756c 743b 0a20 2020 2020 2020  .result;.       
-00001ce0: 2076 6172 2064 6174 6120 3d20 7061 7273   var data = pars
-00001cf0: 6543 5356 2863 6f6e 7465 6e74 7329 3b0a  eCSV(contents);.
-00001d00: 0a20 2020 2020 2020 2068 6f74 2e75 7064  .        hot.upd
-00001d10: 6174 6544 6174 6128 6461 7461 290a 0a20  ateData(data).. 
-00001d20: 2020 2020 2020 2063 6f6c 756d 6e5f 7365         column_se
-00001d30: 6c65 6374 6f72 732e 6d61 7028 636f 6c75  lectors.map(colu
-00001d40: 6d6e 203d 3e20 7b0a 0a20 2020 2020 2020  mn => {..       
-00001d50: 2020 202f 2f20 7072 6570 6f70 756c 6174     // prepopulat
-00001d60: 6520 7365 6c65 6374 2077 6974 6820 6f70  e select with op
-00001d70: 7469 6f6e 7320 6279 206f 7264 6572 200a  tions by order .
-00001d80: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
-00001d90: 7465 5365 6c65 6374 496e 7075 7428 636f  teSelectInput(co
-00001da0: 6c75 6d6e 2e64 6f6d 5f69 642c 2063 6f6c  lumn.dom_id, col
-00001db0: 756d 6e48 6561 6465 7273 2c20 636f 6c75  umnHeaders, colu
-00001dc0: 6d6e 2e69 6e64 6578 290a 2020 2020 2020  mn.index).      
-00001dd0: 2020 2020 646f 6375 6d65 6e74 2e67 6574      document.get
-00001de0: 456c 656d 656e 7442 7949 6428 636f 6c75  ElementById(colu
-00001df0: 6d6e 2e64 6f6d 5f69 6429 2e61 6464 4576  mn.dom_id).addEv
-00001e00: 656e 744c 6973 7465 6e65 7228 2763 6861  entListener('cha
-00001e10: 6e67 6527 2c20 6675 6e63 7469 6f6e 2865  nge', function(e
-00001e20: 297b 0a0a 2020 2020 2020 2020 2020 2020  ){..            
-00001e30: 7661 7220 7461 626c 655f 6461 7461 203d  var table_data =
-00001e40: 2068 6f74 2e67 6574 4461 7461 2829 0a20   hot.getData(). 
-00001e50: 200a 2020 2020 2020 2020 2020 2020 7661   .            va
-00001e60: 7220 636f 6c75 6d6e 5f61 7272 203d 205b  r column_arr = [
-00001e70: 5d0a 2020 2020 2020 2020 2020 2020 636f  ].            co
-00001e80: 6e73 7420 7265 6172 7261 6e67 6564 4172  nst rearrangedAr
-00001e90: 7220 3d20 6461 7461 2e6d 6170 2861 7272  r = data.map(arr
-00001ea0: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-00001eb0: 2020 2020 636f 6c75 6d6e 5f61 7272 2e70      column_arr.p
-00001ec0: 7573 6828 6172 725b 652e 7461 7267 6574  ush(arr[e.target
-00001ed0: 2e76 616c 7565 5d29 0a20 2020 2020 2020  .value]).       
-00001ee0: 2020 2020 207d 290a 2020 0a20 2020 2020       }).  .     
-00001ef0: 2020 2020 2020 2074 6162 6c65 5f64 6174         table_dat
-00001f00: 612e 7265 706c 6163 655f 6461 7461 2863  a.replace_data(c
-00001f10: 6f6c 756d 6e2e 696e 6465 782c 636f 6c75  olumn.index,colu
-00001f20: 6d6e 5f61 7272 2029 0a20 200a 2020 2020  mn_arr ).  .    
-00001f30: 2020 2020 2020 2020 686f 742e 7570 6461          hot.upda
-00001f40: 7465 4461 7461 2874 6162 6c65 5f64 6174  teData(table_dat
-00001f50: 6129 0a20 2020 200a 2020 2020 2020 2020  a).    .        
-00001f60: 2020 7d29 0a0a 2020 2020 2020 2020 2020    })..          
-00001f70: 7265 7475 726e 2063 6f6c 756d 6e0a 2020  return column.  
-00001f80: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001f90: 2020 200a 2020 2020 2020 2020 7d20 290a     .        } ).
-00001fa0: 0a20 2020 2020 2020 202f 2f20 7265 6f72  .        // reor
-00001fb0: 6465 725f 636f 6c75 6d6e 7328 6461 7461  der_columns(data
-00001fc0: 2c20 2763 6974 7927 2c20 3029 0a20 2020  , 'city', 0).   
-00001fd0: 2020 2020 200a 2020 2020 2020 7d3b 0a0a       .      };..
-00001fe0: 2020 2020 2020 7265 6164 6572 2e72 6561        reader.rea
-00001ff0: 6441 7354 6578 7428 6669 6c65 293b 0a0a  dAsText(file);..
-00002000: 2020 2020 7d29 3b0a 0a0a 2020 2020 646f      });...    do
-00002010: 6375 6d65 6e74 2e67 6574 456c 656d 656e  cument.getElemen
-00002020: 7442 7949 6428 2766 6f72 6563 6173 745f  tById('forecast_
-00002030: 666f 726d 2729 2e61 6464 4576 656e 744c  form').addEventL
-00002040: 6973 7465 6e65 7228 2773 7562 6d69 7427  istener('submit'
-00002050: 2c20 6675 6e63 7469 6f6e 2028 6576 656e  , function (even
-00002060: 7429 207b 0a20 2020 2020 2065 7665 6e74  t) {.      event
-00002070: 2e70 7265 7665 6e74 4465 6661 756c 7428  .preventDefault(
-00002080: 293b 0a0a 2020 2020 2020 7661 7220 6461  );..      var da
-00002090: 7461 203d 2068 6f74 2e67 6574 4461 7461  ta = hot.getData
-000020a0: 2829 3b0a 0a20 2020 2020 202f 2f20 4669  ();..      // Fi
-000020b0: 6c74 6572 206f 7574 2072 6f77 7320 7468  lter out rows th
-000020c0: 6174 2068 6176 6520 616c 6c20 7661 6c75  at have all valu
-000020d0: 6573 206e 756c 6c20 6f72 2075 6e64 6566  es null or undef
-000020e0: 696e 6564 0a20 2020 2020 206e 6f6e 4e75  ined.      nonNu
-000020f0: 6c6c 526f 7773 203d 2064 6174 612e 6669  llRows = data.fi
-00002100: 6c74 6572 2866 756e 6374 696f 6e20 2872  lter(function (r
-00002110: 6f77 2920 7b0a 2020 2020 2020 2020 7265  ow) {.        re
-00002120: 7475 726e 2072 6f77 2e73 6f6d 6528 6675  turn row.some(fu
-00002130: 6e63 7469 6f6e 2028 6365 6c6c 2920 7b0a  nction (cell) {.
-00002140: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002150: 2063 656c 6c20 213d 3d20 6e75 6c6c 2026   cell !== null &
-00002160: 2620 6365 6c6c 2021 3d3d 2075 6e64 6566  & cell !== undef
-00002170: 696e 6564 2026 2620 6365 6c6c 2021 3d3d  ined && cell !==
-00002180: 2027 273b 0a20 2020 2020 2020 207d 293b   '';.        });
-00002190: 0a20 2020 2020 207d 293b 0a0a 2020 2020  .      });..    
-000021a0: 2020 2f2f 2056 616c 6964 6174 6520 7468    // Validate th
-000021b0: 6520 6461 7461 0a20 2020 2020 2076 6172  e data.      var
-000021c0: 2069 7356 616c 6964 203d 2076 616c 6964   isValid = valid
-000021d0: 6174 6544 6174 6128 293b 0a0a 2020 2020  ateData();..    
-000021e0: 2020 2f2f 2043 7265 6174 6520 616e 2061    // Create an a
-000021f0: 7272 6179 206f 6620 6f62 6a65 6374 7320  rray of objects 
-00002200: 7769 7468 2074 6865 2063 6f6c 756d 6e20  with the column 
-00002210: 6e61 6d65 7320 6173 206b 6579 730a 2020  names as keys.  
-00002220: 2020 2020 7661 7220 706f 7374 4461 7461      var postData
-00002230: 203d 205b 5d3b 0a20 2020 2020 202f 2f20   = [];.      // 
-00002240: 5265 7472 6965 7665 2074 6865 2073 7065  Retrieve the spe
-00002250: 6369 6669 6320 696e 7075 7420 7661 6c75  cific input valu
-00002260: 650a 2020 2020 2020 7661 7220 666f 7265  e.      var fore
-00002270: 6361 7374 5f64 6174 6520 3d20 646f 6375  cast_date = docu
-00002280: 6d65 6e74 2e67 6574 456c 656d 656e 7442  ment.getElementB
-00002290: 7949 6428 2269 645f 6461 7465 2229 2e76  yId("id_date").v
-000022a0: 616c 7565 3b0a 0a20 2020 2020 2069 6620  alue;..      if 
-000022b0: 286e 6f6e 4e75 6c6c 526f 7773 2e6c 656e  (nonNullRows.len
-000022c0: 6774 6820 3e20 3029 207b 0a0a 2020 2020  gth > 0) {..    
-000022d0: 2020 2020 666f 7220 2876 6172 2069 203d      for (var i =
-000022e0: 2030 3b20 6920 3c20 6e6f 6e4e 756c 6c52   0; i < nonNullR
-000022f0: 6f77 732e 6c65 6e67 7468 3b20 692b 2b29  ows.length; i++)
-00002300: 207b 0a20 2020 2020 2020 2020 2076 6172   {.          var
-00002310: 2072 6f77 203d 207b 0a20 2020 2020 2020   row = {.       
-00002320: 2020 2020 2027 6369 7479 273a 2063 6974       'city': cit
-00002330: 795f 6c73 2e66 696e 6428 6369 7479 203d  y_ls.find(city =
-00002340: 3e20 6369 7479 2e66 6965 6c64 732e 6e61  > city.fields.na
-00002350: 6d65 203d 3d3d 206e 6f6e 4e75 6c6c 526f  me === nonNullRo
-00002360: 7773 5b69 5d5b 305d 292e 706b 2c0a 2020  ws[i][0]).pk,.  
-00002370: 2020 2020 2020 2020 2020 276d 696e 5f74            'min_t
-00002380: 656d 7027 3a20 6e6f 6e4e 756c 6c52 6f77  emp': nonNullRow
-00002390: 735b 695d 5b31 5d2c 0a20 2020 2020 2020  s[i][1],.       
-000023a0: 2020 2020 2027 6d61 785f 7465 6d70 273a       'max_temp':
-000023b0: 206e 6f6e 4e75 6c6c 526f 7773 5b69 5d5b   nonNullRows[i][
-000023c0: 325d 2c0a 2020 2020 2020 2020 2020 2020  2],.            
-000023d0: 2763 6f6e 6469 7469 6f6e 273a 206e 6f6e  'condition': non
-000023e0: 4e75 6c6c 526f 7773 5b69 5d5b 335d 2c0a  NullRows[i][3],.
-000023f0: 2020 2020 2020 2020 2020 2020 2766 6f72              'for
-00002400: 6563 6173 745f 6461 7465 273a 2066 6f72  ecast_date': for
-00002410: 6563 6173 745f 6461 7465 2c0a 2020 2020  ecast_date,.    
-00002420: 2020 2020 2020 7d3b 0a20 2020 2020 2020        };.       
-00002430: 2020 2070 6f73 7444 6174 612e 7075 7368     postData.push
-00002440: 2872 6f77 293b 0a0a 2020 2020 2020 2020  (row);..        
-00002450: 7d0a 0a20 2020 2020 2020 202f 2f20 5365  }..        // Se
-00002460: 6e64 2074 6865 204a 534f 4e20 6461 7461  nd the JSON data
-00002470: 2074 6f20 6120 446a 616e 676f 2076 6965   to a Django vie
-00002480: 7720 7669 6120 414a 4158 0a20 2020 2020  w via AJAX.     
-00002490: 2020 2024 2e61 6a61 7828 7b0a 2020 2020     $.ajax({.    
-000024a0: 2020 2020 2020 7572 6c3a 2060 7b25 2075        url: `{% u
-000024b0: 726c 2027 666f 7265 6361 7374 2d6c 6973  rl 'forecast-lis
-000024c0: 7427 257d 602c 0a20 2020 2020 2020 2020  t'%}`,.         
-000024d0: 2074 7970 653a 2027 504f 5354 272c 0a20   type: 'POST',. 
-000024e0: 2020 2020 2020 2020 2068 6561 6465 7273           headers
-000024f0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00002500: 2758 2d43 5352 4654 6f6b 656e 273a 2027  'X-CSRFToken': '
-00002510: 7b7b 2063 7372 665f 746f 6b65 6e20 7d7d  {{ csrf_token }}
-00002520: 272c 2020 2f2f 2052 6570 6c61 6365 2077  ',  // Replace w
-00002530: 6974 6820 7468 6520 6163 7475 616c 2043  ith the actual C
-00002540: 5352 4620 746f 6b65 6e20 7661 6c75 650a  SRF token value.
-00002550: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00002560: 2020 2020 2020 2064 6174 613a 204a 534f         data: JSO
-00002570: 4e2e 7374 7269 6e67 6966 7928 706f 7374  N.stringify(post
-00002580: 4461 7461 292c 0a20 2020 2020 2020 2020  Data),.         
-00002590: 2063 6f6e 7465 6e74 5479 7065 3a20 2761   contentType: 'a
-000025a0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e27  pplication/json'
-000025b0: 2c0a 2020 2020 2020 2020 2020 7375 6363  ,.          succ
-000025c0: 6573 733a 2066 756e 6374 696f 6e20 2872  ess: function (r
-000025d0: 6573 706f 6e73 6529 207b 0a20 2020 2020  esponse) {.     
-000025e0: 2020 2020 2020 202f 2f20 436c 6561 7220         // Clear 
-000025f0: 7468 6520 4861 6e64 736f 6e74 6162 6c65  the Handsontable
-00002600: 2074 6162 6c65 0a20 2020 2020 2020 2020   table.         
-00002610: 2020 2024 2827 2363 7265 6174 5375 6363     $('#creatSucc
-00002620: 6573 7327 292e 7368 6f77 2827 736c 6f77  ess').show('slow
-00002630: 2729 0a0a 2020 2020 2020 2020 2020 2020  ')..            
-00002640: 7365 7454 696d 656f 7574 2866 756e 6374  setTimeout(funct
-00002650: 696f 6e20 2829 207b 0a20 2020 2020 2020  ion () {.       
-00002660: 2020 2020 2020 2024 2827 2363 7265 6174         $('#creat
-00002670: 5375 6363 6573 7327 292e 6869 6465 2827  Success').hide('
-00002680: 736c 6f77 2729 0a0a 2020 2020 2020 2020  slow')..        
-00002690: 2020 2020 7d2c 2035 3030 3029 0a0a 2020      }, 5000)..  
-000026a0: 2020 2020 2020 2020 2020 2f2f 636c 6561            //clea
-000026b0: 7220 7461 626c 6520 6f6e 2073 7563 6365  r table on succe
-000026c0: 7373 6675 6c20 7375 626d 6973 7369 6f6e  ssful submission
-000026d0: 0a20 2020 2020 2020 2020 2020 2068 6f74  .            hot
-000026e0: 2e75 7064 6174 6544 6174 6128 5b5d 290a  .updateData([]).
-000026f0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00002700: 2020 2020 2020 2065 7272 6f72 3a20 6675         error: fu
-00002710: 6e63 7469 6f6e 2028 6a71 5848 522c 2074  nction (jqXHR, t
-00002720: 6578 7453 7461 7475 732c 2065 7272 6f72  extStatus, error
-00002730: 5468 726f 776e 2920 7b0a 200a 2020 2020  Thrown) {. .    
-00002740: 2020 2020 2020 2020 6966 2028 6572 726f          if (erro
-00002750: 7254 6872 6f77 6e29 207b 0a20 2020 2020  rThrown) {.     
-00002760: 2020 2020 2020 2020 2024 2827 2363 7265           $('#cre
-00002770: 6174 4572 726f 7227 292e 7368 6f77 2827  atError').show('
-00002780: 736c 6f77 2729 0a20 2020 2020 2020 2020  slow').         
-00002790: 2020 2020 2024 2827 2363 7265 6174 4572       $('#creatEr
-000027a0: 726f 7227 292e 6874 6d6c 2820 4a53 4f4e  ror').html( JSON
-000027b0: 2e70 6172 7365 286a 7158 4852 2e72 6573  .parse(jqXHR.res
-000027c0: 706f 6e73 6554 6578 7429 2e65 7272 6f72  ponseText).error
-000027d0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-000027e0: 2073 6574 5469 6d65 6f75 7428 6675 6e63   setTimeout(func
-000027f0: 7469 6f6e 2028 2920 7b0a 2020 2020 2020  tion () {.      
-00002800: 2020 2020 2020 2020 2020 2428 2723 6372            $('#cr
-00002810: 6561 7445 7272 6f72 2729 2e68 6964 6528  eatError').hide(
-00002820: 2773 6c6f 7727 290a 0a20 2020 2020 2020  'slow')..       
-00002830: 2020 2020 2020 207d 2c20 3530 3030 290a         }, 5000).
-00002840: 0a20 2020 2020 2020 2020 2020 207d 0a0a  .            }..
-00002850: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00002860: 2020 2020 7d29 0a0a 2020 2020 2020 7d20      })..      } 
-00002870: 656c 7365 207b 0a20 2020 2020 2020 2024  else {.        $
-00002880: 2827 2363 7265 6174 4572 726f 7227 292e  ('#creatError').
-00002890: 7368 6f77 2827 736c 6f77 2729 0a20 2020  show('slow').   
-000028a0: 2020 2020 2024 2827 2363 7265 6174 4572       $('#creatEr
-000028b0: 726f 7227 292e 6874 6d6c 2827 5468 6520  ror').html('The 
-000028c0: 7461 626c 6520 6973 2065 6d70 7479 2e20  table is empty. 
-000028d0: 506c 6561 7365 2069 6e70 7574 2064 6174  Please input dat
-000028e0: 6127 290a 0a20 2020 2020 2020 2073 6574  a')..        set
-000028f0: 5469 6d65 6f75 7428 6675 6e63 7469 6f6e  Timeout(function
-00002900: 2028 2920 7b0a 2020 2020 2020 2020 2020   () {.          
-00002910: 2428 2723 6372 6561 7445 7272 6f72 2729  $('#creatError')
-00002920: 2e68 6964 6528 2773 6c6f 7727 290a 0a20  .hide('slow').. 
-00002930: 2020 2020 2020 207d 2c20 3530 3030 290a         }, 5000).
-00002940: 2020 2020 2020 7d0a 0a20 2020 207d 290a        }..    }).
-00002950: 0a20 2020 2066 756e 6374 696f 6e20 7661  .    function va
-00002960: 6c69 6461 7465 4461 7461 2829 207b 0a20  lidateData() {. 
-00002970: 2020 2020 2076 6172 2069 6e73 7461 6e63       var instanc
-00002980: 6520 3d20 686f 742e 6765 7449 6e73 7461  e = hot.getInsta
-00002990: 6e63 6528 293b 0a20 2020 2020 2076 6172  nce();.      var
-000029a0: 2068 6173 4572 726f 7220 3d20 6661 6c73   hasError = fals
-000029b0: 653b 202f 2f20 4173 7375 6d65 206e 6f20  e; // Assume no 
-000029c0: 6572 726f 7273 2069 6e69 7469 616c 6c79  errors initially
-000029d0: 0a20 200a 2020 2020 2020 666f 7220 2876  .  .      for (v
-000029e0: 6172 2069 203d 2030 3b20 6920 3c20 696e  ar i = 0; i < in
-000029f0: 7374 616e 6365 2e63 6f75 6e74 526f 7773  stance.countRows
-00002a00: 2829 3b20 692b 2b29 207b 0a20 2020 2020  (); i++) {.     
-00002a10: 2020 2076 6172 2072 6f77 4861 7356 616c     var rowHasVal
-00002a20: 7565 203d 2066 616c 7365 3b20 2f2f 2041  ue = false; // A
-00002a30: 7373 756d 6520 7468 6520 726f 7720 6973  ssume the row is
-00002a40: 2065 6d70 7479 2069 6e69 7469 616c 6c79   empty initially
-00002a50: 0a20 200a 2020 2020 2020 2020 666f 7220  .  .        for 
-00002a60: 2876 6172 206a 203d 2030 3b20 6a20 3c20  (var j = 0; j < 
-00002a70: 696e 7374 616e 6365 2e63 6f75 6e74 436f  instance.countCo
-00002a80: 6c73 2829 3b20 6a2b 2b29 207b 0a20 2020  ls(); j++) {.   
-00002a90: 2020 2020 2020 2076 6172 2063 656c 6c44         var cellD
-00002aa0: 6174 6120 3d20 696e 7374 616e 6365 2e67  ata = instance.g
-00002ab0: 6574 4461 7461 4174 4365 6c6c 2869 2c20  etDataAtCell(i, 
-00002ac0: 6a29 3b0a 2020 0a20 2020 2020 2020 2020  j);.  .         
-00002ad0: 202f 2f20 4368 6563 6b20 6966 2074 6865   // Check if the
-00002ae0: 2063 656c 6c20 6973 206e 6f74 206e 756c   cell is not nul
-00002af0: 6c20 6f72 2065 6d70 7479 2073 7472 696e  l or empty strin
-00002b00: 670a 2020 2020 2020 2020 2020 6966 2028  g.          if (
-00002b10: 6365 6c6c 4461 7461 2021 3d3d 206e 756c  cellData !== nul
-00002b20: 6c20 2626 2063 656c 6c44 6174 6120 213d  l && cellData !=
-00002b30: 3d20 2727 2920 7b0a 2020 2020 2020 2020  = '') {.        
-00002b40: 2020 2020 726f 7748 6173 5661 6c75 6520      rowHasValue 
-00002b50: 3d20 7472 7565 3b20 2f2f 204d 6172 6b20  = true; // Mark 
-00002b60: 7468 6520 726f 7720 6173 206e 6f6e 2d65  the row as non-e
-00002b70: 6d70 7479 0a20 200a 2020 2020 2020 2020  mpty.  .        
-00002b80: 2020 2020 696e 7374 616e 6365 2e73 6574      instance.set
-00002b90: 4365 6c6c 4d65 7461 2869 2c20 6a2c 2027  CellMeta(i, j, '
-00002ba0: 7661 6c69 6427 2c20 7472 7565 293b 0a20  valid', true);. 
-00002bb0: 2020 2020 2020 2020 2020 2069 6e73 7461             insta
-00002bc0: 6e63 652e 7365 7443 656c 6c4d 6574 6128  nce.setCellMeta(
-00002bd0: 692c 206a 2c20 2763 6f6d 6d65 6e74 272c  i, j, 'comment',
-00002be0: 2027 2729 3b0a 2020 2020 2020 2020 2020   '');.          
-00002bf0: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
-00002c00: 2020 2020 2069 6e73 7461 6e63 652e 7365       instance.se
-00002c10: 7443 656c 6c4d 6574 6128 692c 206a 2c20  tCellMeta(i, j, 
-00002c20: 2776 616c 6964 272c 2074 7275 6529 3b0a  'valid', true);.
-00002c30: 2020 2020 2020 2020 2020 2020 696e 7374              inst
-00002c40: 616e 6365 2e73 6574 4365 6c6c 4d65 7461  ance.setCellMeta
-00002c50: 2869 2c20 6a2c 2027 636f 6d6d 656e 7427  (i, j, 'comment'
-00002c60: 2c20 2727 293b 0a20 2020 2020 2020 2020  , '');.         
-00002c70: 207d 0a20 2020 2020 2020 207d 0a20 200a   }.        }.  .
-00002c80: 2020 2020 2020 2020 2f2f 204f 6e6c 7920          // Only 
-00002c90: 7661 6c69 6461 7465 2074 6865 2072 6f77  validate the row
-00002ca0: 2069 6620 6974 2068 6173 2061 7420 6c65   if it has at le
-00002cb0: 6173 7420 6f6e 6520 6e6f 6e2d 656d 7074  ast one non-empt
-00002cc0: 7920 6365 6c6c 0a20 2020 2020 2020 2069  y cell.        i
-00002cd0: 6620 2872 6f77 4861 7356 616c 7565 2920  f (rowHasValue) 
-00002ce0: 7b0a 2020 2020 2020 2020 2020 696e 7374  {.          inst
-00002cf0: 616e 6365 2e76 616c 6964 6174 6552 6f77  ance.validateRow
-00002d00: 7328 5b69 5d29 3b0a 2020 2020 2020 2020  s([i]);.        
-00002d10: 2020 6966 2028 696e 7374 616e 6365 2e67    if (instance.g
-00002d20: 6574 4365 6c6c 4d65 7461 2869 2c20 3029  etCellMeta(i, 0)
-00002d30: 2e76 616c 6964 203d 3d3d 2066 616c 7365  .valid === false
-00002d40: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00002d50: 6861 7345 7272 6f72 203d 2074 7275 653b  hasError = true;
-00002d60: 202f 2f20 4d61 726b 2074 6861 7420 7468   // Mark that th
-00002d70: 6572 6520 6973 2061 6e20 6572 726f 720a  ere is an error.
-00002d80: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00002d90: 2020 2020 7d0a 2020 2020 2020 7d0a 2020      }.      }.  
-00002da0: 0a20 2020 2020 202f 2f20 5265 2d72 656e  .      // Re-ren
-00002db0: 6465 7220 7468 6520 7461 626c 6520 746f  der the table to
-00002dc0: 2064 6973 706c 6179 2074 6865 2076 616c   display the val
-00002dd0: 6964 6174 696f 6e20 6665 6564 6261 636b  idation feedback
-00002de0: 0a20 2020 2020 2069 6e73 7461 6e63 652e  .      instance.
-00002df0: 7265 6e64 6572 2829 3b0a 2020 0a20 2020  render();.  .   
-00002e00: 2020 202f 2f20 5368 6f77 2074 6865 206f     // Show the o
-00002e10: 7665 7261 6c6c 2065 7272 6f72 206d 6573  verall error mes
-00002e20: 7361 6765 2069 6620 7468 6572 6520 6973  sage if there is
-00002e30: 2061 6e20 6572 726f 720a 2020 2020 2020   an error.      
-00002e40: 7265 7475 726e 2068 6173 4572 726f 720a  return hasError.
-00002e50: 2020 2020 7d0a 2020 2020 0a0a 636f 6e73      }.    ..cons
-00002e60: 7420 6578 706f 7274 5465 6d70 6c61 7465  t exportTemplate
-00002e70: 203d 206e 6577 2048 616e 6473 6f6e 7461   = new Handsonta
-00002e80: 626c 6528 646f 6375 6d65 6e74 2e67 6574  ble(document.get
-00002e90: 456c 656d 656e 7442 7949 6428 2765 7870  ElementById('exp
-00002ea0: 6f72 7454 656d 706c 6174 6527 292c 207b  ortTemplate'), {
-00002eb0: 0a20 2020 2020 2063 6f6c 4865 6164 6572  .      colHeader
-00002ec0: 733a 205b 0a20 2020 2020 2020 2027 4369  s: [.        'Ci
-00002ed0: 7479 272c 0a20 2020 2020 2020 2027 4d69  ty',.        'Mi
-00002ee0: 6e20 5465 6d70 272c 0a20 2020 2020 2020  n Temp',.       
-00002ef0: 2027 4d61 7820 5465 6d70 272c 0a20 2020   'Max Temp',.   
-00002f00: 2020 2020 2027 436f 6e64 6974 696f 6e27       'Condition'
-00002f10: 5d2c 0a20 2020 2020 2063 6f6c 756d 6e73  ],.      columns
-00002f20: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-00002f30: 2020 2020 2020 2020 7479 7065 3a20 2764          type: 'd
-00002f40: 726f 7064 6f77 6e27 2c0a 2020 2020 2020  ropdown',.      
-00002f50: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00002f60: 2020 2020 2020 2020 2074 7970 653a 2027           type: '
-00002f70: 6e75 6d65 7269 6327 2c0a 2020 2020 2020  numeric',.      
-00002f80: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00002f90: 2020 2020 2020 2020 2074 7970 653a 2027           type: '
-00002fa0: 6e75 6d65 7269 6327 2c0a 2020 2020 2020  numeric',.      
-00002fb0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00002fc0: 2020 2020 2020 2020 2074 7970 653a 2027           type: '
-00002fd0: 6472 6f70 646f 776e 272c 0a0a 2020 2020  dropdown',..    
-00002fe0: 2020 2020 7d2c 0a20 2020 2020 205d 2c0a      },.      ],.
-00002ff0: 2020 2020 2020 6461 7461 3a20 5b0a 0a20        data: [.. 
-00003000: 2020 2020 205d 2c0a 2020 2020 2020 2f2f       ],.      //
-00003010: 2064 726f 7064 6f77 6e4d 656e 753a 2074   dropdownMenu: t
-00003020: 7275 652c 0a20 2020 2020 202f 2f20 6669  rue,.      // fi
-00003030: 6c74 6572 733a 2074 7275 652c 0a20 2020  lters: true,.   
-00003040: 2020 206d 696e 5370 6172 6552 6f77 733a     minSpareRows:
-00003050: 2031 302c 0a20 2020 2020 206c 6963 656e   10,.      licen
-00003060: 7365 4b65 793a 2027 6e6f 6e2d 636f 6d6d  seKey: 'non-comm
-00003070: 6572 6369 616c 2d61 6e64 2d65 7661 6c75  ercial-and-evalu
-00003080: 6174 696f 6e27 202f 2f20 666f 7220 6e6f  ation' // for no
-00003090: 6e2d 636f 6d6d 6572 6369 616c 2075 7365  n-commercial use
-000030a0: 206f 6e6c 790a 2020 2020 7d29 3b0a 0a20   only.    });.. 
-000030b0: 2020 2063 6f6e 7374 2065 7870 6f72 7450     const exportP
-000030c0: 6c75 6769 6e20 3d20 6578 706f 7274 5465  lugin = exportTe
-000030d0: 6d70 6c61 7465 2e67 6574 506c 7567 696e  mplate.getPlugin
-000030e0: 2827 6578 706f 7274 4669 6c65 2729 3b0a  ('exportFile');.
-000030f0: 0a20 2020 2064 6f63 756d 656e 742e 6765  .    document.ge
-00003100: 7445 6c65 6d65 6e74 4279 4964 2827 6578  tElementById('ex
-00003110: 706f 7274 5461 626c 6527 292e 6164 6445  portTable').addE
-00003120: 7665 6e74 4c69 7374 656e 6572 2827 636c  ventListener('cl
-00003130: 6963 6b27 2c20 6675 6e63 7469 6f6e 2028  ick', function (
-00003140: 2920 7b0a 2020 2020 2020 7661 7220 6578  ) {.      var ex
-00003150: 706f 7274 5f63 6974 6965 7320 3d20 5b5d  port_cities = []
-00003160: 0a0a 2020 2020 2020 6369 7479 5f6c 732e  ..      city_ls.
-00003170: 6d61 7028 6369 7479 203d 3e20 6578 706f  map(city => expo
-00003180: 7274 5f63 6974 6965 732e 7075 7368 285b  rt_cities.push([
-00003190: 6369 7479 2e66 6965 6c64 732e 6e61 6d65  city.fields.name
-000031a0: 5d29 290a 0a20 2020 2020 2065 7870 6f72  ]))..      expor
-000031b0: 7454 656d 706c 6174 652e 6c6f 6164 4461  tTemplate.loadDa
-000031c0: 7461 2865 7870 6f72 745f 6369 7469 6573  ta(export_cities
-000031d0: 290a 2020 2020 2020 6578 706f 7274 506c  ).      exportPl
-000031e0: 7567 696e 2e64 6f77 6e6c 6f61 6446 696c  ugin.downloadFil
-000031f0: 6528 2763 7376 272c 207b 0a20 2020 2020  e('csv', {.     
-00003200: 2020 2062 6f6d 3a20 6661 6c73 652c 0a20     bom: false,. 
-00003210: 2020 2020 2020 2063 6f6c 756d 6e44 656c         columnDel
-00003220: 696d 6974 6572 3a20 272c 272c 0a20 2020  imiter: ',',.   
-00003230: 2020 2020 2063 6f6c 756d 6e48 6561 6465       columnHeade
-00003240: 7273 3a20 7472 7565 2c0a 2020 2020 2020  rs: true,.      
-00003250: 2020 6578 706f 7274 4869 6464 656e 436f    exportHiddenCo
-00003260: 6c75 6d6e 733a 2074 7275 652c 0a20 2020  lumns: true,.   
-00003270: 2020 2020 2065 7870 6f72 7448 6964 6465       exportHidde
-00003280: 6e52 6f77 733a 2074 7275 652c 0a20 2020  nRows: true,.   
-00003290: 2020 2020 2066 696c 6545 7874 656e 7369       fileExtensi
-000032a0: 6f6e 3a20 2763 7376 272c 0a20 2020 2020  on: 'csv',.     
-000032b0: 2020 2066 696c 656e 616d 653a 2027 6369     filename: 'ci
-000032c0: 7479 5f66 6f72 6563 6173 7473 5f74 656d  ty_forecasts_tem
-000032d0: 706c 6174 6527 2c0a 2020 2020 2020 2020  plate',.        
-000032e0: 6d69 6d65 5479 7065 3a20 2774 6578 742f  mimeType: 'text/
-000032f0: 6373 7627 2c0a 2020 2020 2020 2020 726f  csv',.        ro
-00003300: 7744 656c 696d 6974 6572 3a20 275c 6e27  wDelimiter: '\n'
-00003310: 2c0a 2020 2020 2020 2020 726f 7748 6561  ,.        rowHea
-00003320: 6465 7273 3a20 6661 6c73 650a 2020 2020  ders: false.    
-00003330: 2020 7d29 3b0a 2020 2020 7d29 0a0a 0a0a    });.    })....
-00003340: 2020 7d29 0a3c 2f73 6372 6970 743e 0a0a    }).</script>..
-00003350: 7b25 2065 6e64 626c 6f63 6b20 257d       {% endblock %}
+00000030: 257d 0a7b 2520 6c6f 6164 2077 6167 7461  %}.{% load wagta
+00000040: 696c 6164 6d69 6e5f 7461 6773 2069 3138  iladmin_tags i18
+00000050: 6e20 7374 6174 6963 2025 7d0a 7b25 206c  n static %}.{% l
+00000060: 6f61 6420 7761 6774 6169 6c73 6574 7469  oad wagtailsetti
+00000070: 6e67 735f 7461 6773 2025 7d0a 7b25 2067  ngs_tags %}.{% g
+00000080: 6574 5f73 6574 7469 6e67 7320 7573 655f  et_settings use_
+00000090: 6465 6661 756c 745f 7369 7465 3d54 7275  default_site=Tru
+000000a0: 6520 257d 0a0a 7b25 2062 6c6f 636b 2065  e %}..{% block e
+000000b0: 7874 7261 5f63 7373 2025 7d0a 2020 2020  xtra_css %}.    
+000000c0: 7b7b 2062 6c6f 636b 2e73 7570 6572 207d  {{ block.super }
+000000d0: 7d0a 2020 2020 3c73 7479 6c65 3e0a 2020  }.    <style>.  
+000000e0: 2020 2020 2020 2366 6f72 6563 6173 745f        #forecast_
+000000f0: 6d61 7020 7b0a 2020 2020 2020 2020 2020  map {.          
+00000100: 2020 6865 6967 6874 3a20 3630 7668 3b0a    height: 60vh;.
+00000110: 2020 2020 2020 2020 2020 2020 7769 6474              widt
+00000120: 683a 2031 3030 253b 0a20 2020 2020 2020  h: 100%;.       
+00000130: 2020 2020 2062 6f78 2d73 6861 646f 773a       box-shadow:
+00000140: 2030 7078 2030 7078 2037 7078 2030 7078   0px 0px 7px 0px
+00000150: 2072 6762 6128 302c 2030 2c20 302c 2030   rgba(0, 0, 0, 0
+00000160: 2e31 293b 0a20 2020 2020 2020 207d 0a20  .1);.        }. 
+00000170: 2020 203c 2f73 7479 6c65 3e0a 7b25 2065     </style>.{% e
+00000180: 6e64 626c 6f63 6b20 6578 7472 615f 6373  ndblock extra_cs
+00000190: 7320 257d 0a0a 7b25 2062 6c6f 636b 2068  s %}..{% block h
+000001a0: 6561 6465 7220 257d 0a20 2020 207b 2520  eader %}.    {% 
+000001b0: 7472 616e 7320 2756 6965 7720 466f 7265  trans 'View Fore
+000001c0: 6361 7374 7327 2061 7320 6865 6164 6572  casts' as header
+000001d0: 5f73 7472 2025 7d0a 2020 2020 7b25 2075  _str %}.    {% u
+000001e0: 726c 2027 6164 645f 666f 7265 6361 7374  rl 'add_forecast
+000001f0: 2720 6173 2061 6464 5f66 6f72 6563 6173  ' as add_forecas
+00000200: 745f 7572 6c20 257d 0a20 2020 207b 2520  t_url %}.    {% 
+00000210: 696e 636c 7564 6520 2277 6167 7461 696c  include "wagtail
+00000220: 6164 6d69 6e2f 7368 6172 6564 2f68 6561  admin/shared/hea
+00000230: 6465 722e 6874 6d6c 2220 7769 7468 2074  der.html" with t
+00000240: 6974 6c65 3d68 6561 6465 725f 7374 7220  itle=header_str 
+00000250: 6963 6f6e 3d22 666f 726d 2220 6163 7469  icon="form" acti
+00000260: 6f6e 5f75 726c 3d61 6464 5f66 6f72 6563  on_url=add_forec
+00000270: 6173 745f 7572 6c20 6163 7469 6f6e 5f74  ast_url action_t
+00000280: 6578 743d 2241 6464 2046 6f72 6563 6173  ext="Add Forecas
+00000290: 7422 2025 7d0a 7b25 2065 6e64 626c 6f63  t" %}.{% endbloc
+000002a0: 6b20 257d 0a0a 7b25 2062 6c6f 636b 2066  k %}..{% block f
+000002b0: 6f72 6563 6173 7420 257d 0a20 2020 203c  orecast %}.    <
+000002c0: 6832 2063 6c61 7373 3d22 772d 7061 6e65  h2 class="w-pane
+000002d0: 6c5f 5f68 6561 6469 6e67 2220 7374 796c  l__heading" styl
+000002e0: 653d 226d 6172 6769 6e2d 626f 7474 6f6d  e="margin-bottom
+000002f0: 3a20 3230 7078 223e 7b25 2074 7261 6e73  : 20px">{% trans
+00000300: 2027 4c61 7465 7374 2041 7661 696c 6162   'Latest Availab
+00000310: 6c65 2046 6f72 6563 6173 7427 2025 7d3c  le Forecast' %}<
+00000320: 2f68 323e 0a20 2020 203c 6469 7620 636c  /h2>.    <div cl
+00000330: 6173 733d 2272 6f77 2072 6f77 2d66 6c75  ass="row row-flu
+00000340: 7368 2220 7374 796c 653d 2264 6973 706c  sh" style="displ
+00000350: 6179 3a66 6c65 783b 2061 6c69 676e 2d69  ay:flex; align-i
+00000360: 7465 6d73 3a62 6173 656c 696e 6522 3e0a  tems:baseline">.
+00000370: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000380: 7373 3d22 636f 6c36 2220 7374 796c 653d  ss="col6" style=
+00000390: 2264 6973 706c 6179 3a66 6c65 783b 2066  "display:flex; f
+000003a0: 6c65 782d 7772 6170 3a20 7772 6170 3b22  lex-wrap: wrap;"
+000003b0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+000003c0: 6976 2063 6c61 7373 3d22 772d 6669 656c  iv class="w-fiel
+000003d0: 645f 5f77 7261 7070 6572 2022 2064 6174  d__wrapper " dat
+000003e0: 612d 6669 656c 642d 7772 6170 7065 723d  a-field-wrapper=
+000003f0: 2222 2073 7479 6c65 3d22 7061 6464 696e  "" style="paddin
+00000400: 672d 7269 6768 743a 3165 6d22 3e0a 2020  g-right:1em">.  
+00000410: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+00000420: 6162 656c 2063 6c61 7373 3d22 772d 6669  abel class="w-fi
+00000430: 656c 645f 5f6c 6162 656c 2220 666f 723d  eld__label" for=
+00000440: 2269 645f 666f 7265 6361 7374 5f64 6174  "id_forecast_dat
+00000450: 6522 2069 643d 2269 645f 666f 7265 6361  e" id="id_foreca
+00000460: 7374 5f64 6174 652d 6c61 6265 6c22 3e0a  st_date-label">.
+00000470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000480: 2020 2020 7b25 2074 7261 6e73 2027 466f      {% trans 'Fo
+00000490: 7265 6361 7374 2044 6174 6527 2025 7d3c  recast Date' %}<
+000004a0: 7370 616e 2063 6c61 7373 3d22 772d 7265  span class="w-re
+000004b0: 7175 6972 6564 2d6d 6172 6b22 3e2a 3c2f  quired-mark">*</
+000004c0: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
+000004d0: 2020 2020 2020 3c2f 6c61 6265 6c3e 0a20        </label>. 
+000004e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000004f0: 6469 7620 636c 6173 733d 2277 2d66 6965  div class="w-fie
+00000500: 6c64 2077 2d66 6965 6c64 2d2d 6368 6f69  ld w-field--choi
+00000510: 6365 5f66 6965 6c64 2077 2d66 6965 6c64  ce_field w-field
+00000520: 2d2d 7365 6c65 6374 2220 6461 7461 2d66  --select" data-f
+00000530: 6965 6c64 3d22 2220 6461 7461 2d63 6f6e  ield="" data-con
+00000540: 7465 6e74 7061 7468 3d22 7365 6c65 6374  tentpath="select
+00000550: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000560: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00000570: 733d 2277 2d66 6965 6c64 5f5f 696e 7075  s="w-field__inpu
+00000580: 7422 2064 6174 612d 6669 656c 642d 696e  t" data-field-in
+00000590: 7075 743d 2222 3e0a 2020 2020 2020 2020  put="">.        
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005b0: 3c73 656c 6563 7420 6e61 6d65 3d22 666f  <select name="fo
+000005c0: 7265 6361 7374 5f64 6174 6522 2069 643d  recast_date" id=
+000005d0: 2269 645f 666f 7265 6361 7374 5f64 6174  "id_forecast_dat
+000005e0: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 7b25 2066 6f72 2064 6179 2069 6e20 666f  {% for day in fo
+00000610: 7265 6361 7374 5f64 6174 6573 2025 7d0a  recast_dates %}.
+00000620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000640: 3c6f 7074 696f 6e20 7661 6c75 653d 227b  <option value="{
+00000650: 7b20 6461 797c 6461 7465 3a27 592d 6d2d  { day|date:'Y-m-
+00000660: 6427 207d 7d22 0a20 2020 2020 2020 2020  d' }}".         
+00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000680: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000690: 2520 6966 2066 6f72 6c6f 6f70 2e66 6972  % if forloop.fir
+000006a0: 7374 2025 7d73 656c 6563 7465 647b 2520  st %}selected{% 
+000006b0: 656e 6469 6620 257d 3e7b 7b20 6461 7920  endif %}>{{ day 
+000006c0: 7d7d 3c2f 6f70 7469 6f6e 3e0a 2020 2020  }}</option>.    
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006e0: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
+000006f0: 7220 257d 0a20 2020 2020 2020 2020 2020  r %}.           
+00000700: 2020 2020 2020 2020 2020 2020 203c 2f73               </s
+00000710: 656c 6563 743e 0a20 2020 2020 2020 2020  elect>.         
+00000720: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000730: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000740: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000750: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000760: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000770: 7373 3d22 772d 6669 656c 645f 5f77 7261  ss="w-field__wra
+00000780: 7070 6572 2022 2064 6174 612d 6669 656c  pper " data-fiel
+00000790: 642d 7772 6170 7065 723d 2222 3e0a 2020  d-wrapper="">.  
+000007a0: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+000007b0: 6162 656c 2063 6c61 7373 3d22 772d 6669  abel class="w-fi
+000007c0: 656c 645f 5f6c 6162 656c 2220 666f 723d  eld__label" for=
+000007d0: 2269 645f 6566 6665 6374 6976 655f 7065  "id_effective_pe
+000007e0: 7269 6f64 2220 6964 3d22 6964 5f65 6666  riod" id="id_eff
+000007f0: 6563 7469 7665 5f70 6572 696f 642d 6c61  ective_period-la
+00000800: 6265 6c22 3e0a 2020 2020 2020 2020 2020  bel">.          
+00000810: 2020 2020 2020 2020 2020 7b25 2074 7261            {% tra
+00000820: 6e73 2027 466f 7265 6361 7374 2045 6666  ns 'Forecast Eff
+00000830: 6563 7469 7665 2050 6572 696f 6427 2025  ective Period' %
+00000840: 7d3c 7370 616e 2063 6c61 7373 3d22 772d  }<span class="w-
+00000850: 7265 7175 6972 6564 2d6d 6172 6b22 3e2a  required-mark">*
+00000860: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+00000870: 2020 2020 2020 2020 3c2f 6c61 6265 6c3e          </label>
+00000880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000890: 203c 6469 7620 636c 6173 733d 2277 2d66   <div class="w-f
+000008a0: 6965 6c64 2077 2d66 6965 6c64 2d2d 6368  ield w-field--ch
+000008b0: 6f69 6365 5f66 6965 6c64 2077 2d66 6965  oice_field w-fie
+000008c0: 6c64 2d2d 7365 6c65 6374 2220 6461 7461  ld--select" data
+000008d0: 2d66 6965 6c64 3d22 2220 6461 7461 2d63  -field="" data-c
+000008e0: 6f6e 7465 6e74 7061 7468 3d22 7365 6c65  ontentpath="sele
+000008f0: 6374 223e 0a20 2020 2020 2020 2020 2020  ct">.           
+00000900: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00000910: 6173 733d 2277 2d66 6965 6c64 5f5f 696e  ass="w-field__in
+00000920: 7075 7422 2064 6174 612d 6669 656c 642d  put" data-field-
+00000930: 696e 7075 743d 2222 3e0a 2020 2020 2020  input="">.      
+00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000950: 2020 3c73 656c 6563 7420 6e61 6d65 3d22    <select name="
+00000960: 7365 6c65 6374 2220 6964 3d22 6964 5f65  select" id="id_e
+00000970: 6666 6563 7469 7665 5f70 6572 696f 6422  ffective_period"
+00000980: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000990: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000009a0: 2066 6f72 2070 6572 696f 6420 696e 2066   for period in f
+000009b0: 6f72 6563 6173 745f 7065 7269 6f64 732e  orecast_periods.
+000009c0: 616c 6c20 257d 0a20 2020 2020 2020 2020  all %}.         
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 2020 2020 203c 6f70 7469 6f6e 2076         <option v
+000009f0: 616c 7565 3d22 7b7b 2070 6572 696f 642e  alue="{{ period.
+00000a00: 706b 207d 7d22 0a20 2020 2020 2020 2020  pk }}".         
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a20: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000a30: 2520 6966 2066 6f72 6c6f 6f70 2e66 6972  % if forloop.fir
+00000a40: 7374 2025 7d73 656c 6563 7465 647b 2520  st %}selected{% 
+00000a50: 656e 6469 6620 257d 3e7b 7b20 7065 7269  endif %}>{{ peri
+00000a60: 6f64 2e6c 6162 656c 207d 7d3c 2f6f 7074  od.label }}</opt
+00000a70: 696f 6e3e 0a20 2020 2020 2020 2020 2020  ion>.           
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a90: 207b 2520 656e 6466 6f72 2025 7d0a 2020   {% endfor %}.  
+00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ab0: 2020 2020 2020 3c2f 7365 6c65 6374 3e0a        </select>.
+00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ad0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00000ae0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000af0: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00000b00: 6469 763e 0a20 2020 2020 2020 203c 2f64  div>.        </d
+00000b10: 6976 3e0a 2020 2020 3c2f 6469 763e 0a20  iv>.    </div>. 
+00000b20: 2020 203c 6469 7620 7374 796c 653d 2270     <div style="p
+00000b30: 6164 6469 6e67 3a32 656d 2030 223e 0a20  adding:2em 0">. 
+00000b40: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00000b50: 733d 2272 6f77 2072 6f77 2d66 6c75 7368  s="row row-flush
+00000b60: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
+00000b70: 6469 7620 636c 6173 733d 2263 6f6c 3722  div class="col7"
+00000b80: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000b90: 2020 3c64 6976 2069 643d 226c 6174 6573    <div id="lates
+00000ba0: 7446 6f72 6563 6173 7422 2073 7479 6c65  tForecast" style
+00000bb0: 3d7a 2d69 6e64 6578 3a31 3e3c 2f64 6976  =z-index:1></div
+00000bc0: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00000bd0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00000be0: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
+00000bf0: 3522 3e0a 2020 2020 2020 2020 2020 2020  5">.            
+00000c00: 2020 2020 3c64 6976 2069 643d 2266 6f72      <div id="for
+00000c10: 6563 6173 745f 6d61 7022 3e3c 2f64 6976  ecast_map"></div
+00000c20: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00000c30: 6469 763e 0a20 2020 2020 2020 203c 2f64  div>.        </d
+00000c40: 6976 3e0a 2020 2020 3c2f 6469 763e 0a7b  iv>.    </div>.{
+00000c50: 2520 656e 6462 6c6f 636b 2066 6f72 6563  % endblock forec
+00000c60: 6173 7420 257d 0a0a 0a7b 2520 626c 6f63  ast %}...{% bloc
+00000c70: 6b20 6578 7472 615f 6a73 2025 7d0a 2020  k extra_js %}.  
+00000c80: 2020 7b7b 2062 6c6f 636b 2e73 7570 6572    {{ block.super
+00000c90: 207d 7d0a 0a20 2020 203c 7363 7269 7074   }}..    <script
+00000ca0: 2074 7970 653d 2274 6578 742f 6a61 7661   type="text/java
+00000cb0: 7363 7269 7074 223e 0a0a 2020 2020 2020  script">..      
+00000cc0: 2020 636f 6e73 7420 6461 7461 5061 7261    const dataPara
+00000cd0: 6d73 203d 207b 7b20 6461 7461 5f70 6172  ms = {{ data_par
+00000ce0: 616d 6574 6572 5f76 616c 7565 737c 7361  ameter_values|sa
+00000cf0: 6665 7c64 6566 6175 6c74 5f69 665f 6e6f  fe|default_if_no
+00000d00: 6e65 3a22 2220 7d7d 3b0a 0a0a 2020 2020  ne:"" }};...    
+00000d10: 2020 2020 2428 646f 6375 6d65 6e74 292e      $(document).
+00000d20: 7265 6164 7928 6675 6e63 7469 6f6e 2028  ready(function (
+00000d30: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00000d40: 636f 6e73 7420 7374 6174 6963 5f70 6174  const static_pat
+00000d50: 6820 3d20 277b 2520 7374 6174 6963 2022  h = '{% static "
+00000d60: 666f 7265 6361 7374 6d61 6e61 6765 722f  forecastmanager/
+00000d70: 696d 672f 2220 257d 270a 0a20 2020 2020  img/" %}'..     
+00000d80: 2020 2020 2020 2063 6f6e 7374 2024 6461         const $da
+00000d90: 7465 496e 7075 7420 3d20 2428 2223 6964  teInput = $("#id
+00000da0: 5f66 6f72 6563 6173 745f 6461 7465 2229  _forecast_date")
+00000db0: 3b0a 2020 2020 2020 2020 2020 2020 636f  ;.            co
+00000dc0: 6e73 7420 2470 6572 696f 6449 6e70 7574  nst $periodInput
+00000dd0: 203d 2024 2822 2369 645f 6566 6665 6374   = $("#id_effect
+00000de0: 6976 655f 7065 7269 6f64 2229 3b0a 0a20  ive_period");.. 
+00000df0: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
+00000e00: 2066 6f72 6563 6173 7443 6f6e 7461 696e   forecastContain
+00000e10: 6572 203d 2064 6f63 756d 656e 742e 6765  er = document.ge
+00000e20: 7445 6c65 6d65 6e74 4279 4964 2827 6c61  tElementById('la
+00000e30: 7465 7374 466f 7265 6361 7374 2729 3b0a  testForecast');.
+00000e40: 0a20 2020 2020 2020 2020 2020 202f 2f20  .            // 
+00000e50: 696e 6974 6961 6c69 7a65 206d 6170 2020  initialize map  
+00000e60: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+00000e70: 636f 6e73 7420 666f 7265 6361 7374 4d61  const forecastMa
+00000e80: 7020 3d20 6e65 7720 6d61 706c 6962 7265  p = new maplibre
+00000e90: 676c 2e4d 6170 287b 0a20 2020 2020 2020  gl.Map({.       
+00000ea0: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
+00000eb0: 6572 3a20 2766 6f72 6563 6173 745f 6d61  er: 'forecast_ma
+00000ec0: 7027 2c0a 2020 2020 2020 2020 2020 2020  p',.            
+00000ed0: 2020 2020 7374 796c 653a 2062 6173 656d      style: basem
+00000ee0: 6170 2c0a 2020 2020 2020 2020 2020 2020  ap,.            
+00000ef0: 2020 2020 6365 6e74 6572 3a20 5b33 392e      center: [39.
+00000f00: 3637 3435 3831 3636 3430 3935 3334 2c20  67458166409534, 
+00000f10: 382e 3730 3930 3534 3633 3237 3536 3339  8.70905463275639
+00000f20: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00000f30: 2020 2020 7a6f 6f6d 3a20 342e 350a 2020      zoom: 4.5.  
+00000f40: 2020 2020 2020 2020 2020 7d29 0a0a 2020            })..  
+00000f50: 2020 2020 2020 2020 2020 2f2f 2043 7265            // Cre
+00000f60: 6174 6520 6120 706f 7075 7020 6f62 6a65  ate a popup obje
+00000f70: 6374 0a20 2020 2020 2020 2020 2020 2063  ct.            c
+00000f80: 6f6e 7374 2070 6f70 7570 203d 206e 6577  onst popup = new
+00000f90: 206d 6170 6c69 6272 6567 6c2e 506f 7075   maplibregl.Popu
+00000fa0: 7028 7b0a 2020 2020 2020 2020 2020 2020  p({.            
+00000fb0: 2020 2020 636c 6f73 6542 7574 746f 6e3a      closeButton:
+00000fc0: 2066 616c 7365 2c0a 2020 2020 2020 2020   false,.        
+00000fd0: 2020 2020 2020 2020 636c 6f73 654f 6e43          closeOnC
+00000fe0: 6c69 636b 3a20 6661 6c73 650a 2020 2020  lick: false.    
+00000ff0: 2020 2020 2020 2020 7d29 3b0a 0a20 2020          });..   
+00001000: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
+00001010: 744d 6170 2e61 6464 436f 6e74 726f 6c28  tMap.addControl(
+00001020: 6e65 7720 6d61 706c 6962 7265 676c 2e4e  new maplibregl.N
+00001030: 6176 6967 6174 696f 6e43 6f6e 7472 6f6c  avigationControl
+00001040: 2829 290a 0a20 2020 2020 2020 2020 2020  ())..           
+00001050: 202f 2f20 696e 6974 6961 6c69 7a65 0a20   // initialize. 
+00001060: 2020 2020 2020 2020 2020 2067 6574 466f             getFo
+00001070: 7265 6361 7374 4461 7461 2829 0a0a 2020  recastData()..  
+00001080: 2020 2020 2020 2020 2020 2f2f 2069 6e69            // ini
+00001090: 7469 616c 697a 6520 7461 626c 650a 2020  tialize table.  
+000010a0: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
+000010b0: 666f 7265 6361 7374 5461 626c 6520 3d20  forecastTable = 
+000010c0: 6e65 7720 4861 6e64 736f 6e74 6162 6c65  new Handsontable
+000010d0: 2866 6f72 6563 6173 7443 6f6e 7461 696e  (forecastContain
+000010e0: 6572 2c20 7b0a 2020 2020 2020 2020 2020  er, {.          
+000010f0: 2020 2020 2020 7265 6164 4f6e 6c79 3a20        readOnly: 
+00001100: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+00001110: 2020 2020 2020 7769 6474 683a 2027 3130        width: '10
+00001120: 3025 272c 0a20 2020 2020 2020 2020 2020  0%',.           
+00001130: 2020 2020 2072 6f77 4865 6164 6572 733a       rowHeaders:
+00001140: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
+00001150: 2020 2020 2020 2063 6f6c 4865 6164 6572         colHeader
+00001160: 733a 205b 0a20 2020 2020 2020 2020 2020  s: [.           
+00001170: 2020 2020 2020 2020 2027 4369 7479 272c           'City',
+00001180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001190: 2020 2020 202e 2e2e 6461 7461 5061 7261       ...dataPara
+000011a0: 6d73 2e6d 6170 2870 203d 3e20 702e 6e61  ms.map(p => p.na
+000011b0: 6d65 292c 0a20 2020 2020 2020 2020 2020  me),.           
+000011c0: 2020 2020 2020 2020 2027 436f 6e64 6974           'Condit
+000011d0: 696f 6e27 0a20 2020 2020 2020 2020 2020  ion'.           
+000011e0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+000011f0: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
+00001200: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00001210: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001230: 2064 6174 613a 2027 6369 7479 5f6e 616d   data: 'city_nam
+00001240: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+00001250: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001260: 2020 2020 2020 2020 2020 2020 2020 202e                 .
+00001270: 2e2e 6461 7461 5061 7261 6d73 2e6d 6170  ..dataParams.map
+00001280: 2828 7029 203d 3e20 287b 0a20 2020 2020  ((p) => ({.     
+00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012a0: 2020 2064 6174 613a 2070 2e70 6172 616d     data: p.param
+000012b0: 6574 6572 2c0a 2020 2020 2020 2020 2020  eter,.          
+000012c0: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+000012d0: 7065 3a20 702e 7061 7261 6d65 7465 725f  pe: p.parameter_
+000012e0: 7479 7065 2c0a 2020 2020 2020 2020 2020  type,.          
+000012f0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00001300: 6d65 466f 726d 6174 3a20 2768 3a6d 6d27  meFormat: 'h:mm'
+00001310: 203f 2070 2e70 6172 616d 6574 6572 5f74   ? p.parameter_t
+00001320: 7970 6520 3d3d 3d20 2774 696d 6527 203a  ype === 'time' :
+00001330: 2027 272c 0a20 2020 2020 2020 2020 2020   '',.           
+00001340: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
+00001350: 7265 6374 466f 726d 6174 3a20 7472 7565  rectFormat: true
+00001360: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001370: 2020 2020 2020 7d29 292c 0a20 2020 2020        })),.     
+00001380: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00001390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013a0: 2020 2020 2020 2020 2064 6174 613a 2027           data: '
+000013b0: 636f 6e64 6974 696f 6e27 2c0a 2020 2020  condition',.    
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013d0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+000013e0: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+000013f0: 2020 2020 2020 6461 7461 3a20 5b5d 2c0a        data: [],.
+00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001410: 2f2f 2064 726f 7064 6f77 6e4d 656e 753a  // dropdownMenu:
+00001420: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
+00001430: 2020 2020 2020 206d 756c 7469 436f 6c75         multiColu
+00001440: 6d6e 536f 7274 696e 673a 2074 7275 652c  mnSorting: true,
+00001450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001460: 202f 2f20 6669 6c74 6572 733a 2074 7275   // filters: tru
+00001470: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001480: 2020 206d 616e 7561 6c43 6f6c 756d 6e52     manualColumnR
+00001490: 6573 697a 653a 2074 7275 652c 0a20 2020  esize: true,.   
+000014a0: 2020 2020 2020 2020 2020 2020 206d 696e               min
+000014b0: 5370 6172 6552 6f77 733a 2031 2c0a 2020  SpareRows: 1,.  
+000014c0: 2020 2020 2020 2020 2020 2020 2020 6865                he
+000014d0: 6967 6874 3a20 2761 7574 6f27 2c0a 2020  ight: 'auto',.  
+000014e0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000014f0: 7265 7463 6848 3a20 2261 6c6c 222c 0a20  retchH: "all",. 
+00001500: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00001510: 6963 656e 7365 4b65 793a 2027 6e6f 6e2d  icenseKey: 'non-
+00001520: 636f 6d6d 6572 6369 616c 2d61 6e64 2d65  commercial-and-e
+00001530: 7661 6c75 6174 696f 6e27 202f 2f20 666f  valuation' // fo
+00001540: 7220 6e6f 6e2d 636f 6d6d 6572 6369 616c  r non-commercial
+00001550: 2075 7365 206f 6e6c 790a 2020 2020 2020   use only.      
+00001560: 2020 2020 2020 7d29 3b0a 0a0a 2020 2020        });...    
+00001570: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
+00001580: 2070 6f70 756c 6174 654d 6170 2864 6174   populateMap(dat
+00001590: 6129 207b 0a0a 2020 2020 2020 2020 2020  a) {..          
+000015a0: 2020 2020 2020 6966 2866 6f72 6563 6173        if(forecas
+000015b0: 744d 6170 2e67 6574 4c61 7965 7228 2263  tMap.getLayer("c
+000015c0: 6974 792d 666f 7265 6361 7374 7322 2929  ity-forecasts"))
+000015d0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000015e0: 2020 2020 2020 666f 7265 6361 7374 4d61        forecastMa
+000015f0: 702e 7265 6d6f 7665 4c61 7965 7228 2263  p.removeLayer("c
+00001600: 6974 792d 666f 7265 6361 7374 7322 290a  ity-forecasts").
+00001610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001620: 7d0a 0a20 2020 2020 2020 2020 2020 2020  }..             
+00001630: 2020 2069 6628 666f 7265 6361 7374 4d61     if(forecastMa
+00001640: 702e 6765 7453 6f75 7263 6528 2263 6974  p.getSource("cit
+00001650: 792d 666f 7265 6361 7374 7322 2929 7b0a  y-forecasts")){.
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2020 666f 7265 6361 7374 4d61 702e      forecastMap.
+00001680: 7265 6d6f 7665 536f 7572 6365 2822 6369  removeSource("ci
+00001690: 7479 2d66 6f72 6563 6173 7473 2229 0a0a  ty-forecasts")..
+000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000016c0: 2020 6966 2864 6174 612e 6665 6174 7572    if(data.featur
+000016d0: 6573 2e6c 656e 6774 6820 3e30 297b 0a20  es.length >0){. 
+000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016f0: 2020 2066 6f72 6563 6173 744d 6170 2e61     forecastMap.a
+00001700: 6464 536f 7572 6365 2822 6369 7479 2d66  ddSource("city-f
+00001710: 6f72 6563 6173 7473 222c 207b 0a20 2020  orecasts", {.   
+00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001730: 2020 2020 2074 7970 653a 2022 6765 6f6a       type: "geoj
+00001740: 736f 6e22 2c0a 2020 2020 2020 2020 2020  son",.          
+00001750: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00001760: 7461 3a20 6461 7461 0a20 2020 2020 2020  ta: data.       
+00001770: 2020 2020 2020 2020 2020 2020 207d 290a               }).
+00001780: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00001790: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
+000017a0: 744d 6170 2e61 6464 4c61 7965 7228 7b0a  tMap.addLayer({.
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017c0: 2020 2020 2020 2020 2269 6422 3a20 2263          "id": "c
+000017d0: 6974 792d 666f 7265 6361 7374 7322 2c0a  ity-forecasts",.
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00001800: 2273 796d 626f 6c22 2c0a 2020 2020 2020  "symbol",.      
+00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001820: 2020 226c 6179 6f75 7422 3a20 7b0a 2020    "layout": {.  
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 2020 2020 2020 2020 2020 2769 636f 6e2d            'icon-
+00001850: 696d 6167 6527 3a20 5b27 6765 7427 2c20  image': ['get', 
+00001860: 2763 6f6e 6469 7469 6f6e 5f69 636f 6e27  'condition_icon'
+00001870: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00001880: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001890: 6963 6f6e 2d73 697a 6527 3a20 302e 332c  icon-size': 0.3,
+000018a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018b0: 2020 2020 2020 2020 2020 2020 2027 6963               'ic
+000018c0: 6f6e 2d61 6c6c 6f77 2d6f 7665 726c 6170  on-allow-overlap
+000018d0: 273a 2074 7275 650a 2020 2020 2020 2020  ': true.        
+000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018f0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00001900: 2020 2020 2020 2020 2020 2073 6f75 7263             sourc
+00001910: 653a 2022 6369 7479 2d66 6f72 6563 6173  e: "city-forecas
+00001920: 7473 220a 2020 2020 2020 2020 2020 2020  ts".            
+00001930: 2020 2020 2020 2020 7d29 0a20 2020 200a          }).    .
+00001940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001950: 2020 2020 636f 6e73 7420 6262 6f78 203d      const bbox =
+00001960: 2074 7572 662e 6262 6f78 2864 6174 6129   turf.bbox(data)
+00001970: 0a20 2020 200a 2020 2020 2020 2020 2020  .    .          
+00001980: 2020 2020 2020 2020 2020 666f 7265 6361            foreca
+00001990: 7374 4d61 702e 6669 7442 6f75 6e64 7328  stMap.fitBounds(
+000019a0: 6262 6f78 2c20 7b0a 2020 2020 2020 2020  bbox, {.        
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 7061 6464 696e 673a 207b 746f 703a 2031  padding: {top: 1
+000019d0: 3030 2c20 626f 7474 6f6d 3a20 3130 302c  00, bottom: 100,
+000019e0: 206c 6566 743a 2031 3030 2c20 7269 6768   left: 100, righ
+000019f0: 743a 2031 3030 7d2c 0a20 2020 2020 2020  t: 100},.       
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 2064 7572 6174 696f 6e3a 2031 3030 302c   duration: 1000,
+00001a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a30: 2020 2020 2020 2020 2065 6173 696e 673a           easing:
+00001a40: 2066 756e 6374 696f 6e20 2874 2920 7b0a   function (t) {.
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001a70: 726e 2074 202a 2028 3220 2d20 7429 3b20  rn t * (2 - t); 
+00001a80: 2f2f 2043 7562 6963 2065 6173 696e 6720  // Cubic easing 
+00001a90: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
+00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ab0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+00001ac0: 2020 2020 2020 207d 290a 2020 2020 2020         }).      
+00001ad0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00001ae0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+00001af0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00001b00: 2020 2020 2020 2066 756e 6374 696f 6e20         function 
+00001b10: 6765 7446 6f72 6563 6173 7444 6174 6128  getForecastData(
+00001b20: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+00001b30: 2020 2020 636f 6e73 7420 666f 7265 6361      const foreca
+00001b40: 7374 4461 7465 203d 2024 6461 7465 496e  stDate = $dateIn
+00001b50: 7075 742e 7661 6c28 290a 2020 2020 2020  put.val().      
+00001b60: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
+00001b70: 6566 6665 6374 6976 6550 6572 696f 6420  effectivePeriod 
+00001b80: 3d20 2470 6572 696f 6449 6e70 7574 2e76  = $periodInput.v
+00001b90: 616c 2829 0a0a 0a20 2020 2020 2020 2020  al()...         
+00001ba0: 2020 2020 2020 2069 6620 2866 6f72 6563         if (forec
+00001bb0: 6173 7444 6174 6520 7c7c 2065 6666 6563  astDate || effec
+00001bc0: 7469 7665 5065 7269 6f64 2920 7b0a 2020  tivePeriod) {.  
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 2f2f 204d 616b 6520 616e 2048 5454    // Make an HTT
+00001bf0: 5020 4745 5420 7265 7175 6573 7420 746f  P GET request to
+00001c00: 2074 6865 2041 5049 2065 6e64 706f 696e   the API endpoin
+00001c10: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00001c20: 2020 2020 2020 6665 7463 6828 607b 2520        fetch(`{% 
+00001c30: 7572 6c20 2766 6f72 6563 6173 742d 6c69  url 'forecast-li
+00001c40: 7374 2725 7d3f 666f 7265 6361 7374 5f64  st'%}?forecast_d
+00001c50: 6174 653d 247b 666f 7265 6361 7374 4461  ate=${forecastDa
+00001c60: 7465 7d26 6566 6665 6374 6976 655f 7065  te}&effective_pe
+00001c70: 7269 6f64 3d24 7b65 6666 6563 7469 7665  riod=${effective
+00001c80: 5065 7269 6f64 7d60 290a 2020 2020 2020  Period}`).      
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ca0: 2020 2e74 6865 6e28 7265 7370 6f6e 7365    .then(response
+00001cb0: 203d 3e20 7265 7370 6f6e 7365 2e6a 736f   => response.jso
+00001cc0: 6e28 2929 2020 2f2f 2050 6172 7365 2074  n())  // Parse t
+00001cd0: 6865 2072 6573 706f 6e73 6520 6173 204a  he response as J
+00001ce0: 534f 4e0a 2020 2020 2020 2020 2020 2020  SON.            
+00001cf0: 2020 2020 2020 2020 2020 2020 2e74 6865              .the
+00001d00: 6e28 6461 7461 203d 3e20 7b0a 2020 2020  n(data => {.    
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 2020 2020 2020 2020 2f2f 2050 726f 6365          // Proce
+00001d30: 7373 2074 6865 2072 6574 7269 6576 6564  ss the retrieved
+00001d40: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d60: 2020 6461 7461 2e6d 6170 2869 636f 6e20    data.map(icon 
+00001d70: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2020 206c 6574 2069 6d67 203d 206e       let img = n
+00001da0: 6577 2049 6d61 6765 2829 0a20 2020 2020  ew Image().     
+00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dc0: 2020 2020 2020 2020 2020 2069 6d67 2e6f             img.o
+00001dd0: 6e6c 6f61 6420 3d20 2829 203d 3e20 7b0a  nload = () => {.
+00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e00: 2020 2020 6966 2028 2166 6f72 6563 6173      if (!forecas
+00001e10: 744d 6170 2e68 6173 496d 6167 6528 6963  tMap.hasImage(ic
+00001e20: 6f6e 2e70 726f 7065 7274 6965 732e 636f  on.properties.co
+00001e30: 6e64 6974 696f 6e5f 6963 6f6e 2929 207b  ndition_icon)) {
+00001e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001e70: 666f 7265 6361 7374 4d61 702e 6164 6449  forecastMap.addI
+00001e80: 6d61 6765 2860 247b 6963 6f6e 2e70 726f  mage(`${icon.pro
+00001e90: 7065 7274 6965 732e 636f 6e64 6974 696f  perties.conditio
+00001ea0: 6e5f 6963 6f6e 7d60 2c20 696d 6729 0a20  n_icon}`, img). 
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ed0: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
+00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ef0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f10: 2020 2020 2020 2020 696d 672e 7372 6320          img.src 
+00001f20: 3d20 6024 7b73 7461 7469 635f 7061 7468  = `${static_path
+00001f30: 7d24 7b69 636f 6e2e 7072 6f70 6572 7469  }${icon.properti
+00001f40: 6573 2e63 6f6e 6469 7469 6f6e 5f69 636f  es.condition_ico
+00001f50: 6e7d 600a 2020 2020 2020 2020 2020 2020  n}`.            
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2020 7265 7475 726e 2069 6d67 2e73      return img.s
+00001f80: 7263 0a0a 2020 2020 2020 2020 2020 2020  rc..            
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 7d29 0a20 2020 2020 2020 2020 2020 2020  }).             
+00001fb0: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+00001fc0: 2f20 4163 6365 7373 2061 6e64 2075 7365  / Access and use
+00001fd0: 2074 6865 2064 6174 6120 6173 206e 6565   the data as nee
+00001fe0: 6465 640a 2020 2020 2020 2020 2020 2020  ded.            
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002000: 706f 7075 6c61 7465 4d61 7028 7b0a 2020  populateMap({.  
+00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002020: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+00002030: 7065 3a20 2246 6561 7475 7265 436f 6c6c  pe: "FeatureColl
+00002040: 6563 7469 6f6e 222c 0a20 2020 2020 2020  ection",.       
+00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002060: 2020 2020 2020 2020 2066 6561 7475 7265           feature
+00002070: 733a 2064 6174 610a 2020 2020 2020 2020  s: data.        
+00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002090: 2020 2020 7d29 0a0a 2020 2020 2020 2020      })..        
+000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020b0: 2020 2020 636f 6e73 7420 666f 7265 6361      const foreca
+000020c0: 7374 735f 7072 6f70 7320 3d20 5b5d 0a20  sts_props = []. 
+000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020e0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+000020f0: 6d61 7028 6c61 7465 7374 5f66 6f72 6563  map(latest_forec
+00002100: 6173 7420 3d3e 207b 0a20 2020 2020 2020  ast => {.       
+00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002120: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
+00002130: 7473 5f70 726f 7073 2e70 7573 6828 6c61  ts_props.push(la
+00002140: 7465 7374 5f66 6f72 6563 6173 742e 7072  test_forecast.pr
+00002150: 6f70 6572 7469 6573 290a 2020 2020 2020  operties).      
+00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002170: 2020 2020 2020 7d29 0a0a 2020 2020 2020        })..      
+00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002190: 2020 2020 2020 666f 7265 6361 7374 5461        forecastTa
+000021a0: 626c 652e 6c6f 6164 4461 7461 2866 6f72  ble.loadData(for
+000021b0: 6563 6173 7473 5f70 726f 7073 290a 2020  ecasts_props).  
+000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021d0: 2020 2020 2020 7d29 0a20 2020 2020 2020        }).       
+000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021f0: 202e 6361 7463 6828 6572 726f 7220 3d3e   .catch(error =>
+00002200: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00002210: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+00002220: 2f20 4861 6e64 6c65 2061 6e79 2065 7272  / Handle any err
+00002230: 6f72 7320 7468 6174 206f 6363 7572 7265  ors that occurre
+00002240: 6420 6475 7269 6e67 2074 6865 2072 6571  d during the req
+00002250: 7565 7374 0a20 2020 2020 2020 2020 2020  uest.           
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2063 6f6e 736f 6c65 2e65 7272 6f72 2827   console.error('
+00002280: 4572 726f 723a 272c 2065 7272 6f72 293b  Error:', error);
+00002290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000022a0: 2020 2020 2020 2020 207d 293b 0a20 2020           });.   
+000022b0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+000022c0: 2020 2020 2020 2020 2020 207d 0a0a 0a20             }... 
+000022d0: 2020 2020 2020 2020 2020 2063 6f6e 7374             const
+000022e0: 2067 6574 506f 7075 7048 544d 4c20 3d20   getPopupHTML = 
+000022f0: 2870 726f 7073 2920 3d3e 207b 0a20 2020  (props) => {.   
+00002300: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00002310: 7374 2070 6172 616d 5661 6c75 6573 203d  st paramValues =
+00002320: 2064 6174 6150 6172 616d 732e 7265 6475   dataParams.redu
+00002330: 6365 2828 616c 6c2c 2070 6172 616d 2920  ce((all, param) 
+00002340: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
+00002350: 2020 2020 2020 2020 2069 6620 2870 726f           if (pro
+00002360: 7073 5b70 6172 616d 2e70 6172 616d 6574  ps[param.paramet
+00002370: 6572 5d29 207b 0a20 2020 2020 2020 2020  er]) {.         
+00002380: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00002390: 6c6c 5b70 6172 616d 2e6e 616d 655d 203d  ll[param.name] =
+000023a0: 2070 726f 7073 5b70 6172 616d 2e70 6172   props[param.par
+000023b0: 616d 6574 6572 5d0a 2020 2020 2020 2020  ameter].        
+000023c0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023e0: 2020 7265 7475 726e 2061 6c6c 0a20 2020    return all.   
+000023f0: 2020 2020 2020 2020 2020 2020 207d 2c20               }, 
+00002400: 7b7d 290a 0a20 2020 2020 2020 2020 2020  {})..           
+00002410: 2020 2020 2063 6f6e 7374 2063 6974 794e       const cityN
+00002420: 616d 6520 3d20 7072 6f70 732e 6369 7479  ame = props.city
+00002430: 5f6e 616d 653b 0a20 2020 2020 2020 2020  _name;.         
+00002440: 2020 2020 2020 2063 6f6e 7374 2063 6f6e         const con
+00002450: 6469 7469 6f6e 203d 2070 726f 7073 2e63  dition = props.c
+00002460: 6f6e 6469 7469 6f6e 3b0a 0a20 2020 2020  ondition;..     
+00002470: 2020 2020 2020 2020 2020 206c 6574 2076             let v
+00002480: 616c 7565 7320 3d20 4f62 6a65 6374 2e6b  alues = Object.k
+00002490: 6579 7328 7061 7261 6d56 616c 7565 7329  eys(paramValues)
+000024a0: 2e72 6564 7563 6528 2861 6c6c 2c20 6b65  .reduce((all, ke
+000024b0: 7929 203d 3e20 7b0a 2020 2020 2020 2020  y) => {.        
+000024c0: 2020 2020 2020 2020 2020 2020 616c 6c20              all 
+000024d0: 3d20 616c 6c20 2b20 603c 703e 3c62 3e24  = all + `<p><b>$
+000024e0: 7b6b 6579 7d3a 203c 2f62 3e24 7b70 6172  {key}: </b>${par
+000024f0: 616d 5661 6c75 6573 5b6b 6579 5d7d 3c2f  amValues[key]}</
+00002500: 703e 600a 2020 2020 2020 2020 2020 2020  p>`.            
+00002510: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+00002520: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
+00002530: 2020 207d 2c20 2222 290a 0a20 2020 2020     }, "")..     
+00002540: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00002550: 6e20 603c 6469 7620 636c 6173 733d 2262  n `<div class="b
+00002560: 6c6f 636b 2220 7374 796c 653d 226d 6172  lock" style="mar
+00002570: 6769 6e3a 3130 7078 3b20 7769 6474 683a  gin:10px; width:
+00002580: 3230 3070 7822 3e0a 2020 2020 2020 2020  200px">.        
+00002590: 2020 2020 2020 2020 2020 2020 3c68 3220              <h2 
+000025a0: 636c 6173 733d 2274 6974 6c65 2220 7374  class="title" st
+000025b0: 796c 653d 2266 6f6e 742d 7369 7a65 3a31  yle="font-size:1
+000025c0: 3870 783b 223e 247b 6369 7479 4e61 6d65  8px;">${cityName
+000025d0: 7d3c 2f68 323e 0a20 2020 2020 2020 2020  }</h2>.         
+000025e0: 2020 2020 2020 2020 2020 203c 6832 2063             <h2 c
+000025f0: 6c61 7373 3d22 7375 6274 6974 6c65 2220  lass="subtitle" 
+00002600: 7374 796c 653d 2266 6f6e 742d 7369 7a65  style="font-size
+00002610: 3a31 3470 783b 223e 247b 636f 6e64 6974  :14px;">${condit
+00002620: 696f 6e7d 3c2f 6832 3e0a 2020 2020 2020  ion}</h2>.      
+00002630: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
+00002640: 723e 0a20 2020 2020 2020 2020 2020 2020  r>.             
+00002650: 2020 2020 2020 2024 7b76 616c 7565 737d         ${values}
+00002660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002670: 203c 2f64 6976 3e60 0a20 2020 2020 2020   </div>`.       
+00002680: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00002690: 2020 2020 666f 7265 6361 7374 4d61 702e      forecastMap.
+000026a0: 6f6e 2822 6c6f 6164 222c 2028 2920 3d3e  on("load", () =>
+000026b0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000026c0: 2020 202f 2f20 5768 656e 2061 2063 6c69     // When a cli
+000026d0: 636b 2065 7665 6e74 206f 6363 7572 7320  ck event occurs 
+000026e0: 6f6e 2061 2066 6561 7475 7265 2069 6e20  on a feature in 
+000026f0: 7468 6520 706c 6163 6573 206c 6179 6572  the places layer
+00002700: 2c20 6f70 656e 2061 2070 6f70 7570 2061  , open a popup a
+00002710: 7420 7468 650a 2020 2020 2020 2020 2020  t the.          
+00002720: 2020 2020 2020 2f2f 206c 6f63 6174 696f        // locatio
+00002730: 6e20 6f66 2074 6865 2066 6561 7475 7265  n of the feature
+00002740: 2c20 7769 7468 2064 6573 6372 6970 7469  , with descripti
+00002750: 6f6e 2048 544d 4c20 6672 6f6d 2069 7473  on HTML from its
+00002760: 2070 726f 7065 7274 6965 732e 0a20 2020   properties..   
+00002770: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00002780: 6563 6173 744d 6170 2e6f 6e28 226d 6f75  ecastMap.on("mou
+00002790: 7365 656e 7465 7222 2c20 2263 6974 792d  seenter", "city-
+000027a0: 666f 7265 6361 7374 7322 2c20 2865 2920  forecasts", (e) 
+000027b0: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
+000027c0: 2020 2020 2020 2020 202f 2f20 4765 7420           // Get 
+000027d0: 7468 6520 6665 6174 7572 6520 7468 6174  the feature that
+000027e0: 2077 6173 2068 6f76 6572 6564 206f 7665   was hovered ove
+000027f0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00002800: 2020 2020 2020 636f 6e73 7420 6665 6174        const feat
+00002810: 7572 6520 3d20 652e 6665 6174 7572 6573  ure = e.features
+00002820: 5b30 5d3b 0a20 2020 2020 2020 2020 2020  [0];.           
+00002830: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
+00002840: 744d 6170 2e67 6574 4361 6e76 6173 2829  tMap.getCanvas()
+00002850: 2e73 7479 6c65 2e63 7572 736f 7220 3d20  .style.cursor = 
+00002860: 2270 6f69 6e74 6572 223b 0a0a 2020 2020  "pointer";..    
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 706f 7075 702e 7365 744c 6e67 4c61 7428  popup.setLngLat(
+00002890: 6665 6174 7572 652e 6765 6f6d 6574 7279  feature.geometry
+000028a0: 2e63 6f6f 7264 696e 6174 6573 290a 2020  .coordinates).  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028c0: 2020 2020 2020 2e73 6574 4854 4d4c 2867        .setHTML(g
+000028d0: 6574 506f 7075 7048 544d 4c28 6665 6174  etPopupHTML(feat
+000028e0: 7572 652e 7072 6f70 6572 7469 6573 2929  ure.properties))
+000028f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002900: 2020 2020 2020 2020 202e 6164 6454 6f28           .addTo(
+00002910: 666f 7265 6361 7374 4d61 7029 3b0a 2020  forecastMap);.  
+00002920: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+00002930: 3b0a 0a20 2020 2020 2020 2020 2020 2020  ;..             
+00002940: 2020 202f 2f20 2f2f 2043 6861 6e67 6520     // // Change 
+00002950: 7468 6520 6375 7273 6f72 2074 6f20 6120  the cursor to a 
+00002960: 706f 696e 7465 7220 7768 656e 2074 6865  pointer when the
+00002970: 206d 6f75 7365 2069 7320 6f76 6572 2074   mouse is over t
+00002980: 6865 2070 6c61 6365 7320 6c61 7965 722e  he places layer.
+00002990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029a0: 202f 2f20 666f 7265 6361 7374 4d61 702e   // forecastMap.
+000029b0: 6f6e 2822 6d6f 7573 6565 6e74 6572 222c  on("mouseenter",
+000029c0: 2022 6369 7479 2d66 6f72 6563 6173 7473   "city-forecasts
+000029d0: 222c 2028 2920 3d3e 207b 0a20 2020 2020  ", () => {.     
+000029e0: 2020 2020 2020 2020 2020 202f 2f20 2020             //   
+000029f0: 2020 666f 7265 6361 7374 4d61 702e 6765    forecastMap.ge
+00002a00: 7443 616e 7661 7328 292e 7374 796c 652e  tCanvas().style.
+00002a10: 6375 7273 6f72 203d 2022 706f 696e 7465  cursor = "pointe
+00002a20: 7222 3b0a 2020 2020 2020 2020 2020 2020  r";.            
+00002a30: 2020 2020 2f2f 207d 293b 0a0a 2020 2020      // });..    
+00002a40: 2020 2020 2020 2020 2020 2020 2f2f 2043              // C
+00002a50: 6861 6e67 6520 6974 2062 6163 6b20 746f  hange it back to
+00002a60: 2061 2070 6f69 6e74 6572 2077 6865 6e20   a pointer when 
+00002a70: 6974 206c 6561 7665 732e 0a20 2020 2020  it leaves..     
+00002a80: 2020 2020 2020 2020 2020 2066 6f72 6563             forec
+00002a90: 6173 744d 6170 2e6f 6e28 226d 6f75 7365  astMap.on("mouse
+00002aa0: 6c65 6176 6522 2c20 2263 6974 792d 666f  leave", "city-fo
+00002ab0: 7265 6361 7374 7322 2c20 2829 203d 3e20  recasts", () => 
+00002ac0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002ad0: 2020 2020 2020 706f 7075 702e 7265 6d6f        popup.remo
+00002ae0: 7665 2829 0a20 2020 2020 2020 2020 2020  ve().           
+00002af0: 2020 2020 2020 2020 2066 6f72 6563 6173           forecas
+00002b00: 744d 6170 2e67 6574 4361 6e76 6173 2829  tMap.getCanvas()
+00002b10: 2e73 7479 6c65 2e63 7572 736f 7220 3d20  .style.cursor = 
+00002b20: 2222 3b0a 2020 2020 2020 2020 2020 2020  "";.            
+00002b30: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
+00002b40: 2020 2020 7d29 0a0a 2020 2020 2020 2020      })..        
+00002b50: 2020 2020 2464 6174 6549 6e70 7574 2e6f      $dateInput.o
+00002b60: 6e28 2763 6861 6e67 6527 2c20 2865 2920  n('change', (e) 
+00002b70: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
+00002b80: 2020 2020 2067 6574 466f 7265 6361 7374       getForecast
+00002b90: 4461 7461 2829 0a20 2020 2020 2020 2020  Data().         
+00002ba0: 2020 207d 290a 0a20 2020 2020 2020 2020     })..         
+00002bb0: 2020 2024 7065 7269 6f64 496e 7075 742e     $periodInput.
+00002bc0: 6f6e 2827 6368 616e 6765 272c 2028 6529  on('change', (e)
+00002bd0: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
+00002be0: 2020 2020 2020 6765 7446 6f72 6563 6173        getForecas
+00002bf0: 7444 6174 6128 290a 2020 2020 2020 2020  tData().        
+00002c00: 2020 2020 7d29 0a20 2020 2020 2020 207d      }).        }
+00002c10: 290a 2020 2020 3c2f 7363 7269 7074 3e0a  ).    </script>.
+00002c20: 7b25 2065 6e64 626c 6f63 6b20 6578 7472  {% endblock extr
+00002c30: 615f 6a73 2025 7d                        a_js %}
```

### Comparing `forecastmanager-0.0.7/forecastmanager/templates/forecastmanager/forecast_base.html` & `forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/forecast_base.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,86 @@
-{% extends "wagtailadmin/base.html" %} 
+{% extends "wagtailadmin/base.html" %}
 {% load wagtailadmin_tags i18n static %}
 {% load wagtailsettings_tags %}
 {% get_settings use_default_site=True %}
-{% block extra_css %} 
-{{ block.super }}
+{% block extra_css %}
+    {{ block.super }}
 
-<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/handsontable/dist/handsontable.full.min.css" />
-<link href="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.css" rel="stylesheet" />
+    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/handsontable/dist/handsontable.full.min.css"/>
+    <link href="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.css" rel="stylesheet"/>
 
 
-{{ form.media.css }} {% endblock %}
+    {{ form.media.css }} {% endblock %}
 {% block titletag %}
-{% trans 'Forecast Manager' %}
+    {% trans 'Forecast Manager' %}
 {% endblock %}
 
 {% block extra_js %}
-    <script src="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.js"></script>        
-    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/handsontable/dist/handsontable.full.min.js"></script>
+    <script src="https://unpkg.com/maplibre-gl@3.1.0/dist/maplibre-gl.js"></script>
+    <script type="text/javascript"
+            src="https://cdn.jsdelivr.net/npm/handsontable/dist/handsontable.full.min.js"></script>
+    <script src="https://cdn.jsdelivr.net/npm/moment@2.29.4/moment.min.js"></script>
+
     <script src='https://unpkg.com/@turf/turf@6/turf.min.js'></script>
     <script type="text/javascript" src="{% static 'forecastmanager/js/forecast_basemap.js' %}"></script>
 {% endblock extra_js %}
 
 {% block content %}
 
 
-<div class="messages" role="status">
-    <ul>
-        {% if settings.forecastmanager.ForecastSetting.enable_auto_forecast %}
-        <li class="warning">                            
-            <svg class="icon icon-warning messages-icon" aria-hidden="true"><use href="#icon-warning"></use></svg>
-            Autoforecasting has been enabled and manually added forecasts here will be overidden.
-            <span class="buttons">
-                <a href="/admin/settings/forecastmanager/forecastsetting" class="button button-small button-secondary">Change autoforecasting setting</a>
-            </span>
-        </li>
-        {% endif %}
-        
-        <li class="success" id="creatSuccess" style="display:none">
-            <svg class="icon icon-success messages-icon" aria-hidden="true">
-                <use href="#icon-success"></use>
-            </svg>
-            Data Saved Successfuly
-        </li>
-        <li class="error" id="creatError" style="display:none">
-            <svg class="icon icon-warning messages-icon" aria-hidden="true">
-                <use href="#icon-warning"></use>
-            </svg>
-        </li>
-    </ul>
-</div>
-
-{% trans 'Forecast Manager' as title_str %} 
-{% include "wagtailadmin/shared/header.html" with title=title_str icon='form' %} {% include "wagtailadmin/pages/_editor_js.html" %}
-
-<div class="nice-padding">
-
-    {% block forecast %}
-    
-    {% endblock forecast %}
-
-    {% comment %} <div class="createForecast">
-        {% include 'forecastmanager/create_forecast.html' %}
-    </div> {% endcomment %}
+    <div class="messages" role="status">
+        <ul>
+            {% if settings.forecastmanager.ForecastSetting.enable_auto_forecast %}
+                <li class="warning">
+                    <svg class="icon icon-warning messages-icon" aria-hidden="true">
+                        <use href="#icon-warning"></use>
+                    </svg>
+                    {% trans 'Autoforecasting has been enabled and manually added forecasts here will be overidden.' %}'
+                    <span class="buttons">
+                        <a href="/admin/settings/forecastmanager/forecastsetting"
+                           class="button button-small button-secondary">{% trans 'Change autoforecasting setting' %}</a>
+                    </span>
+                </li>
+            {% endif %}
+
+            <li class="success" id="creatSuccess" style="display:none">
+                <svg class="icon icon-success messages-icon" aria-hidden="true">
+                    <use href="#icon-success"></use>
+                </svg>
+                <span class="successMessage"></span>
+            </li>
+            <li class="error" id="creatError" style="display:none">
+                <svg class="icon icon-warning messages-icon" aria-hidden="true">
+                    <use href="#icon-warning"></use>
+                </svg>
+                <span class="errorMessage"></span>
+
+            </li>
+        </ul>
+    </div>
+    {% block header %}
+        {% trans 'Forecast Manager' as title_str %}
+        {% include "wagtailadmin/shared/header.html" with title=title_str icon='form' %}
+    {% endblock %}
+
+
+    {% include "wagtailadmin/pages/_editor_js.html" %}
+
+    <div class="nice-padding">
+
+        {% block forecast %}
+
+        {% endblock forecast %}
+
+        {% comment %}
+            <div class="createForecast">
+                {% include 'forecastmanager/create_forecast.html' %}
+            </div> {% endcomment %}
 
-</div>
+    </div>
 
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -2,19 +2,20 @@
 {% load wagtailsettings_tags %} {% get_settings use_default_site=True %} {%
 block extra_css %} {{ block.super }}
 
  {{ form.media.css }} {% endblock %} {% block titletag %} {% trans 'Forecast
 Manager' %} {% endblock %} {% block extra_js %}
  {% endblock extra_js %} {% block content %}
     * {% if settings.forecastmanager.ForecastSetting.enable_auto_forecast %}
-    *  Autoforecasting has been enabled and manually added forecasts here will
-      be overidden.  Change_autoforecasting_setting
+    *    {% trans 'Autoforecasting has been enabled and manually added
+      forecasts here will be overidden.' %}'  {%_trans_'Change_autoforecasting
+      setting'_%}
     * {% endif %}
-    *    Data Saved Successfuly
     *
-{% trans 'Forecast Manager' as title_str %} {% include "wagtailadmin/shared/
-header.html" with title=title_str icon='form' %} {% include "wagtailadmin/
-pages/_editor_js.html" %}
+    *
+{% block header %} {% trans 'Forecast Manager' as title_str %} {% include
+"wagtailadmin/shared/header.html" with title=title_str icon='form' %} {%
+endblock %} {% include "wagtailadmin/pages/_editor_js.html" %}
 {% block forecast %} {% endblock forecast %} {% comment %}
 {% include 'forecastmanager/create_forecast.html' %}
 {% endcomment %}
 {% endblock %}
```

### Comparing `forecastmanager-0.0.7/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.0.8/forecastmanager/wagtail_hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,99 +1,101 @@
-from django.urls import path, include, reverse
-from wagtail.admin.menu import MenuItem
-from wagtail import hooks
-# from . import urls
-from django.utils.html import format_html
-from django.templatetags.static import static
-from forecastmanager.models import City, DailyWeather
-from forecastmanager.site_settings import ForecastSetting 
-from django.utils.translation import gettext_lazy as _
 from django.urls import path
-from django.urls import re_path
-from forecastmanager.views import add_forecast, save_data,get_forecast
+from django.urls import reverse
+from django.utils.translation import gettext_lazy as _
+from wagtail import hooks
+from wagtail.admin.menu import MenuItem
 from wagtail.contrib.modeladmin.options import (
-    ModelAdmin, 
+    ModelAdmin,
     modeladmin_register,
     ModelAdminGroup
 )
 
+from forecastmanager.models import City, DailyWeather
+from forecastmanager.site_settings import ForecastSetting
+from forecastmanager.views import add_forecast, view_forecast
+
 
 @hooks.register("register_admin_urls")
 def register_admin_urls():
     """
     Registers forecast urls in the wagtail admin.
     """
     return [
-        # path(
-        #     "forecast/",
-        #     include((urls, "forecast"), namespace="forecast_admin"),
-        # ),
-        path("load_forecast/", get_forecast, name="load_forecast"),
-        path("add_forecast/", add_forecast, name="add_forecast"),
-        path('save-data/', save_data, name='save_data'),
-        
+        path("view-forecast/", view_forecast, name="view_forecast"),
+        path("add-forecast/", add_forecast, name="add_forecast"),
     ]
 
 
 class ForecastSettingAdmin(ModelAdmin):
     model = ForecastSetting
-    menu_label = 'Settings'
+    menu_label = _('Settings')
     menu_icon = 'cog'
     add_to_settings_menu = False
     exclude_from_explorer = False
 
+
 class CitiesAdmin(ModelAdmin):
     model = City
-    menu_label = 'Cities'
+    menu_label = _('Cities')
     menu_icon = 'site'
     add_to_settings_menu = False
     exclude_from_explorer = False
 
+
 class DailyWeatherAdmin(ModelAdmin):
     model = DailyWeather
-    menu_label = 'Daily Weather'
+    menu_label = _('Daily Weather')
     menu_icon = 'site'
     add_to_settings_menu = False
     exclude_from_explorer = False
 
 
 # class ConditionCategoryAdmin(ModelAdmin):
 #     model = ConditionCategory
 #     menu_label = 'Weather Conditions'
 #     menu_icon = 'cog'
 #     add_to_settings_menu = False
 #     exclude_from_explorer = False
 
 class CityForecastGroup(ModelAdminGroup):
-    menu_label = 'City Forecast'
+    menu_label = _('City Forecast')
     menu_icon = 'table'  # change as required
     menu_order = 200  # will put in 3rd place (000 being 1st, 100 2nd)
     items = (CitiesAdmin, DailyWeatherAdmin)
 
     def get_submenu_items(self):
         menu_items = []
         item_order = 1
         for modeladmin in self.modeladmin_instances:
             menu_items.append(modeladmin.get_menu_item(order=item_order))
             item_order += 1
 
             # append raster upload link
-        add_forecast_item = MenuItem(label="Add Forecasts", url=reverse("add_forecast"), icon_name="plus")
-        load_forecast_item = MenuItem(label="Load Forecasts", url=reverse("load_forecast"), icon_name="view")
-        
+        add_forecast_item = MenuItem(label=_("Add Forecasts"), url=reverse("add_forecast"), icon_name="plus")
+        load_forecast_item = MenuItem(label=_("View Forecasts"), url=reverse("view_forecast"), icon_name="view")
+
         menu_items.append(add_forecast_item)
         menu_items.append(load_forecast_item)
 
         try:
             settings_url = reverse(
                 "wagtailsettings:edit",
                 args=[ForecastSetting._meta.app_label, ForecastSetting._meta.model_name, ],
             )
             gm_settings_menu = MenuItem(label=_("Settings"), url=settings_url, icon_name="cog")
             menu_items.append(gm_settings_menu)
         except Exception:
             pass
 
         return menu_items
-    
+
 
 modeladmin_register(CityForecastGroup)
+
+
+@hooks.register('construct_settings_menu')
+def hide_settings_menu_item(request, menu_items):
+    # hide forecast setting from setting menu items.
+    # Will be directly accessed from city forecast menu
+    # This is to avoid crowding settings menu
+    hidden_settings = ["forecast-setting"]
+    menu_items[:] = [item for item in menu_items if item.name not in hidden_settings]
```

### Comparing `forecastmanager-0.0.7/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.0.8/forecastmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.7/forecastmanager.egg-info/SOURCES.txt` & `forecastmanager-0.0.8/forecastmanager.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 forecastmanager.egg-info/dependency_links.txt
 forecastmanager.egg-info/requires.txt
 forecastmanager.egg-info/top_level.txt
 forecastmanager/management/__init__.py
 forecastmanager/management/commands/__init__.py
 forecastmanager/management/commands/generate_forecast.py
 forecastmanager/migrations/0001_initial.py
+forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
+forecastmanager/migrations/0003_alter_forecast_unique_together.py
+forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
 forecastmanager/migrations/__init__.py
 forecastmanager/static/forecastmanager/img/clearsky.png
 forecastmanager/static/forecastmanager/img/cloudy.png
 forecastmanager/static/forecastmanager/img/fair.png
 forecastmanager/static/forecastmanager/img/fog.png
 forecastmanager/static/forecastmanager/img/heavyrain.png
 forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
@@ -63,9 +66,8 @@
 forecastmanager/static/forecastmanager/img/snowandthunder.png
 forecastmanager/static/forecastmanager/img/snowshowers.png
 forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
 forecastmanager/static/forecastmanager/js/forecast_basemap.js
 forecastmanager/static/forecastmanager/js/helpers.js
 forecastmanager/templates/forecastmanager/create_forecast.html
 forecastmanager/templates/forecastmanager/forecast_base.html
-forecastmanager/templates/forecastmanager/load_forecast.html
-forecastmanager/templates/forecastmanager/query_forecast.html
+forecastmanager/templates/forecastmanager/view_forecast.html
```

### Comparing `forecastmanager-0.0.7/setup.cfg` & `forecastmanager-0.0.8/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.0.7
+version = 0.0.8
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
@@ -25,12 +25,13 @@
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
 	wagtail>=4.2.2
 	wagtailgeowidget>=7.0.0
 	pandas>=2.0.2
 	psycopg2-binary>=2.9.5
+	django-filter
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

