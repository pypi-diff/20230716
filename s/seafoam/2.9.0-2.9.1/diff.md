# Comparing `tmp/seafoam-2.9.0.tar.gz` & `tmp/seafoam-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seafoam-2.9.0.tar", last modified: Fri Jul 14 18:15:21 2023, max compression
+gzip compressed data, was "seafoam-2.9.1.tar", last modified: Sun Jul 16 04:35:32 2023, max compression
```

## Comparing `seafoam-2.9.0.tar` & `seafoam-2.9.1.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.965345 seafoam-2.9.0/
--rw-rw-rw-   0        0        0     1133 2023-07-11 04:35:00.000000 seafoam-2.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0      180 2023-07-11 04:35:00.000000 seafoam-2.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0    30907 2023-07-14 18:15:21.965345 seafoam-2.9.0/PKG-INFO
--rw-rw-rw-   0        0        0    29488 2023-07-14 18:03:53.000000 seafoam-2.9.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.087271 seafoam-2.9.0/docs/
--rw-rw-rw-   0        0        0    10154 2023-07-14 18:13:02.000000 seafoam-2.9.0/docs/CHANGELOG.rst
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.076732 seafoam-2.9.0/pelican/
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.076732 seafoam-2.9.0/pelican/plugins/
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.087271 seafoam-2.9.0/pelican/plugins/seafoam/
--rw-rw-rw-   0        0        0      829 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-14 18:15:10.000000 seafoam-2.9.0/pelican/plugins/seafoam/constants.py
--rw-rw-rw-   0        0        0     1005 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/formatting.py
--rw-rw-rw-   0        0        0     7606 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/initialize.py
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.076732 seafoam-2.9.0/pelican/plugins/seafoam/static/
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.107939 seafoam-2.9.0/pelican/plugins/seafoam/static/css/
--rw-rw-rw-   0        0        0   236433 2023-07-12 04:11:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css
--rw-rw-rw-   0        0        0   236036 2023-07-12 04:11:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.169936 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/
--rw-rw-rw-   0        0        0   134808 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/FontAwesome.otf
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.295853 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/
--rw-rw-rw-   0        0        0     2104 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt
--rw-rw-rw-   0        0        0     4460 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt
--rw-rw-rw-   0        0        0    18413 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot
--rw-rw-rw-   0        0        0    50449 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg
--rw-rw-rw-   0        0        0    35472 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf
--rw-rw-rw-   0        0        0    19444 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff
--rw-rw-rw-   0        0        0    15168 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2
--rw-rw-rw-   0        0        0    19294 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot
--rw-rw-rw-   0        0        0    56250 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg
--rw-rw-rw-   0        0        0    35176 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf
--rw-rw-rw-   0        0        0    20280 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff
--rw-rw-rw-   0        0        0    15856 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2
--rw-rw-rw-   0        0        0    19408 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot
--rw-rw-rw-   0        0        0    56028 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg
--rw-rw-rw-   0        0        0    35356 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf
--rw-rw-rw-   0        0        0    20416 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff
--rw-rw-rw-   0        0        0    16020 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2
--rw-rw-rw-   0        0        0    18842 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot
--rw-rw-rw-   0        0        0    50436 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg
--rw-rw-rw-   0        0        0    35700 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf
--rw-rw-rw-   0        0        0    19916 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff
--rw-rw-rw-   0        0        0    15476 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.420648 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/
--rw-rw-rw-   0        0        0    24884 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot
--rw-rw-rw-   0        0        0   128830 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg
--rw-rw-rw-   0        0        0    49124 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf
--rw-rw-rw-   0        0        0    25788 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff
--rw-rw-rw-   0        0        0    21932 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2
--rw-rw-rw-   0        0        0    25468 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot
--rw-rw-rw-   0        0        0   128299 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg
--rw-rw-rw-   0        0        0    47480 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf
--rw-rw-rw-   0        0        0    26508 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff
--rw-rw-rw-   0        0        0    22480 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2
--rw-rw-rw-   0        0        0    23567 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot
--rw-rw-rw-   0        0        0   127687 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg
--rw-rw-rw-   0        0        0    47032 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf
--rw-rw-rw-   0        0        0    24808 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff
--rw-rw-rw-   0        0        0    21020 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2
--rw-rw-rw-   0        0        0    23239 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot
--rw-rw-rw-   0        0        0   128551 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg
--rw-rw-rw-   0        0        0    48900 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf
--rw-rw-rw-   0        0        0    24304 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff
--rw-rw-rw-   0        0        0    20512 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.451440 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/
--rw-rw-rw-   0        0        0     4499 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt
--rw-rw-rw-   0        0        0    11207 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot
--rw-rw-rw-   0        0        0    60057 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg
--rw-rw-rw-   0        0        0    18564 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf
--rw-rw-rw-   0        0        0    13008 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff
--rw-rw-rw-   0        0        0    10084 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2
--rw-rw-rw-   0        0        0   165742 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2
--rw-rw-rw-   0        0        0    20127 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0        0        0   109025 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0        0        0    45404 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0        0        0    23424 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0        0        0    18028 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.482697 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/
--rw-rw-rw-   0        0        0    30028 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot
--rw-rw-rw-   0        0        0    81305 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg
--rw-rw-rw-   0        0        0    78804 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf
--rw-rw-rw-   0        0        0    36788 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff
--rw-rw-rw-   0        0        0    30116 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.597449 seafoam-2.9.0/pelican/plugins/seafoam/static/js/
--rw-rw-rw-   0        0        0    72084 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/bootstrap.js
--rw-rw-rw-   0        0        0    37051 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     2512 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/comments.js
--rw-rw-rw-   0        0        0     1520 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/github.js
--rw-rw-rw-   0        0        0     2558 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/jXHR.js
--rw-rw-rw-   0        0        0    86713 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/jquery.min.js
--rw-rw-rw-   0        0        0     4381 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/js/respond.min.js
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.649899 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.660435 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/img/
--rw-rw-rw-   0        0        0      368 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/img/search.png
--rw-rw-rw-   0        0        0     5734 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
--rw-rw-rw-   0        0        0    33779 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
--rw-rw-rw-   0        0        0    10697 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
--rw-rw-rw-   0        0        0     4537 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
--rw-rw-rw-   0        0        0     3670 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.744268 seafoam-2.9.0/pelican/plugins/seafoam/templates/
--rw-rw-rw-   0        0        0     1110 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/404.html
--rw-rw-rw-   0        0        0     5875 2023-07-12 01:08:09.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/archives.html
--rw-rw-rw-   0        0        0     4657 2023-07-13 02:13:40.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/article.html
--rw-rw-rw-   0        0        0     1551 2023-07-12 03:05:35.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/article_list.html
--rw-rw-rw-   0        0        0      761 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/author.html
--rw-rw-rw-   0        0        0      857 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/authors.html
--rw-rw-rw-   0        0        0    15825 2023-07-13 02:15:55.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/base.html
--rw-rw-rw-   0        0        0     2053 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/categories.html
--rw-rw-rw-   0        0        0      738 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/category.html
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.923061 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/
--rw-rw-rw-   0        0        0      196 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/aboutme.html
--rw-rw-rw-   0        0        0      618 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/addthis.html
--rw-rw-rw-   0        0        0     1481 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/article_info.html
--rw-rw-rw-   0        0        0     3389 2023-07-12 04:29:59.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/article_listing.html
--rw-rw-rw-   0        0        0      978 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/assets-css.html
--rw-rw-rw-   0        0        0      219 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/assets-js.html
--rw-rw-rw-   0        0        0     4405 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/cc-license.html
--rw-rw-rw-   0        0        0      553 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comment_count.html
--rw-rw-rw-   0        0        0     1291 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comments-js.html
--rw-rw-rw-   0        0        0     5874 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comments.html
--rw-rw-rw-   0        0        0      741 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/disqus_script.html
--rw-rw-rw-   0        0        0     3869 2023-07-12 00:31:05.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/footer.html
--rw-rw-rw-   0        0        0     1818 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/ga.html
--rw-rw-rw-   0        0        0     1308 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/github-js.html
--rw-rw-rw-   0        0        0      442 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/github.html
--rw-rw-rw-   0        0        0      434 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/links.html
--rw-rw-rw-   0        0        0     1991 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/neighbors.html
--rw-rw-rw-   0        0        0     2955 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/pagination.html
--rw-rw-rw-   0        0        0      872 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/piwik.html
--rw-rw-rw-   0        0        0      486 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/prjct.html
--rw-rw-rw-   0        0        0      357 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/related-posts.html
--rw-rw-rw-   0        0        0     3520 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/sidebar.html
--rw-rw-rw-   0        0        0      276 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/taglist.html
--rw-rw-rw-   0        0        0      296 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/translations.html
--rw-rw-rw-   0        0        0      703 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/twitter_timeline.html
--rw-rw-rw-   0        0        0      796 2023-07-12 03:06:56.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/index.html
--rw-rw-rw-   0        0        0     2474 2023-07-13 02:04:28.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/page.html
--rw-rw-rw-   0        0        0     7104 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/period_archives.html
--rw-rw-rw-   0        0        0     4517 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/prjct.html
--rw-rw-rw-   0        0        0     1507 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/search.html
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.933608 seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/
--rw-rw-rw-   0        0        0     8939 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html
--rw-rw-rw-   0        0        0     5443 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/pricing.html
--rw-rw-rw-   0        0        0      795 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/tag.html
--rw-rw-rw-   0        0        0     2036 2023-07-11 04:35:00.000000 seafoam-2.9.0/pelican/plugins/seafoam/templates/tags.html
--rw-rw-rw-   0        0        0      429 2023-07-11 04:35:00.000000 seafoam-2.9.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-14 18:15:21.965345 seafoam-2.9.0/seafoam.egg-info/
--rw-rw-rw-   0        0        0    30907 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8286 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-14 18:15:20.000000 seafoam-2.9.0/seafoam.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-07-14 18:15:21.965345 seafoam-2.9.0/setup.cfg
--rw-rw-rw-   0        0        0     4767 2023-07-11 04:35:00.000000 seafoam-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.959628 seafoam-2.9.1/
+-rw-rw-rw-   0        0        0     1133 2023-07-11 04:35:00.000000 seafoam-2.9.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      180 2023-07-11 04:35:00.000000 seafoam-2.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    30907 2023-07-16 04:35:32.959628 seafoam-2.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0    29488 2023-07-14 18:03:53.000000 seafoam-2.9.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.773487 seafoam-2.9.1/docs/
+-rw-rw-rw-   0        0        0    10252 2023-07-16 04:32:30.000000 seafoam-2.9.1/docs/CHANGELOG.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.762817 seafoam-2.9.1/pelican/
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.762817 seafoam-2.9.1/pelican/plugins/
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.773487 seafoam-2.9.1/pelican/plugins/seafoam/
+-rw-rw-rw-   0        0        0      829 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/__init__.py
+-rw-rw-rw-   0        0        0      504 2023-07-16 04:35:10.000000 seafoam-2.9.1/pelican/plugins/seafoam/constants.py
+-rw-rw-rw-   0        0        0     1005 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/formatting.py
+-rw-rw-rw-   0        0        0     7606 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/initialize.py
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.763332 seafoam-2.9.1/pelican/plugins/seafoam/static/
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.773487 seafoam-2.9.1/pelican/plugins/seafoam/static/css/
+-rw-rw-rw-   0        0        0   236433 2023-07-12 04:11:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css
+-rw-rw-rw-   0        0        0   236036 2023-07-12 04:11:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.784029 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/FontAwesome.otf
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.804750 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/
+-rw-rw-rw-   0        0        0     2104 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt
+-rw-rw-rw-   0        0        0     4460 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt
+-rw-rw-rw-   0        0        0    18413 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot
+-rw-rw-rw-   0        0        0    50449 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg
+-rw-rw-rw-   0        0        0    35472 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf
+-rw-rw-rw-   0        0        0    19444 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff
+-rw-rw-rw-   0        0        0    15168 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2
+-rw-rw-rw-   0        0        0    19294 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot
+-rw-rw-rw-   0        0        0    56250 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg
+-rw-rw-rw-   0        0        0    35176 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf
+-rw-rw-rw-   0        0        0    20280 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff
+-rw-rw-rw-   0        0        0    15856 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2
+-rw-rw-rw-   0        0        0    19408 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot
+-rw-rw-rw-   0        0        0    56028 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg
+-rw-rw-rw-   0        0        0    35356 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf
+-rw-rw-rw-   0        0        0    20416 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff
+-rw-rw-rw-   0        0        0    16020 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2
+-rw-rw-rw-   0        0        0    18842 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot
+-rw-rw-rw-   0        0        0    50436 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg
+-rw-rw-rw-   0        0        0    35700 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf
+-rw-rw-rw-   0        0        0    19916 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff
+-rw-rw-rw-   0        0        0    15476 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.816342 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/
+-rw-rw-rw-   0        0        0    24884 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot
+-rw-rw-rw-   0        0        0   128830 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg
+-rw-rw-rw-   0        0        0    49124 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf
+-rw-rw-rw-   0        0        0    25788 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff
+-rw-rw-rw-   0        0        0    21932 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2
+-rw-rw-rw-   0        0        0    25468 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot
+-rw-rw-rw-   0        0        0   128299 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg
+-rw-rw-rw-   0        0        0    47480 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf
+-rw-rw-rw-   0        0        0    26508 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff
+-rw-rw-rw-   0        0        0    22480 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2
+-rw-rw-rw-   0        0        0    23567 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot
+-rw-rw-rw-   0        0        0   127687 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg
+-rw-rw-rw-   0        0        0    47032 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf
+-rw-rw-rw-   0        0        0    24808 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff
+-rw-rw-rw-   0        0        0    21020 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2
+-rw-rw-rw-   0        0        0    23239 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot
+-rw-rw-rw-   0        0        0   128551 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg
+-rw-rw-rw-   0        0        0    48900 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf
+-rw-rw-rw-   0        0        0    24304 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff
+-rw-rw-rw-   0        0        0    20512 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.816342 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/
+-rw-rw-rw-   0        0        0     4499 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt
+-rw-rw-rw-   0        0        0    11207 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot
+-rw-rw-rw-   0        0        0    60057 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg
+-rw-rw-rw-   0        0        0    18564 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf
+-rw-rw-rw-   0        0        0    13008 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff
+-rw-rw-rw-   0        0        0    10084 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2
+-rw-rw-rw-   0        0        0   165742 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2
+-rw-rw-rw-   0        0        0    20127 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0        0        0   109025 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0        0        0    45404 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0        0        0    23424 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0        0        0    18028 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.825416 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/
+-rw-rw-rw-   0        0        0    30028 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot
+-rw-rw-rw-   0        0        0    81305 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg
+-rw-rw-rw-   0        0        0    78804 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf
+-rw-rw-rw-   0        0        0    36788 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff
+-rw-rw-rw-   0        0        0    30116 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.846005 seafoam-2.9.1/pelican/plugins/seafoam/static/js/
+-rw-rw-rw-   0        0        0    72084 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/bootstrap.js
+-rw-rw-rw-   0        0        0    37051 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     2512 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/comments.js
+-rw-rw-rw-   0        0        0     1520 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/github.js
+-rw-rw-rw-   0        0        0     2558 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/jXHR.js
+-rw-rw-rw-   0        0        0    86713 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/jquery.min.js
+-rw-rw-rw-   0        0        0     4381 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/js/respond.min.js
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.866708 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.866708 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/img/
+-rw-rw-rw-   0        0        0      368 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/img/search.png
+-rw-rw-rw-   0        0        0     5901 2023-07-16 04:29:02.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css
+-rw-rw-rw-   0        0        0    33641 2023-07-16 04:29:52.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js
+-rw-rw-rw-   0        0        0    10697 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js
+-rw-rw-rw-   0        0        0     4537 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js
+-rw-rw-rw-   0        0        0     3670 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.876870 seafoam-2.9.1/pelican/plugins/seafoam/templates/
+-rw-rw-rw-   0        0        0     1110 2023-07-16 04:24:25.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/404.html
+-rw-rw-rw-   0        0        0     5875 2023-07-12 01:08:09.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/archives.html
+-rw-rw-rw-   0        0        0     4860 2023-07-16 04:17:25.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/article.html
+-rw-rw-rw-   0        0        0     1551 2023-07-12 03:05:35.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/article_list.html
+-rw-rw-rw-   0        0        0      761 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/author.html
+-rw-rw-rw-   0        0        0      857 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/authors.html
+-rw-rw-rw-   0        0        0    15825 2023-07-13 02:15:55.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/base.html
+-rw-rw-rw-   0        0        0     2053 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/categories.html
+-rw-rw-rw-   0        0        0      738 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/category.html
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.938896 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/
+-rw-rw-rw-   0        0        0      196 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/aboutme.html
+-rw-rw-rw-   0        0        0      618 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/addthis.html
+-rw-rw-rw-   0        0        0     1711 2023-07-16 03:57:48.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/article_info.html
+-rw-rw-rw-   0        0        0     3389 2023-07-12 04:29:59.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/article_listing.html
+-rw-rw-rw-   0        0        0      996 2023-07-16 04:30:06.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/assets-css.html
+-rw-rw-rw-   0        0        0      219 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/assets-js.html
+-rw-rw-rw-   0        0        0     4405 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/cc-license.html
+-rw-rw-rw-   0        0        0      559 2023-07-16 04:30:14.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comment_count.html
+-rw-rw-rw-   0        0        0     1640 2023-07-16 04:30:31.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comments-js.html
+-rw-rw-rw-   0        0        0     7976 2023-07-16 04:30:55.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comments.html
+-rw-rw-rw-   0        0        0      741 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/disqus_script.html
+-rw-rw-rw-   0        0        0     3869 2023-07-12 00:31:05.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/footer.html
+-rw-rw-rw-   0        0        0     1818 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/ga.html
+-rw-rw-rw-   0        0        0     1308 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/github-js.html
+-rw-rw-rw-   0        0        0      442 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/github.html
+-rw-rw-rw-   0        0        0      434 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/links.html
+-rw-rw-rw-   0        0        0     3418 2023-07-16 04:19:58.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/neighbors.html
+-rw-rw-rw-   0        0        0     2955 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/pagination.html
+-rw-rw-rw-   0        0        0      872 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/piwik.html
+-rw-rw-rw-   0        0        0      564 2023-07-16 04:30:40.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/prjct.html
+-rw-rw-rw-   0        0        0      357 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/related-posts.html
+-rw-rw-rw-   0        0        0     3533 2023-07-16 04:22:30.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/sidebar.html
+-rw-rw-rw-   0        0        0      319 2023-07-16 04:22:45.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/taglist.html
+-rw-rw-rw-   0        0        0      329 2023-07-16 04:30:47.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/translations.html
+-rw-rw-rw-   0        0        0      703 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/twitter_timeline.html
+-rw-rw-rw-   0        0        0      796 2023-07-12 03:06:56.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/index.html
+-rw-rw-rw-   0        0        0     2474 2023-07-13 02:04:28.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/page.html
+-rw-rw-rw-   0        0        0     7104 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/period_archives.html
+-rw-rw-rw-   0        0        0     4517 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/prjct.html
+-rw-rw-rw-   0        0        0     1507 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/search.html
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.938896 seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/
+-rw-rw-rw-   0        0        0     8939 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html
+-rw-rw-rw-   0        0        0     5443 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/pricing.html
+-rw-rw-rw-   0        0        0      795 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/tag.html
+-rw-rw-rw-   0        0        0     2036 2023-07-11 04:35:00.000000 seafoam-2.9.1/pelican/plugins/seafoam/templates/tags.html
+-rw-rw-rw-   0        0        0      429 2023-07-11 04:35:00.000000 seafoam-2.9.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-16 04:35:32.959628 seafoam-2.9.1/seafoam.egg-info/
+-rw-rw-rw-   0        0        0    30907 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8286 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2023-07-16 04:35:32.000000 seafoam-2.9.1/seafoam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-16 04:35:32.959628 seafoam-2.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     4767 2023-07-11 04:35:00.000000 seafoam-2.9.1/setup.py
```

### Comparing `seafoam-2.9.0/LICENSE.txt` & `seafoam-2.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/PKG-INFO` & `seafoam-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seafoam
-Version: 2.9.0
+Version: 2.9.1
 Summary: Pelican theme, first used for Minchin.ca.
 Home-page: http://blog.minchin.ca/label/seafoam/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/seafoam/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/seafoam/blob/master/docs/changelog.rst
```

### Comparing `seafoam-2.9.0/README.rst` & `seafoam-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/docs/CHANGELOG.rst` & `seafoam-2.9.1/docs/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Changelog
 =========
 
 .. Added, Changed, Depreciated, Removed, Fixed, Security
 
+- :support:`- minor` convert indentation to spaces
+- :bug:`-` better display of micropost links
 - :release:`2.9.0 <2023-07-14>`
 - :feature:`-` add support for *microblogging*, through my `microblogging
   plugin <https://blog.minchin.ca/label/microblogging-pelican/>`_.
   c.f. `blog.minchin.ca Issue #105
   <https://github.com/MinchinWeb/blog.minchin.ca/issues/105>`_.
 - :bug:`- major` no longer capitalize category names, when displayed on
   sidebar. This is part of the changes to support microblogging.
```

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/__init__.py` & `seafoam-2.9.1/pelican/plugins/seafoam/__init__.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/formatting.py` & `seafoam-2.9.1/pelican/plugins/seafoam/formatting.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/initialize.py` & `seafoam-2.9.1/pelican/plugins/seafoam/initialize.py`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css` & `seafoam-2.9.1/pelican/plugins/seafoam/static/css/bootstrap.seafoam.min.css`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css` & `seafoam-2.9.1/pelican/plugins/seafoam/static/css/bootstrap.strathcona.min.css`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/FontAwesome.otf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/FONTLOG.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/OFL.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/cabin/cabin-v26-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/eb-garamond/eb-garamond-v26-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/OFL.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/expletus-sans/expletus-sans-v24-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2` & `seafoam-2.9.1/pelican/plugins/seafoam/static/fonts/vidaloka/vidaloka-v18-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/js/bootstrap.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/js/bootstrap.min.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/js/comments.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/js/comments.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/js/github.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/js/github.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/js/jXHR.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/js/jXHR.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/js/jquery.min.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/js/respond.min.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css` & `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.css`

 * *Files 11% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 #tipue_search_input
 {
      float: left;
      font: 15px 'Open Sans', sans-serif;
      color: #333;     
      -webkit-font-smoothing: antialiased;
-	-moz-osx-font-smoothing: grayscale;
+     -moz-osx-font-smoothing: grayscale;
      width: 230px;
      background-color: #f3f3f3;
      border: none;
      padding: 9px 0 10px 18px;
      height: 56px;
      border-radius: 3px;
-	-moz-appearance: none;
-	-webkit-appearance: none;
-	box-sizing: border-box;
+     -moz-appearance: none;
+     -webkit-appearance: none;
+     box-sizing: border-box;
      box-shadow: none;
-	outline: 0;
-	margin: 0;
+     outline: 0;
+     margin: 0;
 }
 #tipue_search_input:-webkit-autofill,
 #tipue_search_input:-webkit-autofill:hover, 
 #tipue_search_input:-webkit-autofill:focus
 {
      -webkit-box-shadow: 0 0 0px 1000px #f3f3f3 inset;
 }
@@ -47,30 +47,30 @@
      margin-left: -3px;
      background-color: #f3f3f3;
      border: none;
      border-top-right-radius: 3px;
      border-bottom-right-radius: 3px;
      box-sizing: border-box;
      cursor: pointer;
-	outline: 0;
+     outline: 0;
 }
 .tipue_search_icon
 {
      float: left;
      font: 24px/1 'Open Sans', sans-serif;
      -webkit-font-smoothing: antialiased;
-	-moz-osx-font-smoothing: grayscale;
+     -moz-osx-font-smoothing: grayscale;
      color: #333;
      transform: rotate(-45deg);
-	-moz-appearance: none;
-	-webkit-appearance: none;
-	box-sizing: border-box;
+     -moz-appearance: none;
+     -webkit-appearance: none;
+     box-sizing: border-box;
      box-shadow: none;
-	outline: 0;	
-	margin: -1px 0 0 16px;
+     outline: 0;
+     margin: -1px 0 0 16px;
 }
 .tipue_search_group:after
 {
      content: "";
      display: table;
      clear: both;
 }
@@ -78,20 +78,20 @@
 
 /* search results */
 
 
 #tipue_search_content
 {
      max-width: 100%;
-	margin: 0;
+     margin: 0;
 }
 .tipue_search_content_title
 {
      font: 300 32px/1.4 Merriweather, serif;
-	color: #111;
+     color: #111;
 }
 .tipue_search_content_title a
 {
      color: #111;
      text-decoration: none;
 }
 .tipue_search_content_title a:hover
@@ -101,18 +101,18 @@
 .tipue_search_result
 {
      padding-top: 27px;
 }
 #tipue_search_results_count, .tipue_search_content_debug
 {
      font: 13px/1.5 'Source Code Pro', monospace;
-	text-transform: uppercase;
-	color: #999;
+     text-transform: uppercase;
+     color: #999;
      -webkit-font-smoothing: antialiased;
-	-moz-osx-font-smoothing: grayscale;
+     -moz-osx-font-smoothing: grayscale;
 }
 #tipue_search_results_count
 {
      padding-top: 9px;
 }
 .tipue_search_content_url, .tipue_search_note, .tipue_search_related, #tipue_search_error, #tipue_search_replace
 {
@@ -139,15 +139,15 @@
 {
      color: #333;
      margin-top: 17px;
 }
 .tipue_search_content_text
 {
      font: 300 18px/1.6 Merriweather, serif;
-	color: #333;
+     color: #333;
      word-wrap: break-word;
      hyphens: auto;
      margin-top: 9px;
 }
 .tipue_search_content_bold
 {
      font-weight: 400;
@@ -177,18 +177,18 @@
 .tipue_search_img:hover
 {
      opacity: 0.9;
 }
 #tipue_search_zoom_text
 {
      font: 12px/1.7 'Source Code Pro', monospace;
-	color: #ccc;
-	text-transform: uppercase;
-	letter-spacing: 1px;
-	padding-top: 9px;
+     color: #ccc;
+     text-transform: uppercase;
+     letter-spacing: 1px;
+     padding-top: 9px;
 }
 #tipue_search_zoom_text a
 {
      color: #ccc;
      text-decoration: none;
      border-bottom: 2px solid #f7f7f7;
 }
@@ -214,15 +214,15 @@
 }
 .tipue_search_image_close
 {
      position: absolute;
      top: 0;
      right: 0;
      font: 22px/1 'Source Code Pro', monospace;
-	color: #ccc;
+     color: #ccc;
      padding: 25px 30px;
      cursor: pointer;
 }
 .tipue_search_image_block
 {
      margin: 0 auto;
      max-width: 900px;
@@ -248,46 +248,46 @@
 #tipue_search_foot
 {
      margin: 51px 0 21px 0;
 }
 #tipue_search_foot_boxes
 {
      font: 14px 'Source Code Pro', sans-serif;
-	text-transform: uppercase;
-	color: #333;
-	padding: 0;
-	margin: 0;
-	cursor: pointer;
+     text-transform: uppercase;
+     color: #333;
+     padding: 0;
+     margin: 0;
+     cursor: pointer;
 }
 #tipue_search_foot_boxes li
 {
      display: inline;
-	list-style: none;
-	margin: 0;
-	padding: 0;
+     list-style: none;
+     margin: 0;
+     padding: 0;
 }
 #tipue_search_foot_boxes li a
 {
      background-color: #f7f7f7;
-	color: #666;
-	padding: 10px 17px 11px 17px;
+     color: #666;
+     padding: 10px 17px 11px 17px;
      border-radius: 3px;
-	margin-right: 7px;
-	text-decoration: none;
-	text-align: center;
-	transition: 0.3s;
+     margin-right: 7px;
+     text-decoration: none;
+     text-align: center;
+     transition: 0.3s;
 }
 #tipue_search_foot_boxes li.current
 {
      background: #252525;
-	color: #ccc;
-	padding: 10px 17px 11px 17px;
+     color: #ccc;
+     padding: 10px 17px 11px 17px;
      border-radius: 3px;
-	margin-right: 7px;
-	text-align: center;
+     margin-right: 7px;
+     text-align: center;
 }
 #tipue_search_foot_boxes li a:hover
 {
      background: #252525;
      color: #ccc;
 }
```

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -1517,596 +1517,587 @@
 00005ec0: 2020 7420 3d20 742e 7265 706c 6163 6528    t = t.replace(
 00005ed0: 7061 7472 2c20 223c 7370 616e 2063 6c61  patr, "<span cla
 00005ee0: 7373 3d5c 2274 6970 7565 5f73 6561 7263  ss=\"tipue_searc
 00005ef0: 685f 636f 6e74 656e 745f 626f 6c64 5c22  h_content_bold\"
 00005f00: 3e24 313c 2f73 7061 6e3e 2229 3b0d 0a20  >$1</span>");.. 
 00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f30: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f30: 2020 2020 2020 2020 2020 2020 7d0d 0a0d              }...
+00005f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f60: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00005f70: 7220 745f 6420 3d20 2727 3b0d 0a20 2020  r t_d = '';..   
 00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fc0: 7661 7220 745f 6420 3d20 2727 3b0d 0a20  var t_d = '';.. 
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 2020 2020 2020 2020 2020 7661 7220 745f            var t_
+00005fb0: 7720 3d20 742e 7370 6c69 7428 2720 2729  w = t.split(' ')
+00005fc0: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
 00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ff0: 2020 2020 2020 2020 2020 2020 7661 7220              var 
-00006000: 745f 7720 3d20 742e 7370 6c69 7428 2720  t_w = t.split(' 
-00006010: 2729 3b0d 0a20 2020 2020 2020 2020 2020  ');..           
+00005ff0: 6966 2028 745f 772e 6c65 6e67 7468 203c  if (t_w.length <
+00006000: 2073 6574 2e64 6573 6372 6970 7469 7665   set.descriptive
+00006010: 576f 7264 7329 0d0a 2020 2020 2020 2020  Words)..        
 00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 6966 2028 745f 772e 6c65 6e67 7468    if (t_w.length
-00006050: 203c 2073 6574 2e64 6573 6372 6970 7469   < set.descripti
-00006060: 7665 576f 7264 7329 0d0a 2020 2020 2020  veWords)..      
-00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00006040: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006070: 2020 2020 2020 2020 2020 745f 6420 3d20            t_d = 
+00006080: 743b 0d0a 2020 2020 2020 2020 2020 2020  t;..            
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060c0: 2020 2020 2020 2020 2020 2020 745f 6420              t_d 
-000060d0: 3d20 743b 0d0a 2020 2020 2020 2020 2020  = t;..          
-000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060b0: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060e0: 2065 6c73 650d 0a20 2020 2020 2020 2020   else..         
 000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006100: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
-00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006110: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
 00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006130: 2020 2065 6c73 650d 0a20 2020 2020 2020     else..       
-00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006160: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006140: 2020 2020 2020 2020 2066 6f72 2028 7661           for (va
+00006150: 7220 6620 3d20 303b 2066 203c 2073 6574  r f = 0; f < set
+00006160: 2e64 6573 6372 6970 7469 7665 576f 7264  .descriptiveWord
+00006170: 733b 2066 2b2b 290d 0a20 2020 2020 2020  s; f++)..       
 00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006190: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-000061a0: 7661 7220 6620 3d20 303b 2066 203c 2073  var f = 0; f < s
-000061b0: 6574 2e64 6573 6372 6970 7469 7665 576f  et.descriptiveWo
-000061c0: 7264 733b 2066 2b2b 290d 0a20 2020 2020  rds; f++)..     
+00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061a0: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
+000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
+000061e0: 2020 2020 2074 5f64 202b 3d20 745f 775b       t_d += t_w[
+000061f0: 665d 202b 2027 2027 3b20 0d0a 2020 2020  f] + ' '; ..    
 00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 2020 2074 5f64 202b 3d20 745f         t_d += t_
-00006240: 775b 665d 202b 2027 2027 3b20 090d 0a20  w[f] + ' '; ... 
-00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
+00006230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006250: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
+00006260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006280: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2074 5f64 203d 2024 2e74 7269 6d28 745f   t_d = $.trim(t_
-000062f0: 6429 3b0d 0a20 2020 2020 2020 2020 2020  d);..           
+00006280: 2020 2020 2020 2020 2020 2020 2020 745f                t_
+00006290: 6420 3d20 242e 7472 696d 2874 5f64 293b  d = $.trim(t_d);
+000062a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000062d0: 6620 2874 5f64 2e63 6861 7241 7428 745f  f (t_d.charAt(t_
+000062e0: 642e 6c65 6e67 7468 202d 2031 2920 213d  d.length - 1) !=
+000062f0: 2027 2e27 290d 0a20 2020 2020 2020 2020   '.')..         
 00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006320: 2020 6966 2028 745f 642e 6368 6172 4174    if (t_d.charAt
-00006330: 2874 5f64 2e6c 656e 6774 6820 2d20 3129  (t_d.length - 1)
-00006340: 2021 3d20 272e 2729 0d0a 2020 2020 2020   != '.')..      
-00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006370: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00006320: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2020 2020 2020 2020 2074 5f64 202b 3d20           t_d += 
+00006360: 2720 2e2e 2e27 3b0d 0a20 2020 2020 2020  ' ...';..       
+00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063a0: 2020 2020 2020 2020 2020 2020 745f 6420              t_d 
-000063b0: 2b3d 2027 202e 2e2e 273b 0d0a 2020 2020  += ' ...';..    
-000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063e0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006440: 2020 2020 2020 2020 745f 6420 3d20 745f          t_d = t_
-00006450: 642e 7265 706c 6163 6528 2f68 3030 3131  d.replace(/h0011
-00006460: 2f67 2c20 2773 7061 6e20 636c 6173 733d  /g, 'span class=
-00006470: 5c22 7469 7075 655f 7365 6172 6368 5f63  \"tipue_search_c
-00006480: 6f6e 7465 6e74 5f62 6f6c 645c 2227 293b  ontent_bold\"');
-00006490: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063f0: 2020 2020 2074 5f64 203d 2074 5f64 2e72       t_d = t_d.r
+00006400: 6570 6c61 6365 282f 6830 3031 312f 672c  eplace(/h0011/g,
+00006410: 2027 7370 616e 2063 6c61 7373 3d5c 2274   'span class=\"t
+00006420: 6970 7565 5f73 6561 7263 685f 636f 6e74  ipue_search_cont
+00006430: 656e 745f 626f 6c64 5c22 2729 3b0d 0a20  ent_bold\"');.. 
+00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006460: 2020 2020 2020 2020 2020 2020 745f 6420              t_d 
+00006470: 3d20 745f 642e 7265 706c 6163 6528 2f68  = t_d.replace(/h
+00006480: 3030 3132 2f67 2c20 272f 7370 616e 2729  0012/g, '/span')
+00006490: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
 000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000064c0: 5f64 203d 2074 5f64 2e72 6570 6c61 6365  _d = t_d.replace
-000064d0: 282f 6830 3031 322f 672c 2027 2f73 7061  (/h0012/g, '/spa
-000064e0: 6e27 293b 0d0a 2020 2020 2020 2020 2020  n');..          
-000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006540: 2020 6f75 7420 2b3d 2027 3c64 6976 2063    out += '<div c
-00006550: 6c61 7373 3d22 7469 7075 655f 7365 6172  lass="tipue_sear
-00006560: 6368 5f63 6f6e 7465 6e74 5f74 6578 7422  ch_content_text"
-00006570: 3e27 202b 2074 5f64 202b 2027 3c2f 6469  >' + t_d + '</di
-00006580: 763e 273b 0d0a 2020 2020 2020 2020 2020  v>';..          
+000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064e0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+000064f0: 7574 202b 3d20 273c 6469 7620 636c 6173  ut += '<div clas
+00006500: 733d 2274 6970 7565 5f73 6561 7263 685f  s="tipue_search_
+00006510: 636f 6e74 656e 745f 7465 7874 223e 2720  content_text">' 
+00006520: 2b20 745f 6420 2b20 273c 2f64 6976 3e27  + t_d + '</div>'
+00006530: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
+00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006550: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006580: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065a0: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-000065b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065b0: 6966 2028 666f 756e 645b 695d 2e6e 6f74  if (found[i].not
+000065c0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065e0: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
 000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 2069 6620 2866 6f75 6e64 5b69 5d2e     if (found[i].
-00006610: 6e6f 7465 290d 0a20 2020 2020 2020 2020  note)..         
-00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006630: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00006640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006660: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00006670: 7574 202b 3d20 273c 6469 7620 636c 6173  ut += '<div clas
-00006680: 733d 2274 6970 7565 5f73 6561 7263 685f  s="tipue_search_
-00006690: 6e6f 7465 223e 2720 2b20 666f 756e 645b  note">' + found[
-000066a0: 695d 2e6e 6f74 6520 2b20 273c 2f64 6976  i].note + '</div
-000066b0: 3e27 3b20 2020 200d 0a20 2020 2020 2020  >';    ..       
+00006600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006610: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
+00006620: 2b3d 2027 3c64 6976 2063 6c61 7373 3d22  += '<div class="
+00006630: 7469 7075 655f 7365 6172 6368 5f6e 6f74  tipue_search_not
+00006640: 6522 3e27 202b 2066 6f75 6e64 5b69 5d2e  e">' + found[i].
+00006650: 6e6f 7465 202b 2027 3c2f 6469 763e 273b  note + '</div>';
+00006660: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006680: 2020 2020 2020 2020 2020 2020 2020 7d20                } 
+00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 207d 2020 2020 2020 2020 2020 2020 2020   }              
+000066e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006700: 2020 2020 2020 2020 2020 6f75 7420 2b3d            out +=
+00006710: 2027 3c2f 6469 763e 273b 0d0a 2020 2020   '</div>';..    
 00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006730: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006750: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00006760: 202b 3d20 273c 2f64 6976 3e27 3b0d 0a20   += '</div>';.. 
-00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006730: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00006740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006760: 2020 2020 206c 5f6f 2b2b 3b20 2020 2020       l_o++;     
+00006770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006790: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 2020 2020 2020 6c5f 6f2b 2b3b 2020          l_o++;  
-000067c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 207d 2020 2020 2020 2020 2020 2020     }            
+00006790: 7d20 2020 2020 2020 2020 2020 2020 2020  }               
+000067a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+000067b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067d0: 2069 6620 2863 203e 2073 6574 2e73 686f   if (c > set.sho
+000067e0: 7729 0d0a 2020 2020 2020 2020 2020 2020  w)..            
 000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 2020 0d0a 0d0a 2020 2020 2020 2020 2020    ....          
+00006800: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
 00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006820: 2020 2020 6966 2028 6320 3e20 7365 742e      if (c > set.
-00006830: 7368 6f77 290d 0a20 2020 2020 2020 2020  show)..         
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00006820: 2020 2020 2020 2020 7661 7220 7061 6765          var page
+00006830: 7320 3d20 4d61 7468 2e63 6569 6c28 6320  s = Math.ceil(c 
+00006840: 2f20 7365 742e 7368 6f77 293b 0d0a 2020  / set.show);..  
+00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006870: 2020 2020 2020 2020 2020 2076 6172 2070             var p
-00006880: 6167 6573 203d 204d 6174 682e 6365 696c  ages = Math.ceil
-00006890: 2863 202f 2073 6574 2e73 686f 7729 3b0d  (c / set.show);.
-000068a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000068b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068c0: 2020 2020 7661 7220 7061 6765 203d 2028      var page = (
-000068d0: 7374 6172 7420 2f20 7365 742e 7368 6f77  start / set.show
-000068e0: 293b 0d0a 2020 2020 2020 2020 2020 2020  );..            
-000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006900: 2020 2020 2020 2069 6620 2873 6574 2e66         if (set.f
-00006910: 6f6f 7465 7250 6167 6573 203c 2033 290d  ooterPages < 3).
-00006920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006960: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006970: 6574 2e66 6f6f 7465 7250 6167 6573 203d  et.footerPages =
-00006980: 2033 3b0d 0a20 2020 2020 2020 2020 2020   3;..           
+00006870: 2076 6172 2070 6167 6520 3d20 2873 7461   var page = (sta
+00006880: 7274 202f 2073 6574 2e73 686f 7729 3b0d  rt / set.show);.
+00006890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068b0: 2020 2020 6966 2028 7365 742e 666f 6f74      if (set.foot
+000068c0: 6572 5061 6765 7320 3c20 3329 0d0a 2020  erPages < 3)..  
+000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068f0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00006900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006910: 2020 2020 2020 2020 2020 2020 7365 742e              set.
+00006920: 666f 6f74 6572 5061 6765 7320 3d20 333b  footerPages = 3;
+00006930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006950: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
+00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006970: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069a0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069f0: 2020 206f 7574 202b 3d20 273c 6469 7620     out += '<div 
-00006a00: 6964 3d22 7469 7075 655f 7365 6172 6368  id="tipue_search
-00006a10: 5f66 6f6f 7422 3e3c 756c 2069 643d 2274  _foot"><ul id="t
-00006a20: 6970 7565 5f73 6561 7263 685f 666f 6f74  ipue_search_foot
-00006a30: 5f62 6f78 6573 223e 273b 0d0a 2020 2020  _boxes">';..    
-00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a50: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00006a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069a0: 6f75 7420 2b3d 2027 3c64 6976 2069 643d  out += '<div id=
+000069b0: 2274 6970 7565 5f73 6561 7263 685f 666f  "tipue_search_fo
+000069c0: 6f74 223e 3c75 6c20 6964 3d22 7469 7075  ot"><ul id="tipu
+000069d0: 655f 7365 6172 6368 5f66 6f6f 745f 626f  e_search_foot_bo
+000069e0: 7865 7322 3e27 3b0d 0a20 2020 2020 2020  xes">';..       
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a30: 2069 6620 2873 7461 7274 203e 2030 290d   if (start > 0).
+00006a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
 00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 2020 2020 6966 2028 7374 6172 7420 3e20      if (start > 
-00006a90: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ab0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ae0: 206f 7574 202b 3d20 273c 6c69 2072 6f6c   out += '<li rol
-00006af0: 653d 226e 6176 6967 6174 696f 6e22 3e3c  e="navigation"><
-00006b00: 6120 636c 6173 733d 2274 6970 7565 5f73  a class="tipue_s
-00006b10: 6561 7263 685f 666f 6f74 5f62 6f78 2220  earch_foot_box" 
-00006b20: 6163 6365 7373 6b65 793d 2262 2220 6964  accesskey="b" id
-00006b30: 3d22 2720 2b20 2873 7461 7274 202d 2073  ="' + (start - s
-00006b40: 6574 2e73 686f 7729 202b 2027 5f27 202b  et.show) + '_' +
-00006b50: 2072 6570 6c61 6365 202b 2027 223e 2720   replace + '">' 
-00006b60: 2b20 7469 7075 6573 6561 7263 685f 7374  + tipuesearch_st
-00006b70: 7269 6e67 5f36 202b 2027 3c2f 613e 3c2f  ring_6 + '</a></
-00006b80: 6c69 3e27 3b20 0d0a 2020 2020 2020 2020  li>'; ..        
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ba0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00006a90: 7574 202b 3d20 273c 6c69 2072 6f6c 653d  ut += '<li role=
+00006aa0: 226e 6176 6967 6174 696f 6e22 3e3c 6120  "navigation"><a 
+00006ab0: 636c 6173 733d 2274 6970 7565 5f73 6561  class="tipue_sea
+00006ac0: 7263 685f 666f 6f74 5f62 6f78 2220 6163  rch_foot_box" ac
+00006ad0: 6365 7373 6b65 793d 2262 2220 6964 3d22  cesskey="b" id="
+00006ae0: 2720 2b20 2873 7461 7274 202d 2073 6574  ' + (start - set
+00006af0: 2e73 686f 7729 202b 2027 5f27 202b 2072  .show) + '_' + r
+00006b00: 6570 6c61 6365 202b 2027 223e 2720 2b20  eplace + '">' + 
+00006b10: 7469 7075 6573 6561 7263 685f 7374 7269  tipuesearch_stri
+00006b20: 6e67 5f36 202b 2027 3c2f 613e 3c2f 6c69  ng_6 + '</a></li
+00006b30: 3e27 3b20 0d0a 2020 2020 2020 2020 2020  >'; ..          
+00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b50: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b90: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006bb0: 2020 2020 2020 2020 6966 2028 7061 6765          if (page
+00006bc0: 203c 3d20 3229 0d0a 2020 2020 2020 2020   <= 2)..        
 00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006be0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00006be0: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
 00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c00: 2020 2020 2020 2020 2020 6966 2028 7061            if (pa
-00006c10: 6765 203c 3d20 3229 0d0a 2020 2020 2020  ge <= 2)..      
-00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c30: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 2020 2020 2020 7661 7220 705f 6220 3d20        var p_b = 
+00006c20: 7061 6765 733b 0d0a 2020 2020 2020 2020  pages;..        
+00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c60: 2020 2020 2020 2020 7661 7220 705f 6220          var p_b 
-00006c70: 3d20 7061 6765 733b 0d0a 2020 2020 2020  = pages;..      
+00006c50: 6966 2028 7061 6765 7320 3e20 7365 742e  if (pages > set.
+00006c60: 666f 6f74 6572 5061 6765 7329 0d0a 2020  footerPages)..  
+00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ca0: 2020 6966 2028 7061 6765 7320 3e20 7365    if (pages > se
-00006cb0: 742e 666f 6f74 6572 5061 6765 7329 0d0a  t.footerPages)..
-00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00006c90: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00006ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cc0: 2020 2020 2020 705f 6220 3d20 7365 742e        p_b = set.
+00006cd0: 666f 6f74 6572 5061 6765 733b 0d0a 2020  footerPages;..  
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d10: 2020 2020 2020 2020 705f 6220 3d20 7365          p_b = se
-00006d20: 742e 666f 6f74 6572 5061 6765 733b 0d0a  t.footerPages;..
+00006d00: 2020 2020 2020 7d20 2020 2020 2020 2020        }         
+00006d10: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d50: 2020 2020 2020 2020 7d20 2020 2020 2020          }       
-00006d60: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00006d40: 2020 2020 2066 6f72 2028 7661 7220 6620       for (var f 
+00006d50: 3d20 303b 2066 203c 2070 5f62 3b20 662b  = 0; f < p_b; f+
+00006d60: 2b29 0d0a 2020 2020 2020 2020 2020 2020  +)..            
 00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d90: 2020 2020 2020 2066 6f72 2028 7661 7220         for (var 
-00006da0: 6620 3d20 303b 2066 203c 2070 5f62 3b20  f = 0; f < p_b; 
-00006db0: 662b 2b29 0d0a 2020 2020 2020 2020 2020  f++)..          
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dd0: 2020 2020 2020 2020 2020 2020 2020 7b0d                {.
-00006de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e00: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00006e10: 2028 6620 3d3d 2070 6167 6529 0d0a 2020   (f == page)..  
-00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e40: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e80: 6f75 7420 2b3d 2027 3c6c 6920 636c 6173  out += '<li clas
-00006e90: 733d 2263 7572 7265 6e74 2220 726f 6c65  s="current" role
-00006ea0: 3d22 6e61 7669 6761 7469 6f6e 223e 2720  ="navigation">' 
-00006eb0: 2b20 2866 202b 2031 2920 2b20 273c 2f6c  + (f + 1) + '</l
-00006ec0: 693e 273b 0d0a 2020 2020 2020 2020 2020  i>';..          
-00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d80: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
+00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006db0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00006dc0: 6620 3d3d 2070 6167 6529 0d0a 2020 2020  f == page)..    
+00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006df0: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
+00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e20: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00006e30: 7420 2b3d 2027 3c6c 6920 636c 6173 733d  t += '<li class=
+00006e40: 2263 7572 7265 6e74 2220 726f 6c65 3d22  "current" role="
+00006e50: 6e61 7669 6761 7469 6f6e 223e 2720 2b20  navigation">' + 
+00006e60: 2866 202b 2031 2920 2b20 273c 2f6c 693e  (f + 1) + '</li>
+00006e70: 273b 0d0a 2020 2020 2020 2020 2020 2020  ';..            
+00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ea0: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ed0: 2065 6c73 650d 0a20 2020 2020 2020 2020   else..         
 00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ef0: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
-00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f00: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
 00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f20: 2020 2065 6c73 650d 0a20 2020 2020 2020     else..       
-00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f50: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f80: 2020 2020 2020 2020 2020 206f 7574 202b             out +
-00006f90: 3d20 273c 6c69 2072 6f6c 653d 226e 6176  = '<li role="nav
-00006fa0: 6967 6174 696f 6e22 3e3c 6120 636c 6173  igation"><a clas
-00006fb0: 733d 2274 6970 7565 5f73 6561 7263 685f  s="tipue_search_
-00006fc0: 666f 6f74 5f62 6f78 2220 6964 3d22 2720  foot_box" id="' 
-00006fd0: 2b20 2866 202a 2073 6574 2e73 686f 7729  + (f * set.show)
-00006fe0: 202b 2027 5f27 202b 2072 6570 6c61 6365   + '_' + replace
-00006ff0: 202b 2027 223e 2720 2b20 2866 202b 2031   + '">' + (f + 1
-00007000: 2920 2b20 273c 2f61 3e3c 2f6c 693e 273b  ) + '</a></li>';
-00007010: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f30: 2020 2020 2020 2020 206f 7574 202b 3d20           out += 
+00006f40: 273c 6c69 2072 6f6c 653d 226e 6176 6967  '<li role="navig
+00006f50: 6174 696f 6e22 3e3c 6120 636c 6173 733d  ation"><a class=
+00006f60: 2274 6970 7565 5f73 6561 7263 685f 666f  "tipue_search_fo
+00006f70: 6f74 5f62 6f78 2220 6964 3d22 2720 2b20  ot_box" id="' + 
+00006f80: 2866 202a 2073 6574 2e73 686f 7729 202b  (f * set.show) +
+00006f90: 2027 5f27 202b 2072 6570 6c61 6365 202b   '_' + replace +
+00006fa0: 2027 223e 2720 2b20 2866 202b 2031 2920   '">' + (f + 1) 
+00006fb0: 2b20 273c 2f61 3e3c 2f6c 693e 273b 0d0a  + '</a></li>';..
+00006fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fe0: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
+00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007010: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
 00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00007040: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007030: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
+00007040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007060: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+00007060: 2020 2020 656c 7365 0d0a 2020 2020 2020      else..      
 00007070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007090: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00007080: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
+00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070b0: 2020 2020 2020 656c 7365 0d0a 2020 2020        else..    
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000070e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000070b0: 2020 2020 2020 2020 7661 7220 705f 6220          var p_b 
+000070c0: 3d20 7061 6765 202b 2073 6574 2e66 6f6f  = page + set.foo
+000070d0: 7465 7250 6167 6573 202d 2031 3b0d 0a20  terPages - 1;.. 
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000070f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007100: 2020 2020 2020 2020 2020 7661 7220 705f            var p_
-00007110: 6220 3d20 7061 6765 202b 2073 6574 2e66  b = page + set.f
-00007120: 6f6f 7465 7250 6167 6573 202d 2031 3b0d  ooterPages - 1;.
-00007130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2020 2020 2020 2020 2069 6620 2870 5f62           if (p_b
-00007160: 203e 2070 6167 6573 290d 0a20 2020 2020   > pages)..     
-00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007100: 2020 2020 2020 2069 6620 2870 5f62 203e         if (p_b >
+00007110: 2070 6167 6573 290d 0a20 2020 2020 2020   pages)..       
+00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007140: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 2070 5f62 203d 2070 6167 6573 3b20 0d0a   p_b = pages; ..
 00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007190: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071a0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
 000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071c0: 2020 2070 5f62 203d 2070 6167 6573 3b20     p_b = pages; 
-000071d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071f0: 2020 2020 2020 2020 2020 7d0d 0a20 2020            }..   
+000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071d0: 2020 2066 6f72 2028 7661 7220 6620 3d20     for (var f = 
+000071e0: 7061 6765 202d 2031 3b20 6620 3c20 705f  page - 1; f < p_
+000071f0: 623b 2066 2b2b 290d 0a20 2020 2020 2020  b; f++)..       
 00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2066 6f72 2028 7661 7220 6620       for (var f 
-00007230: 3d20 7061 6765 202d 2031 3b20 6620 3c20  = page - 1; f < 
-00007240: 705f 623b 2066 2b2b 290d 0a20 2020 2020  p_b; f++)..     
-00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00007280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072a0: 2020 2069 6620 2866 203d 3d20 7061 6765     if (f == page
-000072b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072e0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007310: 2020 2020 206f 7574 202b 3d20 273c 6c69       out += '<li
-00007320: 2063 6c61 7373 3d22 6375 7272 656e 7422   class="current"
-00007330: 2072 6f6c 653d 226e 6176 6967 6174 696f   role="navigatio
-00007340: 6e22 3e27 202b 2028 6620 2b20 3129 202b  n">' + (f + 1) +
-00007350: 2027 3c2f 6c69 3e27 3b0d 0a20 2020 2020   '</li>';..     
-00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007220: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00007230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007250: 2069 6620 2866 203d 3d20 7061 6765 290d   if (f == page).
+00007260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 2020 2020 2020 2020 2020 2020 2020 7b0d                {.
+00007290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072c0: 2020 206f 7574 202b 3d20 273c 6c69 2063     out += '<li c
+000072d0: 6c61 7373 3d22 6375 7272 656e 7422 2072  lass="current" r
+000072e0: 6f6c 653d 226e 6176 6967 6174 696f 6e22  ole="navigation"
+000072f0: 3e27 202b 2028 6620 2b20 3129 202b 2027  >' + (f + 1) + '
+00007300: 3c2f 6c69 3e27 3b0d 0a20 2020 2020 2020  </li>';..       
+00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007330: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007360: 2020 2020 2020 656c 7365 0d0a 2020 2020        else..    
 00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007390: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
 000073a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073b0: 2020 2020 2020 2020 656c 7365 0d0a 2020          else..  
-000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073e0: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
-000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007420: 6f75 7420 2b3d 2027 3c6c 6920 726f 6c65  out += '<li role
-00007430: 3d22 6e61 7669 6761 7469 6f6e 223e 3c61  ="navigation"><a
-00007440: 2063 6c61 7373 3d22 7469 7075 655f 7365   class="tipue_se
-00007450: 6172 6368 5f66 6f6f 745f 626f 7822 2069  arch_foot_box" i
-00007460: 643d 2227 202b 2028 6620 2a20 7365 742e  d="' + (f * set.
-00007470: 7368 6f77 2920 2b20 275f 2720 2b20 7265  show) + '_' + re
-00007480: 706c 6163 6520 2b20 2722 3e27 202b 2028  place + '">' + (
-00007490: 6620 2b20 3129 202b 2027 3c2f 613e 3c2f  f + 1) + '</a></
-000074a0: 6c69 3e27 3b0d 0a20 2020 2020 2020 2020  li>';..         
+000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073c0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+000073d0: 7420 2b3d 2027 3c6c 6920 726f 6c65 3d22  t += '<li role="
+000073e0: 6e61 7669 6761 7469 6f6e 223e 3c61 2063  navigation"><a c
+000073f0: 6c61 7373 3d22 7469 7075 655f 7365 6172  lass="tipue_sear
+00007400: 6368 5f66 6f6f 745f 626f 7822 2069 643d  ch_foot_box" id=
+00007410: 2227 202b 2028 6620 2a20 7365 742e 7368  "' + (f * set.sh
+00007420: 6f77 2920 2b20 275f 2720 2b20 7265 706c  ow) + '_' + repl
+00007430: 6163 6520 2b20 2722 3e27 202b 2028 6620  ace + '">' + (f 
+00007440: 2b20 3129 202b 2027 3c2f 613e 3c2f 6c69  + 1) + '</a></li
+00007450: 3e27 3b0d 0a20 2020 2020 2020 2020 2020  >';..           
+00007460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007480: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
+00007490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074a0: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
 000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074d0: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
-000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074f0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00007500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 2020 207d 2020 2020 2020 2020 2020       }          
-00007530: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00007540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074d0: 2020 207d 2020 2020 2020 2020 2020 2020     }            
+000074e0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
+000074f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007510: 2020 2020 6966 2028 7061 6765 202b 2031      if (page + 1
+00007520: 2021 3d20 7061 6765 7329 0d0a 2020 2020   != pages)..    
+00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007540: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00007550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007570: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00007580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007590: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-000075a0: 7061 6765 202b 2031 2021 3d20 7061 6765  page + 1 != page
-000075b0: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-000075c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075d0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007600: 206f 7574 202b 3d20 273c 6c69 2072 6f6c   out += '<li rol
-00007610: 653d 226e 6176 6967 6174 696f 6e22 3e3c  e="navigation"><
-00007620: 6120 636c 6173 733d 2274 6970 7565 5f73  a class="tipue_s
-00007630: 6561 7263 685f 666f 6f74 5f62 6f78 2220  earch_foot_box" 
-00007640: 6163 6365 7373 6b65 793d 226d 2220 6964  accesskey="m" id
-00007650: 3d22 2720 2b20 2873 7461 7274 202b 2073  ="' + (start + s
-00007660: 6574 2e73 686f 7729 202b 2027 5f27 202b  et.show) + '_' +
-00007670: 2072 6570 6c61 6365 202b 2027 223e 2720   replace + '">' 
-00007680: 2b20 7469 7075 6573 6561 7263 685f 7374  + tipuesearch_st
-00007690: 7269 6e67 5f37 202b 2027 3c2f 613e 3c2f  ring_7 + '</a></
-000076a0: 6c69 3e27 3b20 0d0a 2020 2020 2020 2020  li>'; ..        
-000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076c0: 2020 2020 2020 2020 2020 207d 2020 2020             }    
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00007710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007720: 2020 2020 2020 2020 2020 6f75 7420 2b3d            out +=
-00007730: 2027 3c2f 756c 3e3c 2f64 6976 3e27 3b0d   '</ul></div>';.
-00007740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007750: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00007760: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00007770: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
-00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007790: 2020 2020 2020 2020 2065 6c73 650d 0a20           else.. 
+00007570: 2020 2020 2020 2020 2020 6f75 7420 2b3d            out +=
+00007580: 2027 3c6c 6920 726f 6c65 3d22 6e61 7669   '<li role="navi
+00007590: 6761 7469 6f6e 223e 3c61 2063 6c61 7373  gation"><a class
+000075a0: 3d22 7469 7075 655f 7365 6172 6368 5f66  ="tipue_search_f
+000075b0: 6f6f 745f 626f 7822 2061 6363 6573 736b  oot_box" accessk
+000075c0: 6579 3d22 6d22 2069 643d 2227 202b 2028  ey="m" id="' + (
+000075d0: 7374 6172 7420 2b20 7365 742e 7368 6f77  start + set.show
+000075e0: 2920 2b20 275f 2720 2b20 7265 706c 6163  ) + '_' + replac
+000075f0: 6520 2b20 2722 3e27 202b 2074 6970 7565  e + '">' + tipue
+00007600: 7365 6172 6368 5f73 7472 696e 675f 3720  search_string_7 
+00007610: 2b20 273c 2f61 3e3c 2f6c 693e 273b 200d  + '</a></li>'; .
+00007620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007640: 2020 2020 7d20 2020 2020 2020 2020 2020      }           
+00007650: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00007660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007670: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076a0: 2020 206f 7574 202b 3d20 273c 2f75 6c3e     out += '</ul>
+000076b0: 3c2f 6469 763e 273b 0d0a 2020 2020 2020  </div>';..      
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 2020 2020 2020 2020 7d0d 0a0d 0a20 2020          }....   
+000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076f0: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007710: 2020 656c 7365 0d0a 2020 2020 2020 2020    else..        
+00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007730: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007750: 2020 6f75 7420 2b3d 2027 3c64 6976 2069    out += '<div i
+00007760: 643d 2274 6970 7565 5f73 6561 7263 685f  d="tipue_search_
+00007770: 6572 726f 7222 3e27 202b 2074 6970 7565  error">' + tipue
+00007780: 7365 6172 6368 5f73 7472 696e 675f 3820  search_string_8 
+00007790: 2b20 273c 2f64 6976 3e27 3b20 0d0a 2020  + '</div>'; ..  
 000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077b0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077d0: 2020 2020 2020 2020 206f 7574 202b 3d20           out += 
-000077e0: 273c 6469 7620 6964 3d22 7469 7075 655f  '<div id="tipue_
-000077f0: 7365 6172 6368 5f65 7272 6f72 223e 2720  search_error">' 
-00007800: 2b20 7469 7075 6573 6561 7263 685f 7374  + tipuesearch_st
-00007810: 7269 6e67 5f38 202b 2027 3c2f 6469 763e  ring_8 + '</div>
-00007820: 273b 200d 0a20 2020 2020 2020 2020 2020  '; ..           
-00007830: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-00007840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007850: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00007860: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00007870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007880: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078a0: 2020 6966 2028 7368 6f77 5f73 746f 7029    if (show_stop)
-000078b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000078c0: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
-000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
-000078f0: 2b3d 2027 3c64 6976 2069 643d 2274 6970  += '<div id="tip
-00007900: 7565 5f73 6561 7263 685f 6572 726f 7222  ue_search_error"
-00007910: 3e27 202b 2074 6970 7565 7365 6172 6368  >' + tipuesearch
-00007920: 5f73 7472 696e 675f 3820 2b20 2720 2720  _string_8 + ' ' 
-00007930: 2b20 7469 7075 6573 6561 7263 685f 7374  + tipuesearch_st
-00007940: 7269 6e67 5f39 202b 2027 3c2f 6469 763e  ring_9 + '</div>
-00007950: 273b 2020 2020 200d 0a20 2020 2020 2020  ';     ..       
-00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007970: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
-00007980: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00007990: 7365 0d0a 2020 2020 2020 2020 2020 2020  se..            
-000079a0: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000079d0: 2028 7365 742e 6d69 6e69 6d75 6d4c 656e   (set.minimumLen
-000079e0: 6774 6820 3d3d 2031 290d 0a20 2020 2020  gth == 1)..     
-000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a00: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
-00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a20: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00007a30: 7574 202b 3d20 273c 6469 7620 6964 3d22  ut += '<div id="
-00007a40: 7469 7075 655f 7365 6172 6368 5f65 7272  tipue_search_err
-00007a50: 6f72 223e 2720 2b20 7469 7075 6573 6561  or">' + tipuesea
-00007a60: 7263 685f 7374 7269 6e67 5f31 3120 2b20  rch_string_11 + 
-00007a70: 273c 2f64 6976 3e27 3b0d 0a20 2020 2020  '</div>';..     
-00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 2020 2020 2020 2020 2020 656c 7365 0d0a            else..
-00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 7b0d                {.
-00007ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 2020 6f75 7420 2b3d 2027 3c64 6976      out += '<div
-00007b10: 2069 643d 2274 6970 7565 5f73 6561 7263   id="tipue_searc
-00007b20: 685f 6572 726f 7222 3e27 202b 2074 6970  h_error">' + tip
-00007b30: 7565 7365 6172 6368 5f73 7472 696e 675f  uesearch_string_
-00007b40: 3132 202b 2027 2027 202b 2073 6574 2e6d  12 + ' ' + set.m
-00007b50: 696e 696d 756d 4c65 6e67 7468 202b 2027  inimumLength + '
-00007b60: 2027 202b 2074 6970 7565 7365 6172 6368   ' + tipuesearch
-00007b70: 5f73 7472 696e 675f 3133 202b 2027 3c2f  _string_13 + '</
-00007b80: 6469 763e 273b 0d0a 2020 2020 2020 2020  div>';..        
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ba0: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bc0: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
-00007bd0: 2020 2020 2020 2020 207d 2020 2020 2020           }      
-00007be0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007c10: 2020 2020 2020 2428 2723 7469 7075 655f        $('#tipue_
-00007c20: 7365 6172 6368 5f63 6f6e 7465 6e74 2729  search_content')
-00007c30: 2e68 6964 6528 292e 6874 6d6c 286f 7574  .hide().html(out
-00007c40: 292e 736c 6964 6544 6f77 6e28 3230 3029  ).slideDown(200)
-00007c50: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
-00007c60: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00007c70: 2020 2020 2020 2020 2020 2020 2024 2827               $('
-00007c80: 2374 6970 7565 5f73 6561 7263 685f 7265  #tipue_search_re
-00007c90: 706c 6163 6564 2729 2e63 6c69 636b 2866  placed').click(f
-00007ca0: 756e 6374 696f 6e28 290d 0a20 2020 2020  unction()..     
-00007cb0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00007cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007cd0: 2020 2020 2020 2020 2020 2067 6574 5469             getTi
-00007ce0: 7075 6553 6561 7263 6828 302c 2066 616c  pueSearch(0, fal
-00007cf0: 7365 293b 0d0a 2020 2020 2020 2020 2020  se);..          
-00007d00: 2020 2020 2020 2020 2020 7d29 3b0d 0a20            });.. 
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00007d30: 2020 2020 2020 2020 2024 2827 2e74 6970           $('.tip
-00007d40: 7565 5f73 6561 7263 685f 7265 6c61 7465  ue_search_relate
-00007d50: 645f 6274 6e27 292e 636c 6963 6b28 6675  d_btn').click(fu
-00007d60: 6e63 7469 6f6e 2829 0d0a 2020 2020 2020  nction()..      
-00007d70: 2020 2020 2020 2020 2020 2020 2020 7b0d                {.
-00007d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007d90: 2020 2020 2020 2020 2020 2428 2723 7469            $('#ti
-00007da0: 7075 655f 7365 6172 6368 5f69 6e70 7574  pue_search_input
-00007db0: 2729 2e76 616c 2824 2874 6869 7329 2e61  ').val($(this).a
-00007dc0: 7474 7228 2769 6427 2929 3b0d 0a20 2020  ttr('id'));..   
-00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 2020 2020 2020 6765 7454 6970 7565 5365        getTipueSe
-00007df0: 6172 6368 2830 2c20 7472 7565 293b 0d0a  arch(0, true);..
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e10: 2020 2020 7d29 3b0d 0a20 2020 2020 2020      });..       
-00007e20: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e40: 2020 2024 2827 2e74 6970 7565 5f73 6561     $('.tipue_sea
-00007e50: 7263 685f 696d 6167 655f 7a6f 6f6d 2729  rch_image_zoom')
-00007e60: 2e63 6c69 636b 2866 756e 6374 696f 6e28  .click(function(
-00007e70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007e80: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
-00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2020 2024 2827 2374 6970 7565 5f73 6561     $('#tipue_sea
-00007eb0: 7263 685f 696d 6167 655f 6d6f 6461 6c27  rch_image_modal'
-00007ec0: 292e 6661 6465 496e 2833 3030 293b 0d0a  ).fadeIn(300);..
-00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 2020 2020 2020 2024 2827 2374 6970           $('#tip
-00007ef0: 7565 5f73 6561 7263 685f 7a6f 6f6d 5f69  ue_search_zoom_i
-00007f00: 6d67 2729 2e61 7474 7228 2773 7263 272c  mg').attr('src',
-00007f10: 2074 6869 732e 7372 6329 3b0d 0a20 2020   this.src);..   
-00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f30: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000077b0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+000077c0: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
+000077d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077e0: 2020 2020 2065 6c73 650d 0a20 2020 2020       else..     
+000077f0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00007800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007810: 2020 2020 2020 2020 2020 2069 6620 2873             if (s
+00007820: 686f 775f 7374 6f70 290d 0a20 2020 2020  how_stop)..     
+00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007840: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007860: 2020 2020 206f 7574 202b 3d20 273c 6469       out += '<di
+00007870: 7620 6964 3d22 7469 7075 655f 7365 6172  v id="tipue_sear
+00007880: 6368 5f65 7272 6f72 223e 2720 2b20 7469  ch_error">' + ti
+00007890: 7075 6573 6561 7263 685f 7374 7269 6e67  puesearch_string
+000078a0: 5f38 202b 2027 2027 202b 2074 6970 7565  _8 + ' ' + tipue
+000078b0: 7365 6172 6368 5f73 7472 696e 675f 3920  search_string_9 
+000078c0: 2b20 273c 2f64 6976 3e27 3b20 2020 2020  + '</div>';     
+000078d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000078e0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007900: 2020 2020 2020 2065 6c73 650d 0a20 2020         else..   
+00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007920: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007940: 2020 2020 2020 2069 6620 2873 6574 2e6d         if (set.m
+00007950: 696e 696d 756d 4c65 6e67 7468 203d 3d20  inimumLength == 
+00007960: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007980: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00007990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079a0: 2020 2020 2020 2020 6f75 7420 2b3d 2027          out += '
+000079b0: 3c64 6976 2069 643d 2274 6970 7565 5f73  <div id="tipue_s
+000079c0: 6561 7263 685f 6572 726f 7222 3e27 202b  earch_error">' +
+000079d0: 2074 6970 7565 7365 6172 6368 5f73 7472   tipuesearch_str
+000079e0: 696e 675f 3131 202b 2027 3c2f 6469 763e  ing_11 + '</div>
+000079f0: 273b 0d0a 2020 2020 2020 2020 2020 2020  ';..            
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
+00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a30: 2020 2065 6c73 650d 0a20 2020 2020 2020     else..       
+00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a50: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a70: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00007a80: 202b 3d20 273c 6469 7620 6964 3d22 7469   += '<div id="ti
+00007a90: 7075 655f 7365 6172 6368 5f65 7272 6f72  pue_search_error
+00007aa0: 223e 2720 2b20 7469 7075 6573 6561 7263  ">' + tipuesearc
+00007ab0: 685f 7374 7269 6e67 5f31 3220 2b20 2720  h_string_12 + ' 
+00007ac0: 2720 2b20 7365 742e 6d69 6e69 6d75 6d4c  ' + set.minimumL
+00007ad0: 656e 6774 6820 2b20 2720 2720 2b20 7469  ength + ' ' + ti
+00007ae0: 7075 6573 6561 7263 685f 7374 7269 6e67  puesearch_string
+00007af0: 5f31 3320 2b20 273c 2f64 6976 3e27 3b0d  _13 + '</div>';.
+00007b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b10: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00007b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007b30: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b50: 2020 7d20 2020 2020 2020 2020 2020 2020    }             
+00007b60: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00007b70: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00007b80: 2020 2020 2020 2020 2020 2020 2020 2024                 $
+00007b90: 2827 2374 6970 7565 5f73 6561 7263 685f  ('#tipue_search_
+00007ba0: 636f 6e74 656e 7427 292e 6869 6465 2829  content').hide()
+00007bb0: 2e68 746d 6c28 6f75 7429 2e73 6c69 6465  .html(out).slide
+00007bc0: 446f 776e 2832 3030 293b 0d0a 2020 2020  Down(200);..    
+00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007be0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007bf0: 2020 2020 2020 2428 2723 7469 7075 655f        $('#tipue_
+00007c00: 7365 6172 6368 5f72 6570 6c61 6365 6427  search_replaced'
+00007c10: 292e 636c 6963 6b28 6675 6e63 7469 6f6e  ).click(function
+00007c20: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00007c30: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c50: 2020 2020 6765 7454 6970 7565 5365 6172      getTipueSear
+00007c60: 6368 2830 2c20 6661 6c73 6529 3b0d 0a20  ch(0, false);.. 
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 2020 207d 293b 0d0a 2020 2020 2020 2020     });..        
+00007c90: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cb0: 2020 2428 272e 7469 7075 655f 7365 6172    $('.tipue_sear
+00007cc0: 6368 5f72 656c 6174 6564 5f62 746e 2729  ch_related_btn')
+00007cd0: 2e63 6c69 636b 2866 756e 6374 696f 6e28  .click(function(
+00007ce0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00007cf0: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
+00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d10: 2020 2024 2827 2374 6970 7565 5f73 6561     $('#tipue_sea
+00007d20: 7263 685f 696e 7075 7427 292e 7661 6c28  rch_input').val(
+00007d30: 2428 7468 6973 292e 6174 7472 2827 6964  $(this).attr('id
+00007d40: 2729 293b 0d0a 2020 2020 2020 2020 2020  '));..          
+00007d50: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00007d60: 6574 5469 7075 6553 6561 7263 6828 302c  etTipueSearch(0,
+00007d70: 2074 7275 6529 3b0d 0a20 2020 2020 2020   true);..       
+00007d80: 2020 2020 2020 2020 2020 2020 207d 293b               });
+00007d90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007da0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00007db0: 2020 2020 2020 2020 2020 2020 2428 272e              $('.
+00007dc0: 7469 7075 655f 7365 6172 6368 5f69 6d61  tipue_search_ima
+00007dd0: 6765 5f7a 6f6f 6d27 292e 636c 6963 6b28  ge_zoom').click(
+00007de0: 6675 6e63 7469 6f6e 2829 0d0a 2020 2020  function()..    
+00007df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e00: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00007e10: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
+00007e20: 7469 7075 655f 7365 6172 6368 5f69 6d61  tipue_search_ima
+00007e30: 6765 5f6d 6f64 616c 2729 2e66 6164 6549  ge_modal').fadeI
+00007e40: 6e28 3330 3029 3b0d 0a20 2020 2020 2020  n(300);..       
+00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e60: 2020 2428 2723 7469 7075 655f 7365 6172    $('#tipue_sear
+00007e70: 6368 5f7a 6f6f 6d5f 696d 6727 292e 6174  ch_zoom_img').at
+00007e80: 7472 2827 7372 6327 2c20 7468 6973 2e73  tr('src', this.s
+00007e90: 7263 293b 0d0a 2020 2020 2020 2020 2020  rc);..          
+00007ea0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00007eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ec0: 2020 2020 2020 2020 2020 7661 7220 7a5f            var z_
+00007ed0: 7520 3d20 2428 7468 6973 292e 6174 7472  u = $(this).attr
+00007ee0: 2827 6461 7461 2d75 726c 2729 3b0d 0a20  ('data-url');.. 
+00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f00: 2020 2020 2020 2020 2428 2723 7469 7075          $('#tipu
+00007f10: 655f 7365 6172 6368 5f7a 6f6f 6d5f 7572  e_search_zoom_ur
+00007f20: 6c27 292e 6174 7472 2827 6872 6566 272c  l').attr('href',
+00007f30: 207a 5f75 293b 0d0a 2020 2020 2020 2020   z_u);..        
 00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f50: 2076 6172 207a 5f75 203d 2024 2874 6869   var z_u = $(thi
-00007f60: 7329 2e61 7474 7228 2764 6174 612d 7572  s).attr('data-ur
-00007f70: 6c27 293b 0d0a 2020 2020 2020 2020 2020  l');..          
-00007f80: 2020 2020 2020 2020 2020 2020 2020 2024                 $
-00007f90: 2827 2374 6970 7565 5f73 6561 7263 685f  ('#tipue_search_
-00007fa0: 7a6f 6f6d 5f75 726c 2729 2e61 7474 7228  zoom_url').attr(
-00007fb0: 2768 7265 6627 2c20 7a5f 7529 3b0d 0a20  'href', z_u);.. 
-00007fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fd0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ff0: 2020 2076 6172 207a 5f6f 203d 2074 6869     var z_o = thi
-00008000: 732e 616c 7420 2b20 273c 6469 7620 636c  s.alt + '<div cl
-00008010: 6173 733d 2274 6970 7565 5f73 6561 7263  ass="tipue_searc
-00008020: 685f 7a6f 6f6d 5f6f 7074 696f 6e73 223e  h_zoom_options">
-00008030: 3c61 2068 7265 663d 2227 202b 2074 6869  <a href="' + thi
-00008040: 732e 7372 6320 2b20 2722 2074 6172 6765  s.src + '" targe
-00008050: 743d 225f 626c 616e 6b22 3e27 202b 2074  t="_blank">' + t
-00008060: 6970 7565 7365 6172 6368 5f73 7472 696e  ipuesearch_strin
-00008070: 675f 3135 202b 2027 3c2f 613e 266e 6273  g_15 + '</a>&nbs
-00008080: 703b 203c 6120 6872 6566 3d22 2720 2b20  p; <a href="' + 
-00008090: 7a5f 7520 2b20 2722 3e27 202b 2074 6970  z_u + '">' + tip
-000080a0: 7565 7365 6172 6368 5f73 7472 696e 675f  uesearch_string_
-000080b0: 3136 202b 2027 3c2f 613e 3c2f 6469 763e  16 + '</a></div>
-000080c0: 273b 0d0a 2020 2020 2020 2020 2020 2020  ';..            
-000080d0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080f0: 2020 2020 2020 2020 2428 2723 7469 7075          $('#tipu
-00008100: 655f 7365 6172 6368 5f7a 6f6f 6d5f 7465  e_search_zoom_te
-00008110: 7874 2729 2e68 746d 6c28 7a5f 6f29 3b0d  xt').html(z_o);.
-00008120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008130: 2020 2020 207d 293b 0d0a 2020 2020 2020       });..      
-00008140: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008160: 2020 2020 2428 272e 7469 7075 655f 7365      $('.tipue_se
-00008170: 6172 6368 5f69 6d61 6765 5f63 6c6f 7365  arch_image_close
-00008180: 2729 2e63 6c69 636b 2866 756e 6374 696f  ').click(functio
-00008190: 6e28 290d 0a20 2020 2020 2020 2020 2020  n()..           
-000081a0: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
-000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081c0: 2020 2020 2024 2827 2374 6970 7565 5f73       $('#tipue_s
-000081d0: 6561 7263 685f 696d 6167 655f 6d6f 6461  earch_image_moda
-000081e0: 6c27 292e 6661 6465 4f75 7428 3330 3029  l').fadeOut(300)
-000081f0: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
-00008200: 2020 2020 2020 207d 293b 2020 2020 2020         });      
-00008210: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00008220: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 2024 2827 2e74 6970 7565 5f73 6561 7263   $('.tipue_searc
-00008250: 685f 666f 6f74 5f62 6f78 2729 2e63 6c69  h_foot_box').cli
-00008260: 636b 2866 756e 6374 696f 6e28 290d 0a20  ck(function().. 
+00007f50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00007f60: 2020 2020 2020 2020 2020 2020 7661 7220              var 
+00007f70: 7a5f 6f20 3d20 7468 6973 2e61 6c74 202b  z_o = this.alt +
+00007f80: 2027 3c64 6976 2063 6c61 7373 3d22 7469   '<div class="ti
+00007f90: 7075 655f 7365 6172 6368 5f7a 6f6f 6d5f  pue_search_zoom_
+00007fa0: 6f70 7469 6f6e 7322 3e3c 6120 6872 6566  options"><a href
+00007fb0: 3d22 2720 2b20 7468 6973 2e73 7263 202b  ="' + this.src +
+00007fc0: 2027 2220 7461 7267 6574 3d22 5f62 6c61   '" target="_bla
+00007fd0: 6e6b 223e 2720 2b20 7469 7075 6573 6561  nk">' + tipuesea
+00007fe0: 7263 685f 7374 7269 6e67 5f31 3520 2b20  rch_string_15 + 
+00007ff0: 273c 2f61 3e26 6e62 7370 3b20 3c61 2068  '</a>&nbsp; <a h
+00008000: 7265 663d 2227 202b 207a 5f75 202b 2027  ref="' + z_u + '
+00008010: 223e 2720 2b20 7469 7075 6573 6561 7263  ">' + tipuesearc
+00008020: 685f 7374 7269 6e67 5f31 3620 2b20 273c  h_string_16 + '<
+00008030: 2f61 3e3c 2f64 6976 3e27 3b0d 0a20 2020  /a></div>';..   
+00008040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008050: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008070: 2024 2827 2374 6970 7565 5f73 6561 7263   $('#tipue_searc
+00008080: 685f 7a6f 6f6d 5f74 6578 7427 292e 6874  h_zoom_text').ht
+00008090: 6d6c 287a 5f6f 293b 0d0a 2020 2020 2020  ml(z_o);..      
+000080a0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+000080b0: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
+000080c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000080d0: 2020 2020 2020 2020 2020 2020 2024 2827               $('
+000080e0: 2e74 6970 7565 5f73 6561 7263 685f 696d  .tipue_search_im
+000080f0: 6167 655f 636c 6f73 6527 292e 636c 6963  age_close').clic
+00008100: 6b28 6675 6e63 7469 6f6e 2829 0d0a 2020  k(function()..  
+00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008120: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00008130: 2020 2020 2020 2020 2020 2020 2020 2428                $(
+00008140: 2723 7469 7075 655f 7365 6172 6368 5f69  '#tipue_search_i
+00008150: 6d61 6765 5f6d 6f64 616c 2729 2e66 6164  mage_modal').fad
+00008160: 654f 7574 2833 3030 293b 0d0a 2020 2020  eOut(300);..    
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 7d29 3b20 2020 2020 2020 2020 2020 2020  });             
+00008190: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000081a0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+000081b0: 2020 2020 2020 2020 2020 2428 272e 7469            $('.ti
+000081c0: 7075 655f 7365 6172 6368 5f66 6f6f 745f  pue_search_foot_
+000081d0: 626f 7827 292e 636c 6963 6b28 6675 6e63  box').click(func
+000081e0: 7469 6f6e 2829 0d0a 2020 2020 2020 2020  tion()..        
+000081f0: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
+00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008210: 2020 2020 2020 2020 7661 7220 6964 5f76          var id_v
+00008220: 203d 2024 2874 6869 7329 2e61 7474 7228   = $(this).attr(
+00008230: 2769 6427 293b 0d0a 2020 2020 2020 2020  'id');..        
+00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008250: 2076 6172 2069 645f 6120 3d20 6964 5f76   var id_a = id_v
+00008260: 2e73 706c 6974 2827 5f27 293b 0d0a 2020  .split('_');..  
 00008270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008280: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00008290: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000082a0: 6172 2069 645f 7620 3d20 2428 7468 6973  ar id_v = $(this
-000082b0: 292e 6174 7472 2827 6964 2729 3b0d 0a20  ).attr('id');.. 
-000082c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082d0: 2020 2020 2020 2020 7661 7220 6964 5f61          var id_a
-000082e0: 203d 2069 645f 762e 7370 6c69 7428 275f   = id_v.split('_
-000082f0: 2729 3b0d 0a20 2020 2020 2020 2020 2020  ');..           
-00008300: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00008310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008320: 2020 2020 6765 7454 6970 7565 5365 6172      getTipueSear
-00008330: 6368 2870 6172 7365 496e 7428 6964 5f61  ch(parseInt(id_a
-00008340: 5b30 5d29 2c20 6964 5f61 5b31 5d29 3b0d  [0]), id_a[1]);.
-00008350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008360: 2020 2020 207d 293b 2020 2020 2020 2020       });        
-00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008390: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-000083a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000083b0: 7d20 2020 2020 2020 2020 200d 0a20 2020  }          ..   
-000083c0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-000083d0: 2020 207d 293b 0d0a 2020 2020 207d 3b0d     });..     };.
-000083e0: 0a20 2020 0d0a 7d29 286a 5175 6572 7929  .   ..})(jQuery)
-000083f0: 3b0d 0a                                  ;..
+00008280: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00008290: 2020 2020 2020 2020 2020 2020 2067 6574               get
+000082a0: 5469 7075 6553 6561 7263 6828 7061 7273  TipueSearch(pars
+000082b0: 6549 6e74 2869 645f 615b 305d 292c 2069  eInt(id_a[0]), i
+000082c0: 645f 615b 315d 293b 0d0a 2020 2020 2020  d_a[1]);..      
+000082d0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
+000082e0: 3b20 2020 2020 2020 2020 2020 2020 2020  ;               
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008310: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00008320: 2020 2020 2020 2020 207d 2020 2020 2020           }      
+00008330: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00008340: 0d0a 2020 2020 2020 2020 2020 7d29 3b0d  ..          });.
+00008350: 0a20 2020 2020 7d3b 0d0a 0d0a 7d29 286a  .     };....})(j
+00008360: 5175 6572 7929 3b0d 0a                   Query);..
```

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_content.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js` & `seafoam-2.9.1/pelican/plugins/seafoam/static/tipuesearch/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/404.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/404.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/archives.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/archives.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/article.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/article.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends "base.html" %}
 
 {% block title -%}
-    {{ article.title|striptags|breaking_spaces }} &mdash; {{ super() }}
+    {{ article.title | striptags | breaking_spaces }} &mdash; {{ super() }}
 {%- endblock %}
 
 {% block html_lang %}{{ article.lang }}{% endblock %}
 
 {% block meta %}
     {% if article.author %}
         <meta name="author" content="{{ article.author }}" />
@@ -59,18 +59,22 @@
 {% block breadcrumbs %}
     {% if DISPLAY_BREADCRUMBS %}
         <ol class="breadcrumb">
             <li><a href="{{ SITE_ROOT_URL | default('/') }}" title="{{ SITENAME }}"><span class="fa fa-home fa-lg"></span></a></li>
             {% if MENUITEMS_2_AT %}
                 <li><a href="{{ SITEURL -}} / {{- MENUITEMS_2_AT_LINK }}" title="{{ MENUITEMS_2_AT }}">{{ MENUITEMS_2_AT }}</a></li>
             {% endif %}
-            {% if DISPLAY_CATEGORY_IN_BREADCRUMBS %}
+            {% if DISPLAY_CATEGORY_IN_BREADCRUMBS or article.micro %}
                 <li><a href="{{ SITEURL -}} / {{- article.category.url }}" title="{{ article.category }}">{{ article.category }}</a></li>
             {% endif %}
-            <li class="active">{{ article.title | striptags }}</li>
+            {% if article.micro %}
+                <li class="active">{{ article.date | datetime("%B %d, %Y at %H:%M") }}</li>
+            {% else %}
+                <li class="active">{{ article.title | striptags }}</li>
+            {% endif %}
         </ol>     
     {% endif %}
 {% endblock %}
 
 {% block content %}
     <section id="content">
         <article>
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-{% extends "base.html" %} {% block title -%} {
-{ article.title|striptags|breaking_spaces }} — {{ super() }} {%- endblock %} {%
-block html_lang %}{{ article.lang }}{% endblock %} {% block meta %} {% if
-article.author %}
+{% extends "base.html" %} {% block title -%} {{ article.title | striptags |
+breaking_spaces }} — {{ super() }} {%- endblock %} {% block html_lang %}{
+{ article.lang }}{% endblock %} {% block meta %} {% if article.author %}
  {% else %}
  {% endif %} {% if article.tags %}
  {% endif %} {% if article.summary %}
  {% endif %} {% endblock %} {# {% block opengraph %} {% if OPEN_GRAPH_FB_APP_ID
 %}
 
 
@@ -19,18 +18,21 @@
  {% elif AUTHOR %}
  {% endif %} {% if article.og_image %}
  {% elif OPEN_GRAPH_IMAGE %}
  {% endif %} {% endif %} {% endblock %} #} {% block canonical_rel %}
  {% endblock %} {% block breadcrumbs %} {% if DISPLAY_BREADCRUMBS %}
    1. {% if MENUITEMS_2_AT %}
    2. {{_MENUITEMS_2_AT_}}
-   3. {% endif %} {% if DISPLAY_CATEGORY_IN_BREADCRUMBS %}
+   3. {% endif %} {% if DISPLAY_CATEGORY_IN_BREADCRUMBS or article.micro %}
    4. {{_article.category_}}
-   5. {% endif %}
-   6. {{ article.title | striptags }}
+   5. {% endif %} {% if article.micro %}
+   6. {{ article.date | datetime("%B %d, %Y at %H:%M") }}
+   7. {% else %}
+   8. {{ article.title | striptags }}
+   9. {% endif %}
 {% endif %} {% endblock %} {% block content %}   {% if article.image %} [{
 { article.title|striptags }}] {% elif CATEGORY_IMAGES and article.category in
 CATEGORY_IMAGES %} [{{ article.category|striptags }}] {% endif %} {% if not
 article.micro %}
 ****** {{_article.title|replace(' ',_'_')_}} ******
  {% endif %}
 {% include "includes/article_info.html" %}
```

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/article_list.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/article_list.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/author.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/author.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/authors.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/authors.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/base.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/base.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/categories.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/categories.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/category.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/category.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/addthis.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/addthis.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/article_info.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/article_info.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 <footer class="post-info">
     <span class="label label-default">Published</span>
     <span class="published">
-        <i class="fa fa-calendar"></i><time datetime="{{ article.date.isoformat() }}"> {{ article.date | article_date }}</time>
+        <i class="fa fa-calendar"></i><time datetime="{{ article.date.isoformat() }}"> 
+            {{ article.date | article_date }}
+            {% if article.micro %}
+                at {{ article.date | datetime("%H:%M") }}
+            {% endif -%}
+            </time>
     </span>
     {# Uncomment if you want the author shown #}
     {#{% if article.author %}#}
     {#<span class="label">By</span>#}
     {#<a href="{{ SITEURL -}} / {{- article.author.url }}"><i class="fa fa-user"></i> {{ article.author }}</a>#}
     {#{% endif -%}-#}
 
-    {%- if article.readtime_minutes -%}
-        <span class="label label-default">Reading Time</span>
-        <i class="fa fa-clock-o"></i> ~{{ article.readtime_minutes }} min
-    {%- elif article.stats -%}
-        <span class="label label-default">Reading Time</span>
-        <i class="fa fa-clock-o"></i> ~{{ article.stats['read_mins'] }} min
+    {%- if not article.micro -%}
+        {%- if article.readtime_minutes -%}
+            <span class="label label-default">Reading Time</span>
+            <i class="fa fa-clock-o"></i> ~{{ article.readtime_minutes }} min
+        {%- elif article.stats -%}
+            <span class="label label-default">Reading Time</span>
+            <i class="fa fa-clock-o"></i> ~{{ article.stats['read_mins'] }} min
+        {%- endif -%}
     {%- endif -%}
 
     {#- Uncomment if you want to show Categories#}
     {#<span class="label label-default">Category</span>#}
     {#<a href="{{ SITEURL -}} / {{- article.category.url }}">{{ article.category }}</a>-#}
 
     {%- if PDF_PROCESSOR %}
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
- Published   {{ article.date | article_date }}  {# Uncomment if you want the
-author shown #} {#{% if article.author %}#} {#By#} {#
+ Published   {{ article.date | article_date }} {% if article.micro %} at {
+{ article.date | datetime("%H:%M") }} {% endif -%}   {# Uncomment if you want
+the author shown #} {#{% if article.author %}#} {#By#} {#
  {{_article.author_}}
-#} {#{% endif -%}-#} {%- if article.readtime_minutes -%} Reading Time  ~{
-{ article.readtime_minutes }} min {%- elif article.stats -%} Reading Time  ~{
-{ article.stats['read_mins'] }} min {%- endif -%} {#- Uncomment if you want to
-show Categories#} {#Category#} {#{{_article.category_}}-#} {%- if PDF_PROCESSOR
-%}  PDF  {% endif -%} {%- include 'includes/taglist.html' %} {% import
-'includes/translations.html' as translations with context %} {
+#} {#{% endif -%}-#} {%- if not article.micro -%} {%- if
+article.readtime_minutes -%} Reading Time  ~{{ article.readtime_minutes }} min
+{%- elif article.stats -%} Reading Time  ~{{ article.stats['read_mins'] }} min
+{%- endif -%} {%- endif -%} {#- Uncomment if you want to show Categories#}
+{#Category#} {#{{_article.category_}}-#} {%- if PDF_PROCESSOR %}  PDF  {% endif
+-%} {%- include 'includes/taglist.html' %} {% import 'includes/
+translations.html' as translations with context %} {
 { translations.translations_for(article) }}
```

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/article_listing.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/article_listing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/assets-css.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/assets-css.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {% if BOOTSTRAP_THEME %}
-	{% set ALL_CSS = ("css/bootstrap." + BOOTSTRAP_THEME + ".min.css", ) %}
+    {% set ALL_CSS = ("css/bootstrap." + BOOTSTRAP_THEME + ".min.css", ) %}
 {% else %}
-	{% set ALL_CSS = ("css/bootstrap.min.css", ) %}
+    {% set ALL_CSS = ("css/bootstrap.min.css", ) %}
 {% endif %}
 {% set ALL_CSS = ALL_CSS + ("css/font-awesome.min.css", ) %}
 {% set ALL_CSS = ALL_CSS + ("css/pygments/" + PYGMENTS_STYLE|default('native') + ".css", ) %}
 {% if DOCUTIL_CSS %}
-	{% set ALL_CSS = ALL_CSS + ("css/html4css1.css", ) %}
+    {% set ALL_CSS = ALL_CSS + ("css/html4css1.css", ) %}
 {% endif %}
 {# DISABLED -- moved this to my Bootstrap theme 
 {% if TYPOGRIFY %}
-	{% set ALL_CSS = ALL_CSS + ("css/typogrify.css", ) %}
+    {% set ALL_CSS = ALL_CSS + ("css/typogrify.css", ) %}
 {% endif %}
 {% set ALL_CSS = ALL_CSS + ("css/style.css", ) %}
 #}
 {% if CUSTOM_CSS %}
-	{% set ALL_CSS = ALL_CSS + (CUSTOM_CSS, ) %}
+    {% set ALL_CSS = ALL_CSS + (CUSTOM_CSS, ) %}
 {% endif %}
 
 <meta name="all css" value= "{{ ALL_CSS }}" />
 
 {# ALL_CSS cannot be a list or a tuple for this to work... #} 
 {% assets filters="cssmin", output="all-css.css", ALL_CSS %}
-	<link href="{{ SITEURL -}} / {{- ASSET_URL }}" rel="stylesheet" type="text/css" />
+    <link href="{{ SITEURL -}} / {{- ASSET_URL }}" rel="stylesheet" type="text/css" />
 {% endassets %}
```

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/cc-license.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/cc-license.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/comment_count.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/comment_count.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 {% if DISQUS_SITENAME and DISQUS_DISPLAY_COUNTS -%}
-	<a href="{{ SITEURL -}} / {{- article.url }}#disqus_thread" {% if not DISQUS_NO_ID %}data-disqus-identifier="{{ article.date|strftime('%Y-%m-') ~ article.slug if DISQUS_ID_PREFIX_SLUG else article.slug }}"{% endif %}> comments</a>
+    <a href="{{ SITEURL -}} / {{- article.url }}#disqus_thread" {% if not DISQUS_NO_ID %}data-disqus-identifier="{{ article.date|strftime('%Y-%m-') ~ article.slug if DISQUS_ID_PREFIX_SLUG else article.slug }}"{% endif %}> comments</a>
 {%- endif -%}
 {%- if PELICAN_COMMENT_SYSTEM and PELICAN_COMMENT_SYSTEM_DISPLAY_COUNTS != false -%}
-	<a href="{{ SITEURL -}} / {{- article.url }}#comments">{{ article.comments_count }}&nbsp;comment{% if article.comments_count != 1 %}s{% endif %}</a>
+    <a href="{{ SITEURL -}} / {{- article.url }}#comments">{{ article.comments_count }}&nbsp;comment{% if article.comments_count != 1 %}s{% endif %}</a>
 {%- endif -%}
```

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/disqus_script.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/disqus_script.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/footer.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/footer.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/ga.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/ga.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/github-js.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/github-js.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/pagination.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/piwik.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/piwik.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/sidebar.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/sidebar.html`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 {% endif %}
 
 <aside>
     <section>
         <ul class="list-group list-group-flush">
             {% if SOCIAL %}
                 <li class="list-group-item"><h4><i class="fa fa-home fa-lg"></i><span class="icon-label">Social</span></h4>
-                  <ul class="list-group" id="social">
+                    <ul class="list-group" id="social">
                     {% for name, link in SOCIAL %}
-                    <li class="list-group-item"><a href="{{ link }}"><i
-                            class="fa fa-{{ name|lower|replace('+','-plus') }}-square fa-lg"></i> {{ name }}
-                    </a></li>
+                        <li class="list-group-item"><a href="{{ link }}">
+                            <i class="fa fa-{{ name|lower|replace('+','-plus') }}-square fa-lg"></i> {{ name }}
+                        </a></li>
                     {% endfor %}
-                  </ul>
+                    </ul>
                 </li>
             {% endif %}
 
             {% if DISPLAY_RECENT_POSTS_ON_SIDEBAR %}
                 {% if RECENT_POST_COUNT is not defined %}
                     {% set RECENT_POST_COUNT = 5 %}
                 {% endif %}
```

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/includes/twitter_timeline.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/includes/twitter_timeline.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/index.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/index.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/page.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/page.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/period_archives.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/period_archives.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/prjct.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/prjct.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/search.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/search.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/dual_pricing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/strathcona/pricing.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/strathcona/pricing.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/tag.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/tag.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/pelican/plugins/seafoam/templates/tags.html` & `seafoam-2.9.1/pelican/plugins/seafoam/templates/tags.html`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/seafoam.egg-info/PKG-INFO` & `seafoam-2.9.1/seafoam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seafoam
-Version: 2.9.0
+Version: 2.9.1
 Summary: Pelican theme, first used for Minchin.ca.
 Home-page: http://blog.minchin.ca/label/seafoam/
 Author: W. Minchin
 Author-email: w_minchin@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/MinchinWeb/seafoam/issues
 Project-URL: Changelog, https://github.com/MinchinWeb/seafoam/blob/master/docs/changelog.rst
```

### Comparing `seafoam-2.9.0/seafoam.egg-info/SOURCES.txt` & `seafoam-2.9.1/seafoam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seafoam-2.9.0/setup.py` & `seafoam-2.9.1/setup.py`

 * *Files identical despite different names*

