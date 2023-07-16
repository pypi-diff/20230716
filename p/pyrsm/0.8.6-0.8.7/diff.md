# Comparing `tmp/pyrsm-0.8.6.tar.gz` & `tmp/pyrsm-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.6.tar", last modified: Sun Jul 16 08:11:29 2023, max compression
+gzip compressed data, was "pyrsm-0.8.7.tar", last modified: Sun Jul 16 08:20:17 2023, max compression
```

## Comparing `pyrsm-0.8.6.tar` & `pyrsm-0.8.7.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.554643 pyrsm-0.8.6/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.6/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      476 2023-07-09 01:34:00.000000 pyrsm-0.8.6/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-16 08:11:29.554746 pyrsm-0.8.6/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.6/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.6/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.530126 pyrsm-0.8.6/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      311 2023-07-16 08:10:18.000000 pyrsm-0.8.6/pyrsm/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.532287 pyrsm-0.8.6/pyrsm/basics/
--rw-r--r--   0 root         (0) staff       (20)      264 2023-07-08 18:41:11.000000 pyrsm-0.8.6/pyrsm/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.8.6/pyrsm/basics/central_limit_theorem.py
--rw-r--r--   0 root         (0) staff       (20)     8826 2023-07-16 07:35:07.000000 pyrsm-0.8.6/pyrsm/basics/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.8.6/pyrsm/basics/compare_props.py
--rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.8.6/pyrsm/basics/correlation.py
--rw-r--r--   0 root         (0) staff       (20)     9615 2023-07-14 07:43:27.000000 pyrsm-0.8.6/pyrsm/basics/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     9503 2023-07-11 07:20:45.000000 pyrsm-0.8.6/pyrsm/basics/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     8394 2023-07-08 22:20:36.000000 pyrsm-0.8.6/pyrsm/basics/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.8.6/pyrsm/basics/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.8.6/pyrsm/basics/single_prop.py
--rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.8.6/pyrsm/basics/utils.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.6/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.532794 pyrsm-0.8.6/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.8.6/pyrsm/data/__radiant-data-convert.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.535689 pyrsm-0.8.6/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/consider.parquet
--rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/consider_description.md
--rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/demand_uk.parquet
--rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/demand_uk_description.md
--rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/newspaper.parquet
--rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/newspaper_description.md
--rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/salary.parquet
--rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/salary_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.538112 pyrsm-0.8.6/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/avengers.parquet
--rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/avengers_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/publishers.parquet
--rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/publishers_description.md
--rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/superheroes.parquet
--rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/superheroes_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.538772 pyrsm-0.8.6/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/design/rndnames.parquet
--rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/design/rndnames_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.543955 pyrsm-0.8.6/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/catalog.parquet
--rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/catalog_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.8.6/pyrsm/data/model/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.8.6/pyrsm/data/model/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/direct_marketing.parquet
--rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/direct_marketing_description.md
--rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/dvd.parquet
--rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/dvd_description.md
--rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/fraud_data_description.md
--rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/houseprices.parquet
--rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/houseprices_description.md
--rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ideal.parquet
--rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ideal_description.md
--rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ketchup.parquet
--rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ketchup_description.md
--rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ratings.parquet
--rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ratings_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.547884 pyrsm-0.8.6/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/carpet.parquet
--rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/carpet_description.md
--rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/city.parquet
--rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/city2.parquet
--rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/city2_description.md
--rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/city_description.md
--rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/computer.parquet
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/computer_description.md
--rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/movie.parquet
--rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/movie_description.md
--rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/mp3.parquet
--rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/mp3_description.md
--rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/retailers.parquet
--rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/retailers_description.md
--rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/shopping.parquet
--rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/shopping_description.md
--rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/toothpaste.parquet
--rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/toothpaste_description.md
--rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/tpbrands.parquet
--rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/tpbrands_description.md
--rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.8.6/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     9526 2023-07-10 08:03:17.000000 pyrsm-0.8.6/pyrsm/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    25699 2023-07-15 19:24:16.000000 pyrsm-0.8.6/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.6/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.6/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.550130 pyrsm-0.8.6/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)      153 2023-07-16 07:42:42.000000 pyrsm-0.8.6/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9387 2023-07-16 07:42:19.000000 pyrsm-0.8.6/pyrsm/radiant/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5829 2023-07-14 07:44:09.000000 pyrsm-0.8.6/pyrsm/radiant/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     6284 2023-07-12 20:32:35.000000 pyrsm-0.8.6/pyrsm/radiant/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     5158 2023-07-15 20:25:11.000000 pyrsm-0.8.6/pyrsm/radiant/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    11074 2023-07-15 21:26:00.000000 pyrsm-0.8.6/pyrsm/radiant/model_utils.py
--rw-r--r--   0 root         (0) staff       (20)     4841 2023-07-15 20:20:45.000000 pyrsm-0.8.6/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5376 2023-07-15 21:24:23.000000 pyrsm-0.8.6/pyrsm/radiant/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)    19570 2023-07-15 23:38:49.000000 pyrsm-0.8.6/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.551022 pyrsm-0.8.6/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.8.6/pyrsm/radiant/www/.DS_Store
--rw-r--r--   0 root         (0) staff       (20)      550 2023-07-10 19:04:28.000000 pyrsm-0.8.6/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     9338 2023-07-15 19:22:58.000000 pyrsm-0.8.6/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.6/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.8.6/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.8.6/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.530908 pyrsm-0.8.6/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3644 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      226 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-16 08:11:29.555138 pyrsm-0.8.6/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.554390 pyrsm-0.8.6/tests/
--rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.8.6/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.8.6/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.8.6/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.8.6/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.8.6/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.8.6/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.8.6/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.401275 pyrsm-0.8.7/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.7/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      476 2023-07-09 01:34:00.000000 pyrsm-0.8.7/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-16 08:20:17.401376 pyrsm-0.8.7/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.7/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.7/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.372392 pyrsm-0.8.7/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-07-16 08:19:56.000000 pyrsm-0.8.7/pyrsm/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.376279 pyrsm-0.8.7/pyrsm/basics/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-07-08 18:41:11.000000 pyrsm-0.8.7/pyrsm/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.8.7/pyrsm/basics/central_limit_theorem.py
+-rw-r--r--   0 root         (0) staff       (20)     8826 2023-07-16 07:35:07.000000 pyrsm-0.8.7/pyrsm/basics/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.8.7/pyrsm/basics/compare_props.py
+-rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.8.7/pyrsm/basics/correlation.py
+-rw-r--r--   0 root         (0) staff       (20)     9615 2023-07-14 07:43:27.000000 pyrsm-0.8.7/pyrsm/basics/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     9503 2023-07-11 07:20:45.000000 pyrsm-0.8.7/pyrsm/basics/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     8394 2023-07-08 22:20:36.000000 pyrsm-0.8.7/pyrsm/basics/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.8.7/pyrsm/basics/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.8.7/pyrsm/basics/single_prop.py
+-rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.8.7/pyrsm/basics/utils.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.7/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.376669 pyrsm-0.8.7/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.7/pyrsm/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.8.7/pyrsm/data/__radiant-data-convert.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.378842 pyrsm-0.8.7/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.7/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/basics/consider.parquet
+-rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/basics/consider_description.md
+-rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/basics/demand_uk.parquet
+-rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/basics/demand_uk_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/basics/newspaper.parquet
+-rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/basics/newspaper_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/basics/salary.parquet
+-rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/basics/salary_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.381133 pyrsm-0.8.7/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.7/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/avengers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/avengers_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/publishers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/publishers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/superheroes.parquet
+-rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/superheroes_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/data/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.381690 pyrsm-0.8.7/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.7/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/design/rndnames.parquet
+-rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/design/rndnames_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.387412 pyrsm-0.8.7/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.7/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/catalog.parquet
+-rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/catalog_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.8.7/pyrsm/data/model/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.8.7/pyrsm/data/model/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/direct_marketing.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/direct_marketing_description.md
+-rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/dvd.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/dvd_description.md
+-rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/fraud_data_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/houseprices.parquet
+-rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/houseprices_description.md
+-rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/ideal.parquet
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/ideal_description.md
+-rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/ketchup.parquet
+-rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/ketchup_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/ratings.parquet
+-rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/model/ratings_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.391816 pyrsm-0.8.7/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.7/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/carpet.parquet
+-rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/carpet_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/city.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/city2.parquet
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/city2_description.md
+-rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/city_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/computer.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/computer_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/movie.parquet
+-rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/movie_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/mp3.parquet
+-rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/mp3_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/retailers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/retailers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/shopping.parquet
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/shopping_description.md
+-rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/toothpaste.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/toothpaste_description.md
+-rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/tpbrands.parquet
+-rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.8.7/pyrsm/data/multivariate/tpbrands_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.8.7/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     9526 2023-07-10 08:03:17.000000 pyrsm-0.8.7/pyrsm/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    25699 2023-07-15 19:24:16.000000 pyrsm-0.8.7/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.7/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.7/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.7/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.397812 pyrsm-0.8.7/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)      153 2023-07-16 07:42:42.000000 pyrsm-0.8.7/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9387 2023-07-16 07:42:19.000000 pyrsm-0.8.7/pyrsm/radiant/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5829 2023-07-14 07:44:09.000000 pyrsm-0.8.7/pyrsm/radiant/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     6284 2023-07-12 20:32:35.000000 pyrsm-0.8.7/pyrsm/radiant/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     5158 2023-07-15 20:25:11.000000 pyrsm-0.8.7/pyrsm/radiant/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    11074 2023-07-15 21:26:00.000000 pyrsm-0.8.7/pyrsm/radiant/model_utils.py
+-rw-r--r--   0 root         (0) staff       (20)     4841 2023-07-15 20:20:45.000000 pyrsm-0.8.7/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5376 2023-07-15 21:24:23.000000 pyrsm-0.8.7/pyrsm/radiant/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)    19570 2023-07-15 23:38:49.000000 pyrsm-0.8.7/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.398742 pyrsm-0.8.7/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.8.7/pyrsm/radiant/www/.DS_Store
+-rw-r--r--   0 root         (0) staff       (20)      550 2023-07-10 19:04:28.000000 pyrsm-0.8.7/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9338 2023-07-15 19:22:58.000000 pyrsm-0.8.7/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.7/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.8.7/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.8.7/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.373520 pyrsm-0.8.7/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-16 08:20:17.000000 pyrsm-0.8.7/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3644 2023-07-16 08:20:17.000000 pyrsm-0.8.7/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-16 08:20:17.000000 pyrsm-0.8.7/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      242 2023-07-16 08:20:17.000000 pyrsm-0.8.7/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-16 08:20:17.000000 pyrsm-0.8.7/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1055 2023-07-16 08:20:17.401765 pyrsm-0.8.7/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:20:17.400967 pyrsm-0.8.7/tests/
+-rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.8.7/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.8.7/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.8.7/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.8.7/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.8.7/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.8.7/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.8.7/tests/test_utils.py
```

### Comparing `pyrsm-0.8.6/LICENSE` & `pyrsm-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/PKG-INFO` & `pyrsm-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.6
+Version: 0.8.7
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.6/README.md` & `pyrsm-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/central_limit_theorem.py` & `pyrsm-0.8.7/pyrsm/basics/central_limit_theorem.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/compare_means.py` & `pyrsm-0.8.7/pyrsm/basics/compare_means.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/compare_props.py` & `pyrsm-0.8.7/pyrsm/basics/compare_props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/correlation.py` & `pyrsm-0.8.7/pyrsm/basics/correlation.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/cross_tabs.py` & `pyrsm-0.8.7/pyrsm/basics/cross_tabs.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/goodness.py` & `pyrsm-0.8.7/pyrsm/basics/goodness.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/probability_calculator.py` & `pyrsm-0.8.7/pyrsm/basics/probability_calculator.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/single_mean.py` & `pyrsm-0.8.7/pyrsm/basics/single_mean.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/basics/single_prop.py` & `pyrsm-0.8.7/pyrsm/basics/single_prop.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/bins.py` & `pyrsm-0.8.7/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/__radiant-data-convert.py` & `pyrsm-0.8.7/pyrsm/data/__radiant-data-convert.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/basics/consider.parquet` & `pyrsm-0.8.7/pyrsm/data/basics/consider.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/basics/consider_description.md` & `pyrsm-0.8.7/pyrsm/data/basics/consider_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/basics/demand_uk.parquet` & `pyrsm-0.8.7/pyrsm/data/basics/demand_uk.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/basics/newspaper.parquet` & `pyrsm-0.8.7/pyrsm/data/basics/newspaper.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/basics/newspaper_description.md` & `pyrsm-0.8.7/pyrsm/data/basics/newspaper_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/basics/salary.parquet` & `pyrsm-0.8.7/pyrsm/data/basics/salary.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/basics/salary_description.md` & `pyrsm-0.8.7/pyrsm/data/basics/salary_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/data/avengers.parquet` & `pyrsm-0.8.7/pyrsm/data/data/avengers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/data/diamonds.parquet` & `pyrsm-0.8.7/pyrsm/data/data/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/data/diamonds_description.md` & `pyrsm-0.8.7/pyrsm/data/data/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/data/publishers.parquet` & `pyrsm-0.8.7/pyrsm/data/data/publishers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/data/superheroes.parquet` & `pyrsm-0.8.7/pyrsm/data/data/superheroes.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/data/titanic.parquet` & `pyrsm-0.8.7/pyrsm/data/data/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/data/titanic_description.md` & `pyrsm-0.8.7/pyrsm/data/data/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/design/rndnames.parquet` & `pyrsm-0.8.7/pyrsm/data/design/rndnames.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/catalog.parquet` & `pyrsm-0.8.7/pyrsm/data/model/catalog.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/catalog_description.md` & `pyrsm-0.8.7/pyrsm/data/model/catalog_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/diamonds.parquet` & `pyrsm-0.8.7/pyrsm/data/model/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/diamonds_description.md` & `pyrsm-0.8.7/pyrsm/data/model/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/direct_marketing.parquet` & `pyrsm-0.8.7/pyrsm/data/model/direct_marketing.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/direct_marketing_description.md` & `pyrsm-0.8.7/pyrsm/data/model/direct_marketing_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/dvd.parquet` & `pyrsm-0.8.7/pyrsm/data/model/dvd.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/dvd_description.md` & `pyrsm-0.8.7/pyrsm/data/model/dvd_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/fraud_data_description.md` & `pyrsm-0.8.7/pyrsm/data/model/fraud_data_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/houseprices.parquet` & `pyrsm-0.8.7/pyrsm/data/model/houseprices.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/houseprices_description.md` & `pyrsm-0.8.7/pyrsm/data/model/houseprices_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/ideal.parquet` & `pyrsm-0.8.7/pyrsm/data/model/ideal.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/ketchup.parquet` & `pyrsm-0.8.7/pyrsm/data/model/ketchup.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/ketchup_description.md` & `pyrsm-0.8.7/pyrsm/data/model/ketchup_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/model/ratings.parquet` & `pyrsm-0.8.7/pyrsm/data/model/ratings.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/carpet.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/carpet.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/carpet_description.md` & `pyrsm-0.8.7/pyrsm/data/multivariate/carpet_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/city.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/city.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/city2.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/city2.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/computer.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/computer.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/computer_description.md` & `pyrsm-0.8.7/pyrsm/data/multivariate/computer_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/movie.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/movie.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/movie_description.md` & `pyrsm-0.8.7/pyrsm/data/multivariate/movie_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/mp3.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/mp3.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/mp3_description.md` & `pyrsm-0.8.7/pyrsm/data/multivariate/mp3_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/retailers.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/retailers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/retailers_description.md` & `pyrsm-0.8.7/pyrsm/data/multivariate/retailers_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/shopping.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/shopping.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/shopping_description.md` & `pyrsm-0.8.7/pyrsm/data/multivariate/shopping_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/toothpaste.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/toothpaste.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/toothpaste_description.md` & `pyrsm-0.8.7/pyrsm/data/multivariate/toothpaste_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/tpbrands.parquet` & `pyrsm-0.8.7/pyrsm/data/multivariate/tpbrands.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/data/multivariate/tpbrands_description.md` & `pyrsm-0.8.7/pyrsm/data/multivariate/tpbrands_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/example_data.py` & `pyrsm-0.8.7/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/logistic.py` & `pyrsm-0.8.7/pyrsm/logistic.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/model.py` & `pyrsm-0.8.7/pyrsm/model.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/notebook.py` & `pyrsm-0.8.7/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/perf.py` & `pyrsm-0.8.7/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/props.py` & `pyrsm-0.8.7/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/compare_means.py` & `pyrsm-0.8.7/pyrsm/radiant/compare_means.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/cross_tabs.py` & `pyrsm-0.8.7/pyrsm/radiant/cross_tabs.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/goodness.py` & `pyrsm-0.8.7/pyrsm/radiant/goodness.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/logistic.py` & `pyrsm-0.8.7/pyrsm/radiant/logistic.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/model_utils.py` & `pyrsm-0.8.7/pyrsm/radiant/model_utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/regress.py` & `pyrsm-0.8.7/pyrsm/radiant/regress.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/single_mean.py` & `pyrsm-0.8.7/pyrsm/radiant/single_mean.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/utils.py` & `pyrsm-0.8.7/pyrsm/radiant/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/www/.DS_Store` & `pyrsm-0.8.7/pyrsm/radiant/www/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/radiant/www/style.css` & `pyrsm-0.8.7/pyrsm/radiant/www/style.css`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/regress.py` & `pyrsm-0.8.7/pyrsm/regress.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/stats.py` & `pyrsm-0.8.7/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/utils.py` & `pyrsm-0.8.7/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm/visualize.py` & `pyrsm-0.8.7/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.7/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.6
+Version: 0.8.7
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.6/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.8.7/pyrsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/setup.cfg` & `pyrsm-0.8.7/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	matplotlib>=3.1.1
 	statsmodels>=0.10.1
 	scipy>=1.4.1
 	scikit-learn>=1.0.2
 	IPython>=8.0.1
 	nest-asyncio>=1.5.6
 	black>=22.6.0
+	pyarrow>=12.0.1
 
 [options.packages.find]
 exclude = 
 	*.tests
 	*.tests.*
 	tests.*
 	tests
```

### Comparing `pyrsm-0.8.6/tests/test_basics.py` & `pyrsm-0.8.7/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/tests/test_bins.py` & `pyrsm-0.8.7/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/tests/test_example_data.py` & `pyrsm-0.8.7/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/tests/test_perf.py` & `pyrsm-0.8.7/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/tests/test_regression.py` & `pyrsm-0.8.7/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/tests/test_stats.py` & `pyrsm-0.8.7/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.6/tests/test_utils.py` & `pyrsm-0.8.7/tests/test_utils.py`

 * *Files identical despite different names*

