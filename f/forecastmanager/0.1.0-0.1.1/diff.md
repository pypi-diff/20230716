# Comparing `tmp/forecastmanager-0.1.0.tar.gz` & `tmp/forecastmanager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.1.0.tar", last modified: Sun Jul 16 18:29:08 2023, max compression
+gzip compressed data, was "forecastmanager-0.1.1.tar", last modified: Sun Jul 16 18:52:22 2023, max compression
```

## Comparing `forecastmanager-0.1.0.tar` & `forecastmanager-0.1.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.955564 forecastmanager-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 18:29:08.955564 forecastmanager-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.951564 forecastmanager-0.1.0/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/migrations/0003_alter_forecast_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/site_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.955564 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/clearsky.png
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/cloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/fair.png
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/fog.png
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavyrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/partlycloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/rain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/rainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/rainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/sleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/sleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/sleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/snow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/snowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/snowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.955564 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/js/
--rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/js/forecast_basemap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/static/forecastmanager/js/helpers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.943564 forecastmanager-0.1.0/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.955564 forecastmanager-0.1.0/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/templates/forecastmanager/forecast_base.html
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/templates/forecastmanager/view_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/forecastmanager/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:29:08.947564 forecastmanager-0.1.0/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 18:29:08.000000 forecastmanager-0.1.0/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-16 18:29:08.000000 forecastmanager-0.1.0/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:29:08.000000 forecastmanager-0.1.0/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-16 18:29:08.000000 forecastmanager-0.1.0/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 18:29:08.000000 forecastmanager-0.1.0/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 18:28:50.000000 forecastmanager-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-16 18:29:08.955564 forecastmanager-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.060727 forecastmanager-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 18:52:22.060727 forecastmanager-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.048727 forecastmanager-0.1.1/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.048727 forecastmanager-0.1.1/forecastmanager/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    15641 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.048727 forecastmanager-0.1.1/forecastmanager/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.048727 forecastmanager-0.1.1/forecastmanager/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.048727 forecastmanager-0.1.1/forecastmanager/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.052727 forecastmanager-0.1.1/forecastmanager/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.052727 forecastmanager-0.1.1/forecastmanager/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.052727 forecastmanager-0.1.1/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.052727 forecastmanager-0.1.1/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.052727 forecastmanager-0.1.1/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/migrations/0003_alter_forecast_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/site_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.060727 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/clearsky.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/cloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/fair.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/fog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavyrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/partlycloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/rain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/rainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/rainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/sleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/sleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/sleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/snow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/snowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/snowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.060727 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/js/forecast_basemap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/static/forecastmanager/js/helpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.044727 forecastmanager-0.1.1/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.060727 forecastmanager-0.1.1/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/templates/forecastmanager/forecast_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/templates/forecastmanager/view_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/forecastmanager/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:52:22.048727 forecastmanager-0.1.1/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-16 18:52:22.000000 forecastmanager-0.1.1/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-16 18:52:22.000000 forecastmanager-0.1.1/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:52:22.000000 forecastmanager-0.1.1/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-16 18:52:22.000000 forecastmanager-0.1.1/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 18:52:22.000000 forecastmanager-0.1.1/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 18:52:01.000000 forecastmanager-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-16 18:52:22.064728 forecastmanager-0.1.1/setup.cfg
```

### Comparing `forecastmanager-0.1.0/PKG-INFO` & `forecastmanager-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.1.0/forecastmanager/blocks.py` & `forecastmanager-0.1.1/forecastmanager/blocks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/am/LC_MESSAGES/django.mo` & `forecastmanager-0.1.1/forecastmanager/locale/am/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -322,14 +322,17 @@
 
 msgid "Text"
 msgstr "ጽሑፍ"
 
 msgid "The table is empty. Please input data"
 msgstr "ጠረጴዛው ባዶ ነው። እባክዎን ውሂብ ያስገቡ"
 
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr "የተሰቀለው ፋይል በቀኝ በኩል ካለው ሰንጠረዥ ጋር ተመሳሳይ የሆነ ሲኤስቪ መሆን አለበት።"
+
 msgid "Time"
 msgstr "ጊዜ"
 
 msgid "Topics, references, & how-tos"
 msgstr "ርዕሶች፣ ማጣቀሻዎች እና እንዴት እንደሚደረግ"
 
 msgid "Tutorial"
@@ -372,7 +375,12 @@
 msgstr "የንፋስ ፍጥነት"
 
 msgid "You can"
 msgstr "ትችላለህ"
 
 msgid "download a template"
 msgstr "አብነት አውርድ"
+
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr "የCSV ከመስመር ውጭ አርትዖት እና እዚህ ይስቀሉት። አብነቱ በሁሉም ቅድመ-ነባር ከተሞች ቀድሞ ተሞልቷል።"
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/am/LC_MESSAGES/django.po` & `forecastmanager-0.1.1/forecastmanager/locale/am/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,80 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-16 17:25+0000\n"
+"POT-Creation-Date: 2023-07-16 18:40+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
+#: sandbox/home/templates/home/welcome_page.html:6
+msgid "Visit the Wagtail website"
+msgstr "የWagtail ድህረ ገጽን ይጎብኙ"
+
+#: sandbox/home/templates/home/welcome_page.html:15
+msgid "View the release notes"
+msgstr "የመልቀቂያ ማስታወሻዎችን ይመልከቱ"
+
+#: sandbox/home/templates/home/welcome_page.html:27
+msgid "Welcome to your new Wagtail site!"
+msgstr "ወደ አዲሱ የዋግቴል ጣቢያ እንኳን በደህና መጡ!"
+
+#: sandbox/home/templates/home/welcome_page.html:28
+msgid ""
+"Please feel free to <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
+" Slack</a>, or get started with one of the links below."
+msgstr ""
+"እባክዎ <a href=\"https://github.com/wagtail/wagtail/wiki/Slack\">በSlack ላይ "
+"ማህበረሰባችንን ለመቀላቀል</a>፣ ወይም ከታች ካሉት ማገናኛዎች በአንዱ ይጀምሩ።"
+
+#: sandbox/home/templates/home/welcome_page.html:35
+msgid "Wagtail Documentation"
+msgstr "Wagtail ሰነድ"
+
+#: sandbox/home/templates/home/welcome_page.html:36
+msgid "Topics, references, & how-tos"
+msgstr "ርዕሶች፣ ማጣቀሻዎች እና እንዴት እንደሚደረግ"
+
+#: sandbox/home/templates/home/welcome_page.html:42
+msgid "Tutorial"
+msgstr "አጋዥ ስልጠና"
+
+#: sandbox/home/templates/home/welcome_page.html:43
+msgid "Build your first Wagtail site"
+msgstr "የመጀመሪያውን የWagtail ጣቢያዎን ይገንቡ"
+
+#: sandbox/home/templates/home/welcome_page.html:49
+msgid "Admin Interface"
+msgstr "የአስተዳዳሪ በይነገጽ"
+
+#: sandbox/home/templates/home/welcome_page.html:50
+msgid "Create your superuser first!"
+msgstr "መጀመሪያ ሱፐር ተጠቃሚዎን ይፍጠሩ!"
+
+#: sandbox/home/templates/integration/dailyweather_include.html:3
+#: forecastmanager/wagtail_hooks.py:46
+msgid "Daily Weather"
+msgstr "ዕለታዊ የአየር ሁኔታ"
+
+#: sandbox/home/templates/integration/forecasts_include.html:3
+#: forecastmanager/models.py:127
+msgid "Forecasts"
+msgstr "ትንበያዎች"
+
 #: forecastmanager/models.py:16
-#: forecastmanager/templates/forecastmanager/create_forecast.html:57
+#: forecastmanager/templates/forecastmanager/create_forecast.html:54
 #: forecastmanager/templates/forecastmanager/view_forecast.html:29
 msgid "Forecast Date"
 msgstr "የትንበያ ቀን"
 
 #: forecastmanager/models.py:17
 msgid "Weather Forecast Description"
 msgstr "የአየር ሁኔታ ትንበያ መግለጫ"
@@ -48,15 +103,15 @@
 msgstr "የከተማ ስም"
 
 #: forecastmanager/models.py:54
 msgid "City Location (Lat, Lng)"
 msgstr "የከተማ አካባቢ (ላት፣ ኤልንግ)"
 
 #: forecastmanager/models.py:62 forecastmanager/models.py:117
-#: forecastmanager/templates/forecastmanager/create_forecast.html:138
+#: forecastmanager/templates/forecastmanager/create_forecast.html:134
 msgid "City"
 msgstr "ከተማ"
 
 #: forecastmanager/models.py:63 forecastmanager/wagtail_hooks.py:38
 msgid "Cities"
 msgstr "ከተሞች"
 
@@ -224,19 +279,14 @@
 msgid "E.g Light Showers"
 msgstr "ለምሳሌ የብርሃን ሻወር"
 
 #: forecastmanager/models.py:126
 msgid "Forecast"
 msgstr "ትንበያ"
 
-#: forecastmanager/models.py:127
-#: sandbox/home/templates/integration/forecasts_include.html:3
-msgid "Forecasts"
-msgstr "ትንበያዎች"
-
 #: forecastmanager/site_settings.py:20
 msgid "Enable automated forecasts"
 msgstr "ራስ-ሰር ትንበያዎችን አንቃ"
 
 #: forecastmanager/site_settings.py:36
 msgid "Temperature"
 msgstr "የሙቀት መጠን"
@@ -373,43 +423,53 @@
 msgid "You can"
 msgstr "ትችላለህ"
 
 #: forecastmanager/templates/forecastmanager/create_forecast.html:46
 msgid "download a template"
 msgstr "አብነት አውርድ"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:61
+#: forecastmanager/templates/forecastmanager/create_forecast.html:46
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr "የCSV ከመስመር ውጭ አርትዖት እና እዚህ ይስቀሉት። አብነቱ በሁሉም ቅድመ-ነባር ከተሞች ቀድሞ ተሞልቷል።"
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:58
 msgid "Date of forecast"
 msgstr "የትንበያ ቀን"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:84
+#: forecastmanager/templates/forecastmanager/create_forecast.html:81
 msgid "Forecast effective period"
 msgstr "ውጤታማ ጊዜ ትንበያ"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:107
+#: forecastmanager/templates/forecastmanager/create_forecast.html:104
 msgid "Forecast Upload"
 msgstr "የትንበያ ጭነት"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:132
+#: forecastmanager/templates/forecastmanager/create_forecast.html:111
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr "የተሰቀለው ፋይል በቀኝ በኩል ካለው ሰንጠረዥ ጋር ተመሳሳይ የሆነ ሲኤስቪ መሆን አለበት።"
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:128
 msgid "Verify that all columns match correctly"
 msgstr "ሁሉም አምዶች በትክክል የሚዛመዱ መሆናቸውን ያረጋግጡ"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:159
+#: forecastmanager/templates/forecastmanager/create_forecast.html:155
 msgid "Condition"
 msgstr "ሁኔታ"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:170
+#: forecastmanager/templates/forecastmanager/create_forecast.html:166
 msgid "Publish"
 msgstr "አትም"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:356
+#: forecastmanager/templates/forecastmanager/create_forecast.html:352
 msgid "The table is empty. Please input data"
 msgstr "ጠረጴዛው ባዶ ነው። እባክዎን ውሂብ ያስገቡ"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:362
+#: forecastmanager/templates/forecastmanager/create_forecast.html:358
 msgid "Table contains invalid inputs"
 msgstr "ሠንጠረዥ ልክ ያልሆኑ ግብዓቶችን ይዟል"
 
 #: forecastmanager/templates/forecastmanager/forecast_base.html:14
 #: forecastmanager/templates/forecastmanager/forecast_base.html:61
 msgid "Forecast Manager"
 msgstr "ትንበያ አስተዳዳሪ"
@@ -449,64 +509,14 @@
 msgid "Invalid request"
 msgstr "ልክ ያልሆነ ጥያቄ"
 
 #: forecastmanager/wagtail_hooks.py:30 forecastmanager/wagtail_hooks.py:84
 msgid "Settings"
 msgstr "ቅንብሮች"
 
-#: forecastmanager/wagtail_hooks.py:46
-#: sandbox/home/templates/integration/dailyweather_include.html:3
-msgid "Daily Weather"
-msgstr "ዕለታዊ የአየር ሁኔታ"
-
 #: forecastmanager/wagtail_hooks.py:60
 msgid "City Forecast"
 msgstr "የከተማ ትንበያ"
 
 #: forecastmanager/wagtail_hooks.py:73
 msgid "Add Forecasts"
 msgstr "ትንበያዎችን ያክሉ"
-
-#: sandbox/home/templates/home/welcome_page.html:6
-msgid "Visit the Wagtail website"
-msgstr "የWagtail ድህረ ገጽን ይጎብኙ"
-
-#: sandbox/home/templates/home/welcome_page.html:15
-msgid "View the release notes"
-msgstr "የመልቀቂያ ማስታወሻዎችን ይመልከቱ"
-
-#: sandbox/home/templates/home/welcome_page.html:27
-msgid "Welcome to your new Wagtail site!"
-msgstr "ወደ አዲሱ የዋግቴል ጣቢያ እንኳን በደህና መጡ!"
-
-#: sandbox/home/templates/home/welcome_page.html:28
-msgid ""
-"Please feel free to <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
-" Slack</a>, or get started with one of the links below."
-msgstr ""
-"እባክዎ <a href=\"https://github.com/wagtail/wagtail/wiki/Slack\">በSlack ላይ "
-"ማህበረሰባችንን ለመቀላቀል</a>፣ ወይም ከታች ካሉት ማገናኛዎች በአንዱ ይጀምሩ።"
-
-#: sandbox/home/templates/home/welcome_page.html:35
-msgid "Wagtail Documentation"
-msgstr "Wagtail ሰነድ"
-
-#: sandbox/home/templates/home/welcome_page.html:36
-msgid "Topics, references, & how-tos"
-msgstr "ርዕሶች፣ ማጣቀሻዎች እና እንዴት እንደሚደረግ"
-
-#: sandbox/home/templates/home/welcome_page.html:42
-msgid "Tutorial"
-msgstr "አጋዥ ስልጠና"
-
-#: sandbox/home/templates/home/welcome_page.html:43
-msgid "Build your first Wagtail site"
-msgstr "የመጀመሪያውን የWagtail ጣቢያዎን ይገንቡ"
-
-#: sandbox/home/templates/home/welcome_page.html:49
-msgid "Admin Interface"
-msgstr "የአስተዳዳሪ በይነገጽ"
-
-#: sandbox/home/templates/home/welcome_page.html:50
-msgid "Create your superuser first!"
-msgstr "መጀመሪያ ሱፐር ተጠቃሚዎን ይፍጠሩ!"
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/ar/LC_MESSAGES/django.mo` & `forecastmanager-0.1.1/forecastmanager/locale/ar/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -324,14 +324,19 @@
 
 msgid "Text"
 msgstr "نص"
 
 msgid "The table is empty. Please input data"
 msgstr "الجدول فارغ. الرجاء إدخال البيانات"
 
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr ""
+"يجب أن يكون الملف الذي تم تحميله بتنسيق CSV ، مشابهًا للجدول الموجود على "
+"اليسار"
+
 msgid "Time"
 msgstr "وقت"
 
 msgid "Topics, references, & how-tos"
 msgstr "الموضوعات والمراجع وطرق التنفيذ"
 
 msgid "Tutorial"
@@ -374,7 +379,14 @@
 msgstr "سرعة الرياح"
 
 msgid "You can"
 msgstr "أنت تستطيع"
 
 msgid "download a template"
 msgstr "تنزيل نموذج"
+
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"من ملف CSV للتحرير في وضع عدم الاتصال وتحميله هنا. يأتي النموذج معبأ مسبقًا "
+"بجميع المدن الموجودة مسبقًا."
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/ar/LC_MESSAGES/django.po` & `forecastmanager-0.1.1/forecastmanager/locale/ar/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,81 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-16 17:21+0000\n"
+"POT-Creation-Date: 2023-07-16 18:40+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
+#: sandbox/home/templates/home/welcome_page.html:6
+msgid "Visit the Wagtail website"
+msgstr "قم بزيارة موقع Wagtail"
+
+#: sandbox/home/templates/home/welcome_page.html:15
+msgid "View the release notes"
+msgstr "عرض ملاحظات الإصدار"
+
+#: sandbox/home/templates/home/welcome_page.html:27
+msgid "Welcome to your new Wagtail site!"
+msgstr "مرحبا بكم في موقع الذعرة الجديد الخاص بك!"
+
+#: sandbox/home/templates/home/welcome_page.html:28
+msgid ""
+"Please feel free to <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
+" Slack</a>, or get started with one of the links below."
+msgstr ""
+"لا تتردد في <a href=\"https://github.com/wagtail/wagtail/wiki/Slack\"> "
+"الانضمام إلى مجتمعنا على Slack </a> ، أو البدء باستخدام أحد الروابط أدناه."
+
+#: sandbox/home/templates/home/welcome_page.html:35
+msgid "Wagtail Documentation"
+msgstr "توثيق الذعرة"
+
+#: sandbox/home/templates/home/welcome_page.html:36
+msgid "Topics, references, & how-tos"
+msgstr "الموضوعات والمراجع وطرق التنفيذ"
+
+#: sandbox/home/templates/home/welcome_page.html:42
+msgid "Tutorial"
+msgstr "درس تعليمي"
+
+#: sandbox/home/templates/home/welcome_page.html:43
+msgid "Build your first Wagtail site"
+msgstr "بناء موقع الذعرة الأول الخاص بك"
+
+#: sandbox/home/templates/home/welcome_page.html:49
+msgid "Admin Interface"
+msgstr "واجهة المسؤول"
+
+#: sandbox/home/templates/home/welcome_page.html:50
+msgid "Create your superuser first!"
+msgstr "قم بإنشاء المستخدم المتميز الخاص بك أولاً!"
+
+#: sandbox/home/templates/integration/dailyweather_include.html:3
+#: forecastmanager/wagtail_hooks.py:46
+msgid "Daily Weather"
+msgstr "الطقس اليومي"
+
+#: sandbox/home/templates/integration/forecasts_include.html:3
+#: forecastmanager/models.py:127
+msgid "Forecasts"
+msgstr "التنبؤ"
+
 #: forecastmanager/models.py:16
-#: forecastmanager/templates/forecastmanager/create_forecast.html:57
+#: forecastmanager/templates/forecastmanager/create_forecast.html:54
 #: forecastmanager/templates/forecastmanager/view_forecast.html:29
 msgid "Forecast Date"
 msgstr "تاريخ التنبؤ"
 
 #: forecastmanager/models.py:17
 msgid "Weather Forecast Description"
 msgstr "وصف توقعات الطقس"
@@ -49,15 +104,15 @@
 msgstr "اسم المدينة"
 
 #: forecastmanager/models.py:54
 msgid "City Location (Lat, Lng)"
 msgstr "موقع المدينة (Lat ، Lng)"
 
 #: forecastmanager/models.py:62 forecastmanager/models.py:117
-#: forecastmanager/templates/forecastmanager/create_forecast.html:138
+#: forecastmanager/templates/forecastmanager/create_forecast.html:134
 msgid "City"
 msgstr "مدينة"
 
 #: forecastmanager/models.py:63 forecastmanager/wagtail_hooks.py:38
 msgid "Cities"
 msgstr "مدن"
 
@@ -225,19 +280,14 @@
 msgid "E.g Light Showers"
 msgstr "على سبيل المثال الاستحمام الخفيفة"
 
 #: forecastmanager/models.py:126
 msgid "Forecast"
 msgstr "تنبؤ بالمناخ"
 
-#: forecastmanager/models.py:127
-#: sandbox/home/templates/integration/forecasts_include.html:3
-msgid "Forecasts"
-msgstr "التنبؤ"
-
 #: forecastmanager/site_settings.py:20
 msgid "Enable automated forecasts"
 msgstr "تمكين التنبؤات الآلية"
 
 #: forecastmanager/site_settings.py:36
 msgid "Temperature"
 msgstr "درجة حرارة"
@@ -374,43 +424,57 @@
 msgid "You can"
 msgstr "أنت تستطيع"
 
 #: forecastmanager/templates/forecastmanager/create_forecast.html:46
 msgid "download a template"
 msgstr "تنزيل نموذج"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:61
+#: forecastmanager/templates/forecastmanager/create_forecast.html:46
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"من ملف CSV للتحرير في وضع عدم الاتصال وتحميله هنا. يأتي النموذج معبأ مسبقًا "
+"بجميع المدن الموجودة مسبقًا."
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:58
 msgid "Date of forecast"
 msgstr "تاريخ التوقعات"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:84
+#: forecastmanager/templates/forecastmanager/create_forecast.html:81
 msgid "Forecast effective period"
 msgstr "فترة فعالية التنبؤ"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:107
+#: forecastmanager/templates/forecastmanager/create_forecast.html:104
 msgid "Forecast Upload"
 msgstr "تحميل التوقعات"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:132
+#: forecastmanager/templates/forecastmanager/create_forecast.html:111
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr ""
+"يجب أن يكون الملف الذي تم تحميله بتنسيق CSV ، مشابهًا للجدول الموجود على "
+"اليسار"
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:128
 msgid "Verify that all columns match correctly"
 msgstr "تحقق من تطابق جميع الأعمدة بشكل صحيح"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:159
+#: forecastmanager/templates/forecastmanager/create_forecast.html:155
 msgid "Condition"
 msgstr "حالة"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:170
+#: forecastmanager/templates/forecastmanager/create_forecast.html:166
 msgid "Publish"
 msgstr "ينشر"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:356
+#: forecastmanager/templates/forecastmanager/create_forecast.html:352
 msgid "The table is empty. Please input data"
 msgstr "الجدول فارغ. الرجاء إدخال البيانات"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:362
+#: forecastmanager/templates/forecastmanager/create_forecast.html:358
 msgid "Table contains invalid inputs"
 msgstr "يحتوي الجدول على مدخلات غير صالحة"
 
 #: forecastmanager/templates/forecastmanager/forecast_base.html:14
 #: forecastmanager/templates/forecastmanager/forecast_base.html:61
 msgid "Forecast Manager"
 msgstr "مدير التنبؤ"
@@ -450,64 +514,14 @@
 msgid "Invalid request"
 msgstr "طلب غير صالح"
 
 #: forecastmanager/wagtail_hooks.py:30 forecastmanager/wagtail_hooks.py:84
 msgid "Settings"
 msgstr "إعدادات"
 
-#: forecastmanager/wagtail_hooks.py:46
-#: sandbox/home/templates/integration/dailyweather_include.html:3
-msgid "Daily Weather"
-msgstr "الطقس اليومي"
-
 #: forecastmanager/wagtail_hooks.py:60
 msgid "City Forecast"
 msgstr "توقعات المدينة"
 
 #: forecastmanager/wagtail_hooks.py:73
 msgid "Add Forecasts"
 msgstr "أضف التوقعات"
-
-#: sandbox/home/templates/home/welcome_page.html:6
-msgid "Visit the Wagtail website"
-msgstr "قم بزيارة موقع Wagtail"
-
-#: sandbox/home/templates/home/welcome_page.html:15
-msgid "View the release notes"
-msgstr "عرض ملاحظات الإصدار"
-
-#: sandbox/home/templates/home/welcome_page.html:27
-msgid "Welcome to your new Wagtail site!"
-msgstr "مرحبا بكم في موقع الذعرة الجديد الخاص بك!"
-
-#: sandbox/home/templates/home/welcome_page.html:28
-msgid ""
-"Please feel free to <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
-" Slack</a>, or get started with one of the links below."
-msgstr ""
-"لا تتردد في <a href=\"https://github.com/wagtail/wagtail/wiki/Slack\"> "
-"الانضمام إلى مجتمعنا على Slack </a> ، أو البدء باستخدام أحد الروابط أدناه."
-
-#: sandbox/home/templates/home/welcome_page.html:35
-msgid "Wagtail Documentation"
-msgstr "توثيق الذعرة"
-
-#: sandbox/home/templates/home/welcome_page.html:36
-msgid "Topics, references, & how-tos"
-msgstr "الموضوعات والمراجع وطرق التنفيذ"
-
-#: sandbox/home/templates/home/welcome_page.html:42
-msgid "Tutorial"
-msgstr "درس تعليمي"
-
-#: sandbox/home/templates/home/welcome_page.html:43
-msgid "Build your first Wagtail site"
-msgstr "بناء موقع الذعرة الأول الخاص بك"
-
-#: sandbox/home/templates/home/welcome_page.html:49
-msgid "Admin Interface"
-msgstr "واجهة المسؤول"
-
-#: sandbox/home/templates/home/welcome_page.html:50
-msgid "Create your superuser first!"
-msgstr "قم بإنشاء المستخدم المتميز الخاص بك أولاً!"
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/en/LC_MESSAGES/django.mo` & `forecastmanager-0.1.1/forecastmanager/locale/en/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -326,14 +326,17 @@
 
 msgid "Text"
 msgstr "Text"
 
 msgid "The table is empty. Please input data"
 msgstr "The table is empty. Please input data"
 
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr "The uploaded file should be a CSV, similar to the table on the right"
+
 msgid "Time"
 msgstr "Time"
 
 msgid "Topics, references, & how-tos"
 msgstr "Topics, references, & how-tos"
 
 msgid "Tutorial"
@@ -376,7 +379,14 @@
 msgstr "Wind Speed"
 
 msgid "You can"
 msgstr "You can"
 
 msgid "download a template"
 msgstr "download a template"
+
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/en/LC_MESSAGES/django.po` & `forecastmanager-0.1.1/forecastmanager/locale/en/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,82 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-16 17:25+0000\n"
+"POT-Creation-Date: 2023-07-16 18:40+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+#: sandbox/home/templates/home/welcome_page.html:6
+msgid "Visit the Wagtail website"
+msgstr "Visit the Wagtail website"
+
+#: sandbox/home/templates/home/welcome_page.html:15
+msgid "View the release notes"
+msgstr "View the release notes"
+
+#: sandbox/home/templates/home/welcome_page.html:27
+msgid "Welcome to your new Wagtail site!"
+msgstr "Welcome to your new Wagtail site!"
+
+#: sandbox/home/templates/home/welcome_page.html:28
+msgid ""
+"Please feel free to <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
+" Slack</a>, or get started with one of the links below."
+msgstr ""
+"Please feel free to <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
+" Slack</a>, or get started with one of the links below."
+
+#: sandbox/home/templates/home/welcome_page.html:35
+msgid "Wagtail Documentation"
+msgstr "Wagtail Documentation"
+
+#: sandbox/home/templates/home/welcome_page.html:36
+msgid "Topics, references, & how-tos"
+msgstr "Topics, references, & how-tos"
+
+#: sandbox/home/templates/home/welcome_page.html:42
+msgid "Tutorial"
+msgstr "Tutorial"
+
+#: sandbox/home/templates/home/welcome_page.html:43
+msgid "Build your first Wagtail site"
+msgstr "Build your first Wagtail site"
+
+#: sandbox/home/templates/home/welcome_page.html:49
+msgid "Admin Interface"
+msgstr "Admin Interface"
+
+#: sandbox/home/templates/home/welcome_page.html:50
+msgid "Create your superuser first!"
+msgstr "Create your superuser first!"
+
+#: sandbox/home/templates/integration/dailyweather_include.html:3
+#: forecastmanager/wagtail_hooks.py:46
+msgid "Daily Weather"
+msgstr "Daily Weather"
+
+#: sandbox/home/templates/integration/forecasts_include.html:3
+#: forecastmanager/models.py:127
+msgid "Forecasts"
+msgstr "Forecasts"
+
 #: forecastmanager/models.py:16
-#: forecastmanager/templates/forecastmanager/create_forecast.html:57
+#: forecastmanager/templates/forecastmanager/create_forecast.html:54
 #: forecastmanager/templates/forecastmanager/view_forecast.html:29
 msgid "Forecast Date"
 msgstr "Forecast Date"
 
 #: forecastmanager/models.py:17
 msgid "Weather Forecast Description"
 msgstr "Weather Forecast Description"
@@ -49,15 +105,15 @@
 msgstr "City Name"
 
 #: forecastmanager/models.py:54
 msgid "City Location (Lat, Lng)"
 msgstr "City Location (Lat, Lng)"
 
 #: forecastmanager/models.py:62 forecastmanager/models.py:117
-#: forecastmanager/templates/forecastmanager/create_forecast.html:138
+#: forecastmanager/templates/forecastmanager/create_forecast.html:134
 msgid "City"
 msgstr "City"
 
 #: forecastmanager/models.py:63 forecastmanager/wagtail_hooks.py:38
 msgid "Cities"
 msgstr "Cities"
 
@@ -225,19 +281,14 @@
 msgid "E.g Light Showers"
 msgstr "E.g Light Showers"
 
 #: forecastmanager/models.py:126
 msgid "Forecast"
 msgstr "Forecast"
 
-#: forecastmanager/models.py:127
-#: sandbox/home/templates/integration/forecasts_include.html:3
-msgid "Forecasts"
-msgstr "Forecasts"
-
 #: forecastmanager/site_settings.py:20
 msgid "Enable automated forecasts"
 msgstr "Enable automated forecasts"
 
 #: forecastmanager/site_settings.py:36
 msgid "Temperature"
 msgstr "Temperature"
@@ -374,43 +425,55 @@
 msgid "You can"
 msgstr "You can"
 
 #: forecastmanager/templates/forecastmanager/create_forecast.html:46
 msgid "download a template"
 msgstr "download a template"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:61
+#: forecastmanager/templates/forecastmanager/create_forecast.html:46
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:58
 msgid "Date of forecast"
 msgstr "Date of forecast"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:84
+#: forecastmanager/templates/forecastmanager/create_forecast.html:81
 msgid "Forecast effective period"
 msgstr "Forecast effective period"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:107
+#: forecastmanager/templates/forecastmanager/create_forecast.html:104
 msgid "Forecast Upload"
 msgstr "Forecast Upload"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:132
+#: forecastmanager/templates/forecastmanager/create_forecast.html:111
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr "The uploaded file should be a CSV, similar to the table on the right"
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:128
 msgid "Verify that all columns match correctly"
 msgstr "Verify that all columns match correctly"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:159
+#: forecastmanager/templates/forecastmanager/create_forecast.html:155
 msgid "Condition"
 msgstr "Condition"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:170
+#: forecastmanager/templates/forecastmanager/create_forecast.html:166
 msgid "Publish"
 msgstr "Publish"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:356
+#: forecastmanager/templates/forecastmanager/create_forecast.html:352
 msgid "The table is empty. Please input data"
 msgstr "The table is empty. Please input data"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:362
+#: forecastmanager/templates/forecastmanager/create_forecast.html:358
 msgid "Table contains invalid inputs"
 msgstr "Table contains invalid inputs"
 
 #: forecastmanager/templates/forecastmanager/forecast_base.html:14
 #: forecastmanager/templates/forecastmanager/forecast_base.html:61
 msgid "Forecast Manager"
 msgstr "Forecast Manager"
@@ -452,65 +515,14 @@
 msgid "Invalid request"
 msgstr "Invalid request"
 
 #: forecastmanager/wagtail_hooks.py:30 forecastmanager/wagtail_hooks.py:84
 msgid "Settings"
 msgstr "Settings"
 
-#: forecastmanager/wagtail_hooks.py:46
-#: sandbox/home/templates/integration/dailyweather_include.html:3
-msgid "Daily Weather"
-msgstr "Daily Weather"
-
 #: forecastmanager/wagtail_hooks.py:60
 msgid "City Forecast"
 msgstr "City Forecast"
 
 #: forecastmanager/wagtail_hooks.py:73
 msgid "Add Forecasts"
 msgstr "Add Forecasts"
-
-#: sandbox/home/templates/home/welcome_page.html:6
-msgid "Visit the Wagtail website"
-msgstr "Visit the Wagtail website"
-
-#: sandbox/home/templates/home/welcome_page.html:15
-msgid "View the release notes"
-msgstr "View the release notes"
-
-#: sandbox/home/templates/home/welcome_page.html:27
-msgid "Welcome to your new Wagtail site!"
-msgstr "Welcome to your new Wagtail site!"
-
-#: sandbox/home/templates/home/welcome_page.html:28
-msgid ""
-"Please feel free to <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
-" Slack</a>, or get started with one of the links below."
-msgstr ""
-"Please feel free to <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
-" Slack</a>, or get started with one of the links below."
-
-#: sandbox/home/templates/home/welcome_page.html:35
-msgid "Wagtail Documentation"
-msgstr "Wagtail Documentation"
-
-#: sandbox/home/templates/home/welcome_page.html:36
-msgid "Topics, references, & how-tos"
-msgstr "Topics, references, & how-tos"
-
-#: sandbox/home/templates/home/welcome_page.html:42
-msgid "Tutorial"
-msgstr "Tutorial"
-
-#: sandbox/home/templates/home/welcome_page.html:43
-msgid "Build your first Wagtail site"
-msgstr "Build your first Wagtail site"
-
-#: sandbox/home/templates/home/welcome_page.html:49
-msgid "Admin Interface"
-msgstr "Admin Interface"
-
-#: sandbox/home/templates/home/welcome_page.html:50
-msgid "Create your superuser first!"
-msgstr "Create your superuser first!"
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/es/LC_MESSAGES/django.mo` & `forecastmanager-0.1.1/forecastmanager/locale/es/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -326,14 +326,17 @@
 
 msgid "Text"
 msgstr "Texto"
 
 msgid "The table is empty. Please input data"
 msgstr "La mesa está vacía. Por favor ingrese datos"
 
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr "El archivo cargado debe ser un CSV, similar a la tabla de la derecha"
+
 msgid "Time"
 msgstr "Tiempo"
 
 msgid "Topics, references, & how-tos"
 msgstr "Temas, referencias y procedimientos"
 
 msgid "Tutorial"
@@ -376,7 +379,14 @@
 msgstr "Velocidad del viento"
 
 msgid "You can"
 msgstr "Puede"
 
 msgid "download a template"
 msgstr "descargar una plantilla"
+
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"del CSV para editarlo sin conexión y cargarlo aquí. La plantilla viene "
+"rellenada previamente con todas las ciudades preexistentes."
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/es/LC_MESSAGES/django.po` & `forecastmanager-0.1.1/forecastmanager/locale/es/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,82 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-16 17:25+0000\n"
+"POT-Creation-Date: 2023-07-16 18:40+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+#: sandbox/home/templates/home/welcome_page.html:6
+msgid "Visit the Wagtail website"
+msgstr "Visite el sitio web de Lavandera"
+
+#: sandbox/home/templates/home/welcome_page.html:15
+msgid "View the release notes"
+msgstr "Ver las notas de la versión"
+
+#: sandbox/home/templates/home/welcome_page.html:27
+msgid "Welcome to your new Wagtail site!"
+msgstr "¡Bienvenido a su nuevo sitio de Wagtail!"
+
+#: sandbox/home/templates/home/welcome_page.html:28
+msgid ""
+"Please feel free to <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
+" Slack</a>, or get started with one of the links below."
+msgstr ""
+"Siéntete libre de <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">únete a nuestra "
+"comunidad en Slack</a>, o comienza con uno de los enlaces a continuación."
+
+#: sandbox/home/templates/home/welcome_page.html:35
+msgid "Wagtail Documentation"
+msgstr "Documentación de lavandera"
+
+#: sandbox/home/templates/home/welcome_page.html:36
+msgid "Topics, references, & how-tos"
+msgstr "Temas, referencias y procedimientos"
+
+#: sandbox/home/templates/home/welcome_page.html:42
+msgid "Tutorial"
+msgstr "Tutorial"
+
+#: sandbox/home/templates/home/welcome_page.html:43
+msgid "Build your first Wagtail site"
+msgstr "Crea tu primer sitio de Wagtail"
+
+#: sandbox/home/templates/home/welcome_page.html:49
+msgid "Admin Interface"
+msgstr "Interfaz de administración"
+
+#: sandbox/home/templates/home/welcome_page.html:50
+msgid "Create your superuser first!"
+msgstr "¡Crea tu superusuario primero!"
+
+#: sandbox/home/templates/integration/dailyweather_include.html:3
+#: forecastmanager/wagtail_hooks.py:46
+msgid "Daily Weather"
+msgstr "Clima diario"
+
+#: sandbox/home/templates/integration/forecasts_include.html:3
+#: forecastmanager/models.py:127
+msgid "Forecasts"
+msgstr "Pronósticos"
+
 #: forecastmanager/models.py:16
-#: forecastmanager/templates/forecastmanager/create_forecast.html:57
+#: forecastmanager/templates/forecastmanager/create_forecast.html:54
 #: forecastmanager/templates/forecastmanager/view_forecast.html:29
 msgid "Forecast Date"
 msgstr "Fecha pronóstico"
 
 #: forecastmanager/models.py:17
 msgid "Weather Forecast Description"
 msgstr "Descripción del pronóstico del tiempo"
@@ -49,15 +105,15 @@
 msgstr "Nombre de la ciudad"
 
 #: forecastmanager/models.py:54
 msgid "City Location (Lat, Lng)"
 msgstr "Ciudad Ubicación (Lat, Lng)"
 
 #: forecastmanager/models.py:62 forecastmanager/models.py:117
-#: forecastmanager/templates/forecastmanager/create_forecast.html:138
+#: forecastmanager/templates/forecastmanager/create_forecast.html:134
 msgid "City"
 msgstr "Ciudad"
 
 #: forecastmanager/models.py:63 forecastmanager/wagtail_hooks.py:38
 msgid "Cities"
 msgstr "Ciudades"
 
@@ -225,19 +281,14 @@
 msgid "E.g Light Showers"
 msgstr "Por ejemplo, lluvias ligeras"
 
 #: forecastmanager/models.py:126
 msgid "Forecast"
 msgstr "Pronóstico"
 
-#: forecastmanager/models.py:127
-#: sandbox/home/templates/integration/forecasts_include.html:3
-msgid "Forecasts"
-msgstr "Pronósticos"
-
 #: forecastmanager/site_settings.py:20
 msgid "Enable automated forecasts"
 msgstr "Habilitar pronósticos automatizados"
 
 #: forecastmanager/site_settings.py:36
 msgid "Temperature"
 msgstr "Temperatura"
@@ -374,43 +425,55 @@
 msgid "You can"
 msgstr "Puede"
 
 #: forecastmanager/templates/forecastmanager/create_forecast.html:46
 msgid "download a template"
 msgstr "descargar una plantilla"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:61
+#: forecastmanager/templates/forecastmanager/create_forecast.html:46
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"del CSV para editarlo sin conexión y cargarlo aquí. La plantilla viene "
+"rellenada previamente con todas las ciudades preexistentes."
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:58
 msgid "Date of forecast"
 msgstr "Fecha de pronóstico"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:84
+#: forecastmanager/templates/forecastmanager/create_forecast.html:81
 msgid "Forecast effective period"
 msgstr "Período de vigencia de la previsión"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:107
+#: forecastmanager/templates/forecastmanager/create_forecast.html:104
 msgid "Forecast Upload"
 msgstr "Carga de pronóstico"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:132
+#: forecastmanager/templates/forecastmanager/create_forecast.html:111
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr "El archivo cargado debe ser un CSV, similar a la tabla de la derecha"
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:128
 msgid "Verify that all columns match correctly"
 msgstr "Verifique que todas las columnas coincidan correctamente"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:159
+#: forecastmanager/templates/forecastmanager/create_forecast.html:155
 msgid "Condition"
 msgstr "Condición"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:170
+#: forecastmanager/templates/forecastmanager/create_forecast.html:166
 msgid "Publish"
 msgstr "Publicar"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:356
+#: forecastmanager/templates/forecastmanager/create_forecast.html:352
 msgid "The table is empty. Please input data"
 msgstr "La mesa está vacía. Por favor ingrese datos"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:362
+#: forecastmanager/templates/forecastmanager/create_forecast.html:358
 msgid "Table contains invalid inputs"
 msgstr "La tabla contiene entradas no válidas"
 
 #: forecastmanager/templates/forecastmanager/forecast_base.html:14
 #: forecastmanager/templates/forecastmanager/forecast_base.html:61
 msgid "Forecast Manager"
 msgstr "Gerente de Pronóstico"
@@ -452,65 +515,14 @@
 msgid "Invalid request"
 msgstr "Solicitud no válida"
 
 #: forecastmanager/wagtail_hooks.py:30 forecastmanager/wagtail_hooks.py:84
 msgid "Settings"
 msgstr "Ajustes"
 
-#: forecastmanager/wagtail_hooks.py:46
-#: sandbox/home/templates/integration/dailyweather_include.html:3
-msgid "Daily Weather"
-msgstr "Clima diario"
-
 #: forecastmanager/wagtail_hooks.py:60
 msgid "City Forecast"
 msgstr "Pronóstico de la ciudad"
 
 #: forecastmanager/wagtail_hooks.py:73
 msgid "Add Forecasts"
 msgstr "Añadir previsiones"
-
-#: sandbox/home/templates/home/welcome_page.html:6
-msgid "Visit the Wagtail website"
-msgstr "Visite el sitio web de Lavandera"
-
-#: sandbox/home/templates/home/welcome_page.html:15
-msgid "View the release notes"
-msgstr "Ver las notas de la versión"
-
-#: sandbox/home/templates/home/welcome_page.html:27
-msgid "Welcome to your new Wagtail site!"
-msgstr "¡Bienvenido a su nuevo sitio de Wagtail!"
-
-#: sandbox/home/templates/home/welcome_page.html:28
-msgid ""
-"Please feel free to <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
-" Slack</a>, or get started with one of the links below."
-msgstr ""
-"Siéntete libre de <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">únete a nuestra "
-"comunidad en Slack</a>, o comienza con uno de los enlaces a continuación."
-
-#: sandbox/home/templates/home/welcome_page.html:35
-msgid "Wagtail Documentation"
-msgstr "Documentación de lavandera"
-
-#: sandbox/home/templates/home/welcome_page.html:36
-msgid "Topics, references, & how-tos"
-msgstr "Temas, referencias y procedimientos"
-
-#: sandbox/home/templates/home/welcome_page.html:42
-msgid "Tutorial"
-msgstr "Tutorial"
-
-#: sandbox/home/templates/home/welcome_page.html:43
-msgid "Build your first Wagtail site"
-msgstr "Crea tu primer sitio de Wagtail"
-
-#: sandbox/home/templates/home/welcome_page.html:49
-msgid "Admin Interface"
-msgstr "Interfaz de administración"
-
-#: sandbox/home/templates/home/welcome_page.html:50
-msgid "Create your superuser first!"
-msgstr "¡Crea tu superusuario primero!"
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/fr/LC_MESSAGES/django.mo` & `forecastmanager-0.1.1/forecastmanager/locale/fr/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -326,14 +326,17 @@
 
 msgid "Text"
 msgstr "Texte"
 
 msgid "The table is empty. Please input data"
 msgstr "Le tableau est vide. Veuillez entrer des données"
 
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr "Le fichier téléchargé doit être un CSV, similaire au tableau de droite"
+
 msgid "Time"
 msgstr "Temps"
 
 msgid "Topics, references, & how-tos"
 msgstr "Sujets, références et procédures"
 
 msgid "Tutorial"
@@ -376,7 +379,14 @@
 msgstr "Vitesse du vent"
 
 msgid "You can"
 msgstr "Tu peux"
 
 msgid "download a template"
 msgstr "télécharger un modèle"
+
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"du CSV pour une édition hors ligne et téléchargez-le ici. Le modèle est "
+"prérempli avec toutes les villes préexistantes."
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/fr/LC_MESSAGES/django.po` & `forecastmanager-0.1.1/forecastmanager/locale/fr/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,82 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-16 17:25+0000\n"
+"POT-Creation-Date: 2023-07-16 18:40+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
+#: sandbox/home/templates/home/welcome_page.html:6
+msgid "Visit the Wagtail website"
+msgstr "Visitez le site Web de Bergeronnette"
+
+#: sandbox/home/templates/home/welcome_page.html:15
+msgid "View the release notes"
+msgstr "Consulter les notes de version"
+
+#: sandbox/home/templates/home/welcome_page.html:27
+msgid "Welcome to your new Wagtail site!"
+msgstr "Bienvenue sur votre nouveau site Bergeronnette !"
+
+#: sandbox/home/templates/home/welcome_page.html:28
+msgid ""
+"Please feel free to <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
+" Slack</a>, or get started with one of the links below."
+msgstr ""
+"N'hésitez pas à <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">rejoindre notre "
+"communauté sur Slack</a>, ou commencez avec l'un des liens ci-dessous."
+
+#: sandbox/home/templates/home/welcome_page.html:35
+msgid "Wagtail Documentation"
+msgstr "Documentation de la bergeronnette"
+
+#: sandbox/home/templates/home/welcome_page.html:36
+msgid "Topics, references, & how-tos"
+msgstr "Sujets, références et procédures"
+
+#: sandbox/home/templates/home/welcome_page.html:42
+msgid "Tutorial"
+msgstr "Didacticiel"
+
+#: sandbox/home/templates/home/welcome_page.html:43
+msgid "Build your first Wagtail site"
+msgstr "Créez votre premier site Wagtail"
+
+#: sandbox/home/templates/home/welcome_page.html:49
+msgid "Admin Interface"
+msgstr "Interface d'administration"
+
+#: sandbox/home/templates/home/welcome_page.html:50
+msgid "Create your superuser first!"
+msgstr "Créez d'abord votre superutilisateur !"
+
+#: sandbox/home/templates/integration/dailyweather_include.html:3
+#: forecastmanager/wagtail_hooks.py:46
+msgid "Daily Weather"
+msgstr "Météo quotidienne"
+
+#: sandbox/home/templates/integration/forecasts_include.html:3
+#: forecastmanager/models.py:127
+msgid "Forecasts"
+msgstr "Prévisions"
+
 #: forecastmanager/models.py:16
-#: forecastmanager/templates/forecastmanager/create_forecast.html:57
+#: forecastmanager/templates/forecastmanager/create_forecast.html:54
 #: forecastmanager/templates/forecastmanager/view_forecast.html:29
 msgid "Forecast Date"
 msgstr "Date de prévision"
 
 #: forecastmanager/models.py:17
 msgid "Weather Forecast Description"
 msgstr "Description des prévisions météorologiques"
@@ -49,15 +105,15 @@
 msgstr "Nom de Ville"
 
 #: forecastmanager/models.py:54
 msgid "City Location (Lat, Lng)"
 msgstr "Emplacement de la ville (Lat, Lng)"
 
 #: forecastmanager/models.py:62 forecastmanager/models.py:117
-#: forecastmanager/templates/forecastmanager/create_forecast.html:138
+#: forecastmanager/templates/forecastmanager/create_forecast.html:134
 msgid "City"
 msgstr "Ville"
 
 #: forecastmanager/models.py:63 forecastmanager/wagtail_hooks.py:38
 msgid "Cities"
 msgstr "Villes"
 
@@ -225,19 +281,14 @@
 msgid "E.g Light Showers"
 msgstr "Par exemple, les averses légères"
 
 #: forecastmanager/models.py:126
 msgid "Forecast"
 msgstr "Prévision"
 
-#: forecastmanager/models.py:127
-#: sandbox/home/templates/integration/forecasts_include.html:3
-msgid "Forecasts"
-msgstr "Prévisions"
-
 #: forecastmanager/site_settings.py:20
 msgid "Enable automated forecasts"
 msgstr "Activer les prévisions automatisées"
 
 #: forecastmanager/site_settings.py:36
 msgid "Temperature"
 msgstr "Température"
@@ -374,43 +425,56 @@
 msgid "You can"
 msgstr "Tu peux"
 
 #: forecastmanager/templates/forecastmanager/create_forecast.html:46
 msgid "download a template"
 msgstr "télécharger un modèle"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:61
+#: forecastmanager/templates/forecastmanager/create_forecast.html:46
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"du CSV pour une édition hors ligne et téléchargez-le ici. Le modèle est "
+"prérempli avec toutes les villes préexistantes."
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:58
 msgid "Date of forecast"
 msgstr "Date de prévision"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:84
+#: forecastmanager/templates/forecastmanager/create_forecast.html:81
 msgid "Forecast effective period"
 msgstr "Période effective prévisionnelle"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:107
+#: forecastmanager/templates/forecastmanager/create_forecast.html:104
 msgid "Forecast Upload"
 msgstr "Téléchargement des prévisions"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:132
+#: forecastmanager/templates/forecastmanager/create_forecast.html:111
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr ""
+"Le fichier téléchargé doit être un CSV, similaire au tableau de droite"
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:128
 msgid "Verify that all columns match correctly"
 msgstr "Vérifiez que toutes les colonnes correspondent correctement"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:159
+#: forecastmanager/templates/forecastmanager/create_forecast.html:155
 msgid "Condition"
 msgstr "Condition"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:170
+#: forecastmanager/templates/forecastmanager/create_forecast.html:166
 msgid "Publish"
 msgstr "Publier"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:356
+#: forecastmanager/templates/forecastmanager/create_forecast.html:352
 msgid "The table is empty. Please input data"
 msgstr "Le tableau est vide. Veuillez entrer des données"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:362
+#: forecastmanager/templates/forecastmanager/create_forecast.html:358
 msgid "Table contains invalid inputs"
 msgstr "Le tableau contient des entrées non valides"
 
 #: forecastmanager/templates/forecastmanager/forecast_base.html:14
 #: forecastmanager/templates/forecastmanager/forecast_base.html:61
 msgid "Forecast Manager"
 msgstr "Gestionnaire des prévisions"
@@ -452,65 +516,14 @@
 msgid "Invalid request"
 msgstr "Requête invalide"
 
 #: forecastmanager/wagtail_hooks.py:30 forecastmanager/wagtail_hooks.py:84
 msgid "Settings"
 msgstr "Paramètres"
 
-#: forecastmanager/wagtail_hooks.py:46
-#: sandbox/home/templates/integration/dailyweather_include.html:3
-msgid "Daily Weather"
-msgstr "Météo quotidienne"
-
 #: forecastmanager/wagtail_hooks.py:60
 msgid "City Forecast"
 msgstr "Prévisions de la ville"
 
 #: forecastmanager/wagtail_hooks.py:73
 msgid "Add Forecasts"
 msgstr "Ajouter des prévisions"
-
-#: sandbox/home/templates/home/welcome_page.html:6
-msgid "Visit the Wagtail website"
-msgstr "Visitez le site Web de Bergeronnette"
-
-#: sandbox/home/templates/home/welcome_page.html:15
-msgid "View the release notes"
-msgstr "Consulter les notes de version"
-
-#: sandbox/home/templates/home/welcome_page.html:27
-msgid "Welcome to your new Wagtail site!"
-msgstr "Bienvenue sur votre nouveau site Bergeronnette !"
-
-#: sandbox/home/templates/home/welcome_page.html:28
-msgid ""
-"Please feel free to <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
-" Slack</a>, or get started with one of the links below."
-msgstr ""
-"N'hésitez pas à <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">rejoindre notre "
-"communauté sur Slack</a>, ou commencez avec l'un des liens ci-dessous."
-
-#: sandbox/home/templates/home/welcome_page.html:35
-msgid "Wagtail Documentation"
-msgstr "Documentation de la bergeronnette"
-
-#: sandbox/home/templates/home/welcome_page.html:36
-msgid "Topics, references, & how-tos"
-msgstr "Sujets, références et procédures"
-
-#: sandbox/home/templates/home/welcome_page.html:42
-msgid "Tutorial"
-msgstr "Didacticiel"
-
-#: sandbox/home/templates/home/welcome_page.html:43
-msgid "Build your first Wagtail site"
-msgstr "Créez votre premier site Wagtail"
-
-#: sandbox/home/templates/home/welcome_page.html:49
-msgid "Admin Interface"
-msgstr "Interface d'administration"
-
-#: sandbox/home/templates/home/welcome_page.html:50
-msgid "Create your superuser first!"
-msgstr "Créez d'abord votre superutilisateur !"
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/sw/LC_MESSAGES/django.mo` & `forecastmanager-0.1.1/forecastmanager/locale/sw/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -324,14 +324,18 @@
 
 msgid "Text"
 msgstr "Maandishi"
 
 msgid "The table is empty. Please input data"
 msgstr "Jedwali ni tupu. Tafadhali ingiza data"
 
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr ""
+"Faili iliyopakiwa inapaswa kuwa CSV, sawa na jedwali lililo upande wa kulia"
+
 msgid "Time"
 msgstr "Wakati"
 
 msgid "Topics, references, & how-tos"
 msgstr "Mada, marejeleo na jinsi ya kufanya"
 
 msgid "Tutorial"
@@ -374,7 +378,14 @@
 msgstr "Kasi ya Upepo"
 
 msgid "You can"
 msgstr "Unaweza"
 
 msgid "download a template"
 msgstr "pakua kiolezo"
+
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"ya CSV kwa uhariri wa nje ya mtandao na uipakie hapa. Kiolezo huja na miji "
+"yote iliyokuwepo awali."
```

### Comparing `forecastmanager-0.1.0/forecastmanager/locale/sw/LC_MESSAGES/django.po` & `forecastmanager-0.1.1/forecastmanager/locale/sw/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,82 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-16 17:25+0000\n"
+"POT-Creation-Date: 2023-07-16 18:40+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+#: sandbox/home/templates/home/welcome_page.html:6
+msgid "Visit the Wagtail website"
+msgstr "Tembelea tovuti ya Wagtail"
+
+#: sandbox/home/templates/home/welcome_page.html:15
+msgid "View the release notes"
+msgstr "Tazama maelezo ya kutolewa"
+
+#: sandbox/home/templates/home/welcome_page.html:27
+msgid "Welcome to your new Wagtail site!"
+msgstr "Karibu kwenye tovuti yako mpya ya Wagtail!"
+
+#: sandbox/home/templates/home/welcome_page.html:28
+msgid ""
+"Please feel free to <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
+" Slack</a>, or get started with one of the links below."
+msgstr ""
+"Tafadhali jisikie huru <a "
+"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">kujiunga na jumuiya "
+"yetu kwenye Slack</a>, au anza na mojawapo ya viungo vilivyo hapa chini."
+
+#: sandbox/home/templates/home/welcome_page.html:35
+msgid "Wagtail Documentation"
+msgstr "Nyaraka za Wagtail"
+
+#: sandbox/home/templates/home/welcome_page.html:36
+msgid "Topics, references, & how-tos"
+msgstr "Mada, marejeleo na jinsi ya kufanya"
+
+#: sandbox/home/templates/home/welcome_page.html:42
+msgid "Tutorial"
+msgstr "Mafunzo"
+
+#: sandbox/home/templates/home/welcome_page.html:43
+msgid "Build your first Wagtail site"
+msgstr "Jenga tovuti yako ya kwanza ya Wagtail"
+
+#: sandbox/home/templates/home/welcome_page.html:49
+msgid "Admin Interface"
+msgstr "Kiolesura cha Msimamizi"
+
+#: sandbox/home/templates/home/welcome_page.html:50
+msgid "Create your superuser first!"
+msgstr "Unda mtumiaji wako mkuu kwanza!"
+
+#: sandbox/home/templates/integration/dailyweather_include.html:3
+#: forecastmanager/wagtail_hooks.py:46
+msgid "Daily Weather"
+msgstr "Hali ya hewa ya kila siku"
+
+#: sandbox/home/templates/integration/forecasts_include.html:3
+#: forecastmanager/models.py:127
+msgid "Forecasts"
+msgstr "Utabiri"
+
 #: forecastmanager/models.py:16
-#: forecastmanager/templates/forecastmanager/create_forecast.html:57
+#: forecastmanager/templates/forecastmanager/create_forecast.html:54
 #: forecastmanager/templates/forecastmanager/view_forecast.html:29
 msgid "Forecast Date"
 msgstr "Tarehe ya Utabiri"
 
 #: forecastmanager/models.py:17
 msgid "Weather Forecast Description"
 msgstr "Maelezo ya Utabiri wa Hali ya Hewa"
@@ -49,15 +105,15 @@
 msgstr "Jina la Mji"
 
 #: forecastmanager/models.py:54
 msgid "City Location (Lat, Lng)"
 msgstr "Mahali pa Jiji (Lat, Lng)"
 
 #: forecastmanager/models.py:62 forecastmanager/models.py:117
-#: forecastmanager/templates/forecastmanager/create_forecast.html:138
+#: forecastmanager/templates/forecastmanager/create_forecast.html:134
 msgid "City"
 msgstr "Jiji"
 
 #: forecastmanager/models.py:63 forecastmanager/wagtail_hooks.py:38
 msgid "Cities"
 msgstr "Miji"
 
@@ -225,19 +281,14 @@
 msgid "E.g Light Showers"
 msgstr "K.m. Manyunyu ya Mwanga"
 
 #: forecastmanager/models.py:126
 msgid "Forecast"
 msgstr "Utabiri"
 
-#: forecastmanager/models.py:127
-#: sandbox/home/templates/integration/forecasts_include.html:3
-msgid "Forecasts"
-msgstr "Utabiri"
-
 #: forecastmanager/site_settings.py:20
 msgid "Enable automated forecasts"
 msgstr "Washa utabiri wa kiotomatiki"
 
 #: forecastmanager/site_settings.py:36
 msgid "Temperature"
 msgstr "Halijoto"
@@ -374,43 +425,56 @@
 msgid "You can"
 msgstr "Unaweza"
 
 #: forecastmanager/templates/forecastmanager/create_forecast.html:46
 msgid "download a template"
 msgstr "pakua kiolezo"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:61
+#: forecastmanager/templates/forecastmanager/create_forecast.html:46
+msgid ""
+"of the CSV for offline editing and upload it here. The template comes "
+"prepopulated with all pre-exisiting cities."
+msgstr ""
+"ya CSV kwa uhariri wa nje ya mtandao na uipakie hapa. Kiolezo huja na miji "
+"yote iliyokuwepo awali."
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:58
 msgid "Date of forecast"
 msgstr "Tarehe ya utabiri"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:84
+#: forecastmanager/templates/forecastmanager/create_forecast.html:81
 msgid "Forecast effective period"
 msgstr "Utabiri wa kipindi cha ufanisi"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:107
+#: forecastmanager/templates/forecastmanager/create_forecast.html:104
 msgid "Forecast Upload"
 msgstr "Upakiaji wa Utabiri"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:132
+#: forecastmanager/templates/forecastmanager/create_forecast.html:111
+msgid "The uploaded file should be a CSV, similar to the table on the right"
+msgstr ""
+"Faili iliyopakiwa inapaswa kuwa CSV, sawa na jedwali lililo upande wa kulia"
+
+#: forecastmanager/templates/forecastmanager/create_forecast.html:128
 msgid "Verify that all columns match correctly"
 msgstr "Thibitisha kuwa safu wima zote zinalingana ipasavyo"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:159
+#: forecastmanager/templates/forecastmanager/create_forecast.html:155
 msgid "Condition"
 msgstr "Hali"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:170
+#: forecastmanager/templates/forecastmanager/create_forecast.html:166
 msgid "Publish"
 msgstr "Kuchapisha"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:356
+#: forecastmanager/templates/forecastmanager/create_forecast.html:352
 msgid "The table is empty. Please input data"
 msgstr "Jedwali ni tupu. Tafadhali ingiza data"
 
-#: forecastmanager/templates/forecastmanager/create_forecast.html:362
+#: forecastmanager/templates/forecastmanager/create_forecast.html:358
 msgid "Table contains invalid inputs"
 msgstr "Jedwali lina ingizo batili"
 
 #: forecastmanager/templates/forecastmanager/forecast_base.html:14
 #: forecastmanager/templates/forecastmanager/forecast_base.html:61
 msgid "Forecast Manager"
 msgstr "Meneja Utabiri"
@@ -450,65 +514,14 @@
 msgid "Invalid request"
 msgstr "Ombi batili"
 
 #: forecastmanager/wagtail_hooks.py:30 forecastmanager/wagtail_hooks.py:84
 msgid "Settings"
 msgstr "Mipangilio"
 
-#: forecastmanager/wagtail_hooks.py:46
-#: sandbox/home/templates/integration/dailyweather_include.html:3
-msgid "Daily Weather"
-msgstr "Hali ya hewa ya kila siku"
-
 #: forecastmanager/wagtail_hooks.py:60
 msgid "City Forecast"
 msgstr "Utabiri wa Jiji"
 
 #: forecastmanager/wagtail_hooks.py:73
 msgid "Add Forecasts"
 msgstr "Ongeza Utabiri"
-
-#: sandbox/home/templates/home/welcome_page.html:6
-msgid "Visit the Wagtail website"
-msgstr "Tembelea tovuti ya Wagtail"
-
-#: sandbox/home/templates/home/welcome_page.html:15
-msgid "View the release notes"
-msgstr "Tazama maelezo ya kutolewa"
-
-#: sandbox/home/templates/home/welcome_page.html:27
-msgid "Welcome to your new Wagtail site!"
-msgstr "Karibu kwenye tovuti yako mpya ya Wagtail!"
-
-#: sandbox/home/templates/home/welcome_page.html:28
-msgid ""
-"Please feel free to <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">join our community on"
-" Slack</a>, or get started with one of the links below."
-msgstr ""
-"Tafadhali jisikie huru <a "
-"href=\"https://github.com/wagtail/wagtail/wiki/Slack\">kujiunga na jumuiya "
-"yetu kwenye Slack</a>, au anza na mojawapo ya viungo vilivyo hapa chini."
-
-#: sandbox/home/templates/home/welcome_page.html:35
-msgid "Wagtail Documentation"
-msgstr "Nyaraka za Wagtail"
-
-#: sandbox/home/templates/home/welcome_page.html:36
-msgid "Topics, references, & how-tos"
-msgstr "Mada, marejeleo na jinsi ya kufanya"
-
-#: sandbox/home/templates/home/welcome_page.html:42
-msgid "Tutorial"
-msgstr "Mafunzo"
-
-#: sandbox/home/templates/home/welcome_page.html:43
-msgid "Build your first Wagtail site"
-msgstr "Jenga tovuti yako ya kwanza ya Wagtail"
-
-#: sandbox/home/templates/home/welcome_page.html:49
-msgid "Admin Interface"
-msgstr "Kiolesura cha Msimamizi"
-
-#: sandbox/home/templates/home/welcome_page.html:50
-msgid "Create your superuser first!"
-msgstr "Unda mtumiaji wako mkuu kwanza!"
```

### Comparing `forecastmanager-0.1.0/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.1.1/forecastmanager/management/commands/generate_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/migrations/0001_initial.py` & `forecastmanager-0.1.1/forecastmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py` & `forecastmanager-0.1.1/forecastmanager/migrations/0002_remove_forecast_max_temp_remove_forecast_min_temp_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py` & `forecastmanager-0.1.1/forecastmanager/migrations/0004_forecastdataparameters_parameter_type_and_more.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py` & `forecastmanager-0.1.1/forecastmanager/migrations/0005_alter_forecastdataparameters_parameter.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/models.py` & `forecastmanager-0.1.1/forecastmanager/models.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/serializers.py` & `forecastmanager-0.1.1/forecastmanager/serializers.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/site_settings.py` & `forecastmanager-0.1.1/forecastmanager/site_settings.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/clearsky.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/clearsky.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/cloudy.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/cloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/fair.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/fair.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/fog.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/fog.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavyrain.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavyrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavyrainshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavyrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysleet.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysleetshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysnow.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysnowshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightrain.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightrainandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightrainshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsleet.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsleetshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsnow.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightsnowshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightsnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/partlycloudy.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/partlycloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/rain.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/rain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/rainandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/rainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/rainshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/rainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/sleet.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/sleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/sleetandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/sleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/sleetshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/sleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/snow.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/snow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/snowandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/snowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/snowshowers.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/snowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/js/forecast_basemap.js` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/js/forecast_basemap.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/static/forecastmanager/js/helpers.js` & `forecastmanager-0.1.1/forecastmanager/static/forecastmanager/js/helpers.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/templates/forecastmanager/create_forecast.html` & `forecastmanager-0.1.1/forecastmanager/templates/forecastmanager/create_forecast.html`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,15 @@
             <form enctype="multipart/form-data" id="forecast_form" method='post'>
                 {% csrf_token %}
                 <div class="help-block help-info">
                     <svg class="icon icon-warning icon" aria-hidden="true">
                         <use href="#icon-info-circle"></use>
                     </svg>
                     <div>
-                        {% trans 'You can' %} <a style="cursor:pointer"><b id="exportTable">{% trans 'download a template' %}</b></a> {% trans 'of the CSV for
-                        offline
-                        editing and upload it here. The template comes prepopulated
-                        with all pre-exisiting cities.' %}
+                        {% trans 'You can' %} <a style="cursor:pointer"><b id="exportTable">{% trans 'download a template' %}</b></a> {% trans 'of the CSV for offline editing and upload it here. The template comes prepopulated with all pre-exisiting cities.' %}
                     </div>
                 </div>
                 <ul class="fields forecast">
                     <div class="forecast-date-input">
                     <li>
                         <div class="w-field__wrapper" data-field-wrapper="">
                             <label class="w-field__label" for="id_forecast_date" id="id_forecast_date-label">
@@ -107,16 +104,15 @@
                                 {% trans 'Forecast Upload' %}
                             </label>
                             <div class="w-field w-field--file_field w-field--file_input" data-field=""
                                  data-contentpath="csv">
                                 <div class="w-field__errors" data-field-errors="">
                                 </div>
                                 <div class="w-field__help" data-field-help="">
-                                    <div class="help">{% trans 'The uploaded file should be a CSV, similar to the table on the
-                                        right' %}
+                                    <div class="help">{% trans 'The uploaded file should be a CSV, similar to the table on the right' %}
                                     </div>
                                 </div>
                                 <div class="w-field__input" data-field-input="">
                                     <input type="file" name="csv" accept=".csv" id="id_csv_data">
                                 </div>
                             </div>
                         </div>
```

### Comparing `forecastmanager-0.1.0/forecastmanager/templates/forecastmanager/forecast_base.html` & `forecastmanager-0.1.1/forecastmanager/templates/forecastmanager/forecast_base.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/templates/forecastmanager/view_forecast.html` & `forecastmanager-0.1.1/forecastmanager/templates/forecastmanager/view_forecast.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
             box-shadow: 0px 0px 7px 0px rgba(0, 0, 0, 0.1);
         }
     </style>
 {% endblock extra_css %}
 
 {% block header %}
     {% trans 'View Forecasts' as header_str %}
+    {% trans 'Add Forecasts' as add_forecast %}
     {% url 'add_forecast' as add_forecast_url %}
-    {% include "wagtailadmin/shared/header.html" with title=header_str icon="form" action_url=add_forecast_url action_text="Add Forecast" %}
+    {% include "wagtailadmin/shared/header.html" with title=header_str icon="form" action_url=add_forecast_url action_text=add_forecast %}
 {% endblock %}
 
 {% block forecast %}
     <h2 class="w-panel__heading" style="margin-bottom: 20px">{% trans 'Latest Available Forecast' %}</h2>
     <div class="row row-flush" style="display:flex; align-items:baseline">
         <div class="col6" style="display:flex; flex-wrap: wrap;">
             <div class="w-field__wrapper " data-field-wrapper="" style="padding-right:1em">
```

### Comparing `forecastmanager-0.1.0/forecastmanager/views.py` & `forecastmanager-0.1.1/forecastmanager/views.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.1.1/forecastmanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.1.1/forecastmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.1.0/forecastmanager.egg-info/SOURCES.txt` & `forecastmanager-0.1.1/forecastmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.1.0/setup.cfg` & `forecastmanager-0.1.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.1.0
+version = 0.1.1
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

