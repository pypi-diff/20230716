# Comparing `tmp/pyrsm-0.8.5.tar.gz` & `tmp/pyrsm-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.5.tar", last modified: Mon Jul 10 07:40:09 2023, max compression
+gzip compressed data, was "pyrsm-0.8.6.tar", last modified: Sun Jul 16 08:11:29 2023, max compression
```

## Comparing `pyrsm-0.8.5.tar` & `pyrsm-0.8.6.tar`

### file list

```diff
@@ -1,153 +1,129 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.300743 pyrsm-0.8.5/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.5/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      476 2023-07-09 01:34:00.000000 pyrsm-0.8.5/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-10 07:40:09.300825 pyrsm-0.8.5/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.5/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.5/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.280155 pyrsm-0.8.5/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      311 2023-07-09 05:08:38.000000 pyrsm-0.8.5/pyrsm/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.282462 pyrsm-0.8.5/pyrsm/basics/
--rw-r--r--   0 root         (0) staff       (20)      264 2023-07-08 18:41:11.000000 pyrsm-0.8.5/pyrsm/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.8.5/pyrsm/basics/central_limit_theorem.py
--rw-r--r--   0 root         (0) staff       (20)     5674 2023-07-08 23:31:10.000000 pyrsm-0.8.5/pyrsm/basics/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5446 2023-07-08 22:24:23.000000 pyrsm-0.8.5/pyrsm/basics/compare_props.py
--rw-r--r--   0 root         (0) staff       (20)     7460 2023-07-08 22:19:48.000000 pyrsm-0.8.5/pyrsm/basics/correlation.py
--rw-r--r--   0 root         (0) staff       (20)     9696 2023-07-08 23:21:46.000000 pyrsm-0.8.5/pyrsm/basics/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     9944 2023-07-08 22:40:14.000000 pyrsm-0.8.5/pyrsm/basics/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     8394 2023-07-08 22:20:36.000000 pyrsm-0.8.5/pyrsm/basics/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)     3854 2023-07-08 23:08:05.000000 pyrsm-0.8.5/pyrsm/basics/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)     3141 2023-07-08 23:50:35.000000 pyrsm-0.8.5/pyrsm/basics/single_prop.py
--rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.8.5/pyrsm/basics/utils.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.5/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.282734 pyrsm-0.8.5/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.8.5/pyrsm/data/__radiant-data-convert.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.284725 pyrsm-0.8.5/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/consider.parquet
--rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/consider.pkl
--rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/consider_description.md
--rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/demand_uk.parquet
--rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/demand_uk.pkl
--rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/demand_uk_description.md
--rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/newspaper.parquet
--rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/newspaper.pkl
--rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/newspaper_description.md
--rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/salary.parquet
--rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/basics/salary.pkl
--rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/basics/salary_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.287487 pyrsm-0.8.5/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/avengers.parquet
--rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/avengers.pkl
--rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/avengers_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/diamonds.pkl
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/publishers.parquet
--rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/publishers.pkl
--rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/publishers_description.md
--rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/superheroes.parquet
--rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/superheroes.pkl
--rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/superheroes_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/data/titanic.pkl
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/data/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.288179 pyrsm-0.8.5/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/design/rndnames.parquet
--rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/design/rndnames.pkl
--rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/design/rndnames_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.292164 pyrsm-0.8.5/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/catalog.parquet
--rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/catalog.pkl
--rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/catalog_description.md
--rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/direct_marketing.parquet
--rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/direct_marketing.pkl
--rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/direct_marketing_description.md
--rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/dvd.parquet
--rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/dvd.pkl
--rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/dvd_description.md
--rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/fraud_data_description.md
--rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/houseprices.parquet
--rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/houseprices.pkl
--rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/houseprices_description.md
--rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ideal.parquet
--rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/ideal.pkl
--rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ideal_description.md
--rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ketchup.parquet
--rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/ketchup.pkl
--rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ketchup_description.md
--rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ratings.parquet
--rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/model/ratings.pkl
--rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/model/ratings_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.297766 pyrsm-0.8.5/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/carpet.parquet
--rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/carpet.pkl
--rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/carpet_description.md
--rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city.parquet
--rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city.pkl
--rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city2.parquet
--rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city2.pkl
--rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city2_description.md
--rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/city_description.md
--rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/computer.parquet
--rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/computer.pkl
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/computer_description.md
--rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/movie.parquet
--rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/movie.pkl
--rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/movie_description.md
--rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/mp3.parquet
--rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/mp3.pkl
--rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/mp3_description.md
--rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/retailers.parquet
--rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/retailers.pkl
--rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/retailers_description.md
--rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/shopping.parquet
--rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/shopping.pkl
--rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/shopping_description.md
--rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste.parquet
--rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste.pkl
--rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste_description.md
--rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands.parquet
--rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands.pkl
--rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands_description.md
--rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.8.5/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     9526 2023-07-10 04:08:57.000000 pyrsm-0.8.5/pyrsm/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    25570 2023-07-04 04:09:06.000000 pyrsm-0.8.5/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.5/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.5/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.5/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.298728 pyrsm-0.8.5/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)      100 2023-07-09 05:08:44.000000 pyrsm-0.8.5/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6036 2023-07-10 07:37:12.000000 pyrsm-0.8.5/pyrsm/radiant/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     4945 2023-07-10 07:15:59.000000 pyrsm-0.8.5/pyrsm/radiant/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    10678 2023-07-10 07:32:46.000000 pyrsm-0.8.5/pyrsm/radiant/model_utils.py
--rw-r--r--   0 root         (0) staff       (20)     4756 2023-07-10 07:08:33.000000 pyrsm-0.8.5/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     6006 2023-07-10 07:36:25.000000 pyrsm-0.8.5/pyrsm/radiant/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)    14896 2023-07-10 07:11:35.000000 pyrsm-0.8.5/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.299159 pyrsm-0.8.5/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)      290 2023-07-07 20:52:09.000000 pyrsm-0.8.5/pyrsm/radiant/www/copy.js
--rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.5/pyrsm/radiant/www/returnTextAreaBinding.js
--rw-r--r--   0 root         (0) staff       (20)      534 2023-07-07 22:43:29.000000 pyrsm-0.8.5/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     9390 2023-07-10 01:21:40.000000 pyrsm-0.8.5/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.5/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.8.5/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22924 2023-06-13 07:22:05.000000 pyrsm-0.8.5/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.280815 pyrsm-0.8.5/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     4423 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      226 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-07-10 07:40:09.000000 pyrsm-0.8.5/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-10 07:40:09.301169 pyrsm-0.8.5/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 07:40:09.300614 pyrsm-0.8.5/tests/
--rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.8.5/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.8.5/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.8.5/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.8.5/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.8.5/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.8.5/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.8.5/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.554643 pyrsm-0.8.6/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.6/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      476 2023-07-09 01:34:00.000000 pyrsm-0.8.6/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-16 08:11:29.554746 pyrsm-0.8.6/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.6/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.6/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.530126 pyrsm-0.8.6/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-07-16 08:10:18.000000 pyrsm-0.8.6/pyrsm/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.532287 pyrsm-0.8.6/pyrsm/basics/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-07-08 18:41:11.000000 pyrsm-0.8.6/pyrsm/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.8.6/pyrsm/basics/central_limit_theorem.py
+-rw-r--r--   0 root         (0) staff       (20)     8826 2023-07-16 07:35:07.000000 pyrsm-0.8.6/pyrsm/basics/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.8.6/pyrsm/basics/compare_props.py
+-rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.8.6/pyrsm/basics/correlation.py
+-rw-r--r--   0 root         (0) staff       (20)     9615 2023-07-14 07:43:27.000000 pyrsm-0.8.6/pyrsm/basics/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     9503 2023-07-11 07:20:45.000000 pyrsm-0.8.6/pyrsm/basics/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     8394 2023-07-08 22:20:36.000000 pyrsm-0.8.6/pyrsm/basics/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.8.6/pyrsm/basics/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.8.6/pyrsm/basics/single_prop.py
+-rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.8.6/pyrsm/basics/utils.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.6/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.532794 pyrsm-0.8.6/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.8.6/pyrsm/data/__radiant-data-convert.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.535689 pyrsm-0.8.6/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/consider.parquet
+-rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/consider_description.md
+-rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/demand_uk.parquet
+-rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/demand_uk_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/newspaper.parquet
+-rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/newspaper_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/salary.parquet
+-rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/basics/salary_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.538112 pyrsm-0.8.6/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/avengers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/avengers_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/publishers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/publishers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/superheroes.parquet
+-rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/superheroes_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/data/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.538772 pyrsm-0.8.6/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/design/rndnames.parquet
+-rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/design/rndnames_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.543955 pyrsm-0.8.6/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/catalog.parquet
+-rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/catalog_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.8.6/pyrsm/data/model/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.8.6/pyrsm/data/model/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/direct_marketing.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/direct_marketing_description.md
+-rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/dvd.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/dvd_description.md
+-rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/fraud_data_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/houseprices.parquet
+-rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/houseprices_description.md
+-rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ideal.parquet
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ideal_description.md
+-rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ketchup.parquet
+-rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ketchup_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ratings.parquet
+-rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/model/ratings_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.547884 pyrsm-0.8.6/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/carpet.parquet
+-rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/carpet_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/city.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/city2.parquet
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/city2_description.md
+-rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/city_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/computer.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/computer_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/movie.parquet
+-rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/movie_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/mp3.parquet
+-rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/mp3_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/retailers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/retailers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/shopping.parquet
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/shopping_description.md
+-rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/toothpaste.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/toothpaste_description.md
+-rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/tpbrands.parquet
+-rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.8.6/pyrsm/data/multivariate/tpbrands_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.8.6/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     9526 2023-07-10 08:03:17.000000 pyrsm-0.8.6/pyrsm/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    25699 2023-07-15 19:24:16.000000 pyrsm-0.8.6/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.6/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.6/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.6/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.550130 pyrsm-0.8.6/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)      153 2023-07-16 07:42:42.000000 pyrsm-0.8.6/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9387 2023-07-16 07:42:19.000000 pyrsm-0.8.6/pyrsm/radiant/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5829 2023-07-14 07:44:09.000000 pyrsm-0.8.6/pyrsm/radiant/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     6284 2023-07-12 20:32:35.000000 pyrsm-0.8.6/pyrsm/radiant/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     5158 2023-07-15 20:25:11.000000 pyrsm-0.8.6/pyrsm/radiant/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    11074 2023-07-15 21:26:00.000000 pyrsm-0.8.6/pyrsm/radiant/model_utils.py
+-rw-r--r--   0 root         (0) staff       (20)     4841 2023-07-15 20:20:45.000000 pyrsm-0.8.6/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5376 2023-07-15 21:24:23.000000 pyrsm-0.8.6/pyrsm/radiant/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)    19570 2023-07-15 23:38:49.000000 pyrsm-0.8.6/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.551022 pyrsm-0.8.6/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.8.6/pyrsm/radiant/www/.DS_Store
+-rw-r--r--   0 root         (0) staff       (20)      550 2023-07-10 19:04:28.000000 pyrsm-0.8.6/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9338 2023-07-15 19:22:58.000000 pyrsm-0.8.6/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.6/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.8.6/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.8.6/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.530908 pyrsm-0.8.6/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3644 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      226 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-16 08:11:29.000000 pyrsm-0.8.6/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-16 08:11:29.555138 pyrsm-0.8.6/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:11:29.554390 pyrsm-0.8.6/tests/
+-rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.8.6/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.8.6/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.8.6/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.8.6/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.8.6/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.8.6/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.8.6/tests/test_utils.py
```

### Comparing `pyrsm-0.8.5/LICENSE` & `pyrsm-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/PKG-INFO` & `pyrsm-0.8.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.5/README.md` & `pyrsm-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/basics/central_limit_theorem.py` & `pyrsm-0.8.6/pyrsm/basics/central_limit_theorem.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/basics/compare_means.py` & `pyrsm-0.8.6/pyrsm/basics/single_mean.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,116 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy import stats
 from ..model import sig_stars
 from ..utils import ifelse
-from statsmodels.stats import multitest
 import pyrsm.basics.utils as bu
+from typing import Union
 
 
-class compare_means:
+class single_mean:
     def __init__(
         self,
-        data: pd.DataFrame,
-        var1: str,
-        var2: str,
-        combinations: list[tuple[str, str]] = None,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
+        var: str,
         alt_hyp: str = "two-sided",
         conf: float = 0.95,
-        sample_type: str = "independent",
-        adjust: str = None,
-    ) -> None:
+        comp_value: float = 0,
+    ):
         if isinstance(data, dict):
             self.name = list(data.keys())[0]
-            self.data = data[self.name]
+            self.data = data[self.name].copy()
         else:
-            self.data = data
+            self.data = data.copy()
             self.name = "Not provided"
-        self.var1 = var1
-        self.var2 = var2
-        self.combinations = combinations
+        self.var = var
         self.alt_hyp = alt_hyp
         self.conf = conf
-        self.sample_type = sample_type
-        self.adjust = adjust
-        self.test_type = "t-test"
-
-        def welch_dof(v1: str, v2: str) -> float:
-            # stats.ttest_ind uses Welch's t-test when equal_var=False
-            # but does not return the degrees of freedom
-            x = self.data[self.data[self.var1] == v1][self.var2]
-            y = self.data[self.data[self.var1] == v2][self.var2]
-            dof = (x.var() / x.size + y.var() / y.size) ** 2 / (
-                (x.var() / x.size) ** 2 / (x.size - 1)
-                + (y.var() / y.size) ** 2 / (y.size - 1)
-            )
-
-            return dof
-
-        combinations_elements = set()
-        for combination in self.combinations:
-            combinations_elements.add(combination[0])
-            combinations_elements.add(combination[1])
-        combinations_elements = list(combinations_elements)
-
-        rows1 = []
-        mean = 0
-        for element in combinations_elements:
-            subset = self.data[self.data[self.var1] == element][self.var2]
-            row = []
-            mean = np.nanmean(subset)
-            n_missing = subset.isna().sum()
-            n = len(subset) - n_missing
-            sd = subset.std()
-            se = subset.sem()
-            tscore = stats.t.ppf((1 + self.conf) / 2, n - 1)
-            me = (tscore * se).real
-            row = [element, mean, n, n_missing, sd, se, me]
-            rows1.append(row)
+        self.comp_value = comp_value
 
-        self.table1 = pd.DataFrame(
-            rows1, columns=[self.var1, "mean", "n", "n_missing", "sd", "se", "me"]
+        result = stats.ttest_1samp(
+            a=self.data[self.var],
+            popmean=self.comp_value,
+            nan_policy="omit",
+            alternative=self.alt_hyp,
         )
 
-        if self.alt_hyp == "less":
-            alt_hyp_sign = " < "
-        elif self.alt_hyp == "two-sided":
-            alt_hyp_sign = " != "
-        else:
-            alt_hyp_sign = " > "
-
-        rows2 = []
-        for v1, v2 in self.combinations:
-            null_hyp = v1 + " = " + v2
-            alt_hyp = v1 + alt_hyp_sign + v2
-            diff = np.nanmean(
-                self.data[self.data[self.var1] == v1][self.var2]
-            ) - np.nanmean(self.data[self.data[self.var1] == v2][self.var2])
-
-            if self.sample_type == "independent":
-                result = stats.ttest_ind(
-                    self.data[self.data[self.var1] == v1][self.var2],
-                    self.data[self.data[self.var1] == v2][self.var2],
-                    equal_var=False,
-                    nan_policy="omit",
-                    alternative=self.alt_hyp,
-                )
-            else:
-                result = stats.ttest_rel(
-                    self.data[self.data[self.var1] == v1][self.var2],
-                    self.data[self.data[self.var1] == v2][self.var2],
-                    nan_policy="omit",
-                    alternative=self.alt_hyp,
-                )
-
-            t_val, p_val = result.statistic, result.pvalue
-            se = diff / t_val
-            df = welch_dof(v1, v2)
-
-            if self.alt_hyp == "two-sided":
-                tscore = stats.t.ppf((1 + self.conf) / 2, df)
-            else:
-                tscore = stats.t.ppf(self.conf, df)
-            me = (tscore * se).real
-
-            if self.alt_hyp == "less":
-                ci = [-np.inf, diff + me]
-            elif self.alt_hyp == "two-sided":
-                ci = [diff - me, diff + me]
-            else:
-                ci = [diff - me, np.inf]
-
-            rows2.append(
-                [
-                    null_hyp,
-                    alt_hyp,
-                    diff,
-                    ifelse(p_val < 0.001, "< .001", p_val),
-                    se,
-                    t_val,
-                    df,
-                    ci[0],
-                    ci[1],
-                    sig_stars([p_val])[0],
-                ]
-            )
+        self.t_val, self.p_val = result.statistic, result.pvalue
+        self.ci = result.confidence_interval(confidence_level=conf)
 
-        cl = bu.ci_label(self.alt_hyp, self.conf)
-        self.table2 = pd.DataFrame(
-            rows2,
-            columns=[
-                "Null hyp.",
-                "Alt. hyp.",
-                "diff",
-                "p.value",
-                "se",
-                "t.value",
-                "df",
-                cl[0],
-                cl[1],
-                "",
-            ],
-        )
-
-        if self.adjust is not None:
-            self.table2["p.value"] = multitest.multipletests(
-                self.table2["p.value"], method=self.adjust
-            )[1]
+        self.mean = np.nanmean(self.data[self.var])
+        self.n = len(self.data[self.var])
+        self.n_missing = self.data[self.var].isna().sum()
+
+        self.sd = self.data[self.var].std()
+        self.se = self.data[self.var].sem()
+        tscore = stats.t.ppf((1 + self.conf) / 2, self.n - 1)
+
+        self.me = (tscore * self.se).real
+        self.diff = self.mean - self.comp_value
+        self.df = self.n - 1
 
     def summary(self, dec=3) -> None:
-        print(f"Pairwise mean comparisons ({self.test_type})")
+        print("Single mean test")
         print(f"Data      : {self.name}")
-        print(f"Variables : {self.var1}, {self.var2}")
-        print(f"Samples   : {self.sample_type}")
+        print(f"Variables : {self.var}")
         print(f"Confidence: {self.conf}")
-        print(f"Adjustment: {self.adjust}")
+        print(f"Comparison: {self.comp_value}\n")
+        print(f"Null hyp. : the mean of {self.var} is equal to {self.comp_value}")
+
+        if self.alt_hyp == "less":
+            alt_hyp = "less than"
+        elif self.alt_hyp == "two-sided":
+            alt_hyp = "not equal to"
+        else:
+            alt_hyp = "greater than"
+
+        cl = bu.ci_label(self.alt_hyp, self.conf, dec=dec)
 
-        print(self.table1.round(dec).to_string(index=False))
-        print(self.table2.round(dec).to_string(index=False))
+        print(f"Alt. hyp. : the mean of {self.var} is {alt_hyp} {self.comp_value}\n")
 
-    def plot(self) -> None:
-        pass
+        row1 = [[self.mean, self.n, self.n_missing, self.sd, self.se, self.me]]
+        row2 = [
+            [
+                self.diff,
+                self.se,
+                self.t_val,
+                ifelse(self.p_val < 0.001, "< .001", self.p_val),
+                self.df,
+                self.ci[0],
+                self.ci[1],
+                sig_stars([self.p_val])[0],
+            ]
+        ]
+
+        col_names1 = ["mean", "n", "n_missing", "sd", "se", "me"]
+        col_names2 = ["diff", "se", "t.value", "p.value", "df", cl[0], cl[1], ""]
+
+        table1 = pd.DataFrame(row1, columns=col_names1).round(dec)
+        table2 = pd.DataFrame(row2, columns=col_names2).round(dec)
+
+        print(table1.to_string(index=False))
+        print(table2.to_string(index=False))
+        print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
+
+    def plot(self, plots: str = "hist") -> None:
+
+        if plots == "hist":
+            fig = self.data[self.var].plot.hist(title=self.var, color="slateblue")
+            plt.vlines(
+                x=(self.comp_value, self.ci[0], self.mean, self.ci[1]),
+                ymin=fig.get_ylim()[0],
+                ymax=fig.get_ylim()[1],
+                colors=("r", "k", "k", "k"),
+                linestyles=("solid", "dashed", "solid", "dashed"),
+            )
+        elif plots == "sim":
+            print("Plot type not available yet")
+            # self.data[self.var].plot.hist(title=self.var, color="slateblue")
+            # plt.vlines(
+            #     x=[self.comp_value, self.me, self.mean],
+            #     colors=["r", "k", "k"],
+            #     linestyles=["solid", "dashed", "dashed"],
+            # )
+        else:
+            print("Invalid plot type")
```

### Comparing `pyrsm-0.8.5/pyrsm/basics/compare_props.py` & `pyrsm-0.8.6/pyrsm/basics/compare_props.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 from cmath import sqrt
-import matplotlib
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy import stats
-import seaborn as sns
-from ..model import sig_stars
-from ..utils import ifelse
-from typing import Any, Optional
-from scipy.stats import chisquare
-from statsmodels.stats import multitest
+from typing import Union
 
 
 class compare_props:
     def __init__(
         self,
-        data: pd.DataFrame,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
         grouping_var: str,
         var: str,
         level: str,
         combinations: list[tuple[str, str]],
         alt_hyp: str,
         conf: float,
         multiple_comp_adjustment: str = "none",
```

### Comparing `pyrsm-0.8.5/pyrsm/basics/correlation.py` & `pyrsm-0.8.6/pyrsm/basics/correlation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy import stats
 import seaborn as sns
 from ..model import sig_stars
-from typing import Optional
+from typing import Optional, Union
 
 
 class correlation:
     def __init__(
-        self, data: pd.DataFrame, figsize: Optional[tuple[float, float]] = None
+        self,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
+        figsize: Optional[tuple[float, float]] = None
     ) -> None:
         """
         Calculate correlations between numeric variables in a Pandas dataframe
 
         Parameters
         ----------
         data : Pandas dataframe with numeric variables
```

### Comparing `pyrsm-0.8.5/pyrsm/basics/cross_tabs.py` & `pyrsm-0.8.6/pyrsm/basics/cross_tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from cmath import sqrt
-import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy import stats
-import seaborn as sns
-from ..model import sig_stars
 from ..utils import ifelse
-from typing import Any, Optional
-from scipy.stats import chisquare
-from statsmodels.stats import multitest
+from typing import Union
 
 
 class cross_tabs:
-    def __init__(self, data: pd.DataFrame, var1: str, var2: str) -> None:
+    def __init__(
+        self,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
+        var1: str,
+        var2: str,
+    ) -> None:
         """
         Calculate a Chi-square test between two categorical variables contained
         in a Pandas dataframe
 
         Parameters
         ----------
         data : Pandas dataframe with categorical variables or a
```

### Comparing `pyrsm-0.8.5/pyrsm/basics/goodness.py` & `pyrsm-0.8.6/pyrsm/basics/goodness.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,114 +3,114 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy import stats
 import seaborn as sns
 from ..model import sig_stars
 from ..utils import ifelse
-from typing import Any, Optional
+from typing import Any, Optional, Union
 from scipy.stats import chisquare
-from statsmodels.stats import multitest
 
 
-class goodness_of_fit:
+class goodness:
     def __init__(
         self,
-        data: pd.DataFrame,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
         variable: str,
         figsize: tuple[float, float] = None,
         probabilities: Optional[tuple[float, ...]] = None,
-        params: Optional[tuple[str, ...]] = None,
     ) -> None:
-        self.data = data
+        if isinstance(data, dict):
+            self.name = list(data.keys())[0]
+            self.data = data[self.name]
+        else:
+            self.data = data
+            self.name = "Not provided"
+
         self.variable = variable
         self.figsize = figsize
         self.probabilities = probabilities
-        if params is not None:
-            params = map(str.lower, params)
-            self.params = tuple(params)
-        else:
-            self.params = params
-
         self._observed_frequencies = self.data[self.variable].value_counts().to_dict()
-        if self.params is not None:
-            self._observed_df = pd.DataFrame(
-                {
-                    key: [
-                        item,
-                    ]
-                    for key, item in self._observed_frequencies.items()
-                },
-                columns=sorted(self._observed_frequencies.keys()),
-            )
-            self._observed_df["Total"] = self._observed_df[
-                list(self._observed_df.columns)
-            ].sum(axis=1)
-
-            self._expected_df = pd.DataFrame(
-                {
-                    sorted(self._observed_frequencies.keys())[i]: [
-                        self.probabilities[i] * self._observed_df.at[0, "Total"],
-                    ]
-                    for i in range(len(self._observed_frequencies.keys()))
-                },
-                columns=sorted(self._observed_frequencies.keys()),
-            )
-            self._expected_df["Total"] = self._expected_df[
-                list(self._expected_df.columns)
-            ].sum(axis=1)
-
-            self._chisquared_df = pd.DataFrame(
-                {
-                    column: [
-                        round(
-                            (
-                                (
-                                    self._observed_df.at[0, column]
-                                    - self._expected_df.at[0, column]
-                                )
-                                ** 2
-                            )
-                            / self._expected_df.at[0, column],
-                            2,
-                        ),
-                    ]
-                    for column in self._expected_df.columns.tolist()[:-1]
-                },
-                columns=self._expected_df.columns.tolist(),
-            )
-            self._chisquared_df["Total"] = self._chisquared_df[
-                list(self._chisquared_df.columns)
-            ].sum(axis=1)
-
-            self._stdev_df = pd.DataFrame(
-                {
-                    column: [
-                        round(
+        self._observed_df = pd.DataFrame(
+            {
+                key: [
+                    item,
+                ]
+                for key, item in self._observed_frequencies.items()
+            },
+            columns=sorted(self._observed_frequencies.keys()),
+        )
+        self._observed_df["Total"] = self._observed_df[
+            list(self._observed_df.columns)
+        ].sum(axis=1)
+
+        self._expected_df = pd.DataFrame(
+            {
+                sorted(self._observed_frequencies.keys())[i]: [
+                    self.probabilities[i] * self._observed_df.at[0, "Total"],
+                ]
+                for i in range(len(self._observed_frequencies.keys()))
+            },
+            columns=sorted(self._observed_frequencies.keys()),
+        )
+        self._expected_df["Total"] = self._expected_df[
+            list(self._expected_df.columns)
+        ].sum(axis=1)
+
+        self._chisquared_df = pd.DataFrame(
+            {
+                column: [
+                    round(
+                        (
                             (
                                 self._observed_df.at[0, column]
                                 - self._expected_df.at[0, column]
                             )
-                            / sqrt(self._expected_df.at[0, column]).real,
-                            2,
-                        ),
-                    ]
-                    for column in self._expected_df.columns.tolist()[:-1]
-                },
-                columns=self._expected_df.columns.tolist()[:-1],
-            )
+                            ** 2
+                        )
+                        / self._expected_df.at[0, column],
+                        2,
+                    ),
+                ]
+                for column in self._expected_df.columns.tolist()[:-1]
+            },
+            columns=self._expected_df.columns.tolist(),
+        )
+        self._chisquared_df["Total"] = self._chisquared_df[
+            list(self._chisquared_df.columns)
+        ].sum(axis=1)
+
+        self._stdev_df = pd.DataFrame(
+            {
+                column: [
+                    round(
+                        (
+                            self._observed_df.at[0, column]
+                            - self._expected_df.at[0, column]
+                        )
+                        / sqrt(self._expected_df.at[0, column]).real,
+                        2,
+                    ),
+                ]
+                for column in self._expected_df.columns.tolist()[:-1]
+            },
+            columns=self._expected_df.columns.tolist()[:-1],
+        )
 
-    def summary(self) -> None:
-        print("Goodness of fit test")
-        if hasattr(self.data, "description"):
-            data_name = self.data.description.split("\n")[0].split()[1].lower()
-        else:
-            data_name = "Not available"
+    def summary(
+        self, output: list[str] = ["observed", "expected"], dec: int = 2
+    ) -> None:
 
-        print(f"Data: {data_name}")
+        pd.set_option("display.max_columns", 20)
+        pd.set_option("display.max_rows", 20)
+
+        output = ifelse(isinstance(output, str), [output], output)
+
+        print("Goodness of fit test")
+        print(f"Data: {self.name}")
         if self.variable not in self.data.columns:
             print(f"{self.variable} does not exist in chosen dataset")
             return
 
         print(f"Variable: {self.variable}")
         num_levels = self.data[self.variable].nunique()
         if self.probabilities is None:
@@ -134,37 +134,34 @@
         print(
             f"Null hyp.: The distribution of {self.variable} is consistent with the specified distribution"
         )
         print(
             f"Alt. hyp.: The distribution of {self.variable} is not consistent with the specified distribution"
         )
 
-        if self.params is not None:
-            if "observed" in self.params:
-                print("Observed:")
-                print(self._observed_df.to_string(index=False))
-                print()
-
-            if "expected" in self.params:
-                print("Expected: total x p")
-                print(self._expected_df.to_string(index=False))
-                print()
-
-            if "chi-squared" in self.params:
-                print(
-                    "Contribution to chi-squared: (observed - expected) ^ 2 / expected"
-                )
-                print(self._chisquared_df.to_string(index=False))
-                print()
-
-            if "deviation std" in self.params:
-                print("Deviation standardized: (observed - expected) / sqrt(expected)")
-                print()
-                print(self._stdev_df.to_string(index=False))
-                print()
+        if "observed" in output:
+            print("Observed:")
+            print(self._observed_df.to_string(index=False))
+            print()
+
+        if "expected" in output:
+            print("Expected: total x p")
+            print(self._expected_df.to_string(index=False))
+            print()
+
+        if "chisq" in output:
+            print("Contribution to chi-squared: (observed - expected) ^ 2 / expected")
+            print(self._chisquared_df.to_string(index=False))
+            print()
+
+        if "dev_std" in output:
+            print("Deviation standardized: (observed - expected) / sqrt(expected)")
+            print()
+            print(self._stdev_df.to_string(index=False))
+            print()
 
         chisq, p_val = chisquare(
             [
                 self._observed_frequencies[key]
                 for key in sorted(self._observed_frequencies.keys())
             ],
             [
@@ -174,19 +171,19 @@
         )
         chisq = round(chisq, 3)
 
         if p_val < 0.001:
             p_val = "< .001"
         print(f"Chi-squared: {chisq} df ({num_levels - 1}), p.value {p_val}")
 
-    def plot(self) -> None:
+    def plot(self, output: list[str] = [], **kwargs) -> None:
         _, axes = plt.subplots(2, 2, figsize=self.figsize)
         plt.subplots_adjust(wspace=0.2, hspace=0.2)
 
-        if "observed" in self.params:
+        if "observed" in output:
             plt.axes(axes[0][0])
             observed_frequency_percentages_df = pd.DataFrame(
                 {
                     "levels": self._observed_df.columns.tolist()[:-1],
                     "percentages": [
                         (
                             self._observed_df.at[0, level]
@@ -197,15 +194,15 @@
                     ],
                 }
             )
             sns.barplot(
                 data=observed_frequency_percentages_df, x="levels", y="percentages"
             ).plot()
 
-        if "expected" in self.params:
+        if "expected" in output:
             plt.axes(axes[0][1])
             expected_frequency_percentages_df = pd.DataFrame(
                 {
                     "levels": self._expected_df.columns.tolist()[:-1],
                     "percentages": [
                         (
                             self._expected_df.at[0, level]
@@ -216,30 +213,30 @@
                     ],
                 }
             )
             sns.barplot(
                 data=expected_frequency_percentages_df, x="levels", y="percentages"
             ).plot()
 
-        if "chi-squared" in self.params:
+        if "chisq" in output:
             plt.axes(axes[1][0])
             chisquared_contribution_df = pd.DataFrame(
                 {
                     "levels": self._chisquared_df.columns.tolist()[:-1],
                     "contribution": [
                         self._chisquared_df.at[0, level]
                         for level in self._chisquared_df.columns.tolist()[:-1]
                     ],
                 }
             )
             sns.barplot(
                 data=chisquared_contribution_df, x="levels", y="contribution"
             ).plot()
 
-        if "deviation std" in self.params:
+        if "dev_std" in output:
             plt.axes(axes[1][1])
             standardized_deviation_df = pd.DataFrame(
                 {
                     "levels": self._stdev_df.columns.tolist(),
                     "stdev": [
                         self._stdev_df.at[0, level]
                         for level in self._stdev_df.columns.tolist()
```

### Comparing `pyrsm-0.8.5/pyrsm/basics/probability_calculator.py` & `pyrsm-0.8.6/pyrsm/basics/probability_calculator.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/basics/single_prop.py` & `pyrsm-0.8.6/pyrsm/basics/single_prop.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from cmath import sqrt
-import matplotlib.pyplot as plt
 import pandas as pd
 from scipy import stats
+from typing import Union
 
 
 class single_prop:
     def __init__(
         self,
-        data: pd.DataFrame,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
         variable: str,
         level: str,
         alt_hyp: str,
         conf: float,
         comp_value: float,
         test_type: str = "binomial",
     ) -> None:
         if isinstance(data, dict):
             self.name = list(data.keys())[0]
-            self.data = data[self.name]
+            self.data = data[self.name].copy()
         else:
-            self.data = data
+            self.data = data.copy()
             self.name = "Not provided"
         self.variable = variable
         self.level = level
         self.alt_hyp = alt_hyp
         self.conf = conf
         self.comp_value = comp_value
         self.test_type = test_type
```

### Comparing `pyrsm-0.8.5/pyrsm/bins.py` & `pyrsm-0.8.6/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/__radiant-data-convert.py` & `pyrsm-0.8.6/pyrsm/data/__radiant-data-convert.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/basics/consider.parquet` & `pyrsm-0.8.6/pyrsm/data/basics/consider.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/basics/consider_description.md` & `pyrsm-0.8.6/pyrsm/data/basics/consider_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/basics/demand_uk.parquet` & `pyrsm-0.8.6/pyrsm/data/basics/demand_uk.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/basics/newspaper.parquet` & `pyrsm-0.8.6/pyrsm/data/basics/newspaper.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/basics/newspaper_description.md` & `pyrsm-0.8.6/pyrsm/data/basics/newspaper_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/basics/salary.parquet` & `pyrsm-0.8.6/pyrsm/data/basics/salary.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/basics/salary_description.md` & `pyrsm-0.8.6/pyrsm/data/basics/salary_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/data/avengers.parquet` & `pyrsm-0.8.6/pyrsm/data/data/avengers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/data/diamonds.parquet` & `pyrsm-0.8.6/pyrsm/data/data/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/data/diamonds_description.md` & `pyrsm-0.8.6/pyrsm/data/data/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/data/publishers.parquet` & `pyrsm-0.8.6/pyrsm/data/data/publishers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/data/superheroes.parquet` & `pyrsm-0.8.6/pyrsm/data/data/superheroes.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/data/titanic.parquet` & `pyrsm-0.8.6/pyrsm/data/data/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/data/titanic_description.md` & `pyrsm-0.8.6/pyrsm/data/data/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/design/rndnames.parquet` & `pyrsm-0.8.6/pyrsm/data/design/rndnames.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/catalog.parquet` & `pyrsm-0.8.6/pyrsm/data/model/catalog.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/catalog_description.md` & `pyrsm-0.8.6/pyrsm/data/model/catalog_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/direct_marketing.parquet` & `pyrsm-0.8.6/pyrsm/data/model/direct_marketing.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/direct_marketing_description.md` & `pyrsm-0.8.6/pyrsm/data/model/direct_marketing_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/dvd.parquet` & `pyrsm-0.8.6/pyrsm/data/model/dvd.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/dvd_description.md` & `pyrsm-0.8.6/pyrsm/data/model/dvd_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/fraud_data_description.md` & `pyrsm-0.8.6/pyrsm/data/model/fraud_data_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/houseprices.parquet` & `pyrsm-0.8.6/pyrsm/data/model/houseprices.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/houseprices_description.md` & `pyrsm-0.8.6/pyrsm/data/model/houseprices_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/ideal.parquet` & `pyrsm-0.8.6/pyrsm/data/model/ideal.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/ketchup.parquet` & `pyrsm-0.8.6/pyrsm/data/model/ketchup.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/ketchup_description.md` & `pyrsm-0.8.6/pyrsm/data/model/ketchup_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/model/ratings.parquet` & `pyrsm-0.8.6/pyrsm/data/model/ratings.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/carpet.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/carpet.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/carpet_description.md` & `pyrsm-0.8.6/pyrsm/data/multivariate/carpet_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/city.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/city.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/city2.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/city2.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/computer.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/computer.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/computer_description.md` & `pyrsm-0.8.6/pyrsm/data/multivariate/computer_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/movie.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/movie.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/movie_description.md` & `pyrsm-0.8.6/pyrsm/data/multivariate/movie_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/mp3.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/mp3.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/mp3_description.md` & `pyrsm-0.8.6/pyrsm/data/multivariate/mp3_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/retailers.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/retailers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/retailers_description.md` & `pyrsm-0.8.6/pyrsm/data/multivariate/retailers_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/shopping.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/shopping.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/shopping_description.md` & `pyrsm-0.8.6/pyrsm/data/multivariate/shopping_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/toothpaste.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/toothpaste_description.md` & `pyrsm-0.8.6/pyrsm/data/multivariate/toothpaste_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands.parquet` & `pyrsm-0.8.6/pyrsm/data/multivariate/tpbrands.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/data/multivariate/tpbrands_description.md` & `pyrsm-0.8.6/pyrsm/data/multivariate/tpbrands_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/example_data.py` & `pyrsm-0.8.6/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/logistic.py` & `pyrsm-0.8.6/pyrsm/logistic.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/model.py` & `pyrsm-0.8.6/pyrsm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,24 +58,28 @@
     mfit_dct = None
     model_type = None
     if isinstance(fitted, sm.genmod.generalized_linear_model.GLMResultsWrapper):
         fw = None
         if fitted.model._has_freq_weights:
             fw = fitted.model.freq_weights
 
+        # gets same results as in R
+        lrtest = -2 * (fitted.llnull - fitted.llf)
         mfit_dct = {
             "pseudo_rsq_mcf": [1 - fitted.llf / fitted.llnull],
             "pseudo_rsq_mcf_adj": [1 - (fitted.llf - fitted.df_model) / fitted.llnull],
             "AUC": [auc(fitted.model.endog, fitted.fittedvalues, weights=fw)],
             "log_likelihood": fitted.llf,
             "AIC": [fitted.aic],
             "BIC": [fitted.bic_llf],
-            "chisq": [fitted.pearson_chi2],
+            # "chisq": [fitted.pearson_chi2],
+            "chisq": [lrtest],
             "chisq_df": [fitted.df_model],
-            "chisq_pval": [1 - stats.chi2.cdf(fitted.pearson_chi2, fitted.df_model)],
+            # "chisq_pval": [1 - stats.chi2.cdf(fitted.pearson_chi2, fitted.df_model)],
+            "chisq_pval": [stats.chi2.sf(lrtest, fitted.df_model)],
             "nobs": [fitted.nobs],
         }
 
         model_type = "logistic"
 
     elif isinstance(fitted, sm.regression.linear_model.RegressionResultsWrapper):
         mfit_dct = {
@@ -518,17 +522,14 @@
             fitted.pvalues < 0.001, "< .001", fitted.pvalues.round(dec)
         )
 
     df["  "] = sig_stars(fitted.pvalues)
     if intercept is False:
         df = df[df.index != "Intercept"]
 
-    # df = df.set_index("index")
-    # df.index.name = None
-
     return df
 
 
 def evalreg(df, rvar: str, pred: str, dec: int = 3):
     """
     Evaluate regression models. Calculates R-squared, MSE, and MAE
```

### Comparing `pyrsm-0.8.5/pyrsm/notebook.py` & `pyrsm-0.8.6/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/perf.py` & `pyrsm-0.8.6/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/props.py` & `pyrsm-0.8.6/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/radiant/cross_tabs.py` & `pyrsm-0.8.6/pyrsm/radiant/cross_tabs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 import webbrowser, nest_asyncio, uvicorn
-import io, os, signal
+import io
 import pyrsm as rsm
 from contextlib import redirect_stdout, redirect_stderr
 import pyrsm.radiant.utils as ru
 
 choices = {
     "observed": "Observed",
     "expected": "Expected",
@@ -108,15 +108,15 @@
             return f"""rsm.basics.cross_tabs({args_string})""", code
 
         def show_code():
             sc = estimation_code()
             return f"""{sc[1]}\nct = {sc[0]}"""
 
         @reactive.Calc
-        def cross_tabs():
+        def estimate():
             locals()[input.datasets()] = self.datasets[
                 input.datasets()
             ]  # get data into local scope
             return eval(estimation_code()[0])
 
         def summary_code():
             args = [c for c in input.select_output()]
@@ -169,25 +169,24 @@
     """
     Launch a Radiant-for-Python app for linear regression analysis
     """
     rc = basics_cross_tabs(data_dct, descriptions_dct, open=open)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
-    print(
-        "Pyrsm and Radiant are open source tools and free to use. If you\nare a student or instructor using pyrsm or Radiant for a class,\nas a favor to the developers, please send an email to\n<radiant@rady.ucsd.edu> with the name of the school and class."
-    )
+    ru.message()
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     import pyrsm as rsm
 
-    newspaper, newspaper_description = rsm.load_data(name="newspaper")
-    cross_tabs(
+    newspaper, newspaper_description = rsm.load_data(pkg="basics", name="newspaper")
+    rc = cross_tabs(
         {"newspaper": newspaper}, {"newspaper": newspaper_description}, open=True
     )
+    app = App(rc.shiny_ui(), rc.shiny_server)
```

### Comparing `pyrsm-0.8.5/pyrsm/radiant/logistic.py` & `pyrsm-0.8.6/pyrsm/radiant/single_mean.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,185 @@
-from shiny import App, ui, render, Inputs, Outputs, Session
+from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 import webbrowser, nest_asyncio, uvicorn
+import signal, os
 import pyrsm as rsm
-from faicons import icon_svg
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
-choices = {
-    "None": "None",
-    "dist": "Distribution",
-    "corr": "Correlation",
-    "pred": "Prediction plot",
-    "vimp": "Permutation importance",
-    "or": "OR plot",
-}
-
-controls = {
-    "ci": "Confidence intervals",
-    "vif": "VIF",
-}
 
-summary_extra = (
-    ui.input_radio_buttons(
-        "show_interactions",
-        "Interactions:",
-        choices={0: "None", 2: "2-way", 3: "3-way"},
-        inline=True,
-    ),
-    ui.panel_conditional(
-        "input.show_interactions > 0",
-        ui.output_ui("ui_interactions"),
-    ),
-    ui.input_checkbox_group(
-        "controls",
-        "Additional output:",
-        choices=controls,
-    ),
-    ui.output_ui("ui_evar_test"),
-)
-
-plots_extra = (
-    ui.panel_conditional(
-        "input.plots == 'corr'",
-        ui.input_select(
-            "nobs",
-            "Number of data points plotted:",
-            {1000: "1,000", -1: "All"},
+def ui_summary():
+    return (
+        ui.panel_conditional(
+            "input.tabs == 'Summary'",
+            ui.panel_well(
+                ui.output_ui("ui_var"),
+                ui.input_select(
+                    id="alt_hyp",
+                    label="Alternative hypothesis:",
+                    selected="two-sided",
+                    choices={
+                        "two-sided": "Two sided",
+                        "greater": "Greater than",
+                        "less": "Less than",
+                    },
+                ),
+                ui.input_slider(
+                    id="conf",
+                    label="Confidence level:",
+                    min=0,
+                    max=1,
+                    value=0.95,
+                ),
+                ui.input_numeric(
+                    id="comp_value",
+                    label="Comparison value:",
+                    value=0,
+                ),
+            ),
         ),
-    ),
-    ui.panel_conditional(
-        "input.plots == 'pred'",
-        ui.output_ui("ui_incl_evar"),
-        ui.output_ui("ui_incl_interactions"),
-    ),
-)
+    )
+
 
+choices = {
+    # "None": "None",
+    "hist": "Histogram",
+    # "sim": "Simulate",
+}
 
-class model_logistic:
+
+class basics_single_mean:
     def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, open=open)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Model > Logistic regression (GLM)",
+                "Basics > Single mean",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
-                        ru.ui_summary(summary_extra),
-                        mu.ui_predict(self),
-                        ru.ui_plot(choices, plots_extra),
+                        ui_summary(),
+                        ru.ui_plot(choices),
                     ),
-                    ui.column(8, ru.ui_main_model()),
+                    ui.column(8, ru.ui_main_basics()),
                 ),
             ),
             ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/model-logistic-regression.ipynb",
-                "Logistic regression (GLM) example notebook",
+                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-single-mean.ipynb",
+                "Single mean example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data, stop_app = ru.standard_reactives(self, input, session)
-        ru.make_data_outputs(self, input, output)
-
-        # --- section standard for all model apps ---
-        run_refresh, run_done = ru.reestimate(input)
+        get_data = ru.make_data_elements(self, input, output)
 
         # --- section unique to each app ---
-        mu.make_model_inputs(input, output, get_data, "isBin")
-
-        @output(id="ui_lev")
+        @output(id="ui_var")
         @render.ui
-        def ui_lev():
-            levs = list(get_data()["data"][input.rvar()].unique())
+        def ui_var():
+            isNum = get_data()["var_types"]["isNum"]
             return ui.input_select(
-                id="lev",
-                label="Choose level:",
-                selected=levs[0],
-                choices=levs,
+                id="var",
+                label="Variable (select one)",
+                selected=None,
+                choices=isNum,
             )
 
-        mu.make_int_inputs(input, output, get_data)
+        def estimation_code():
+            data_name, code = (get_data()[k] for k in ["data_name", "code"])
+
+            args = {
+                "data": f"""{{"{data_name}": {data_name}}}""",
+                "var": input.var(),
+                "alt_hyp": input.alt_hyp(),
+                "conf": input.conf(),
+                "comp_value": input.comp_value(),
+            }
+
+            args_string = ru.drop_default_args(args, rsm.basics.single_mean)
+            return f"""rsm.basics.single_mean({args_string})""", code
+
         show_code, estimate = mu.make_estimate(
-            self, input, output, get_data, fun="logistic", ret="lr", debug=True
-        )
-        mu.make_summary(
             self,
             input,
             output,
-            show_code,
-            estimate,
-            ret="lr",
-            sum_fun=rsm.logistic.summary,
+            get_data,
+            fun="basics.single_mean",
+            ret="sm",
+            ec=estimation_code,
+            run=False,
+            debug=True,
         )
-        mu.make_predict(
+
+        def summary_code():
+            return f"""sm.summary()"""
+
+        mu.make_summary(
             self,
             input,
             output,
             show_code,
             estimate,
-            ret="lr",
-            pred_fun=rsm.logistic.predict,
+            ret="sm",
+            sum_fun=rsm.basics.single_mean.summary,
+            sc=summary_code,
         )
+
         mu.make_plot(
             self,
             input,
             output,
             show_code,
             estimate,
-            ret="lr",
+            ret="sm",
         )
 
+        # --- section standard for all apps ---
+        # stops returning code if moved to utils
+        @reactive.Effect
+        @reactive.event(input.stop, ignore_none=True)
+        async def stop_app():
+            rsm.md(f"```python\n{self.stop_code}\n```")
+            await session.app.stop()
+            os.kill(os.getpid(), signal.SIGTERM)
+
 
-def logistic(
-    data_dct: dict,
+def single_mean(
+    data_dct: dict = None,
     descriptions_dct: dict = None,
     open: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
-    Launch a Radiant-for-Python app for logistic regression analysis
+    Launch a Radiant-for-Python app for single_mean hypothesis testing
     """
-    rc = model_logistic(data_dct, descriptions_dct, open=open)
+    if data_dct is None:
+        data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="demand_uk")
+    rc = basics_single_mean(data_dct, descriptions_dct, open)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
-    print(
-        "Pyrsm and Radiant are open source tools and free to use. If you\nare a student or instructor using pyrsm or Radiant for a class,\nas a favor to the developers, please send an email to\n<radiant@rady.ucsd.edu> with the name of the school and class."
-    )
+    ru.message()
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     import pyrsm as rsm
 
-    titanic, titanic_description = rsm.load_data(pkg="data", name="titanic")
-    logistic({"titanic": titanic}, {"titanic": titanic_description}, open=True)
+    # demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
+    # data_dct, descriptions_dct = ru.get_dfs(name="demand_uk")
+    # single_mean(data_dct, descriptions_dct, open=True)
+    single_mean()
```

### Comparing `pyrsm-0.8.5/pyrsm/radiant/model_utils.py` & `pyrsm-0.8.6/pyrsm/radiant/model_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
-from shiny import render, ui, reactive
+import matplotlib.pyplot as plt
+from shiny import render, ui, reactive, req
 from contextlib import redirect_stdout, redirect_stderr
 import pyrsm.radiant.utils as ru
-from ..utils import intersect, ifelse
+from ..utils import intersect
 import numpy as np
 import pandas as pd
 import pyrsm as rsm
 
 
 def ui_predict(self):
     return ui.panel_conditional(
@@ -139,93 +140,100 @@
                 choices=choices,
                 multiple=True,
                 size=min(8, len(choices)),
                 selectize=False,
             )
 
 
-def new_estimation_code():
-    data_name, code = (get_data()[k] for k in ["data_name", "code"])
-    args = {
-        "data": {f"{data_name}": data_name},
-        "rvar": input.rvar(),
-        "lev": input.lev(),
-        "evar": list(input.evar()),
-        "int": list(input.interactions()),
-    }
-
-    if int(input.show_interactions()) > 0 and len(input.interactions()) > 0:
-        args["int"] = None
-
-    args_str = ", ".join(f"{k}={ru.quote(v)}" for k, v in args.items() if v is not None)
-    return f"""rsm.{fun}({args_str})""", code
-
-
-def make_estimate(self, input, output, get_data, fun, ret, debug=False):
-    def estimation_code():
-        data_name, code = (get_data()[k] for k in ["data_name", "code"])
-        try:
-            inp = input.lev()
-        except:
-            inp = None
-
-        args = {
-            "data": f"""{{"{data_name}": {data_name}}}""",
-            "rvar": input.rvar(),
-            "lev": inp,
-            "evar": list(input.evar()),
-        }
+def make_estimate(
+    self, input, output, get_data, fun, ret, run=True, ec=None, debug=False
+):
+    if ec is None:
+
+        def estimation_code():
+            data_name, code = (get_data()[k] for k in ["data_name", "code"])
+            # from https://discord.com/channels/1109483223987277844/1127817202804985917/1129530385429176371
+            # does not work with ifelse for some reason
+            # inp = ifelse("lev" in input, input.lev(), None)
+            if "lev" in input:
+                inp = input.lev()
+            else:
+                inp = None
+
+            args = {
+                "data": f"""{{"{data_name}": {data_name}}}""",
+                "rvar": input.rvar(),
+                "lev": inp,
+                "evar": list(input.evar()),
+            }
 
-        if int(input.show_interactions()) > 0 and len(input.interactions()) > 0:
-            args["ivar"] = list(input.interactions())
+            if int(input.show_interactions()) > 0 and len(input.interactions()) > 0:
+                args["ivar"] = list(input.interactions())
 
-        args_str = ", ".join(
-            f"{k}={ru.quote(v, k)}" for k, v in args.items() if v is not None
-        )
-        return f"""rsm.{fun}({args_str})""", code
+            args_str = ", ".join(
+                f"{k}={ru.quote(v, k)}" for k, v in args.items() if v is not None
+            )
+            return f"""rsm.{fun}({args_str})""", code
+
+    else:
+        estimation_code = ec
 
     if debug:
 
         @output(id="show_estimation_code")
         @render.text
         def show_estimation_code():
             out = io.StringIO()
             with redirect_stdout(out), redirect_stderr(out):
-                try:
-                    print(input.x())  # why is there no error printed anywhere?
-                except Exception as err:
-                    print(err)  # why is there no error printed anywhere?
-
                 print(estimation_code())
+                eval(estimation_code()[0])
+
             return out.getvalue()
 
     def show_code():
         sc = estimation_code()
         return f"""{sc[1]}\n{ret} = {sc[0]}"""
 
-    @reactive.Calc
-    @reactive.event(input.run, ignore_none=True)
-    def estimate():
-        locals()[input.datasets()] = self.datasets[
-            input.datasets()
-        ]  # get data into local scope
-        return eval(estimation_code()[0])
+    if run:
+
+        @reactive.Calc
+        @reactive.event(input.run, ignore_none=True)
+        def estimate():
+            locals()[input.datasets()] = self.datasets[
+                input.datasets()
+            ]  # get data into local scope
+
+            return eval(estimation_code()[0])
+
+    else:
+
+        @reactive.Calc
+        def estimate():
+            locals()[input.datasets()] = self.datasets[
+                input.datasets()
+            ]  # get data into local scope
+
+            return eval(estimation_code()[0])
 
     return show_code, estimate
 
 
-def make_summary(self, input, output, show_code, estimate, ret, sum_fun):
-    def summary_code():
-        args = {c: True for c in input.controls()}
-        if input.evar_test() is not None and len(input.evar_test()) > 0:
-            args["test"] = list(input.evar_test())
-
-        args_string = ru.drop_default_args(args, sum_fun)
-        return f"""{ret}.summary({args_string})"""
-        # return f"""{ret}.summary()"""
+def make_summary(self, input, output, show_code, estimate, ret, sum_fun, sc=None):
+    if sc is None:
+
+        def summary_code():
+            args = {c: True for c in input.controls()}
+            if input.evar_test() is not None and len(input.evar_test()) > 0:
+                args["test"] = list(input.evar_test())
+
+            args_string = ru.drop_default_args(args, sum_fun)
+            return f"""{ret}.summary({args_string})"""
+
+    else:
+        summary_code = sc
 
     @output(id="show_summary_code")
     @render.text
     def show_summary_code():
         cmd = f"""{show_code()}\n{summary_code()}"""
         return ru.code_formatter(cmd, self)
 
@@ -315,15 +323,28 @@
     # def plot_height():
     #     plots = input.plots()
     #     if plots == "pred":
     #         return "800px"
     #     else:
     #         return "1000px"
 
+    @reactive.Calc
+    def gen_plot():
+        locals()[ret] = estimate()
+        eval(f"""{plot_code()}""")
+        fig = plt.gcf()
+        width, height = fig.get_size_inches()  # Get the size in inches
+        return fig, width * 96, height * 96
+
     @output(id="plot")
-    # @render.plot(height=plot_height)
     @render.plot
     def plot():
         plots = input.plots()
         if plots != "None":
-            locals()[ret] = estimate()  # get model object into local scope
-            return eval(f"""{plot_code()}""")
+            return gen_plot()[0]
+
+    @output(id="plot_container")
+    @render.ui
+    def plot_container():
+        req(estimate(), input.plots())
+        width, height = gen_plot()[1:]
+        return ui.output_plot("plot", height=f"{height}px", width=f"{width}px")
```

### Comparing `pyrsm-0.8.5/pyrsm/radiant/regress.py` & `pyrsm-0.8.6/pyrsm/radiant/regress.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from shiny import App, ui, Inputs, Outputs, Session
-import webbrowser, nest_asyncio, uvicorn
+from shiny import App, ui, reactive, Inputs, Outputs, Session
+import webbrowser, nest_asyncio, uvicorn, os, signal
 import pyrsm as rsm
-from faicons import icon_svg
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "None": "None",
     "dist": "Distribution",
     "corr": "Correlation",
@@ -87,19 +86,18 @@
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data, stop_app = ru.standard_reactives(self, input, session)
-        ru.make_data_outputs(self, input, output)
+        get_data = ru.make_data_elements(self, input, output)
 
         # --- section standard for all model apps ---
-        run_refresh, run_done = ru.reestimate(input)
+        ru.reestimate(input)
 
         # --- section unique to each app ---
         mu.make_model_inputs(input, output, get_data, "isNum")
         mu.make_int_inputs(input, output, get_data)
         show_code, estimate = mu.make_estimate(
             self, input, output, get_data, fun="regress", ret="reg", debug=False
         )
@@ -126,39 +124,47 @@
             input,
             output,
             show_code,
             estimate,
             ret="reg",
         )
 
+        # --- section standard for all apps ---
+        # stops returning code if moved to utils
+        @reactive.Effect
+        @reactive.event(input.stop, ignore_none=True)
+        async def stop_app():
+            rsm.md(f"```python\n{self.stop_code}\n```")
+            await session.app.stop()
+            os.kill(os.getpid(), signal.SIGTERM)
+
 
 def regress(
-    data_dct: dict,
+    data_dct: dict = None,
     descriptions_dct: dict = None,
     open: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
     Launch a Radiant-for-Python app for linear regression analysis
     """
+    if data_dct is None:
+        data_dct, descriptions_dct = ru.get_dfs(pkg="model")
     rc = model_regress(data_dct, descriptions_dct, open=open)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
-    print(
-        "Pyrsm and Radiant are open source tools and free to use. If you\nare a student or instructor using pyrsm or Radiant for a class,\nas a favor to the developers, please send an email to\n<radiant@rady.ucsd.edu> with the name of the school and class."
-    )
+    ru.message()
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
-    import pyrsm as rsm
-
-    diamonds, diamonds_description = rsm.load_data(pkg="data", name="diamonds")
-    regress({"diamonds": diamonds}, {"diamonds": diamonds_description}, open=True)
+    # diamonds, diamonds_description = rsm.load_data(pkg="data", name="diamonds")
+    # regress({"diamonds": diamonds}, {"diamonds": diamonds_description}, open=True)
+    regress()
```

### Comparing `pyrsm-0.8.5/pyrsm/radiant/single_mean.py` & `pyrsm-0.8.6/pyrsm/radiant/goodness.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,98 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 import webbrowser, nest_asyncio, uvicorn
-import io
+import io, os, signal
 import pyrsm as rsm
-from contextlib import redirect_stdout, redirect_stderr
+from contextlib import redirect_stdout
 import pyrsm.radiant.utils as ru
 
+choices = {
+    "observed": "Observed",
+    "expected": "Expected",
+    "chisq": "Chi-squared",
+    "dev_std": "Deviation std.",
+}
+
 
 def ui_summary():
+    return ui.panel_conditional(
+        "input.tabs == 'Summary'",
+        ui.panel_well(
+            ui.output_ui("ui_var"),
+            ui.input_numeric(
+                "prob_1", "Probability 1", value=0.9, min=0, max=1, step=0.01
+            ),
+            ui.input_numeric(
+                "prob_2", "Probability 2", value=0.9, min=0, max=1, step=0.01
+            ),
+            ui.input_checkbox_group(
+                id="select_output",
+                label="Select output tables:",
+                choices=choices,
+            ),
+        ),
+    )
+
+
+def ui_plot():
+    plots = {"None": "None"}
+    plots.update(choices)
     return (
         ui.panel_conditional(
-            "input.tabs == 'Summary'",
+            "input.tabs == 'Plot'",
             ui.panel_well(
-                ui.output_ui("ui_var"),
                 ui.input_select(
-                    id="alt_hyp",
-                    label="Alternative hypothesis:",
-                    selected="two-sided",
-                    choices={
-                        "two-sided": "Two sided",
-                        "greater": "Greater than",
-                        "less": "Less than",
-                    },
-                ),
-                ui.input_slider(
-                    id="conf",
-                    label="Confidence level:",
-                    min=0,
-                    max=1,
-                    value=0.95,
-                ),
-                ui.input_numeric(
-                    id="comp_value",
-                    label="Comparison value:",
-                    value=0,
+                    id="select_plot",
+                    label="Select plot:",
+                    choices=plots,
                 ),
             ),
         ),
     )
 
 
-choices = {
-    "None": "None",
-    "hist": "Histogram",
-    "sim": "Simulate",
-}
+def ui_main():
+    return ui.navset_tab_card(
+        ru.ui_data_main(),
+        ui.nav(
+            "Summary",
+            ui.output_ui("show_summary_code"),
+            ui.output_text_verbatim("summary"),
+        ),
+        ui.nav(
+            "Plot",
+            ui.output_ui("show_plot_code"),
+            ui.output_plot("plot", height="500px", width="700px"),
+        ),
+        id="tabs",
+    )
 
 
-class basics_single_mean:
+class basics_goodness:
     def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, open=open)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Single mean",
+                "Basics > Goodness-of-fit",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
-                        ru.ui_plot(choices),
+                        ui_plot(),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
             ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-single-mean.ipynb",
-                "Single mean example notebook",
+                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-cross-tabs.ipynb",  # no example notebook for goodness of fit
+                "Goodness-of-fit example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
@@ -79,113 +100,111 @@
         # --- section standard for all apps ---
         get_data, stop_app = ru.standard_reactives(self, input, session)
         ru.make_data_outputs(self, input, output)
 
         # --- section unique to each app ---
         @output(id="ui_var")
         @render.ui
-        def ui_var():
-            isNum = get_data()["var_types"]["isNum"]
+        def ui_var1():
+            isCat = get_data()["var_types"]["isCat"]
             return ui.input_select(
                 id="var",
-                label="Variable (select one)",
+                label="Select a categorical variable:",
                 selected=None,
-                choices=isNum,
+                choices=isCat,
             )
 
         def estimation_code():
             data_name, code = (get_data()[k] for k in ["data_name", "code"])
 
             args = {
                 "data": f"""{{"{data_name}": {data_name}}}""",
-                "var": input.var(),
-                "alt_hyp": input.alt_hyp(),
-                "conf": input.conf(),
-                "comp_value": input.comp_value(),
+                "variable": input.var(),
+                "probabilities": (input.prob_1(), input.prob_2()),
             }
 
-            args_string = ru.drop_default_args(args, rsm.basics.single_mean)
-            return f"""rsm.basics.single_mean({args_string})""", code
+            args_string = ru.drop_default_args(args, rsm.basics.goodness)
+            return f"""rsm.basics.goodness({args_string})""", code
 
         def show_code():
             sc = estimation_code()
-            return f"""{sc[1]}\nsm = {sc[0]}"""
+            return f"""{sc[1]}\nct = {sc[0]}"""
 
         @reactive.Calc
-        def single_mean():
+        def estimate():
             locals()[input.datasets()] = self.datasets[
                 input.datasets()
             ]  # get data into local scope
             return eval(estimation_code()[0])
 
         def summary_code():
-            return f"""sm.summary()"""
+            args = [c for c in input.select_output()]
+            return f"""gf.summary(output={args})"""
 
         @output(id="show_summary_code")
         @render.text
         def show_summary_code():
             cmd = f"""{show_code()}\n{summary_code()}"""
             return ru.code_formatter(cmd, self)
 
         @output(id="summary")
         @render.text
         def summary():
             out = io.StringIO()
-            with redirect_stdout(out), redirect_stderr(out):
-                sm = single_mean()  # get the reactive object into local scope
-                sm.summary()
+            with redirect_stdout(out):
+                gf = estimate()  # get the reactive object into local scope
+                eval(summary_code())
             return out.getvalue()
 
         def plot_code():
-            return f"""sm.plot("{input.plots()}")"""
+            return f"""gf.plot(output="{input.select_plot()}")"""
 
         @output(id="show_plot_code")
         @render.text
         def show_plot_code():
-            plots = input.plots()
+            plots = input.select_plot()
             if plots != "None":
                 cmd = f"""{show_code()}\n{plot_code()}"""
                 return ru.code_formatter(cmd, self)
 
         @output(id="plot")
         @render.plot
         def plot():
-            plots = input.plots()
+            plots = input.select_plot()
             if plots != "None":
-                sm = single_mean()  # get reactive object into local scope
+                gf = estimate()  # get reactive object into local scope
                 cmd = f"""{plot_code()}"""
                 return eval(cmd)
 
 
-def single_mean(
+def goodness(
     data_dct: dict,
     descriptions_dct: dict = None,
     open: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
-    Launch a Radiant-for-Python app for single_mean hypothesis testing
+    Launch a Radiant-for-Python app for goodness of fit analysis
     """
-    rc = basics_single_mean(data_dct, descriptions_dct, open)
+    rc = basics_goodness(data_dct, descriptions_dct, open=open)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
-    print(
-        "Pyrsm and Radiant are open source tools and free to use. If you\nare a student or instructor using pyrsm or Radiant for a class,\nas a favor to the developers, please send an email to\n<radiant@rady.ucsd.edu> with the name of the school and class."
-    )
+    ru.message()
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
         port=port,
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     import pyrsm as rsm
 
-    demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
-    single_mean(
-        {"demand_uk": demand_uk}, {"demand_uk": demand_uk_description}, open=True
+    newspaper, newspaper_description = rsm.load_data(pkg="basics", name="newspaper")
+    rc = basics_goodness(
+        {"newspaper": newspaper}, {"newspaper": newspaper_description}, open=True
     )
+    app = App(rc.shiny_ui(), rc.shiny_server)
```

### Comparing `pyrsm-0.8.5/pyrsm/radiant/utils.py` & `pyrsm-0.8.6/pyrsm/radiant/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,73 @@
-import black, os, signal, inspect
+import black, os, signal, inspect, time
 from htmltools import tags, div, css
 from itertools import combinations
 from shiny import render, ui, reactive
 from faicons import icon_svg
 from pathlib import Path
 import pandas as pd
+import polars as pl
 from pyrsm.utils import ifelse, md
+from pyrsm.example_data import load_data
+
+
+def get_dfs(pkg=None, name=None, obj=pd.DataFrame):
+    data_dct = {k: v for k, v in globals().items() if isinstance(v, obj)}
+    descriptions_dct = {
+        k: globals()[f"{k}_description"]
+        for k in data_dct
+        if f"{k}_description" in globals()
+    }
+    if len(data_dct) == 0 and name is not None:
+        data, description = load_data(pkg=pkg, name=name)
+        data_dct = {name: data}
+        descriptions_dct = {name: description}
+    elif len(data_dct) == 0 and pkg is not None:
+        data_dct, descriptions_dct = load_data(pkg=pkg)
+
+    return ifelse(len(data_dct) == 0, None, data_dct), ifelse(
+        len(descriptions_dct) == 0, None, descriptions_dct
+    )
+
+
+def message():
+    print(
+        "Pyrsm and Radiant are open source tools and free to use. If you\nare a student or instructor using pyrsm or Radiant for a class,\nas a favor to the developers, please send an email to\n<radiant@rady.ucsd.edu> with the name of the school and class.\nIf you are using Radiant in your company, as a favor to the\ndeveloper, please share the name of your company and what types\nof activites you are supporting with the tool."
+    )
 
 
 def head_content():
     """
     Return the head content for the shiny app
     """
+
+    www_dir = Path(__file__).parent / "www"  # (8)
     return ui.head_content(
-        ui.tags.script(
-            (Path(__file__).parent / "www/returnTextAreaBinding.js").read_text()
-        ),
-        ui.tags.script((Path(__file__).parent / "www/copy.js").read_text()),
         # from https://github.com/rstudio/py-shiny/issues/491#issuecomment-1579138681
         ui.tags.link(
             href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/agate.min.css",
             rel="stylesheet",
         ),
+        ui.tags.link(rel="shortcut icon", href=f"{www_dir}/imgs/icon.png"),
+        ui.tags.style((www_dir / "style.css").read_text()),
+        ui.tags.script(
+            (www_dir / "js/returnTextAreaBinding.js").read_text(),
+        ),
+        ui.tags.script(
+            (www_dir / "js/radiantUI.js").read_text(),
+        ),
         ui.tags.script(
-            src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js"
+            (www_dir / "js/screenshot.js").read_text(),
+        ),
+        ui.tags.script(
+            src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js",
+        ),
+        ui.tags.script(
+            src="//html2canvas.hertzen.com/dist/html2canvas.min.js",
         ),
-        ui.tags.style((Path(__file__).parent / "www/style.css").read_text()),
     )
 
 
 def init(self, datasets, descriptions=None, open=True):
     """
     Initialize key 'self' values to be used in an app class
     """
@@ -63,15 +101,15 @@
 
 def copy_icon(cmd):
     cmd = escape_quotes(cmd).replace("\n", "\\n")
     return (
         ui.input_action_link(
             "copy",
             None,
-            icon=icon_svg("copy", width="1.2em", height="1.2em"),
+            icon=icon_svg("copy", width="1.5em", height="1.5em"),
             title="Copy to clipboard",
             onclick=f'copyToClipboard("{cmd}");',
         ),
     )
 
 
 def code_formatter(code, self):
@@ -151,30 +189,15 @@
         "data_name": data_name,
         "description": description,
         "var_types": var_types,
         "code": code,
     }
 
 
-def standard_reactives(self, input, session):
-    @reactive.Calc
-    def rget_data():
-        return get_data(self, input)
-
-    @reactive.Effect
-    @reactive.event(input.stop, ignore_none=True)
-    async def stop_app():
-        md(f"```python\n{input.stop_code}\n```")
-        await session.app.stop()
-        os.kill(os.getpid(), signal.SIGTERM)
-
-    return rget_data, stop_app
-
-
-def make_data_outputs(self, input, output):
+def make_data_elements(self, input, output):
     @output(id="show_data_code")
     @render.ui
     def show_data_code():
         return code_formatter(get_data(self, input)["code"], self)
 
     @output(id="show_data")
     @render.data_frame
@@ -188,14 +211,20 @@
         return render.DataTable(data, summary=summary)
 
     @output(id="show_description")
     @render.ui
     def show_description():
         return ui.markdown(get_data(self, input)["description"])
 
+    @reactive.Calc
+    def rget_data():
+        return get_data(self, input)
+
+    return rget_data
+
 
 def input_return_text_area(id, label, value="", rows=1, placeholder=""):
     classes = ["form-control", "returnTextArea"]
     area = tags.textarea(
         value,
         id=id,
         class_=" ".join(classes),
@@ -237,15 +266,15 @@
 
 def ui_data(self):
     return (
         ui.panel_conditional(
             "input.tabs == 'Data'",
             ui.panel_well(
                 ui.input_select("datasets", "Datasets:", self.dataset_list),
-                ui.input_checkbox("show_filter", "Show data filter"),
+                ui.input_checkbox("show_filter", "Show data filter", value=True),
                 ui.panel_conditional(
                     "input.show_filter == true",
                     # ui.input_radio_buttons(
                     #     "data_language",
                     #     "Data language",
                     #     ["Pandas", "Polars", "SQL"],
                     #     inline=True,
@@ -314,26 +343,27 @@
         ui.output_ui("show_data_code"),
         ui.output_data_frame("show_data"),
         ui.output_ui("show_description"),
     )
     return data_main
 
 
-def ui_main_basics():
+def ui_main_basics(height="500px", width="700px"):
     return ui.navset_tab_card(
         ui_data_main(),
         ui.nav(
             "Summary",
             ui.output_ui("show_summary_code"),
             ui.output_text_verbatim("summary"),
         ),
         ui.nav(
             "Plot",
             ui.output_ui("show_plot_code"),
-            ui.output_plot("plot", height="500px", width="700px"),
+            # ui.output_plot("plot", height=height, width=width),
+            ui.output_ui("plot_container"),
         ),
         id="tabs",
     )
 
 
 def ui_main_model():
     return ui.navset_tab_card(
@@ -348,26 +378,35 @@
             "Predict",
             ui.output_ui("show_predict_code"),
             ui.output_data_frame("predict"),
         ),
         ui.nav(
             "Plot",
             ui.output_ui("show_plot_code"),
-            ui.output_plot("plot", height="800px", width="700px"),
+            # ui.output_plot("plot", height="800px", width="700px"),
+            ui.output_ui("plot_container"),
         ),
         id="tabs",
     )
 
 
 def ui_stop():
     return (
         ui.nav_control(
             ui.input_action_link(
+                "screenshot",
+                "Screenshot",
+                icon=icon_svg("camera"),
+                onclick="generate_screenshot();",
+            ),
+        ),
+        ui.nav_control(
+            ui.input_action_link(
                 "stop", "Stop", icon=icon_svg("stop"), onclick="window.close();"
-            )
+            ),
         ),
     )
 
 
 def ui_help(link, example):
     return (
         ui.nav_menu(
@@ -424,25 +463,109 @@
         if not is_empty(input.evar()) and not is_empty(input.rvar()):
             update()
 
         # not clear why this needs to be separate from the above
         if not is_empty(input.interactions()):
             update()
 
+    ## first bit works but can't reset on a timer
+    # @reactive.Effect
+    # @reactive.event(input.copy, ignore_none=True)
+    # def copy_success():
+    #     ui.update_action_link(
+    #         "copy",
+    #         icon=icon_svg("check", width="1.5em", height="1.5em"),
+    #     )
+
+    # @reactive.Effect
+    # @reactive.event(input.copy, ignore_none=True)
+    # def copy_reset():
+    #     reactive.invalidate_later(0.5)
+    #     ui.update_action_link(
+    #         "copy",
+    #         icon=icon_svg("copy", width="1.5em", height="1.5em"),
+    #     )
+
     @reactive.Effect
     @reactive.event(input.run, ignore_none=True)
     def run_done():
         ui.update_action_button(
             "run",
             label="Estimate model",
             icon=icon_svg("play"),
         )
 
-    return run_refresh, run_done
+    return run_refresh, run_done  # , copy_success, copy_reset
+
 
+# radiant_screenshot_modal <- function(report_on = "") {
+#   add_button <- function() {
+#     if (is.empty(report_on)) {
+#       ""
+#     } else {
+#       actionButton(report_on, "Report", icon = icon("edit", verify_fa = FALSE), class = "btn-success")
+#     }
+#   }
+#   showModal(
+#     modalDialog(
+#       title = "Radiant screenshot",
+#       span(shiny::tags$div(id = "screenshot_preview")),
+#       span(HTML("</br>To include a screenshot in a report first save it to disk by clicking on the <em>Save</em> button. Then click the <em>Report</em> button to insert a reference to the screenshot into <em>Report > Rmd</em>.")),
+#       footer = tagList(
+#         tags$table(
+#           tags$td(download_button("screenshot_save", "Save", ic = "download")),
+#           tags$td(add_button()),
+#           tags$td(modalButton("Cancel")),
+#           align = "right"
+#         )
+#       ),
+#       size = "l",
+#       easyClose = TRUE
+#     )
+#   )
+# }
+
+# observeEvent(input$screenshot_link, {
+#   radiant_screenshot_modal()
+# })
+
+# render_screenshot <- function() {
+#   plt <- sub("data:.+base64,", "", input$img_src)
+#   png::readPNG(base64enc::base64decode(what = plt))
+# }
+
+# download_handler_screenshot <- function(path, plot, ...) {
+#   plot <- try(plot(), silent = TRUE)
+#   if (inherits(plot, "try-error") || is.character(plot) || is.null(plot)) {
+#     plot <- ggplot() +
+#       labs(title = "Plot not available")
+#     png(file = path, width = 500, height = 100, res = 96)
+#     print(plot)
+#     dev.off()
+#   } else {
+#     ppath <- parse_path(path, pdir = getOption("radiant.launch_dir", find_home()), mess = FALSE)
+#     # r_info[["latest_screenshot"]] <- glue("![]({ppath$rpath})")
+#     # r_info[["latest_screenshot"]] <- glue("<details>\n<summary>Click to show screenshot</summary>\n<img src='{ppath$rpath}' alt='Radiant screenshot'>\n</details>")
+#     r_info[["latest_screenshot"]] <- glue("\n<details>\n<summary>Click to show screenshot with Radiant settings to generate output shown below</summary>\n\n![]({ppath$rpath})\n</details></br>\n")
+#     png::writePNG(plot, path, dpi = 144)
+#   }
+# }
+
+# download_handler(
+#   id = "screenshot_save",
+#   fun = download_handler_screenshot,
+#   fn = function() paste0(r_info[["radiant_tab_name"]], "-screenshot"),
+#   type = "png",
+#   caption = "Save radiant screenshot",
+#   plot = render_screenshot,
+#   btn = "button",
+#   label = "Save",
+#   class = "btn-primary",
+#   onclick = "get_img_src();"
+# )
 
 # getting data to work as a separate nav item caused problems
 # def ui_data(self):
 #     return ui.nav(
 #         "Data",
 #         ui.row(
 #             ui.column(
```

### Comparing `pyrsm-0.8.5/pyrsm/radiant/www/style.css` & `pyrsm-0.8.6/pyrsm/radiant/www/style.css`

 * *Files 23% similar despite different names*

```diff
@@ -32,10 +32,13 @@
 }
 
 #copy:hover {
     opacity: 0.9;
 }
 
 #copy:active {
-    color: "grey";
+    opacity: 0.5;
+}
+
+#run:active {
     opacity: 0.5;
 }
```

### Comparing `pyrsm-0.8.5/pyrsm/regress.py` & `pyrsm-0.8.6/pyrsm/regress.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,15 @@
         df.index.name = None
         print(f"\n{df.to_string()}")
         print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
         print(f"\n{model_fit(self.fitted)}")
 
         if ci:
             print("\nConfidence intervals:")
-            df = coef_ci(self.fitted).set_index("index")
-            df.index.name = None
+            df = coef_ci(self.fitted)
             print(f"\n{df.to_string()}")
 
         if ssq:
             print("\nSum of squares:")
             index = ["Regression", "Error", "Total"]
             sum_of_squares = [
                 self.fitted.ess,
```

### Comparing `pyrsm-0.8.5/pyrsm/stats.py` & `pyrsm-0.8.6/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/utils.py` & `pyrsm-0.8.6/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm/visualize.py` & `pyrsm-0.8.6/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.6/pyrsm.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.5/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.8.6/pyrsm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -31,108 +31,84 @@
 pyrsm/basics/single_mean.py
 pyrsm/basics/single_prop.py
 pyrsm/basics/utils.py
 pyrsm/data/__init__.py
 pyrsm/data/__radiant-data-convert.py
 pyrsm/data/basics/__init__.py
 pyrsm/data/basics/consider.parquet
-pyrsm/data/basics/consider.pkl
 pyrsm/data/basics/consider_description.md
 pyrsm/data/basics/demand_uk.parquet
-pyrsm/data/basics/demand_uk.pkl
 pyrsm/data/basics/demand_uk_description.md
 pyrsm/data/basics/newspaper.parquet
-pyrsm/data/basics/newspaper.pkl
 pyrsm/data/basics/newspaper_description.md
 pyrsm/data/basics/salary.parquet
-pyrsm/data/basics/salary.pkl
 pyrsm/data/basics/salary_description.md
 pyrsm/data/data/__init__.py
 pyrsm/data/data/avengers.parquet
-pyrsm/data/data/avengers.pkl
 pyrsm/data/data/avengers_description.md
 pyrsm/data/data/diamonds.parquet
-pyrsm/data/data/diamonds.pkl
 pyrsm/data/data/diamonds_description.md
 pyrsm/data/data/publishers.parquet
-pyrsm/data/data/publishers.pkl
 pyrsm/data/data/publishers_description.md
 pyrsm/data/data/superheroes.parquet
-pyrsm/data/data/superheroes.pkl
 pyrsm/data/data/superheroes_description.md
 pyrsm/data/data/titanic.parquet
-pyrsm/data/data/titanic.pkl
 pyrsm/data/data/titanic_description.md
 pyrsm/data/design/__init__.py
 pyrsm/data/design/rndnames.parquet
-pyrsm/data/design/rndnames.pkl
 pyrsm/data/design/rndnames_description.md
 pyrsm/data/model/__init__.py
 pyrsm/data/model/catalog.parquet
-pyrsm/data/model/catalog.pkl
 pyrsm/data/model/catalog_description.md
+pyrsm/data/model/diamonds.parquet
+pyrsm/data/model/diamonds_description.md
 pyrsm/data/model/direct_marketing.parquet
-pyrsm/data/model/direct_marketing.pkl
 pyrsm/data/model/direct_marketing_description.md
 pyrsm/data/model/dvd.parquet
-pyrsm/data/model/dvd.pkl
 pyrsm/data/model/dvd_description.md
 pyrsm/data/model/fraud_data_description.md
 pyrsm/data/model/houseprices.parquet
-pyrsm/data/model/houseprices.pkl
 pyrsm/data/model/houseprices_description.md
 pyrsm/data/model/ideal.parquet
-pyrsm/data/model/ideal.pkl
 pyrsm/data/model/ideal_description.md
 pyrsm/data/model/ketchup.parquet
-pyrsm/data/model/ketchup.pkl
 pyrsm/data/model/ketchup_description.md
 pyrsm/data/model/ratings.parquet
-pyrsm/data/model/ratings.pkl
 pyrsm/data/model/ratings_description.md
 pyrsm/data/multivariate/__init__.py
 pyrsm/data/multivariate/carpet.parquet
-pyrsm/data/multivariate/carpet.pkl
 pyrsm/data/multivariate/carpet_description.md
 pyrsm/data/multivariate/city.parquet
-pyrsm/data/multivariate/city.pkl
 pyrsm/data/multivariate/city2.parquet
-pyrsm/data/multivariate/city2.pkl
 pyrsm/data/multivariate/city2_description.md
 pyrsm/data/multivariate/city_description.md
 pyrsm/data/multivariate/computer.parquet
-pyrsm/data/multivariate/computer.pkl
 pyrsm/data/multivariate/computer_description.md
 pyrsm/data/multivariate/movie.parquet
-pyrsm/data/multivariate/movie.pkl
 pyrsm/data/multivariate/movie_description.md
 pyrsm/data/multivariate/mp3.parquet
-pyrsm/data/multivariate/mp3.pkl
 pyrsm/data/multivariate/mp3_description.md
 pyrsm/data/multivariate/retailers.parquet
-pyrsm/data/multivariate/retailers.pkl
 pyrsm/data/multivariate/retailers_description.md
 pyrsm/data/multivariate/shopping.parquet
-pyrsm/data/multivariate/shopping.pkl
 pyrsm/data/multivariate/shopping_description.md
 pyrsm/data/multivariate/toothpaste.parquet
-pyrsm/data/multivariate/toothpaste.pkl
 pyrsm/data/multivariate/toothpaste_description.md
 pyrsm/data/multivariate/tpbrands.parquet
-pyrsm/data/multivariate/tpbrands.pkl
 pyrsm/data/multivariate/tpbrands_description.md
 pyrsm/radiant/__init__.py
+pyrsm/radiant/compare_means.py
 pyrsm/radiant/cross_tabs.py
+pyrsm/radiant/goodness.py
 pyrsm/radiant/logistic.py
 pyrsm/radiant/model_utils.py
 pyrsm/radiant/regress.py
 pyrsm/radiant/single_mean.py
 pyrsm/radiant/utils.py
-pyrsm/radiant/www/copy.js
-pyrsm/radiant/www/returnTextAreaBinding.js
+pyrsm/radiant/www/.DS_Store
 pyrsm/radiant/www/style.css
 tests/test_basics.py
 tests/test_bins.py
 tests/test_example_data.py
 tests/test_perf.py
 tests/test_regression.py
 tests/test_stats.py
```

### Comparing `pyrsm-0.8.5/setup.cfg` & `pyrsm-0.8.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/tests/test_basics.py` & `pyrsm-0.8.6/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/tests/test_bins.py` & `pyrsm-0.8.6/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/tests/test_example_data.py` & `pyrsm-0.8.6/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/tests/test_perf.py` & `pyrsm-0.8.6/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/tests/test_regression.py` & `pyrsm-0.8.6/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/tests/test_stats.py` & `pyrsm-0.8.6/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.5/tests/test_utils.py` & `pyrsm-0.8.6/tests/test_utils.py`

 * *Files identical despite different names*

