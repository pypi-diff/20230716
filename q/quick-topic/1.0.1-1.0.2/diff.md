# Comparing `tmp/quick-topic-1.0.1.tar.gz` & `tmp/quick-topic-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick-topic-1.0.1.tar", last modified: Sat Jul 15 13:11:31 2023, max compression
+gzip compressed data, was "quick-topic-1.0.2.tar", last modified: Sun Jul 16 00:39:20 2023, max compression
```

## Comparing `quick-topic-1.0.1.tar` & `quick-topic-1.0.2.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.274165 quick-topic-1.0.1/
--rw-rw-rw-   0        0        0     1106 2023-07-15 13:11:14.000000 quick-topic-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      270 2023-07-15 13:11:14.000000 quick-topic-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    15169 2023-07-15 13:11:31.274165 quick-topic-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    14084 2023-07-15 13:11:14.000000 quick-topic-1.0.1/README.md
--rw-rw-rw-   0        0        0       81 2023-07-15 13:11:31.275165 quick-topic-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     8905 2023-07-15 13:11:14.000000 quick-topic-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.005224 quick-topic-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.016224 quick-topic-1.0.1/src/quick_topic/
--rw-rw-rw-   0        0        0       25 2022-02-25 13:51:54.000000 quick-topic-1.0.1/src/quick_topic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.047232 quick-topic-1.0.1/src/quick_topic/__pycache__/
--rw-rw-rw-   0        0        0      196 2022-02-25 14:01:49.000000 quick-topic-1.0.1/src/quick_topic/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      204 2022-03-22 18:01:28.000000 quick-topic-1.0.1/src/quick_topic/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      243 2022-03-22 07:38:41.000000 quick-topic-1.0.1/src/quick_topic/__pycache__/cli.cpython-36.pyc
--rw-rw-rw-   0        0        0      251 2022-03-22 18:01:28.000000 quick-topic-1.0.1/src/quick_topic/__pycache__/cli.cpython-39.pyc
--rw-rw-rw-   0        0        0       73 2022-03-21 19:30:28.000000 quick-topic-1.0.1/src/quick_topic/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.079827 quick-topic-1.0.1/src/quick_topic/gui/
--rw-rw-rw-   0        0        0        0 2022-03-20 16:53:12.000000 quick-topic-1.0.1/src/quick_topic/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.084830 quick-topic-1.0.1/src/quick_topic/gui/__pycache__/
--rw-rw-rw-   0        0        0      172 2022-03-20 17:07:55.000000 quick-topic-1.0.1/src/quick_topic/gui/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      180 2022-03-22 18:01:28.000000 quick-topic-1.0.1/src/quick_topic/gui/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     9051 2022-03-22 07:35:59.000000 quick-topic-1.0.1/src/quick_topic/gui/__pycache__/main.cpython-36.pyc
--rw-rw-rw-   0        0        0    10762 2022-03-28 08:29:07.000000 quick-topic-1.0.1/src/quick_topic/gui/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0    20582 2022-03-22 07:38:41.000000 quick-topic-1.0.1/src/quick_topic/gui/__pycache__/run.cpython-36.pyc
--rw-rw-rw-   0        0        0    22465 2022-03-28 05:34:34.000000 quick-topic-1.0.1/src/quick_topic/gui/__pycache__/run.cpython-39.pyc
--rw-rw-rw-   0        0        0    22421 2022-03-28 08:29:02.000000 quick-topic-1.0.1/src/quick_topic/gui/main.py
--rw-rw-rw-   0        0        0    26468 2022-03-28 05:36:45.000000 quick-topic-1.0.1/src/quick_topic/gui/main.ui
--rw-rw-rw-   0        0        0    17701 2022-03-22 19:28:48.000000 quick-topic-1.0.1/src/quick_topic/gui/qtt.png
--rw-rw-rw-   0        0        0     1163 2022-03-22 21:58:48.000000 quick-topic-1.0.1/src/quick_topic/gui/quick_topic.config
--rw-rw-rw-   0        0        0    35374 2022-03-23 04:07:14.000000 quick-topic-1.0.1/src/quick_topic/gui/run.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.116096 quick-topic-1.0.1/src/quick_topic/gui_functions/
--rw-rw-rw-   0        0        0        0 2022-03-20 18:11:14.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.132394 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/
--rw-rw-rw-   0        0        0      182 2022-03-20 18:26:01.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      190 2022-03-22 18:03:50.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1676 2022-03-21 19:50:20.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_keywordstat.cpython-36.pyc
--rw-rw-rw-   0        0        0     1690 2022-03-22 20:04:20.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_keywordstat.cpython-39.pyc
--rw-rw-rw-   0        0        0     1082 2022-03-22 21:41:37.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_explore.cpython-39.pyc
--rw-rw-rw-   0        0        0     1854 2022-03-21 18:31:43.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_interaction.cpython-36.pyc
--rw-rw-rw-   0        0        0     1903 2022-03-22 19:11:02.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_interaction.cpython-39.pyc
--rw-rw-rw-   0        0        0     1198 2022-03-22 02:28:25.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_modeling.cpython-36.pyc
--rw-rw-rw-   0        0        0     1260 2022-03-22 21:41:37.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_modeling.cpython-39.pyc
--rw-rw-rw-   0        0        0     1632 2022-03-22 16:04:12.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_prevalence.cpython-36.pyc
--rw-rw-rw-   0        0        0     1660 2022-03-22 20:04:20.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_prevalence.cpython-39.pyc
--rw-rw-rw-   0        0        0     1176 2022-03-22 03:20:19.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_similarity.cpython-36.pyc
--rw-rw-rw-   0        0        0     1206 2022-03-22 20:41:18.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_similarity.cpython-39.pyc
--rw-rw-rw-   0        0        0     1381 2022-03-22 02:51:00.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_term_year.cpython-36.pyc
--rw-rw-rw-   0        0        0     1408 2022-03-22 20:04:20.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_term_year.cpython-39.pyc
--rw-rw-rw-   0        0        0     1748 2022-03-22 16:04:13.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_topic_year.cpython-36.pyc
--rw-rw-rw-   0        0        0     1769 2022-03-22 20:04:20.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_topic_year.cpython-39.pyc
--rw-rw-rw-   0        0        0     1130 2022-03-21 15:57:50.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_trends.cpython-36.pyc
--rw-rw-rw-   0        0        0     1153 2022-03-22 20:04:20.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_trends.cpython-39.pyc
--rw-rw-rw-   0        0        0     1866 2022-03-22 03:15:47.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_trends_correlation.cpython-36.pyc
--rw-rw-rw-   0        0        0     1898 2022-03-22 20:04:20.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_trends_correlation.cpython-39.pyc
--rw-rw-rw-   0        0        0     2206 2022-03-22 20:04:18.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_keywordstat.py
--rw-rw-rw-   0        0        0     1179 2022-03-22 21:26:37.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_explore.py
--rw-rw-rw-   0        0        0     2573 2022-03-22 19:05:08.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_interaction.py
--rw-rw-rw-   0        0        0     1705 2022-03-22 21:11:44.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_modeling.py
--rw-rw-rw-   0        0        0     2268 2022-03-22 20:04:18.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_prevalence.py
--rw-rw-rw-   0        0        0     1617 2022-03-22 20:40:48.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_similarity.py
--rw-rw-rw-   0        0        0     2206 2022-03-22 20:04:18.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_transition_term_year.py
--rw-rw-rw-   0        0        0     2293 2022-03-22 20:04:18.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_transition_topic_year.py
--rw-rw-rw-   0        0        0     1402 2022-03-22 20:04:18.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_trends.py
--rw-rw-rw-   0        0        0     2103 2022-03-22 20:04:18.000000 quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_trends_correlation.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.151918 quick-topic-1.0.1/src/quick_topic/topic_interaction/
--rw-rw-rw-   0        0        0        0 2022-02-25 15:41:01.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.160919 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/
--rw-rw-rw-   0        0        0      186 2022-02-25 15:58:13.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      194 2022-03-22 18:03:50.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2253 2022-03-20 04:06:48.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/divide_by_tag.cpython-36.pyc
--rw-rw-rw-   0        0        0     2271 2022-03-22 20:19:28.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/divide_by_tag.cpython-39.pyc
--rw-rw-rw-   0        0        0     4049 2022-03-22 16:04:12.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/interaction_among_tag.cpython-36.pyc
--rw-rw-rw-   0        0        0     3975 2022-03-22 18:09:43.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/interaction_among_tag.cpython-39.pyc
--rw-rw-rw-   0        0        0     7885 2022-03-22 16:03:56.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/lda_by_tag_each.cpython-36.pyc
--rw-rw-rw-   0        0        0     7734 2022-03-22 20:19:28.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/lda_by_tag_each.cpython-39.pyc
--rw-rw-rw-   0        0        0     1533 2022-03-21 18:29:00.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/main.cpython-36.pyc
--rw-rw-rw-   0        0        0     1553 2022-03-22 18:03:50.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0     3682 2022-03-22 20:19:01.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/divide_by_tag.py
--rw-rw-rw-   0        0        0     7170 2022-03-22 15:58:27.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/interaction_among_tag.py
--rw-rw-rw-   0        0        0     3641 2022-03-22 15:58:27.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/lda_by_tag_all.py
--rw-rw-rw-   0        0        0    11038 2023-07-15 13:05:30.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/lda_by_tag_each.py
--rw-rw-rw-   0        0        0     2529 2022-03-21 18:29:00.000000 quick-topic-1.0.1/src/quick_topic/topic_interaction/main.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.169914 quick-topic-1.0.1/src/quick_topic/topic_modeling/
--rw-rw-rw-   0        0        0        0 2022-02-26 12:47:44.000000 quick-topic-1.0.1/src/quick_topic/topic_modeling/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.172916 quick-topic-1.0.1/src/quick_topic/topic_modeling/__pycache__/
--rw-rw-rw-   0        0        0      183 2022-02-26 12:59:28.000000 quick-topic-1.0.1/src/quick_topic/topic_modeling/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      191 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_modeling/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5665 2022-03-22 16:04:13.000000 quick-topic-1.0.1/src/quick_topic/topic_modeling/__pycache__/lda.cpython-36.pyc
--rw-rw-rw-   0        0        0     5713 2022-03-22 20:47:38.000000 quick-topic-1.0.1/src/quick_topic/topic_modeling/__pycache__/lda.cpython-39.pyc
--rw-rw-rw-   0        0        0    10127 2023-07-15 13:09:17.000000 quick-topic-1.0.1/src/quick_topic/topic_modeling/lda.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.185921 quick-topic-1.0.1/src/quick_topic/topic_prevalence/
--rw-rw-rw-   0        0        0        0 2022-02-25 13:51:07.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.194923 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/
--rw-rw-rw-   0        0        0      185 2022-02-25 14:01:49.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      193 2022-03-22 18:09:43.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1208 2022-03-07 13:50:26.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/divide_per_year.cpython-36.pyc
--rw-rw-rw-   0        0        0     1216 2022-03-22 18:09:43.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/divide_per_year.cpython-39.pyc
--rw-rw-rw-   0        0        0     5238 2022-03-15 15:24:39.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/lda_per_year.cpython-36.pyc
--rw-rw-rw-   0        0        0     5234 2022-03-22 18:09:43.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/lda_per_year.cpython-39.pyc
--rw-rw-rw-   0        0        0     1222 2022-03-21 19:27:44.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/main.cpython-36.pyc
--rw-rw-rw-   0        0        0     1242 2022-03-22 18:09:43.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0     2678 2022-03-21 18:59:12.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/trends_per_year.cpython-36.pyc
--rw-rw-rw-   0        0        0     2619 2022-03-22 18:09:43.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/trends_per_year.cpython-39.pyc
--rw-rw-rw-   0        0        0     1616 2022-03-07 13:50:26.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/divide_per_year.py
--rw-rw-rw-   0        0        0     8260 2022-03-15 15:19:14.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/lda_per_year.py
--rw-rw-rw-   0        0        0     1731 2022-03-21 19:27:41.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/main.py
--rw-rw-rw-   0        0        0     4023 2022-03-21 18:59:09.000000 quick-topic-1.0.1/src/quick_topic/topic_prevalence/trends_per_year.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.197919 quick-topic-1.0.1/src/quick_topic/topic_similarity/
--rw-rw-rw-   0        0        0        0 2022-02-26 10:43:06.000000 quick-topic-1.0.1/src/quick_topic/topic_similarity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.201916 quick-topic-1.0.1/src/quick_topic/topic_similarity/__pycache__/
--rw-rw-rw-   0        0        0      185 2022-02-26 10:57:01.000000 quick-topic-1.0.1/src/quick_topic/topic_similarity/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      193 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_similarity/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3098 2022-03-22 16:04:13.000000 quick-topic-1.0.1/src/quick_topic/topic_similarity/__pycache__/topic_similarity_by_category.cpython-36.pyc
--rw-rw-rw-   0        0        0     3088 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_similarity/__pycache__/topic_similarity_by_category.cpython-39.pyc
--rw-rw-rw-   0        0        0     4320 2022-04-09 17:57:15.000000 quick-topic-1.0.1/src/quick_topic/topic_similarity/topic_similarity_by_category.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.203915 quick-topic-1.0.1/src/quick_topic/topic_stat/
--rw-rw-rw-   0        0        0        0 2022-02-26 11:15:43.000000 quick-topic-1.0.1/src/quick_topic/topic_stat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.206917 quick-topic-1.0.1/src/quick_topic/topic_stat/__pycache__/
--rw-rw-rw-   0        0        0      179 2022-02-26 12:37:38.000000 quick-topic-1.0.1/src/quick_topic/topic_stat/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      187 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_stat/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1345 2022-03-15 10:38:23.000000 quick-topic-1.0.1/src/quick_topic/topic_stat/__pycache__/stat_by_keyword.cpython-36.pyc
--rw-rw-rw-   0        0        0     1339 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_stat/__pycache__/stat_by_keyword.cpython-39.pyc
--rw-rw-rw-   0        0        0     1712 2022-03-15 10:37:30.000000 quick-topic-1.0.1/src/quick_topic/topic_stat/stat_by_keyword.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.219918 quick-topic-1.0.1/src/quick_topic/topic_transition/
--rw-rw-rw-   0        0        0        0 2022-02-25 15:41:01.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.233566 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/
--rw-rw-rw-   0        0        0      185 2022-02-25 17:28:27.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      193 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1255 2022-03-21 16:52:26.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/divide_by_year.cpython-36.pyc
--rw-rw-rw-   0        0        0     1261 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/divide_by_year.cpython-39.pyc
--rw-rw-rw-   0        0        0     1288 2022-03-05 18:56:11.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/divide_by_year_month.cpython-36.pyc
--rw-rw-rw-   0        0        0     1294 2022-03-22 19:52:44.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/divide_by_year_month.cpython-39.pyc
--rw-rw-rw-   0        0        0     1102 2022-02-25 17:59:19.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year.cpython-36.pyc
--rw-rw-rw-   0        0        0     3707 2022-03-05 19:06:41.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_term.cpython-36.pyc
--rw-rw-rw-   0        0        0     3675 2022-03-22 19:52:43.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_term.cpython-39.pyc
--rw-rw-rw-   0        0        0     2323 2022-02-25 17:46:55.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_topic.cpython-36.pyc
--rw-rw-rw-   0        0        0     3553 2022-03-22 16:04:13.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_term.cpython-36.pyc
--rw-rw-rw-   0        0        0     3541 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_term.cpython-39.pyc
--rw-rw-rw-   0        0        0     2354 2022-03-22 16:04:13.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_topic.cpython-36.pyc
--rw-rw-rw-   0        0        0     2360 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_topic.cpython-39.pyc
--rw-rw-rw-   0        0        0     1627 2022-03-21 16:52:23.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/divide_by_year.py
--rw-rw-rw-   0        0        0     1695 2022-03-05 18:56:11.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/divide_by_year_month.py
--rw-rw-rw-   0        0        0     1077 2022-02-25 17:59:19.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year.py
--rw-rw-rw-   0        0        0     4858 2022-03-05 19:06:41.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year_month_term.py
--rw-rw-rw-   0        0        0     2423 2022-02-25 17:46:55.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year_month_topic.py
--rw-rw-rw-   0        0        0     5024 2022-03-22 15:58:27.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year_term.py
--rw-rw-rw-   0        0        0     2796 2022-03-22 15:58:27.000000 quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year_topic.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.244579 quick-topic-1.0.1/src/quick_topic/topic_trends/
--rw-rw-rw-   0        0        0        0 2022-02-26 08:14:48.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.251082 quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/
--rw-rw-rw-   0        0        0      181 2022-02-26 08:32:50.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      189 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2684 2022-03-15 14:43:18.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/trends_by_year_fulltext.cpython-36.pyc
--rw-rw-rw-   0        0        0     2691 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/trends_by_year_fulltext.cpython-39.pyc
--rw-rw-rw-   0        0        0     2772 2022-02-26 08:46:59.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/trends_by_year_month.cpython-36.pyc
--rw-rw-rw-   0        0        0     4370 2022-03-15 14:02:24.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/trends_by_year_month_fulltext.cpython-36.pyc
--rw-rw-rw-   0        0        0     3925 2022-03-15 14:43:17.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/trends_by_year_fulltext.py
--rw-rw-rw-   0        0        0     3967 2022-02-26 08:46:59.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/trends_by_year_month.py
--rw-rw-rw-   0        0        0     7752 2022-03-15 14:51:06.000000 quick-topic-1.0.1/src/quick_topic/topic_trends/trends_by_year_month_fulltext.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.254090 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/
--rw-rw-rw-   0        0        0        0 2022-02-26 08:56:34.000000 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.258091 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/
--rw-rw-rw-   0        0        0      186 2022-02-26 09:07:19.000000 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      201 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2500 2022-02-26 09:19:43.000000 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_matrix.cpython-36.pyc
--rw-rw-rw-   0        0        0     3212 2022-03-22 16:04:13.000000 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_two.cpython-36.pyc
--rw-rw-rw-   0        0        0     3148 2022-03-22 18:09:44.000000 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_two.cpython-39.pyc
--rw-rw-rw-   0        0        0     3395 2022-03-22 15:58:27.000000 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/topic_trends_correlation_matrix.py
--rw-rw-rw-   0        0        0     4648 2022-03-22 15:58:27.000000 quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/topic_trends_correlation_two.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.269169 quick-topic-1.0.1/src/quick_topic/topic_visualization/
--rw-rw-rw-   0        0        0        0 2022-03-06 08:04:31.000000 quick-topic-1.0.1/src/quick_topic/topic_visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.273168 quick-topic-1.0.1/src/quick_topic/topic_visualization/__pycache__/
--rw-rw-rw-   0        0        0      188 2022-03-06 15:30:11.000000 quick-topic-1.0.1/src/quick_topic/topic_visualization/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      196 2022-03-22 21:41:37.000000 quick-topic-1.0.1/src/quick_topic/topic_visualization/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    22951 2022-03-15 15:13:47.000000 quick-topic-1.0.1/src/quick_topic/topic_visualization/__pycache__/topic_modeling_pipeline.cpython-36.pyc
--rw-rw-rw-   0        0        0    22444 2022-03-28 05:34:40.000000 quick-topic-1.0.1/src/quick_topic/topic_visualization/__pycache__/topic_modeling_pipeline.cpython-39.pyc
--rw-rw-rw-   0        0        0    31014 2022-03-23 04:29:23.000000 quick-topic-1.0.1/src/quick_topic/topic_visualization/topic_modeling_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:11:31.044230 quick-topic-1.0.1/src/quick_topic.egg-info/
--rw-rw-rw-   0        0        0    15169 2023-07-15 13:11:30.000000 quick-topic-1.0.1/src/quick_topic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9742 2023-07-15 13:11:31.000000 quick-topic-1.0.1/src/quick_topic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 13:11:30.000000 quick-topic-1.0.1/src/quick_topic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-15 13:11:30.000000 quick-topic-1.0.1/src/quick_topic.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      174 2023-07-15 13:11:30.000000 quick-topic-1.0.1/src/quick_topic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-15 13:11:30.000000 quick-topic-1.0.1/src/quick_topic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:20.004509 quick-topic-1.0.2/
+-rw-rw-rw-   0        0        0     1106 2023-07-16 00:39:02.000000 quick-topic-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      270 2023-07-16 00:39:02.000000 quick-topic-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    15169 2023-07-16 00:39:20.004509 quick-topic-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14084 2023-07-16 00:39:02.000000 quick-topic-1.0.2/README.md
+-rw-rw-rw-   0        0        0       81 2023-07-16 00:39:20.004509 quick-topic-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     8905 2023-07-16 00:39:02.000000 quick-topic-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.863121 quick-topic-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.863121 quick-topic-1.0.2/src/quick_topic/
+-rw-rw-rw-   0        0        0       25 2022-02-25 13:51:54.000000 quick-topic-1.0.2/src/quick_topic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.894727 quick-topic-1.0.2/src/quick_topic/__pycache__/
+-rw-rw-rw-   0        0        0      196 2022-02-25 14:01:49.000000 quick-topic-1.0.2/src/quick_topic/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      204 2022-03-22 18:01:28.000000 quick-topic-1.0.2/src/quick_topic/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      243 2022-03-22 07:38:41.000000 quick-topic-1.0.2/src/quick_topic/__pycache__/cli.cpython-36.pyc
+-rw-rw-rw-   0        0        0      251 2022-03-22 18:01:28.000000 quick-topic-1.0.2/src/quick_topic/__pycache__/cli.cpython-39.pyc
+-rw-rw-rw-   0        0        0       73 2022-03-21 19:30:28.000000 quick-topic-1.0.2/src/quick_topic/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.910361 quick-topic-1.0.2/src/quick_topic/gui/
+-rw-rw-rw-   0        0        0        0 2022-03-20 16:53:12.000000 quick-topic-1.0.2/src/quick_topic/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.910361 quick-topic-1.0.2/src/quick_topic/gui/__pycache__/
+-rw-rw-rw-   0        0        0      172 2022-03-20 17:07:55.000000 quick-topic-1.0.2/src/quick_topic/gui/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      180 2022-03-22 18:01:28.000000 quick-topic-1.0.2/src/quick_topic/gui/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9051 2022-03-22 07:35:59.000000 quick-topic-1.0.2/src/quick_topic/gui/__pycache__/main.cpython-36.pyc
+-rw-rw-rw-   0        0        0    10762 2022-03-28 08:29:07.000000 quick-topic-1.0.2/src/quick_topic/gui/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0    20582 2022-03-22 07:38:41.000000 quick-topic-1.0.2/src/quick_topic/gui/__pycache__/run.cpython-36.pyc
+-rw-rw-rw-   0        0        0    22465 2022-03-28 05:34:34.000000 quick-topic-1.0.2/src/quick_topic/gui/__pycache__/run.cpython-39.pyc
+-rw-rw-rw-   0        0        0    22421 2022-03-28 08:29:02.000000 quick-topic-1.0.2/src/quick_topic/gui/main.py
+-rw-rw-rw-   0        0        0    26468 2022-03-28 05:36:45.000000 quick-topic-1.0.2/src/quick_topic/gui/main.ui
+-rw-rw-rw-   0        0        0    17701 2022-03-22 19:28:48.000000 quick-topic-1.0.2/src/quick_topic/gui/qtt.png
+-rw-rw-rw-   0        0        0     1163 2022-03-22 21:58:48.000000 quick-topic-1.0.2/src/quick_topic/gui/quick_topic.config
+-rw-rw-rw-   0        0        0    35374 2022-03-23 04:07:14.000000 quick-topic-1.0.2/src/quick_topic/gui/run.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.910361 quick-topic-1.0.2/src/quick_topic/gui_functions/
+-rw-rw-rw-   0        0        0        0 2022-03-20 18:11:14.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.925985 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/
+-rw-rw-rw-   0        0        0      182 2022-03-20 18:26:01.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      190 2022-03-22 18:03:50.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1676 2022-03-21 19:50:20.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_keywordstat.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1690 2022-03-22 20:04:20.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_keywordstat.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1082 2022-03-22 21:41:37.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_explore.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1854 2022-03-21 18:31:43.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_interaction.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1903 2022-03-22 19:11:02.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_interaction.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1198 2022-03-22 02:28:25.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_modeling.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1260 2022-03-22 21:41:37.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_modeling.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1632 2022-03-22 16:04:12.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_prevalence.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1660 2022-03-22 20:04:20.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_prevalence.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1176 2022-03-22 03:20:19.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_similarity.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1206 2022-03-22 20:41:18.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_similarity.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1381 2022-03-22 02:51:00.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_term_year.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1408 2022-03-22 20:04:20.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_term_year.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1748 2022-03-22 16:04:13.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_topic_year.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1769 2022-03-22 20:04:20.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_topic_year.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1130 2022-03-21 15:57:50.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_trends.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1153 2022-03-22 20:04:20.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_trends.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1866 2022-03-22 03:15:47.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_trends_correlation.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1898 2022-03-22 20:04:20.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_trends_correlation.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2206 2022-03-22 20:04:18.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_keywordstat.py
+-rw-rw-rw-   0        0        0     1179 2022-03-22 21:26:37.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_explore.py
+-rw-rw-rw-   0        0        0     2573 2022-03-22 19:05:08.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_interaction.py
+-rw-rw-rw-   0        0        0     1705 2022-03-22 21:11:44.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_modeling.py
+-rw-rw-rw-   0        0        0     2268 2022-03-22 20:04:18.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_prevalence.py
+-rw-rw-rw-   0        0        0     1617 2022-03-22 20:40:48.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_similarity.py
+-rw-rw-rw-   0        0        0     2206 2022-03-22 20:04:18.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_transition_term_year.py
+-rw-rw-rw-   0        0        0     2293 2022-03-22 20:04:18.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_transition_topic_year.py
+-rw-rw-rw-   0        0        0     1402 2022-03-22 20:04:18.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_trends.py
+-rw-rw-rw-   0        0        0     2103 2022-03-22 20:04:18.000000 quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_trends_correlation.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.941611 quick-topic-1.0.2/src/quick_topic/topic_interaction/
+-rw-rw-rw-   0        0        0        0 2022-02-25 15:41:01.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.941611 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/
+-rw-rw-rw-   0        0        0      186 2022-02-25 15:58:13.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      194 2022-03-22 18:03:50.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2253 2022-03-20 04:06:48.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/divide_by_tag.cpython-36.pyc
+-rw-rw-rw-   0        0        0     2271 2022-03-22 20:19:28.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/divide_by_tag.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4049 2022-03-22 16:04:12.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/interaction_among_tag.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3975 2022-03-22 18:09:43.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/interaction_among_tag.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7885 2022-03-22 16:03:56.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/lda_by_tag_each.cpython-36.pyc
+-rw-rw-rw-   0        0        0     7734 2022-03-22 20:19:28.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/lda_by_tag_each.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1533 2022-03-21 18:29:00.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/main.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1553 2022-03-22 18:03:50.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3682 2022-03-22 20:19:01.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/divide_by_tag.py
+-rw-rw-rw-   0        0        0     7170 2022-03-22 15:58:27.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/interaction_among_tag.py
+-rw-rw-rw-   0        0        0     3641 2022-03-22 15:58:27.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/lda_by_tag_all.py
+-rw-rw-rw-   0        0        0    12634 2023-07-16 00:38:35.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/lda_by_tag_each.py
+-rw-rw-rw-   0        0        0     2529 2022-03-21 18:29:00.000000 quick-topic-1.0.2/src/quick_topic/topic_interaction/main.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.941611 quick-topic-1.0.2/src/quick_topic/topic_modeling/
+-rw-rw-rw-   0        0        0        0 2022-02-26 12:47:44.000000 quick-topic-1.0.2/src/quick_topic/topic_modeling/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.941611 quick-topic-1.0.2/src/quick_topic/topic_modeling/__pycache__/
+-rw-rw-rw-   0        0        0      183 2022-02-26 12:59:28.000000 quick-topic-1.0.2/src/quick_topic/topic_modeling/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      191 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_modeling/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5665 2022-03-22 16:04:13.000000 quick-topic-1.0.2/src/quick_topic/topic_modeling/__pycache__/lda.cpython-36.pyc
+-rw-rw-rw-   0        0        0     5713 2022-03-22 20:47:38.000000 quick-topic-1.0.2/src/quick_topic/topic_modeling/__pycache__/lda.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10349 2023-07-16 00:38:35.000000 quick-topic-1.0.2/src/quick_topic/topic_modeling/lda.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.941611 quick-topic-1.0.2/src/quick_topic/topic_prevalence/
+-rw-rw-rw-   0        0        0        0 2022-02-25 13:51:07.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.957238 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/
+-rw-rw-rw-   0        0        0      185 2022-02-25 14:01:49.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      193 2022-03-22 18:09:43.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1208 2022-03-07 13:50:26.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/divide_per_year.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1216 2022-03-22 18:09:43.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/divide_per_year.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5238 2022-03-15 15:24:39.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/lda_per_year.cpython-36.pyc
+-rw-rw-rw-   0        0        0     5234 2022-03-22 18:09:43.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/lda_per_year.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1222 2022-03-21 19:27:44.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/main.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1242 2022-03-22 18:09:43.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2678 2022-03-21 18:59:12.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/trends_per_year.cpython-36.pyc
+-rw-rw-rw-   0        0        0     2619 2022-03-22 18:09:43.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/trends_per_year.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1616 2022-03-07 13:50:26.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/divide_per_year.py
+-rw-rw-rw-   0        0        0     8260 2022-03-15 15:19:14.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/lda_per_year.py
+-rw-rw-rw-   0        0        0     1731 2022-03-21 19:27:41.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/main.py
+-rw-rw-rw-   0        0        0     4023 2022-03-21 18:59:09.000000 quick-topic-1.0.2/src/quick_topic/topic_prevalence/trends_per_year.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.957238 quick-topic-1.0.2/src/quick_topic/topic_similarity/
+-rw-rw-rw-   0        0        0        0 2022-02-26 10:43:06.000000 quick-topic-1.0.2/src/quick_topic/topic_similarity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.957238 quick-topic-1.0.2/src/quick_topic/topic_similarity/__pycache__/
+-rw-rw-rw-   0        0        0      185 2022-02-26 10:57:01.000000 quick-topic-1.0.2/src/quick_topic/topic_similarity/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      193 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_similarity/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3098 2022-03-22 16:04:13.000000 quick-topic-1.0.2/src/quick_topic/topic_similarity/__pycache__/topic_similarity_by_category.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3088 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_similarity/__pycache__/topic_similarity_by_category.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4320 2022-04-09 17:57:15.000000 quick-topic-1.0.2/src/quick_topic/topic_similarity/topic_similarity_by_category.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.957238 quick-topic-1.0.2/src/quick_topic/topic_stat/
+-rw-rw-rw-   0        0        0        0 2022-02-26 11:15:43.000000 quick-topic-1.0.2/src/quick_topic/topic_stat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.972866 quick-topic-1.0.2/src/quick_topic/topic_stat/__pycache__/
+-rw-rw-rw-   0        0        0      179 2022-02-26 12:37:38.000000 quick-topic-1.0.2/src/quick_topic/topic_stat/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      187 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_stat/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1345 2022-03-15 10:38:23.000000 quick-topic-1.0.2/src/quick_topic/topic_stat/__pycache__/stat_by_keyword.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1339 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_stat/__pycache__/stat_by_keyword.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1712 2022-03-15 10:37:30.000000 quick-topic-1.0.2/src/quick_topic/topic_stat/stat_by_keyword.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.972866 quick-topic-1.0.2/src/quick_topic/topic_transition/
+-rw-rw-rw-   0        0        0        0 2022-02-25 15:41:01.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.988489 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/
+-rw-rw-rw-   0        0        0      185 2022-02-25 17:28:27.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      193 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1255 2022-03-21 16:52:26.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/divide_by_year.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1261 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/divide_by_year.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1288 2022-03-05 18:56:11.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/divide_by_year_month.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1294 2022-03-22 19:52:44.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/divide_by_year_month.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1102 2022-02-25 17:59:19.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3707 2022-03-05 19:06:41.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_term.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3675 2022-03-22 19:52:43.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_term.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2323 2022-02-25 17:46:55.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_topic.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3553 2022-03-22 16:04:13.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_term.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3541 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_term.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2354 2022-03-22 16:04:13.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_topic.cpython-36.pyc
+-rw-rw-rw-   0        0        0     2360 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_topic.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1627 2022-03-21 16:52:23.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/divide_by_year.py
+-rw-rw-rw-   0        0        0     1695 2022-03-05 18:56:11.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/divide_by_year_month.py
+-rw-rw-rw-   0        0        0     1077 2022-02-25 17:59:19.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year.py
+-rw-rw-rw-   0        0        0     4858 2022-03-05 19:06:41.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year_month_term.py
+-rw-rw-rw-   0        0        0     2423 2022-02-25 17:46:55.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year_month_topic.py
+-rw-rw-rw-   0        0        0     5024 2022-03-22 15:58:27.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year_term.py
+-rw-rw-rw-   0        0        0     2796 2022-03-22 15:58:27.000000 quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year_topic.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.991500 quick-topic-1.0.2/src/quick_topic/topic_trends/
+-rw-rw-rw-   0        0        0        0 2022-02-26 08:14:48.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.991500 quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/
+-rw-rw-rw-   0        0        0      181 2022-02-26 08:32:50.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      189 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2684 2022-03-15 14:43:18.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/trends_by_year_fulltext.cpython-36.pyc
+-rw-rw-rw-   0        0        0     2691 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/trends_by_year_fulltext.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2772 2022-02-26 08:46:59.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/trends_by_year_month.cpython-36.pyc
+-rw-rw-rw-   0        0        0     4370 2022-03-15 14:02:24.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/trends_by_year_month_fulltext.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3925 2022-03-15 14:43:17.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/trends_by_year_fulltext.py
+-rw-rw-rw-   0        0        0     3967 2022-02-26 08:46:59.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/trends_by_year_month.py
+-rw-rw-rw-   0        0        0     7752 2022-03-15 14:51:06.000000 quick-topic-1.0.2/src/quick_topic/topic_trends/trends_by_year_month_fulltext.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.991500 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/
+-rw-rw-rw-   0        0        0        0 2022-02-26 08:56:34.000000 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.991500 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/
+-rw-rw-rw-   0        0        0      186 2022-02-26 09:07:19.000000 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      201 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2500 2022-02-26 09:19:43.000000 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_matrix.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3212 2022-03-22 16:04:13.000000 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_two.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3148 2022-03-22 18:09:44.000000 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_two.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3395 2022-03-22 15:58:27.000000 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/topic_trends_correlation_matrix.py
+-rw-rw-rw-   0        0        0     4648 2022-03-22 15:58:27.000000 quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/topic_trends_correlation_two.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:20.004509 quick-topic-1.0.2/src/quick_topic/topic_visualization/
+-rw-rw-rw-   0        0        0        0 2022-03-06 08:04:31.000000 quick-topic-1.0.2/src/quick_topic/topic_visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:20.004509 quick-topic-1.0.2/src/quick_topic/topic_visualization/__pycache__/
+-rw-rw-rw-   0        0        0      188 2022-03-06 15:30:11.000000 quick-topic-1.0.2/src/quick_topic/topic_visualization/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      196 2022-03-22 21:41:37.000000 quick-topic-1.0.2/src/quick_topic/topic_visualization/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    22951 2022-03-15 15:13:47.000000 quick-topic-1.0.2/src/quick_topic/topic_visualization/__pycache__/topic_modeling_pipeline.cpython-36.pyc
+-rw-rw-rw-   0        0        0    22444 2022-03-28 05:34:40.000000 quick-topic-1.0.2/src/quick_topic/topic_visualization/__pycache__/topic_modeling_pipeline.cpython-39.pyc
+-rw-rw-rw-   0        0        0    31014 2022-03-23 04:29:23.000000 quick-topic-1.0.2/src/quick_topic/topic_visualization/topic_modeling_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-16 00:39:19.894727 quick-topic-1.0.2/src/quick_topic.egg-info/
+-rw-rw-rw-   0        0        0    15169 2023-07-16 00:39:19.000000 quick-topic-1.0.2/src/quick_topic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9742 2023-07-16 00:39:19.000000 quick-topic-1.0.2/src/quick_topic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 00:39:19.000000 quick-topic-1.0.2/src/quick_topic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-16 00:39:19.000000 quick-topic-1.0.2/src/quick_topic.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      174 2023-07-16 00:39:19.000000 quick-topic-1.0.2/src/quick_topic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 00:39:19.000000 quick-topic-1.0.2/src/quick_topic.egg-info/top_level.txt
```

### Comparing `quick-topic-1.0.1/LICENSE` & `quick-topic-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/PKG-INFO` & `quick-topic-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-topic
-Version: 1.0.1
+Version: 1.0.2
 Summary: A toolkit to quickly analyze topic models using various methods
 Home-page: https://github.com/dhchenx/quick-topic
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-topic/issues
 Project-URL: Source, https://github.com/dhchenx/quick-topic
```

### Comparing `quick-topic-1.0.1/README.md` & `quick-topic-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/setup.py` & `quick-topic-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1',  # Required
+    version='1.0.2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='A toolkit to quickly analyze topic models using various methods',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/__pycache__/main.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui/__pycache__/main.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/__pycache__/main.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/__pycache__/run.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui/__pycache__/run.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/__pycache__/run.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui/__pycache__/run.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/main.py` & `quick-topic-1.0.2/src/quick_topic/gui/main.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/main.ui` & `quick-topic-1.0.2/src/quick_topic/gui/main.ui`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/qtt.png` & `quick-topic-1.0.2/src/quick_topic/gui/qtt.png`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/quick_topic.config` & `quick-topic-1.0.2/src/quick_topic/gui/quick_topic.config`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui/run.py` & `quick-topic-1.0.2/src/quick_topic/gui/run.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_keywordstat.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_keywordstat.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_keywordstat.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_keywordstat.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_explore.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_explore.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_interaction.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_interaction.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_interaction.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_interaction.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_modeling.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_modeling.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_modeling.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_modeling.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_prevalence.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_prevalence.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_prevalence.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_prevalence.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_similarity.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_similarity.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_similarity.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_similarity.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_term_year.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_term_year.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_term_year.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_term_year.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_topic_year.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_topic_year.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_topic_year.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_transition_topic_year.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_trends.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_trends.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_trends.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_trends.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_trends_correlation.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_trends_correlation.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/__pycache__/gui_topic_trends_correlation.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/gui_functions/__pycache__/gui_topic_trends_correlation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_keywordstat.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_keywordstat.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_explore.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_explore.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_interaction.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_interaction.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_modeling.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_modeling.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_prevalence.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_prevalence.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_similarity.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_similarity.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_transition_term_year.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_transition_term_year.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_transition_topic_year.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_transition_topic_year.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_trends.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_trends.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/gui_functions/gui_topic_trends_correlation.py` & `quick-topic-1.0.2/src/quick_topic/gui_functions/gui_topic_trends_correlation.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/divide_by_tag.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/divide_by_tag.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/divide_by_tag.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/divide_by_tag.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/interaction_among_tag.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/interaction_among_tag.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/interaction_among_tag.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/interaction_among_tag.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/lda_by_tag_each.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/lda_by_tag_each.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/lda_by_tag_each.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/lda_by_tag_each.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/main.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/main.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/__pycache__/main.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/divide_by_tag.py` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/divide_by_tag.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/interaction_among_tag.py` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/interaction_among_tag.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/lda_by_tag_all.py` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/lda_by_tag_all.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/lda_by_tag_each.py` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/lda_by_tag_each.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,62 @@
         # stem tokens
         # stemmed_tokens = [p_stemmer.stem(i) for i in tokens]
 
         # add tokens to list
         texts.append(tokens)
     return texts
 
+
+#### revised the quick-topic toolkit
+
+def get_text_chinese_with_selected_words(list_doc, stopwords_path, list_useful_words=None):
+    stopwords = []
+    if os.path.exists(stopwords_path):
+        stopwords = [w.strip() for w in open(stopwords_path, 'r', encoding='utf-8').readlines()
+                     if w.strip() != ""]
+
+    # load data
+    # dict_dataset=pickle.load(open("datasets/weibo_vae_dataset_prepared_with_domain.pickle", "rb"))
+
+    # compile sample documents into a list
+    # doc_set = [doc_a, doc_b, doc_c, doc_d, doc_e]
+
+    doc_set = []
+    for doc in list_doc:
+        # list_words=jieba.cut(doc,cut_all=False)
+        list_words = pseg.cut(doc)
+        list_w = []
+        for w, f in list_words:
+            if f in ['n', 'nr', 'nr1', 'nr2', 'nrj', 'nrf', 'nsf', 'ns', 'nt', 'nz', 'nl', 'ng', 'v', 'vn', 'vd', 'nd',
+                     'nh', 'nl', 'i', 'x', 'a', 'ad']:
+                if w not in stopwords and len(w) != 1:
+                    if list_useful_words != None:
+                        if w in list_useful_words:
+                            list_w.append(w)
+                    else:
+                        list_w.append(w)
+
+        # print(list_w)
+        doc_set.append(list_w)
+
+    # list for tokenized documents in loop
+    texts = []
+
+    # loop through document list
+    for tokens in doc_set:
+        # clean and tokenize document string
+
+        # stem tokens
+        # stemmed_tokens = [p_stemmer.stem(i) for i in tokens]
+
+        # add tokens to list
+        texts.append(tokens)
+    return texts
+
+
 def LDA(field,list_doc,weights_path,list_keywods_path,stopwords_path,num_topics=6,num_words=50,num_pass=5,lang='zh',use_bigram=False,iteration=100,random_state=100,chunk_size=10):
 
     # ============ begin configure ====================
     NUM_TOPICS = num_topics
     NUM_WORDS = num_words
     FIG_V_NUM = 2
     FIG_H_NUM = 3
```

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_interaction/main.py` & `quick-topic-1.0.2/src/quick_topic/topic_interaction/main.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_modeling/__pycache__/lda.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_modeling/__pycache__/lda.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_modeling/__pycache__/lda.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_modeling/__pycache__/lda.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_modeling/lda.py` & `quick-topic-1.0.2/src/quick_topic/topic_modeling/lda.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,19 @@
     # compile sample documents into a list
     # doc_set = [doc_a, doc_b, doc_c, doc_d, doc_e]
 
     texts = None
     if lang == 'zh':
         for pp in list_term_file:
             jieba.load_userdict(pp)
-        texts = get_text_chinese(list_doc, stopwords_path=stopwords_path,list_useful_words=list_useful_words)
+        if list_useful_words!=None:
+            print("Using My Own Dictionary...")
+            texts=get_text_chinese_with_selected_words(list_doc, stopwords_path=stopwords_path,list_useful_words=list_useful_words)
+        else:
+            texts = get_text_chinese_with_selected_words(list_doc, stopwords_path=stopwords_path)
     else:
         texts = get_text_english(list_doc)
 
     # turn our tokenized documents into a id <-> term dictionary
     dictionary = corpora.Dictionary(texts)
 
     # convert tokenized documents into a document-term matrix
```

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/divide_per_year.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/divide_per_year.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/divide_per_year.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/divide_per_year.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/lda_per_year.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/lda_per_year.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/lda_per_year.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/lda_per_year.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/main.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/main.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/main.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/trends_per_year.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/trends_per_year.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/__pycache__/trends_per_year.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/__pycache__/trends_per_year.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/divide_per_year.py` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/divide_per_year.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/lda_per_year.py` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/lda_per_year.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/main.py` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/main.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_prevalence/trends_per_year.py` & `quick-topic-1.0.2/src/quick_topic/topic_prevalence/trends_per_year.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_similarity/__pycache__/topic_similarity_by_category.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_similarity/__pycache__/topic_similarity_by_category.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_similarity/__pycache__/topic_similarity_by_category.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_similarity/__pycache__/topic_similarity_by_category.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_similarity/topic_similarity_by_category.py` & `quick-topic-1.0.2/src/quick_topic/topic_similarity/topic_similarity_by_category.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_stat/__pycache__/stat_by_keyword.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_stat/__pycache__/stat_by_keyword.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_stat/__pycache__/stat_by_keyword.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_stat/__pycache__/stat_by_keyword.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_stat/stat_by_keyword.py` & `quick-topic-1.0.2/src/quick_topic/topic_stat/stat_by_keyword.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/divide_by_year.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/divide_by_year.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/divide_by_year.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/divide_by_year.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/divide_by_year_month.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/divide_by_year_month.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/divide_by_year_month.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/divide_by_year_month.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_term.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_term.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_term.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_term.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_topic.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_month_topic.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_term.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_term.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_term.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_term.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_topic.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_topic.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/__pycache__/transition_by_year_topic.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_transition/__pycache__/transition_by_year_topic.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/divide_by_year.py` & `quick-topic-1.0.2/src/quick_topic/topic_transition/divide_by_year.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/divide_by_year_month.py` & `quick-topic-1.0.2/src/quick_topic/topic_transition/divide_by_year_month.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year.py` & `quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year_month_term.py` & `quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year_month_term.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year_month_topic.py` & `quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year_month_topic.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year_term.py` & `quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year_term.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_transition/transition_by_year_topic.py` & `quick-topic-1.0.2/src/quick_topic/topic_transition/transition_by_year_topic.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/trends_by_year_fulltext.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/trends_by_year_fulltext.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/trends_by_year_fulltext.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/trends_by_year_fulltext.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/trends_by_year_month.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/trends_by_year_month.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends/__pycache__/trends_by_year_month_fulltext.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_trends/__pycache__/trends_by_year_month_fulltext.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends/trends_by_year_fulltext.py` & `quick-topic-1.0.2/src/quick_topic/topic_trends/trends_by_year_fulltext.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends/trends_by_year_month.py` & `quick-topic-1.0.2/src/quick_topic/topic_trends/trends_by_year_month.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends/trends_by_year_month_fulltext.py` & `quick-topic-1.0.2/src/quick_topic/topic_trends/trends_by_year_month_fulltext.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_matrix.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_matrix.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_two.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_two.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_two.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/__pycache__/topic_trends_correlation_two.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/topic_trends_correlation_matrix.py` & `quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/topic_trends_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_trends_correlation/topic_trends_correlation_two.py` & `quick-topic-1.0.2/src/quick_topic/topic_trends_correlation/topic_trends_correlation_two.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_visualization/__pycache__/topic_modeling_pipeline.cpython-36.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_visualization/__pycache__/topic_modeling_pipeline.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_visualization/__pycache__/topic_modeling_pipeline.cpython-39.pyc` & `quick-topic-1.0.2/src/quick_topic/topic_visualization/__pycache__/topic_modeling_pipeline.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic/topic_visualization/topic_modeling_pipeline.py` & `quick-topic-1.0.2/src/quick_topic/topic_visualization/topic_modeling_pipeline.py`

 * *Files identical despite different names*

### Comparing `quick-topic-1.0.1/src/quick_topic.egg-info/PKG-INFO` & `quick-topic-1.0.2/src/quick_topic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quick-topic
-Version: 1.0.1
+Version: 1.0.2
 Summary: A toolkit to quickly analyze topic models using various methods
 Home-page: https://github.com/dhchenx/quick-topic
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/quick-topic/issues
 Project-URL: Source, https://github.com/dhchenx/quick-topic
```

### Comparing `quick-topic-1.0.1/src/quick_topic.egg-info/SOURCES.txt` & `quick-topic-1.0.2/src/quick_topic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

