# Comparing `tmp/forecastmanager-0.0.8.tar.gz` & `tmp/forecastmanager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.0.8.tar", last modified: Sun Jul 16 17:39:04 2023, max compression
+gzip compressed data, was "forecastmanager-0.0.9.tar", last modified: Sun Jul 16 17:49:45 2023, max compression
```

## Comparing `forecastmanager-0.0.8.tar` & `forecastmanager-0.0.9.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/0003_alter_forecast_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/site_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.772605 forecastmanager-0.0.8/forecastmanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.772605 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.780605 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/clearsky.png
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/cloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/fair.png
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/fog.png
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/partlycloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/
--rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/forecast_basemap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/helpers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.772605 forecastmanager-0.0.8/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/forecast_base.html
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/view_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/forecastmanager/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:39:04.776605 forecastmanager-0.0.8/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 17:39:04.000000 forecastmanager-0.0.8/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 17:38:44.000000 forecastmanager-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-16 17:39:04.784605 forecastmanager-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.307843 forecastmanager-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 17:49:45.307843 forecastmanager-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.295842 forecastmanager-0.0.9/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.299842 forecastmanager-0.0.9/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.299842 forecastmanager-0.0.9/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.299842 forecastmanager-0.0.9/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/migrations/0003_alter_forecast_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/site_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.295842 forecastmanager-0.0.9/forecastmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.295842 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.303843 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/clearsky.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/cloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/fair.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/fog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavyrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/partlycloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/rain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/rainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/rainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/sleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/sleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/sleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/snow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/snowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/snowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.303843 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/js/forecast_basemap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/static/forecastmanager/js/helpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.295842 forecastmanager-0.0.9/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.307843 forecastmanager-0.0.9/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/templates/forecastmanager/forecast_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/templates/forecastmanager/view_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/forecastmanager/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:49:45.299842 forecastmanager-0.0.9/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 17:49:45.000000 forecastmanager-0.0.9/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-16 17:49:45.000000 forecastmanager-0.0.9/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:49:45.000000 forecastmanager-0.0.9/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-16 17:49:45.000000 forecastmanager-0.0.9/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 17:49:45.000000 forecastmanager-0.0.9/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 17:49:26.000000 forecastmanager-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-16 17:49:45.307843 forecastmanager-0.0.9/setup.cfg
```

### Comparing `forecastmanager-0.0.8/PKG-INFO` & `forecastmanager-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.8/forecastmanager/blocks.py` & `forecastmanager-0.0.9/forecastmanager/blocks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.0.9/forecastmanager/management/commands/generate_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/migrations/0001_initial.py` & `forecastmanager-0.0.9/forecastmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py` & `forecastmanager-0.0.9/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py` & `forecastmanager-0.0.9/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/models.py` & `forecastmanager-0.0.9/forecastmanager/models.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/serializers.py` & `forecastmanager-0.0.9/forecastmanager/serializers.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/site_settings.py` & `forecastmanager-0.0.9/forecastmanager/site_settings.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/clearsky.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/clearsky.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/cloudy.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/cloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/fair.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/fair.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/fog.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/fog.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrain.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavyrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavyrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleet.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnow.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrain.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrainandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightrainshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleet.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsleetshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnow.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightsnowshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightsnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/partlycloudy.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/partlycloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rain.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/rain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/rainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/rainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleet.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/sleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/sleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/sleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snow.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/snow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/snowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowshowers.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/snowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/forecast_basemap.js` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/js/forecast_basemap.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/static/forecastmanager/js/helpers.js` & `forecastmanager-0.0.9/forecastmanager/static/forecastmanager/js/helpers.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/create_forecast.html` & `forecastmanager-0.0.9/forecastmanager/templates/forecastmanager/create_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/forecast_base.html` & `forecastmanager-0.0.9/forecastmanager/templates/forecastmanager/forecast_base.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/templates/forecastmanager/view_forecast.html` & `forecastmanager-0.0.9/forecastmanager/templates/forecastmanager/view_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/views.py` & `forecastmanager-0.0.9/forecastmanager/views.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.0.9/forecastmanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.8/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.0.9/forecastmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.8
+Version: 0.0.9
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.8/forecastmanager.egg-info/SOURCES.txt` & `forecastmanager-0.0.9/forecastmanager.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 forecastmanager/management/__init__.py
 forecastmanager/management/commands/__init__.py
 forecastmanager/management/commands/generate_forecast.py
 forecastmanager/migrations/0001_initial.py
 forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
 forecastmanager/migrations/0003_alter_forecast_unique_together.py
 forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
+forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
 forecastmanager/migrations/__init__.py
 forecastmanager/static/forecastmanager/img/clearsky.png
 forecastmanager/static/forecastmanager/img/cloudy.png
 forecastmanager/static/forecastmanager/img/fair.png
 forecastmanager/static/forecastmanager/img/fog.png
 forecastmanager/static/forecastmanager/img/heavyrain.png
 forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
```

### Comparing `forecastmanager-0.0.8/setup.cfg` & `forecastmanager-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.0.8
+version = 0.0.9
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

