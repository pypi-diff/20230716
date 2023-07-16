# Comparing `tmp/phables-1.0.0.tar.gz` & `tmp/phables-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phables-1.0.0.tar", last modified: Tue May  9 03:51:30 2023, max compression
+gzip compressed data, was "phables-1.1.0.tar", last modified: Sun Jul 16 03:45:22 2023, max compression
```

## Comparing `phables-1.0.0.tar` & `phables-1.1.0.tar`

### file list

```diff
@@ -1,107 +1,72 @@
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.701600 phables-1.0.0/
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.518041 phables-1.0.0/.github/
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.531479 phables-1.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      650 2023-01-24 03:27:45.000000 phables-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      126 2023-01-10 00:17:29.000000 phables-1.0.0/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      612 2023-01-24 03:27:45.000000 phables-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.532752 phables-1.0.0/.github/workflows/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2948 2023-01-19 06:09:18.000000 phables-1.0.0/.github/workflows/codeql.yml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1747 2023-01-20 03:32:50.000000 phables-1.0.0/.github/workflows/testing.yml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1914 2023-04-21 05:14:19.000000 phables-1.0.0/.gitignore
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      439 2023-01-10 00:17:29.000000 phables-1.0.0/.readthedocs.yaml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5265 2023-01-10 00:17:29.000000 phables-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3497 2023-05-09 03:49:37.000000 phables-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1079 2023-02-19 03:25:45.000000 phables-1.0.0/LICENSE
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      125 2023-01-12 05:31:03.000000 phables-1.0.0/MANIFEST.in
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    11079 2023-05-09 03:51:30.701051 phables-1.0.0/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10428 2023-05-09 03:49:37.000000 phables-1.0.0/README.md
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.538587 phables-1.0.0/docs/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1020 2023-02-10 09:05:34.000000 phables-1.0.0/docs/assemble.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3026 2023-01-16 00:51:18.000000 phables-1.0.0/docs/comparison.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3788 2023-04-21 05:14:19.000000 phables-1.0.0/docs/faq.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3808 2023-02-02 03:28:12.000000 phables-1.0.0/docs/graph_stats.md
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.579830 phables-1.0.0/docs/images/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   523874 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/Phables_workflow.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   133780 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/components.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    58437 2023-01-16 01:26:17.000000 phables-1.0.0/docs/images/histogram_n_nodes.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   344700 2023-02-02 03:25:24.000000 phables-1.0.0/docs/images/pearson_clustermap.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   318753 2023-02-02 03:25:23.000000 phables-1.0.0/docs/images/pearson_heatmap.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   434479 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/phables_logo.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    98145 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/qual_resolved_genome_unitig_boxen.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   174336 2023-01-10 00:17:29.000000 phables-1.0.0/docs/images/qual_resolved_genome_unitig_violin.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1708 2023-04-21 05:14:19.000000 phables-1.0.0/docs/index.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     4204 2023-05-09 03:49:37.000000 phables-1.0.0/docs/install.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1894 2023-01-10 00:17:29.000000 phables-1.0.0/docs/quality.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      301 2023-01-10 00:17:29.000000 phables-1.0.0/docs/requirements.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6246 2023-05-09 03:49:37.000000 phables-1.0.0/docs/usage.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      649 2023-04-21 05:16:05.000000 phables-1.0.0/mkdocs.yml
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.588159 phables-1.0.0/phables/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-02-02 03:00:11.000000 phables-1.0.0/phables/.DS_Store
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-01-12 05:31:03.000000 phables-1.0.0/phables/__init__.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     7248 2023-05-09 03:49:37.000000 phables-1.0.0/phables/__main__.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.593493 phables-1.0.0/phables/__pycache__/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      159 2023-02-18 10:21:30.000000 phables-1.0.0/phables/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5807 2023-02-18 10:21:30.000000 phables-1.0.0/phables/__pycache__/__main__.cpython-310.pyc
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     4923 2023-02-18 10:21:30.000000 phables-1.0.0/phables/__pycache__/util.cpython-310.pyc
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.595610 phables-1.0.0/phables/config/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      438 2023-02-18 10:20:36.000000 phables-1.0.0/phables/config/config.yaml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      533 2023-01-12 05:31:03.000000 phables-1.0.0/phables/config/databases.yaml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      250 2023-05-09 03:49:37.000000 phables-1.0.0/phables/phables.CITATION
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1081 2023-01-12 05:31:03.000000 phables-1.0.0/phables/phables.LICENSE
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        5 2023-05-09 03:49:37.000000 phables-1.0.0/phables/phables.VERSION
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.601223 phables-1.0.0/phables/test_data/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    18772 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/assembly_graph.gfa
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      131 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/edge_coverages.tsv
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      587 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/edges.fasta.hmmout
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      122 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/junction_pe_coverage.pickle
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      272 2023-01-12 06:12:46.000000 phables-1.0.0/phables/test_data/phrogs_annotations.tsv
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     4928 2023-01-13 04:59:11.000000 phables-1.0.0/phables/util.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.603991 phables-1.0.0/phables/workflow/
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.608516 phables-1.0.0/phables/workflow/envs/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       59 2023-02-06 06:39:30.000000 phables-1.0.0/phables/workflow/envs/curl.yaml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       77 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/envs/mapping.yaml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       71 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/envs/mmseqs.yaml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      257 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/envs/phables.yaml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       74 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/envs/smg.yaml
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1755 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/install.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1697 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/phables.smk
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.622068 phables-1.0.0/phables/workflow/rules/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      799 2023-02-06 06:39:30.000000 phables-1.0.0/phables/workflow/rules/00_database_preflight.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2161 2023-02-18 10:20:36.000000 phables-1.0.0/phables/workflow/rules/02_phables_preflight.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1189 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/rules/02_phables_targets.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      920 2023-02-16 05:28:06.000000 phables-1.0.0/phables/workflow/rules/03_test_preflight.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      592 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/rules/03_test_targets.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3343 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/rules/coverage.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2280 2023-04-21 05:14:19.000000 phables-1.0.0/phables/workflow/rules/genes.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      569 2023-02-06 06:39:30.000000 phables-1.0.0/phables/workflow/rules/gfa2fasta.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      898 2023-04-21 05:14:19.000000 phables-1.0.0/phables/workflow/rules/mapping.smk
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1172 2023-02-16 05:28:06.000000 phables-1.0.0/phables/workflow/rules/phables.smk
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.625098 phables-1.0.0/phables/workflow/scripts/
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     2618 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/combine_cov.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     3358 2023-02-19 03:24:59.000000 phables-1.0.0/phables/workflow/scripts/gfa2fasta.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    34730 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.637049 phables-1.0.0/phables/workflow/scripts/phables_utils/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     8077 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/FD_Inexact.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/__init__.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2591 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/component_utils.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3413 2023-02-16 05:28:07.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/coverage_utils.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6480 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/edge_graph_utils.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1760 2023-02-16 05:28:07.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/flow_utils.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2930 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/gene_utils.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1828 2023-04-21 05:14:19.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/genome_utils.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5427 2023-04-21 06:05:21.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/output_utils.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.638106 phables-1.0.0/phables/workflow/scripts/phables_utils/phrogs/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)  3831481 2023-01-12 05:31:03.000000 phables-1.0.0/phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2549 2023-05-09 03:49:37.000000 phables-1.0.0/phables/workflow/test_phables.smk
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.591350 phables-1.0.0/phables.egg-info/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    11079 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2821 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/SOURCES.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/dependency_links.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       50 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/entry_points.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       43 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/requires.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        8 2023-05-09 03:51:30.000000 phables-1.0.0/phables.egg-info/top_level.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)   434479 2023-01-10 00:17:29.000000 phables-1.0.0/phables_logo.png
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-05-09 03:51:30.701782 phables-1.0.0/setup.cfg
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1427 2023-05-09 03:49:37.000000 phables-1.0.0/setup.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-09 03:51:30.697838 phables-1.0.0/tests/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1318 2023-02-19 03:24:59.000000 phables-1.0.0/tests/test_phables.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.065558 phables-1.1.0/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1079 2023-05-16 00:12:10.000000 phables-1.1.0/LICENSE
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      125 2023-05-16 00:12:10.000000 phables-1.1.0/MANIFEST.in
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    11234 2023-07-16 03:45:22.065135 phables-1.1.0/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10583 2023-07-15 23:20:16.000000 phables-1.1.0/README.md
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.027908 phables-1.1.0/phables/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-07-16 03:43:56.000000 phables-1.1.0/phables/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-16 00:12:10.000000 phables-1.1.0/phables/__init__.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     7650 2023-07-15 23:20:16.000000 phables-1.1.0/phables/__main__.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.030993 phables-1.1.0/phables/config/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      462 2023-07-15 23:20:16.000000 phables-1.1.0/phables/config/config.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      533 2023-05-16 00:12:10.000000 phables-1.1.0/phables/config/databases.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      250 2023-05-16 00:12:10.000000 phables-1.1.0/phables/phables.CITATION
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1081 2023-05-16 00:12:10.000000 phables-1.1.0/phables/phables.LICENSE
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        5 2023-07-15 23:20:16.000000 phables-1.1.0/phables/phables.VERSION
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.033072 phables-1.1.0/phables/test_data/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    18772 2023-05-16 00:12:10.000000 phables-1.1.0/phables/test_data/assembly_graph.gfa
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      131 2023-05-16 00:12:10.000000 phables-1.1.0/phables/test_data/edge_coverages.tsv
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      587 2023-05-16 00:12:10.000000 phables-1.1.0/phables/test_data/edges.fasta.hmmout
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      122 2023-05-16 00:12:10.000000 phables-1.1.0/phables/test_data/junction_pe_coverage.pickle
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      272 2023-05-16 00:12:10.000000 phables-1.1.0/phables/test_data/phrogs_annotations.tsv
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     4928 2023-05-16 00:12:10.000000 phables-1.1.0/phables/util.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.034974 phables-1.1.0/phables/workflow/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-07-16 03:43:56.000000 phables-1.1.0/phables/workflow/.DS_Store
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.037284 phables-1.1.0/phables/workflow/envs/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       59 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/envs/curl.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      101 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/envs/koverage.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       77 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/envs/mapping.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       71 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/envs/mmseqs.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      298 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/envs/phables.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       74 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/envs/smg.yaml
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1755 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/install.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1696 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/phables.smk
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.041778 phables-1.1.0/phables/workflow/rules/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      799 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/rules/00_database_preflight.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1784 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/rules/02_phables_preflight.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1200 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/rules/02_phables_targets.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      963 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/rules/03_test_preflight.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      592 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/rules/03_test_targets.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1650 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/rules/coverage.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2280 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/rules/genes.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      569 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/rules/gfa2fasta.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      939 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/rules/mapping.smk
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1213 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/rules/phables.smk
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.043298 phables-1.1.0/phables/workflow/scripts/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-07-16 03:43:56.000000 phables-1.1.0/phables/workflow/scripts/.DS_Store
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     2618 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/scripts/combine_cov.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     3358 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/scripts/gfa2fasta.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    42473 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/scripts/phables.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.047464 phables-1.1.0/phables/workflow/scripts/phables_utils/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-07-16 03:43:51.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     8167 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/FD_Inexact.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/__init__.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2972 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/component_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     3525 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/coverage_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     7229 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/edge_graph_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2488 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/flow_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2930 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/gene_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1828 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/genome_utils.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5427 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/output_utils.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.047893 phables-1.1.0/phables/workflow/scripts/phables_utils/phrogs/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)  3831481 2023-05-16 00:12:10.000000 phables-1.1.0/phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2675 2023-07-15 23:20:16.000000 phables-1.1.0/phables/workflow/test_phables.smk
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-07-16 03:45:22.030205 phables-1.1.0/phables.egg-info/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    11234 2023-07-16 03:45:21.000000 phables-1.1.0/phables.egg-info/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     2111 2023-07-16 03:45:21.000000 phables-1.1.0/phables.egg-info/SOURCES.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-07-16 03:45:21.000000 phables-1.1.0/phables.egg-info/dependency_links.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       50 2023-07-16 03:45:21.000000 phables-1.1.0/phables.egg-info/entry_points.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       43 2023-07-16 03:45:21.000000 phables-1.1.0/phables.egg-info/requires.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        8 2023-07-16 03:45:21.000000 phables-1.1.0/phables.egg-info/top_level.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-07-16 03:45:22.065684 phables-1.1.0/setup.cfg
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1426 2023-07-15 23:20:16.000000 phables-1.1.0/setup.py
```

### Comparing `phables-1.0.0/LICENSE` & `phables-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/PKG-INFO` & `phables-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phables
-Version: 1.0.0
+Version: 1.1.0
 Summary: Phables: from fragmented assemblies to high-quality bacteriophage genomes
 Home-page: https://github.com/Vini2/phables
 Author: Vijini Mallawaarachchi
 Author-email: viji.mallawaarachchi@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,24 +18,26 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/Vini2/phables/master/phables_logo.png" width="600" title="phables logo" alt="phables logo">
 </p>
 
 Phables: from fragmented assemblies to high-quality bacteriophage genomes
 ===============
 
-[![CI](https://github.com/Vini2/phables/actions/workflows/testing.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/testing.yml)
+[![](https://img.shields.io/static/v1?label=CLI&message=Snaketool&color=blueviolet)](https://github.com/beardymcjohnface/Snaketool)
 ![GitHub](https://img.shields.io/github/license/Vini2/phables)
-[![DOI](https://zenodo.org/badge/516191931.svg)](https://zenodo.org/badge/latestdoi/516191931)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/phables/badges/version.svg)](https://anaconda.org/bioconda/phables)
+![Conda](https://img.shields.io/conda/dn/bioconda/phables)
 [![PyPI version](https://badge.fury.io/py/phables.svg)](https://badge.fury.io/py/phables)
-[![Anaconda-Server Badge](https://anaconda.org/bioconda/phables/badges/downloads.svg)](https://anaconda.org/bioconda/phables)
+[![Downloads](https://static.pepy.tech/badge/phables)](https://pepy.tech/project/phables)
+
+[![CI](https://github.com/Vini2/phables/actions/workflows/testing.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/testing.yml)
 [![CodeQL](https://github.com/Vini2/phables/actions/workflows/codeql.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/codeql.yml)
 [![Documentation Status](https://readthedocs.org/projects/phables/badge/?version=latest)](https://phables.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/516191931.svg)](https://zenodo.org/badge/latestdoi/516191931)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Phables is a tool developed to resolve bacteriophage genomes using phage bubbles in viral metagenomic data. It models cyclic phage-like components in the viral metagenomic assembly as flow networks, models as a minimum flow decomposition problem and resolves genomic paths corresponding to flow paths determined. Phables uses the [Minimum Flow Decomposition via Integer Linear Programming](https://github.com/algbio/MFD-ILP) implementation to obtain the flow paths.
 
 For detailed instructions on installation and usage, please refer to the [**documentation hosted at Read the Docs**](https://phables.readthedocs.io/en/latest/).
 
 **NEW:** Phables is now available on bioconda at [https://anaconda.org/bioconda/phables](https://anaconda.org/bioconda/phables) and on PyPI at [https://pypi.org/project/phables/](https://pypi.org/project/phables/). Feel free to pick your package manager, but we recommend that you use [`conda`](https://docs.conda.io/en/latest/).
```

### Comparing `phables-1.0.0/README.md` & `phables-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/Vini2/phables/master/phables_logo.png" width="600" title="phables logo" alt="phables logo">
 </p>
 
 Phables: from fragmented assemblies to high-quality bacteriophage genomes
 ===============
 
-[![CI](https://github.com/Vini2/phables/actions/workflows/testing.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/testing.yml)
+[![](https://img.shields.io/static/v1?label=CLI&message=Snaketool&color=blueviolet)](https://github.com/beardymcjohnface/Snaketool)
 ![GitHub](https://img.shields.io/github/license/Vini2/phables)
-[![DOI](https://zenodo.org/badge/516191931.svg)](https://zenodo.org/badge/latestdoi/516191931)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/phables/badges/version.svg)](https://anaconda.org/bioconda/phables)
+![Conda](https://img.shields.io/conda/dn/bioconda/phables)
 [![PyPI version](https://badge.fury.io/py/phables.svg)](https://badge.fury.io/py/phables)
-[![Anaconda-Server Badge](https://anaconda.org/bioconda/phables/badges/downloads.svg)](https://anaconda.org/bioconda/phables)
+[![Downloads](https://static.pepy.tech/badge/phables)](https://pepy.tech/project/phables)
+
+[![CI](https://github.com/Vini2/phables/actions/workflows/testing.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/testing.yml)
 [![CodeQL](https://github.com/Vini2/phables/actions/workflows/codeql.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/codeql.yml)
 [![Documentation Status](https://readthedocs.org/projects/phables/badge/?version=latest)](https://phables.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/516191931.svg)](https://zenodo.org/badge/latestdoi/516191931)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Phables is a tool developed to resolve bacteriophage genomes using phage bubbles in viral metagenomic data. It models cyclic phage-like components in the viral metagenomic assembly as flow networks, models as a minimum flow decomposition problem and resolves genomic paths corresponding to flow paths determined. Phables uses the [Minimum Flow Decomposition via Integer Linear Programming](https://github.com/algbio/MFD-ILP) implementation to obtain the flow paths.
 
 For detailed instructions on installation and usage, please refer to the [**documentation hosted at Read the Docs**](https://phables.readthedocs.io/en/latest/).
 
 **NEW:** Phables is now available on bioconda at [https://anaconda.org/bioconda/phables](https://anaconda.org/bioconda/phables) and on PyPI at [https://pypi.org/project/phables/](https://pypi.org/project/phables/). Feel free to pick your package manager, but we recommend that you use [`conda`](https://docs.conda.io/en/latest/).
```

### Comparing `phables-1.0.0/phables/__main__.py` & `phables-1.1.0/phables/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     required=False,
     help="minimum length of circular unitigs to consider",
     type=int,
     show_default=True,
 )
 @click.option(
     "--mincov",
-    default=1,
+    default=10,
     required=False,
     help="minimum coverage of paths to output",
     type=int,
     show_default=True,
 )
 @click.option(
     "--compcount",
@@ -183,25 +183,43 @@
     "--seqidentity",
     default=0.3,
     required=False,
     help="minimum sequence identity for phrog annotations",
     type=float,
     show_default=True,
 )
+@click.option(
+    "--covtol",
+    default=100,
+    required=False,
+    help="coverage tolerance for extending subpaths",
+    type=int,
+    show_default=True,
+)
+@click.option(
+    "--alpha",
+    default=1.2,
+    required=False,
+    help="coverage multipler for flow interval modelling",
+    type=float,
+    show_default=True,
+)
 @common_options
 def run(
     input,
     reads,
     minlength,
     mincov,
     compcount,
     maxpaths,
     mgfrac,
     evalue,
     seqidentity,
+    covtol,
+    alpha,
     output,
     log,
     **kwargs
 ):
     """Run Phables"""
     # Config to add or update in configfile
     merge_config = {
@@ -210,14 +228,16 @@
         "minlength": minlength,
         "mincov": mincov,
         "compcount": compcount,
         "maxpaths": maxpaths,
         "mgfrac": mgfrac,
         "evalue": evalue,
         "seqidentity": seqidentity,
+        "covtol": covtol,
+        "alpha": alpha,
         "output": output,
         "log": log,
     }
 
     # run!
     run_snakemake(
         # Full path to Snakefile
```

### Comparing `phables-1.0.0/phables/config/databases.yaml` & `phables-1.1.0/phables/config/databases.yaml`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/phables.LICENSE` & `phables-1.1.0/phables/phables.LICENSE`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/test_data/assembly_graph.gfa` & `phables-1.1.0/phables/test_data/assembly_graph.gfa`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/test_data/edges.fasta.hmmout` & `phables-1.1.0/phables/test_data/edges.fasta.hmmout`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/util.py` & `phables-1.1.0/phables/util.py`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/install.smk` & `phables-1.1.0/phables/workflow/install.smk`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/phables.smk` & `phables-1.1.0/phables/workflow/phables.smk`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 target_rules = []
 
 def targetRule(fn):
     assert fn.__name__.startswith("__")
     target_rules.append(fn.__name__[2:])
     return fn
 
-localrules: all, preprocess, phables, print_stages, rpkm_coverage
+localrules: all, preprocess, phables, print_stages, koverage_tsv
 
 
 """Run stages"""
 @targetRule
 rule all:
     input:
         preprocessTargets,
```

### Comparing `phables-1.0.0/phables/workflow/rules/00_database_preflight.smk` & `phables-1.1.0/phables/workflow/rules/00_database_preflight.smk`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/rules/02_phables_preflight.smk` & `phables-1.1.0/phables/workflow/rules/02_phables_preflight.smk`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Add your preflight checks as pure Python code here.
 e.g. Configure the run, declare directories, validate the input files etc.
 This preflight check to confirm the database filepaths 
 """
 
+from metasnek import fastq_finder
 
 """
 Setting the directory variables
 """
 
 # THREADS = config['threads']
 INPUT = config['input']
@@ -15,42 +16,30 @@
 print(f"Output files will be saved to directory, {OUTDIR}\n")
 
 
 ############################################################################
 # Checking through the reads folder
 ############################################################################
 
-READ_DIR = config['reads']
-SAMPLES,EXTENSIONS, = glob_wildcards(os.path.join(READ_DIR, '{sample}_R1{extn}'))
-
-# Check if there are read files
-if len(SAMPLES) == 0:
-    sys.stderr.write("ERROR: Could not find any FASTQ files in {READ_DIR}. Please check the reads path.\n")
-    sys.exit(0)
-
-if len(set(EXTENSIONS)) != 1:
-    sys.stderr.write("ERROR: You have more than one type of file extension. Please make sure that you have the same file extension.\n")
-    sys.exit(0)
-
-FQEXTN = EXTENSIONS[0]
-PATTERN_R1 = '{sample}_R1' + FQEXTN
-PATTERN_R2 = '{sample}_R2' + FQEXTN
-
+SAMPLE_READS = fastq_finder.parse_samples_to_dictionary(config['reads'])
+SAMPLE_NAMES = list(SAMPLE_READS.keys())
 
 
 ############################################################################
 # Get Phables parameters
 ############################################################################
 ML = config['minlength']
 MC = config['mincov']
 CC = config['compcount']
 MP = config['maxpaths']
 MGF = config['mgfrac']
 EV = config['evalue']
 SI = config['seqidentity']
+CT = config['covtol']
+AL = config['alpha']
 
 
 """DIRECTORIES/FILES etc.
 Declare some directories for pipeline intermediates and outputs.
 """
 LOGSDIR = os.path.join(OUTDIR, 'logs')
```

### Comparing `phables-1.0.0/phables/workflow/rules/02_phables_targets.smk` & `phables-1.1.0/phables/workflow/rules/02_phables_targets.smk`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 phablesTargets = []
 
 
 """PREPROCESSING TARGETS"""
 EDGES_FILE = os.path.join(OUTDIR, "edges.fasta")
 preprocessTargets.append(EDGES_FILE)
 
-BAM_PATH = os.path.join(OUTDIR, 'bam_files/')
-preprocessTargets.append(expand(os.path.join(BAM_PATH, "{sample}.bam"), sample=SAMPLES))
-preprocessTargets.append(expand(os.path.join(BAM_PATH, "{sample}.bam.bai"), sample=SAMPLES))
+BAM_PATH = os.path.join(OUTDIR, 'temp')
+preprocessTargets.append(expand(os.path.join(BAM_PATH, "{sample}.bam"), sample=SAMPLE_NAMES))
+preprocessTargets.append(expand(os.path.join(BAM_PATH, "{sample}.bam.bai"), sample=SAMPLE_NAMES))
 
 COVERAGE_PATH = os.path.join(OUTDIR, 'coverage_rpkm/')
-preprocessTargets.append(expand(os.path.join(COVERAGE_PATH, "{sample}_rpkm.tsv"), sample=SAMPLES))
+# preprocessTargets.append(expand(os.path.join(COVERAGE_PATH, "{sample}_rpkm.tsv"), sample=SAMPLE_NAMES))
 preprocessTargets.append(os.path.join(OUTDIR, "coverage.tsv"))
 preprocessTargets.append(os.path.join(OUTDIR, "edges.fasta.hmmout"))
 
 preprocessTargets.append(os.path.join(OUTDIR, "phrogs_annotations.tsv"))
 
 
 """MISC"""
```

### Comparing `phables-1.0.0/phables/workflow/rules/03_test_preflight.smk` & `phables-1.1.0/phables/workflow/rules/03_test_preflight.smk`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 ML = config['minlength']
 MC = config['mincov']
 CC = config['compcount']
 MP = config['maxpaths']
 MGF = config['mgfrac']
 EV = config['evalue']
 SI = config['seqidentity']
+CT = config['covtol']
+AL = config['alpha']
 
 
 """ONSTART/END/ERROR
 Tasks to perform at various stages the start and end of a run.
 """
 onsuccess:
     """Print a success message"""
```

### Comparing `phables-1.0.0/phables/workflow/rules/03_test_targets.smk` & `phables-1.1.0/phables/workflow/rules/03_test_targets.smk`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/rules/genes.smk` & `phables-1.1.0/phables/workflow/rules/genes.smk`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/rules/gfa2fasta.smk` & `phables-1.1.0/phables/workflow/rules/gfa2fasta.smk`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/rules/mapping.smk` & `phables-1.1.0/phables/workflow/rules/mapping.smk`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Use Minimap2 to map the reads of all the samples to unitigs in the edges.fasta 
 file from step 2 and Samtools to index the BAM files.
 """
 
-rule map_reads_to_unitigs:
-    input:
-        edges = EDGES_FILE,
-        r1 = os.path.join(READ_DIR, PATTERN_R1),
-        r2 = os.path.join(READ_DIR, PATTERN_R2)
-    output:
-        bam = os.path.join(BAM_PATH, "{sample}.bam"),
-        index = os.path.join(BAM_PATH, "{sample}.bam.bai")
-    threads:
-        config["resources"]["jobCPU"]
-    resources:
-        mem_mb = config["resources"]["jobMem"]
-    log:
-        os.path.join(LOGSDIR, "{sample}_mapping.log")
-    conda: 
-        os.path.join("..", "envs", "mapping.yaml")
-    shell:
-        """
-            minimap2 -t {threads} -N 5 -ax sr {input.edges} {input.r1} {input.r2} | samtools sort -@ {threads} > {output.bam}
-            samtools index -@ {threads} {output.bam} {output.index}
-        """
+# rule map_reads_to_unitigs:
+#     input:
+#         edges = EDGES_FILE,
+#         r1 = os.path.join(READ_DIR, PATTERN_R1),
+#         r2 = os.path.join(READ_DIR, PATTERN_R2)
+#     output:
+#         bam = os.path.join(BAM_PATH, "{sample}.bam"),
+#         index = os.path.join(BAM_PATH, "{sample}.bam.bai")
+#     threads:
+#         config["resources"]["jobCPU"]
+#     resources:
+#         mem_mb = config["resources"]["jobMem"]
+#     log:
+#         os.path.join(LOGSDIR, "{sample}_mapping.log")
+#     conda:
+#         os.path.join("..", "envs", "mapping.yaml")
+#     shell:
+#         """
+#             minimap2 -t {threads} -N 5 -ax sr {input.edges} {input.r1} {input.r2} | samtools sort -@ {threads} > {output.bam}
+#             samtools index -@ {threads} {output.bam} {output.index}
+#         """
```

### Comparing `phables-1.0.0/phables/workflow/rules/phables.smk` & `phables-1.1.0/phables/workflow/rules/phables.smk`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         minlength = ML,
         mincov = MC,
         compcount = CC,
         maxpaths = MP,
         mgfrac = MGF,
         evalue = EV,
         seqidentity = SI,
+        covtol = CT,
+        alpha = AL,
         output = OUTDIR,
         log = os.path.join(LOGSDIR, "phables_output.log")
     log:
         os.path.join(LOGSDIR, "phables_output.log")
     conda:
         os.path.join("..", "envs", "phables.yaml")
     script:
```

### Comparing `phables-1.0.0/phables/workflow/scripts/combine_cov.py` & `phables-1.1.0/phables/workflow/scripts/combine_cov.py`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/scripts/gfa2fasta.py` & `phables-1.1.0/phables/workflow/scripts/gfa2fasta.py`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/scripts/phables.py` & `phables-1.1.0/phables/workflow/scripts/phables.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     write_unitigs,
 )
 from tqdm import tqdm
 
 __author__ = "Vijini Mallawaarachchi"
 __copyright__ = "Copyright 2022, Phables Project"
 __license__ = "MIT"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __maintainer__ = "Vijini Mallawaarachchi"
 __email__ = "viji.mallawaarachchi@gmail.com"
 __status__ = "Development"
 
 MAX_VAL = sys.maxsize
 LEN_THRESHOLD = 0.95
 
@@ -45,14 +45,16 @@
     minlength = int(snakemake.params.minlength)
     mincov = int(snakemake.params.mincov)
     compcount = int(snakemake.params.compcount)
     maxpaths = int(snakemake.params.maxpaths)
     mgfrac = float(snakemake.params.mgfrac)
     evalue = float(snakemake.params.evalue)
     seqidentity = float(snakemake.params.seqidentity)
+    covtol = float(snakemake.params.covtol)
+    alpha = float(snakemake.params.alpha)
     output = snakemake.params.output
     log = snakemake.params.log
 
     # Setup logger
     # ----------------------------------------------------------------------
 
     logger = logging.getLogger(__version__)
@@ -86,52 +88,55 @@
     logger.info(f"Minimum length of unitigs to consider: {minlength}")
     logger.info(f"Minimum coverage of paths to output: {mincov}")
     logger.info(f"Minimum unitig count to consider a component: {compcount}")
     logger.info(f"Maximum number of paths to resolve for a component: {maxpaths}")
     logger.info(f"Length threshold to consider single copy marker genes: {mgfrac}")
     logger.info(f"Maximum e-value for phrog annotations: {evalue}")
     logger.info(f"Minimum sequence identity for phrog annotations: {seqidentity}")
+    logger.info(f"Coverage tolerance for extending subpaths: {covtol}")
+    logger.info(f"Coverage multipler for flow interval modelling: {alpha}")
     logger.info(f"Output folder: {output}")
 
     start_time = time.time()
 
     # Get assembly graph
     # ----------------------------------------------------------------------
     (
         assembly_graph,
         oriented_links,
+        link_overlap,
         unitig_names,
         unitig_names_rev,
         graph_unitigs,
         self_looped_nodes,
         edges_lengths,
     ) = edge_graph_utils.build_assembly_graph(graph)
 
     logger.info(
         f"Total number of vertices in the assembly graph: {len(assembly_graph.vs)}"
     )
     logger.info(
         f"Total number of links in the assembly graph: {len(assembly_graph.es)}"
     )
 
-    # Get circular unitigs
+    # Get single unitigs
     # ----------------------------------------------------------------------
     circular = edge_graph_utils.get_circular(self_looped_nodes, graph_unitigs)
 
     # Get unitigs with bacterial single copy marker genes
     # ----------------------------------------------------------------------
     smg_unitigs = gene_utils.get_smg_unitigs(hmmout, mgfrac)
 
     # Get unitigs with PHROGs
     # ----------------------------------------------------------------------
     unitig_phrogs, phrog_dict = gene_utils.get_phrog_unitigs(
         phrogs, evalue, seqidentity
     )
 
-    # Get components with viral bubbles
+    # Get components with viral components
     # ----------------------------------------------------------------------
     pruned_vs, comp_phrogs = component_utils.get_components(
         assembly_graph,
         unitig_names,
         smg_unitigs,
         unitig_phrogs,
         circular,
@@ -153,16 +158,18 @@
     resolved_edges = set()
 
     all_resolved_paths = []
 
     all_components = []
 
     cycle_components = set()
+    linear_components = set()
     resolved_components = set()
-    circular_unitigs = set()
+    resolved_linear = set()
+    single_unitigs = set()
     resolved_cyclic = set()
 
     case1_found = set()
     case1_resolved = set()
     case2_found = set()
     case2_resolved = set()
     case3_found = set()
@@ -245,24 +252,24 @@
                         unitig_to_consider = unitig2
                         unitig_name = unitig2_name
                         repeat_unitig = unitig1
                         repeat_unitig_name = unitig1_name
 
                     if unitig_to_consider != -1:
                         logger.debug(
-                            f"Case 2 bubble: {unitig1_name} is {unitig1_len} bp long and {unitig2_name} is {unitig2_len} bp long."
+                            f"Case 2 component: {unitig1_name} is {unitig1_len} bp long and {unitig2_name} is {unitig2_len} bp long."
                         )
                         cycle_number = 1
                         resolved_edges.add(unitig_to_consider)
                         resolved_edges.add(repeat_unitig)
                         path_string = (
                             str(graph_unitigs[repeat_unitig_name])
-                            + str(graph_unitigs[unitig_name])
+                            + str(graph_unitigs[unitig_name][link_overlap[(repeat_unitig, unitig_to_consider)]:])
                             + str(
-                                graph_unitigs[repeat_unitig_name].reverse_complement()
+                                graph_unitigs[repeat_unitig_name].reverse_complement()[link_overlap[(unitig_to_consider, repeat_unitig)]:]
                             )
                         )
                         logger.debug(
                             f"Terminal repeat detected is {repeat_unitig_name}"
                         )
 
                         genome_path = GenomePath(
@@ -297,17 +304,26 @@
             node_indices = {}
             node_indices_rev = {}
 
             cycle_edges = {}
 
             clean_node_count = 0
 
+            max_comp_cov = -1
+
             for vertex in pruned_graph.vs["id"]:
                 unitig_name = unitig_names[vertex]
 
+                # Find the maximum coverage within the component
+                if (
+                    unitig_name in unitig_coverages
+                    and unitig_coverages[unitig_name] > max_comp_cov
+                ):
+                    max_comp_cov = unitig_coverages[unitig_name]
+
                 if unitig_name not in self_looped_nodes:
                     clean_node_count += 1
 
                 for node in oriented_links[unitig_name]:
                     consider_edge = False
 
                     if not (
@@ -320,15 +336,18 @@
                         cov_2 = MAX_VAL
 
                         if unitig_name in unitig_coverages:
                             cov_1 = unitig_coverages[unitig_name]
                         if node in unitig_coverages:
                             cov_2 = unitig_coverages[node]
 
-                        min_cov = min([cov_1, cov_2])
+                        if min([cov_1, cov_2]) != 0:
+                            min_cov = min([cov_1, cov_2])
+                        else:
+                            min_cov = max([cov_1, cov_2])
 
                         for edge in oriented_links[unitig_name][node]:
                             cycle_edges[(unitig_name + edge[0], node + edge[1])] = int(
                                 min_cov
                             )
 
             logger.debug(f"clean_node_count: {clean_node_count}")
@@ -367,15 +386,15 @@
                     G_edge.remove_nodes_from(dead_ends_to_remove)
 
                     logger.debug(f"Dead-ends found and removed: {dead_ends_to_remove}")
 
                 # Identify source/sink vertex
                 # ----------------------------------------------------------------------
 
-                source_sink_candidates = flow_utils.get_source_sink(
+                source_sink_candidates = flow_utils.get_source_sink_circular(
                     G_edge, graph_unitigs, minlength, self_looped_nodes
                 )
 
                 source_sink = 0
 
                 logger.debug(f"Original candidate_nodes: {candidate_nodes}")
                 logger.debug(
@@ -470,75 +489,167 @@
                 logger.debug(f"G_edge.nodes: {list(G_edge.nodes)}")
                 logger.debug(f"G_edge.edges: {G_edge.edges(data=True)}")
 
                 for u, v, cov in G_edge.edges(data=True):
                     u_name = unitig_names_rev[u[:-1]]
                     v_name = unitig_names_rev[v[:-1]]
 
-                    original_edge = (u[:-1], v[:-1])
-                    rev_original_edge = (v[:-1], u[:-1])
-
                     u_index = candidate_nodes.index(u_name)
                     v_index = candidate_nodes.index(v_name)
 
                     edge_list_indices[u_index] = u
                     edge_list_indices[v_index] = v
 
                     juction_cov = junction_pe_coverage[(u[:-1], v[:-1])]
 
                     if v_index == 0:
-                        if (u_index, len(candidate_nodes)) not in visited_edges and (
-                            len(candidate_nodes),
-                            u_index,
-                        ) not in visited_edges:
-                            if juction_cov < cov["weight"]:
-                                network_edges.append(
-                                    (
-                                        u_index,
-                                        len(candidate_nodes),
-                                        juction_cov,
-                                        cov["weight"],
-                                    )
-                                )
-                            else:
-                                network_edges.append(
-                                    (u_index, len(candidate_nodes), 0, cov["weight"])
-                                )
+                        final_vertex = len(candidate_nodes)
+                    else:
+                        final_vertex = v_index
 
-                            visited_edges.append((u_index, len(candidate_nodes)))
+                    if (u_index, final_vertex) not in visited_edges and (
+                        final_vertex,
+                        u_index,
+                    ) not in visited_edges:
+                        # Get coverage interval
+                        cov_lower_bound = cov["weight"]
+                        cov_upper_bound = int(max_comp_cov * alpha)
 
-                            if juction_cov != 0:
-                                subpaths[subpath_count] = [
+                        logger.debug(
+                            f"({v}, {u}), {juction_cov}, {cov_lower_bound}, {cov_upper_bound}"
+                        )
+
+                        if juction_cov == 0:
+                            network_edges.append(
+                                (u_index, final_vertex, 0, cov_upper_bound)
+                            )
+                        else:
+                            network_edges.append(
+                                (
                                     u_index,
-                                    len(candidate_nodes),
-                                ]
-                                subpath_count += 1
-                    else:
-                        if (u_index, v_index) not in visited_edges and (
-                            v_index,
-                            u_index,
-                        ) not in visited_edges:
-                            cov_upper_bound = cov["weight"]
-
-                            if juction_cov <= cov_upper_bound:
-                                network_edges.append(
-                                    (u_index, v_index, juction_cov, cov_upper_bound)
-                                )
-                            else:
-                                network_edges.append(
-                                    (u_index, v_index, 0, cov_upper_bound)
+                                    final_vertex,
+                                    cov_lower_bound,
+                                    cov_upper_bound,
                                 )
+                            )
+
+                        visited_edges.append((u_index, final_vertex))
+
+                        # Add subpaths
+                        if juction_cov >= mincov:
+                            logger.debug(f"Adding subpath {[u_index, final_vertex]}")
+                            subpaths[subpath_count] = [u_index, final_vertex]
+                            subpath_count += 1
+
+                            # Extend subpaths using coverages of successors and predecessors
+                            u_pred = [x for x in G_edge.predecessors(u)]
+                            v_succ = [x for x in G_edge.successors(v)]
+
+                            # Extend subpath using coverages of predecessors
+                            for u_pred in G_edge.predecessors(u):
+                                u_pred_name = unitig_names_rev[u_pred[:-1]]
+                                u_pred_index = candidate_nodes.index(u_pred_name)
+                                u_pred_cov = unitig_coverages[u_pred[:-1]]
+                                u_cov = unitig_coverages[u[:-1]]
+
+                                if (
+                                    final_vertex != 0
+                                    and u_index != 0
+                                    and u_pred_index != final_vertex
+                                ):
+                                    if (
+                                        abs(min(u_pred_cov, u_cov) - cov["weight"])
+                                        < covtol
+                                    ):
+                                        subpaths[subpath_count] = [
+                                            u_pred_index,
+                                            u_index,
+                                            final_vertex,
+                                        ]
+                                        logger.debug(
+                                            f"Extending subpath based on predecessor coverage {[u_pred_index, u_index, final_vertex]}"
+                                        )
+                                        subpath_count += 1
 
-                            visited_edges.append((u_index, v_index))
+                            # Extend subpath using coverages of successors
+                            for v_succ in G_edge.successors(v):
+                                v_succ_name = unitig_names_rev[v_succ[:-1]]
+                                v_succ_index = candidate_nodes.index(v_succ_name)
+                                v_succ_cov = unitig_coverages[v_succ[:-1]]
+                                v_cov = unitig_coverages[v[:-1]]
+
+                                if (
+                                    v_succ_index != 0
+                                    and u_index != 0
+                                    and final_vertex != 0
+                                    and final_vertex != len(candidate_nodes)
+                                    and v_succ_index != u_index
+                                ):
+                                    if (
+                                        abs(min(v_succ_cov, v_cov) - cov["weight"])
+                                        < covtol
+                                    ):
+                                        subpaths[subpath_count] = [
+                                            u_index,
+                                            final_vertex,
+                                            v_succ_index,
+                                        ]
+                                        logger.debug(
+                                            f"Extending subpath based on successor coverage {[u_index, final_vertex, v_succ_index]}"
+                                        )
+                                        subpath_count += 1
 
-                            if juction_cov != 0:
-                                subpaths[subpath_count] = [u_index, v_index]
-                                subpath_count += 1
+                        else:
+                            # Extend subpaths of l=3 based on paired-end reads
+                            # aligned to successors and predecessors
+                            u_pred = [x for x in G_edge.predecessors(u)]
+                            v_succ = [x for x in G_edge.successors(v)]
+
+                            for u_pred in G_edge.predecessors(u):
+                                if junction_pe_coverage[(u_pred[:-1], v[:-1])] > 0:
+                                    u_pred_name = unitig_names_rev[u_pred[:-1]]
+                                    u_pred_index = candidate_nodes.index(u_pred_name)
+                                    if (
+                                        final_vertex != 0
+                                        and u_index != 0
+                                        and u_pred_index != final_vertex
+                                    ):
+                                        subpaths[subpath_count] = [
+                                            u_pred_index,
+                                            u_index,
+                                            final_vertex,
+                                        ]
+                                        logger.debug(
+                                            f"Extending subpath {[u_pred_index, u_index, final_vertex]}"
+                                        )
+                                        subpath_count += 1
+
+                            for v_succ in G_edge.successors(v):
+                                if junction_pe_coverage[(u[:-1], v_succ[:-1])] > 0:
+                                    v_succ_name = unitig_names_rev[v_succ[:-1]]
+                                    v_succ_index = candidate_nodes.index(v_succ_name)
+                                    if (
+                                        v_succ_index != 0
+                                        and u_index != 0
+                                        and final_vertex != 0
+                                        and final_vertex != len(candidate_nodes)
+                                        and v_succ_index != u_index
+                                    ):
+                                        subpaths[subpath_count] = [
+                                            u_index,
+                                            final_vertex,
+                                            v_succ_index,
+                                        ]
+                                        logger.debug(
+                                            f"Extending subpath {[u_index, final_vertex, v_succ_index]}"
+                                        )
+                                        subpath_count += 1
 
                 logger.debug(f"edge_list_indices: {edge_list_indices}")
+                logger.debug(f"subpaths: {subpaths}")
 
                 # Create flow network and run MFD-ILP
                 # ----------------------------------------------------------------------
                 G_mfd = {
                     "Nodes": len(list(G_edge.nodes)),
                     "list of edges": network_edges,
                     "subpaths": subpaths,
@@ -558,131 +669,158 @@
                     )
 
                     cycle_number = 1
 
                     for solution_path in solution_paths:
                         coverage_val = solution_paths[solution_path]["weight"]
 
-                        logger.debug(f"Path {cycle_number} coverage: {coverage_val}")
-
                         # Filter path by coverage
                         if coverage_val >= mincov:
+                            logger.debug(
+                                f"Path {cycle_number} coverage: {coverage_val}"
+                            )
+
                             # Create graph for path
                             G_path = nx.DiGraph()
 
                             # Fill graph with data
                             G_path.add_edges_from(solution_paths[solution_path]["path"])
                             logger.debug(
                                 f"solution path: {solution_paths[solution_path]['path']}"
                             )
 
                             if 0 in list(G_path.nodes):
                                 # Get all simple paths from node 0 to last node
-                                candidate_paths = list(
-                                    nx.all_simple_paths(G_path, 0, len(candidate_nodes))
-                                )
-
-                                if len(candidate_paths) > 0:
-                                    logger.debug(
-                                        f"candidate_paths: {candidate_paths[0]}"
+                                try:
+                                    candidate_paths = list(
+                                        nx.all_simple_paths(
+                                            G_path, 0, len(candidate_nodes)
+                                        )
                                     )
 
-                                    # Get mapped unitigs in order from the flow network
-                                    path_order = []
-                                    for path_edge in candidate_paths[0]:
-                                        if path_edge != len(candidate_nodes):
-                                            path_order.append(
-                                                edge_list_indices[path_edge]
-                                            )
-
-                                    logger.debug(f"path_order: {path_order}")
+                                    if len(candidate_paths) > 0:
+                                        logger.debug(
+                                            f"candidate_paths: {candidate_paths[0]}"
+                                        )
 
-                                    # Get the order of unitigs in path
-                                    path_string = ""
-                                    total_length = 0
-
-                                    for node in path_order:
-                                        unitig_name = node[:-1]
-                                        if node.endswith("+"):
-                                            path_string += str(
-                                                graph_unitigs[unitig_name]
-                                            )
-                                        else:
-                                            path_string += str(
-                                                graph_unitigs[
-                                                    unitig_name
-                                                ].reverse_complement()
+                                        # Get mapped unitigs in order from the flow network
+                                        path_order = []
+                                        for path_edge in candidate_paths[0]:
+                                            if path_edge != len(candidate_nodes):
+                                                path_order.append(
+                                                    edge_list_indices[path_edge]
+                                                )
+
+                                        logger.debug(f"path_order: {path_order}")
+
+                                        # Get the order of unitigs in path
+                                        path_string = ""
+                                        total_length = 0
+
+                                        previous_edge = 0
+
+                                        for nodeid in range(len(path_order)):
+                                            node = path_order[nodeid]
+                                            unitig_name = node[:-1]
+
+                                            if node.endswith("+"):
+                                                unitig_seq = str(graph_unitigs[unitig_name])
+                                            else:
+                                                unitig_seq = str(graph_unitigs[unitig_name].reverse_complement())
+
+                                            # If first node in path
+                                            if previous_edge == 0:
+                                                path_string += unitig_seq
+                                                total_length += len(unitig_seq)
+                                            
+                                            else:
+                                                trimmed_seq = unitig_seq[link_overlap[(previous_edge, node)]:]
+                                                path_string += trimmed_seq
+                                                total_length += len(trimmed_seq)
+
+                                            previous_edge = node
+
+                                        # Create GenomePath object with path details
+                                        genome_path = GenomePath(
+                                            f"phage_comp_{my_count}_cycle_{cycle_number}",
+                                            "case3",
+                                            [x for x in path_order],
+                                            [
+                                                unitig_names_rev[x[:-1]]
+                                                for x in path_order
+                                            ],
+                                            path_string,
+                                            int(coverage_val),
+                                            total_length,
+                                            (
+                                                path_string.count("G")
+                                                + path_string.count("C")
                                             )
-                                        total_length += len(
-                                            str(graph_unitigs[unitig_name])
+                                            / len(path_string)
+                                            * 100,
                                         )
+                                        my_genomic_paths.append(genome_path)
+                                        logger.debug(f"total_length: {total_length}")
 
-                                    # Create GenomePath object with path details
-                                    genome_path = GenomePath(
-                                        f"phage_comp_{my_count}_cycle_{cycle_number}",
-                                        "case3",
-                                        [x for x in path_order],
-                                        [unitig_names_rev[x[:-1]] for x in path_order],
-                                        path_string,
-                                        int(coverage_val),
-                                        total_length,
-                                        (
-                                            path_string.count("G")
-                                            + path_string.count("C")
-                                        )
-                                        / len(path_string)
-                                        * 100,
-                                    )
-                                    my_genomic_paths.append(genome_path)
-                                    logger.debug(f"total_length: {total_length}")
+                                        cycle_number += 1
 
-                                    cycle_number += 1
+                                except nx.exception.NodeNotFound:
+                                    logger.debug(
+                                        f"Could not resolve a continuous path."
+                                    )
 
                     logger.debug(f"Number of paths selected: {cycle_number-1}")
 
                     if cycle_number > 1:
                         resolved_components.add(my_count)
                         resolved_cyclic.add(my_count)
                         case3_resolved.add(my_count)
 
                 else:
                     logger.debug(f"No paths detected")
                     continue
 
             else:
-                logger.debug(f"No cycles detected. Maybe a linear component?")
+                logger.debug(f"No cycles detected. Found a complex linear component.")
 
-        # Case 1 components - circular unitigs
+        # Case 1 components - single unitigs
         elif len(candidate_nodes) == 1:
             case1_found.add(my_count)
 
             unitig_name = unitig_names[candidate_nodes[0]]
 
+            case_name = ""
+
+            if unitig_name in self_looped_nodes:
+                case_name = "case1_circular"
+            else:
+                case_name = "case1_linear"
+
             resolved_edges.add(candidate_nodes[0])
 
             path_string = str(graph_unitigs[unitig_name])
 
             cycle_number = 1
 
             # Create GenomePath object with path details
             genome_path = GenomePath(
                 f"phage_comp_{my_count}_cycle_{cycle_number}",
-                "case1",
+                case_name,
                 [unitig_names[candidate_nodes[0]]],
                 [candidate_nodes[0]],
                 path_string,
                 int(unitig_coverages[unitig_name]),
                 len(graph_unitigs[unitig_name]),
                 (path_string.count("G") + path_string.count("C"))
                 / len(path_string)
                 * 100,
             )
             my_genomic_paths.append(genome_path)
             resolved_components.add(my_count)
-            circular_unitigs.add(my_count)
+            single_unitigs.add(my_count)
             case1_resolved.add(my_count)
 
             phage_like_edges = phage_like_edges.union(set(candidate_nodes))
 
         # Record final paths for the component
         # ----------------------------------------------------------------------
 
@@ -693,15 +831,15 @@
         comp_resolved_edges = set()
         visited_nodes = set()
         comp_resolved_paths = set()
 
         frac_unitigs = 1
         n_paths = 0
 
-        if len(my_genomic_paths) > 1:
+        if len(my_genomic_paths) > 0:
             # Get the degree of the component
             graph_degree = assembly_graph.degree(original_candidate_nodes)
 
             path_lengths = []
             path_coverages = []
 
             largest_length = my_genomic_paths[0].length
@@ -731,14 +869,16 @@
                     n_paths += 1
 
                     for path_node in genomic_path.node_id_order:
                         comp_resolved_edges.add(path_node)
 
             frac_unitigs = len(visited_nodes) / len(original_candidate_nodes)
 
+            resolved_edges = resolved_edges.union(comp_resolved_edges)
+
             logger.debug(f"frac_unitigs: {frac_unitigs}")
 
             # Filter components
             if (
                 len(final_genomic_paths) > 1
                 and len(in_degree) > 0
                 and len(out_degree) > 0
@@ -765,27 +905,26 @@
                     / path_lengths[path_coverages.index(min(path_coverages))],
                     max(path_coverages),
                     min(path_coverages),
                     max(path_coverages) / min(path_coverages),
                     frac_unitigs,
                 )
                 all_components.append(genome_comp)
-                resolved_edges = resolved_edges.union(comp_resolved_edges)
 
             if len(final_genomic_paths) > 0:
                 resolved_cyclic.add(my_count)
                 resolved_components.add(my_count)
                 all_resolved_paths += final_genomic_paths
                 component_elapsed_time = time.time() - component_time_start
                 logger.debug(
                     f"Elapsed time to resolve component {my_count} with {len(original_candidate_nodes)} nodes: {component_elapsed_time} seconds"
                 )
 
         else:
-            # Circular unitigs
+            # single unitigs
             for genomic_path in my_genomic_paths:
                 final_genomic_paths.append(genomic_path)
                 all_resolved_paths.append(genomic_path)
                 logger.debug(f"{genomic_path.id}\t{genomic_path.length}")
                 resolved_components.add(my_count)
 
         # Write genome path to file
@@ -793,20 +932,22 @@
         write_path(final_genomic_paths, output)
         write_path_fasta(final_genomic_paths, f"{output}/resolved_phages")
 
     # Log final summary information
     # ----------------------------------------------------------------------
     logger.info(f"Total number of cyclic components found: {len(cycle_components)}")
     logger.info(f"Total number of cyclic components resolved: {len(resolved_cyclic)}")
-    logger.info(f"Circular unitigs identified: {len(circular_unitigs)}")
+    logger.info(f"single unitigs identified: {len(single_unitigs)}")
+    logger.info(f"Total number of linear components found: {len(linear_components)}")
+    logger.info(f"Total number of linear components resolved: {len(resolved_linear)}")
     logger.info(
-        f"Total number of cyclic components found including circular unitigs: {len(cycle_components) + len(circular_unitigs)}"
+        f"Total number of cyclic components found including single unitigs: {len(cycle_components) + len(single_unitigs)}"
     )
     logger.info(
-        f"Total number of components resolved: {len(circular_unitigs)+len(resolved_cyclic)}"
+        f"Total number of components resolved: {len(single_unitigs)+len(resolved_cyclic)+len(resolved_linear)}"
     )
     logger.info(f"Case 1 (resolved/found): {len(case1_resolved)}/{len(case1_found)}")
     logger.info(f"Case 2 (resolved/found): {len(case2_resolved)}/{len(case2_found)}")
     logger.info(f"Case 3 (resolved/found): {len(case3_resolved)}/{len(case3_found)}")
     logger.info(f"Total number of genomes resolved: {len(all_resolved_paths)}")
 
     if len(all_resolved_paths) == 0:
```

### Comparing `phables-1.0.0/phables/workflow/scripts/phables_utils/FD_Inexact.py` & `phables-1.1.0/phables/workflow/scripts/phables_utils/FD_Inexact.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 import more_itertools
 import networkx as nx
 
 # create logger
-logger = logging.getLogger("phables 1.0.0")
+logger = logging.getLogger("phables 1.1.0")
 
 
 def read_input(graphfile, number_subpath):
     trip_data = open(graphfile, "r").read().split("\n")
     i = 0
     listOfGraphs = {}
     k = 0
@@ -112,18 +112,21 @@
                 model.addConstr(w[k] - (1 - x[i, j, k]) * W <= z[i, j, k])
                 model.addConstr(z[i, j, k] <= w[k])
 
         # subpath constraints
         for k in range(0, K):
             for sp_len in range(0, len(subpaths)):
                 subpath_edges = list(more_itertools.pairwise(subpaths[sp_len]))
-                model.addConstr(
-                    gp.quicksum(x[i, j, k] for (i, j) in subpath_edges)
-                    >= len(subpath_edges) * r[k, sp_len]
-                )
+                try:
+                    model.addConstr(
+                        gp.quicksum(x[i, j, k] for (i, j) in subpath_edges)
+                        >= len(subpath_edges) * r[k, sp_len]
+                    )
+                except:
+                    continue
 
         model.addConstrs(
             gp.quicksum(r[k, sp_len] for k in range(0, K)) >= 1
             for sp_len in range(0, len(subpaths))
         )
 
         # objective function
```

### Comparing `phables-1.0.0/phables/workflow/scripts/phables_utils/component_utils.py` & `phables-1.1.0/phables/workflow/scripts/phables_utils/component_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                     break
                 elif unitig_names[unitig] in unitig_phrogs:
                     for phrog in unitig_phrogs[unitig_names[unitig]]:
                         if "head and packaging" in phrog_dict[phrog]:
                             head_present = True
                         if "connector" in phrog_dict[phrog]:
                             connector_present = True
-                        if "portal" in phrog_dict[phrog]:
+                        if "tail" in phrog_dict[phrog]:
                             tail_present = True
                         if "lysis" in phrog_dict[phrog]:
                             lysis_present = True
 
                         phrogs_found.add(phrog)
 
             if head_present or connector_present or tail_present or lysis_present:
@@ -54,27 +54,35 @@
 
             if unitig_names[unitig] in unitig_phrogs:
                 for phrog in unitig_phrogs[unitig_names[unitig]]:
                     if "head and packaging" in phrog_dict[phrog]:
                         head_present = True
                     if "connector" in phrog_dict[phrog]:
                         connector_present = True
-                    if "portal" in phrog_dict[phrog]:
+                    if "tail" in phrog_dict[phrog]:
                         tail_present = True
                     if "lysis" in phrog_dict[phrog]:
                         lysis_present = True
 
                     phrogs_found.add(phrog)
 
-            if head_present or connector_present or tail_present or lysis_present:
-                phrogs_present = True
+            if unitig_names[unitig] in circular:
+                # Check PHROG categories in circular component (should contain at least one)
+                if head_present or connector_present or tail_present or lysis_present:
+                    phrogs_present = True
+
+            else:
+                # Check PHROG categories for circular component (should contain all)
+                if (
+                    head_present
+                    and connector_present
+                    and tail_present
+                    and lysis_present
+                ):
+                    phrogs_present = True
 
-            if (
-                phrogs_present
-                and unitig_names[unitig] in circular
-                and edges_lengths[unitig_names[unitig]] > cicular_len
-            ):
+            if phrogs_present and edges_lengths[unitig_names[unitig]] > cicular_len:
                 pruned_vs[i] = component
                 comp_phrogs[i] = phrogs_found
                 i += 1
 
     return pruned_vs, comp_phrogs
```

### Comparing `phables-1.0.0/phables/workflow/scripts/phables_utils/coverage_utils.py` & `phables-1.1.0/phables/workflow/scripts/phables_utils/coverage_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,20 @@
     """
     Generate read pairs in a BAM file or within a region string.
     Reads are added to read_dict until a pair is found.
     """
     read_dict = defaultdict(lambda: [None, None])
 
     for read in bam.fetch(region=region_string):
-        if read.is_secondary or read.is_supplementary:
+        if (
+            read.is_secondary
+            or read.is_supplementary
+            or not read.is_paired
+            or read.mapping_quality <= 30
+        ):
             continue
         qname = read.query_name
         if qname not in read_dict:
             if read.is_read1:
                 read_dict[qname][0] = read
             else:
                 read_dict[qname][1] = read
```

### Comparing `phables-1.0.0/phables/workflow/scripts/phables_utils/edge_graph_utils.py` & `phables-1.1.0/phables/workflow/scripts/phables_utils/edge_graph_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import defaultdict
 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from igraph import *
 
 # Create logger
-logger = logging.getLogger("phables 1.0.0")
+logger = logging.getLogger("phables 1.1.0")
 
 
 class BidirectionalError(Exception):
     """Must set a unique value in a BijectiveMap."""
 
     def __init__(self, value):
         self.value = value
@@ -63,14 +63,15 @@
     Get links from the assembly graph
     """
 
     node_count = 0
     graph_contigs = {}
     edges_lengths = {}
     oriented_links = defaultdict(lambda: defaultdict(list))
+    link_overlap = defaultdict(int)
     links = []
 
     my_map = BidirectionalMap()
 
     # Get links from .gfa file
     with open(assembly_graph_file) as file:
         for line in file.readlines():
@@ -79,44 +80,53 @@
                 strings = line.split("\t")
 
                 link1 = strings[1]
                 link2 = strings[3]
 
                 link1_orientation = strings[2]
                 link2_orientation = strings[4]
+                overlap = int(strings[5].strip()[:-1])
 
                 link = []
                 link.append(link1)
                 link.append(link2)
                 links.append(link)
 
                 if link1 != link2:
                     if link1_orientation == "+" and link2_orientation == "+":
                         oriented_links[link1][link2].append(("+", "+"))
+                        link_overlap[(f"{link1}+", f"{link2}+")] = overlap
                         oriented_links[link2][link1].append(("-", "-"))
+                        link_overlap[(f"{link2}-", f"{link1}-")] = overlap
                     elif link1_orientation == "-" and link2_orientation == "-":
                         oriented_links[link1][link2].append(("-", "-"))
+                        link_overlap[(f"{link1}-", f"{link2}-")] = overlap
                         oriented_links[link2][link1].append(("+", "+"))
+                        link_overlap[(f"{link2}+", f"{link1}+")] = overlap
                     elif link1_orientation == "+" and link2_orientation == "-":
                         oriented_links[link1][link2].append(("+", "-"))
+                        link_overlap[(f"{link1}+", f"{link2}-")] = overlap
                         oriented_links[link2][link1].append(("+", "-"))
+                        link_overlap[(f"{link2}+", f"{link1}-")] = overlap
                     elif link1_orientation == "-" and link2_orientation == "+":
                         oriented_links[link1][link2].append(("-", "+"))
+                        link_overlap[(f"{link1}-", f"{link2}+")] = overlap
                         oriented_links[link2][link1].append(("-", "+"))
+                        link_overlap[(f"{link2}-", f"{link1}+")] = overlap
 
             elif line.startswith("S"):
                 strings = line.strip().split()
                 my_map[node_count] = strings[1]
                 graph_contigs[strings[1]] = Seq(strings[2])
                 edges_lengths[strings[1]] = len(strings[2])
                 node_count += 1
 
             line = file.readline()
 
-    return node_count, graph_contigs, links, oriented_links, my_map, edges_lengths
+    return node_count, graph_contigs, links, oriented_links, link_overlap, my_map, edges_lengths
 
 
 def get_graph_edges(links, contig_names_rev):
     """
     Returns the edges of the assembly graph
     """
 
@@ -142,14 +152,15 @@
     """
 
     (
         node_count,
         graph_contigs,
         links,
         oriented_links,
+        link_overlap,
         contig_names,
         edges_lengths,
     ) = get_links(assembly_graph_file)
 
     # Get reverse mapping of contig identifiers
     contig_names_rev = contig_names.inverse
 
@@ -174,14 +185,15 @@
 
     # Simplify the graph
     assembly_graph.simplify(multiple=True, loops=False, combine_edges=None)
 
     return (
         assembly_graph,
         oriented_links,
+        link_overlap,
         contig_names,
         contig_names_rev,
         graph_contigs,
         self_looped_nodes,
         edges_lengths,
     )
```

### Comparing `phables-1.0.0/phables/workflow/scripts/phables_utils/gene_utils.py` & `phables-1.1.0/phables/workflow/scripts/phables_utils/gene_utils.py`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/scripts/phables_utils/genome_utils.py` & `phables-1.1.0/phables/workflow/scripts/phables_utils/genome_utils.py`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/scripts/phables_utils/output_utils.py` & `phables-1.1.0/phables/workflow/scripts/phables_utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv` & `phables-1.1.0/phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv`

 * *Files identical despite different names*

### Comparing `phables-1.0.0/phables/workflow/test_phables.smk` & `phables-1.1.0/phables/workflow/test_phables.smk`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         ph = os.path.join(TESTDIR, "phrogs_annotations.tsv"),
         hm = os.path.join(TESTDIR, "edges.fasta.hmmout")
     output:
         genomes_fasta = temp(os.path.join(TESTDIR, "resolved_paths.fasta")),
         genomes_folder = temp(directory(os.path.join(TESTDIR, "resolved_phages"))),
         genome_info = temp(os.path.join(TESTDIR, "resolved_genome_info.txt")),
         phage_edges = temp(os.path.join(TESTDIR, "phage_like_edges.fasta")),
+        all_phage_edges = temp(os.path.join(TESTDIR, "all_phage_like_edges.fasta")),
         unitigs = temp(os.path.join(TESTDIR, "resolved_edges.fasta")),
         component_info = temp(os.path.join(TESTDIR, "resolved_component_info.txt")),
         phrog_comp_info = temp(os.path.join(TESTDIR, "component_phrogs.txt")),
         mfd = temp(os.path.join(TESTDIR, "results_MFD.txt")),
         mfd_details = temp(os.path.join(TESTDIR, "results_MFD_details.txt")),
         log = temp(os.path.join(TESTDIR, "phables_output.log"))
     params:
@@ -61,14 +62,16 @@
         minlength = ML,
         mincov = MC,
         compcount = CC,
         maxpaths = MP,
         mgfrac = MGF,
         evalue = EV,
         seqidentity = SI,
+        covtol = CT,
+        alpha = AL,
         output = TESTDIR,
         log = temp(os.path.join(TESTDIR, "phables_output.log"))
     log:
         os.path.join(TESTDIR, "phables_output.log")
     conda: 
         os.path.join("envs", "phables.yaml")
     script:
```

### Comparing `phables-1.0.0/phables.egg-info/PKG-INFO` & `phables-1.1.0/phables.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phables
-Version: 1.0.0
+Version: 1.1.0
 Summary: Phables: from fragmented assemblies to high-quality bacteriophage genomes
 Home-page: https://github.com/Vini2/phables
 Author: Vijini Mallawaarachchi
 Author-email: viji.mallawaarachchi@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,24 +18,26 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/Vini2/phables/master/phables_logo.png" width="600" title="phables logo" alt="phables logo">
 </p>
 
 Phables: from fragmented assemblies to high-quality bacteriophage genomes
 ===============
 
-[![CI](https://github.com/Vini2/phables/actions/workflows/testing.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/testing.yml)
+[![](https://img.shields.io/static/v1?label=CLI&message=Snaketool&color=blueviolet)](https://github.com/beardymcjohnface/Snaketool)
 ![GitHub](https://img.shields.io/github/license/Vini2/phables)
-[![DOI](https://zenodo.org/badge/516191931.svg)](https://zenodo.org/badge/latestdoi/516191931)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/phables/badges/version.svg)](https://anaconda.org/bioconda/phables)
+![Conda](https://img.shields.io/conda/dn/bioconda/phables)
 [![PyPI version](https://badge.fury.io/py/phables.svg)](https://badge.fury.io/py/phables)
-[![Anaconda-Server Badge](https://anaconda.org/bioconda/phables/badges/downloads.svg)](https://anaconda.org/bioconda/phables)
+[![Downloads](https://static.pepy.tech/badge/phables)](https://pepy.tech/project/phables)
+
+[![CI](https://github.com/Vini2/phables/actions/workflows/testing.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/testing.yml)
 [![CodeQL](https://github.com/Vini2/phables/actions/workflows/codeql.yml/badge.svg)](https://github.com/Vini2/phables/actions/workflows/codeql.yml)
 [![Documentation Status](https://readthedocs.org/projects/phables/badge/?version=latest)](https://phables.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/516191931.svg)](https://zenodo.org/badge/latestdoi/516191931)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Phables is a tool developed to resolve bacteriophage genomes using phage bubbles in viral metagenomic data. It models cyclic phage-like components in the viral metagenomic assembly as flow networks, models as a minimum flow decomposition problem and resolves genomic paths corresponding to flow paths determined. Phables uses the [Minimum Flow Decomposition via Integer Linear Programming](https://github.com/algbio/MFD-ILP) implementation to obtain the flow paths.
 
 For detailed instructions on installation and usage, please refer to the [**documentation hosted at Read the Docs**](https://phables.readthedocs.io/en/latest/).
 
 **NEW:** Phables is now available on bioconda at [https://anaconda.org/bioconda/phables](https://anaconda.org/bioconda/phables) and on PyPI at [https://pypi.org/project/phables/](https://pypi.org/project/phables/). Feel free to pick your package manager, but we recommend that you use [`conda`](https://docs.conda.io/en/latest/).
```

### Comparing `phables-1.0.0/phables.egg-info/SOURCES.txt` & `phables-1.1.0/phables.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,59 @@
-.gitignore
-.readthedocs.yaml
-CODE_OF_CONDUCT.md
-CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
-mkdocs.yml
-phables_logo.png
 setup.py
-.github/ISSUE_TEMPLATE/bug_report.md
-.github/ISSUE_TEMPLATE/custom.md
-.github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/codeql.yml
-.github/workflows/testing.yml
-docs/assemble.md
-docs/comparison.md
-docs/faq.md
-docs/graph_stats.md
-docs/index.md
-docs/install.md
-docs/quality.md
-docs/requirements.txt
-docs/usage.md
-docs/images/Phables_workflow.png
-docs/images/components.png
-docs/images/histogram_n_nodes.png
-docs/images/pearson_clustermap.png
-docs/images/pearson_heatmap.png
-docs/images/phables_logo.png
-docs/images/qual_resolved_genome_unitig_boxen.png
-docs/images/qual_resolved_genome_unitig_violin.png
 phables/.DS_Store
 phables/__init__.py
 phables/__main__.py
 phables/phables.CITATION
 phables/phables.LICENSE
 phables/phables.VERSION
 phables/util.py
 phables.egg-info/PKG-INFO
 phables.egg-info/SOURCES.txt
 phables.egg-info/dependency_links.txt
 phables.egg-info/entry_points.txt
 phables.egg-info/requires.txt
 phables.egg-info/top_level.txt
-phables/__pycache__/__init__.cpython-310.pyc
-phables/__pycache__/__main__.cpython-310.pyc
-phables/__pycache__/util.cpython-310.pyc
 phables/config/config.yaml
 phables/config/databases.yaml
 phables/test_data/assembly_graph.gfa
 phables/test_data/edge_coverages.tsv
 phables/test_data/edges.fasta.hmmout
 phables/test_data/junction_pe_coverage.pickle
 phables/test_data/phrogs_annotations.tsv
+phables/workflow/.DS_Store
 phables/workflow/install.smk
 phables/workflow/phables.smk
 phables/workflow/test_phables.smk
 phables/workflow/envs/curl.yaml
+phables/workflow/envs/koverage.yaml
 phables/workflow/envs/mapping.yaml
 phables/workflow/envs/mmseqs.yaml
 phables/workflow/envs/phables.yaml
 phables/workflow/envs/smg.yaml
 phables/workflow/rules/00_database_preflight.smk
 phables/workflow/rules/02_phables_preflight.smk
 phables/workflow/rules/02_phables_targets.smk
 phables/workflow/rules/03_test_preflight.smk
 phables/workflow/rules/03_test_targets.smk
 phables/workflow/rules/coverage.smk
 phables/workflow/rules/genes.smk
 phables/workflow/rules/gfa2fasta.smk
 phables/workflow/rules/mapping.smk
 phables/workflow/rules/phables.smk
+phables/workflow/scripts/.DS_Store
 phables/workflow/scripts/combine_cov.py
 phables/workflow/scripts/gfa2fasta.py
 phables/workflow/scripts/phables.py
+phables/workflow/scripts/phables_utils/.DS_Store
 phables/workflow/scripts/phables_utils/FD_Inexact.py
 phables/workflow/scripts/phables_utils/__init__.py
 phables/workflow/scripts/phables_utils/component_utils.py
 phables/workflow/scripts/phables_utils/coverage_utils.py
 phables/workflow/scripts/phables_utils/edge_graph_utils.py
 phables/workflow/scripts/phables_utils/flow_utils.py
 phables/workflow/scripts/phables_utils/gene_utils.py
 phables/workflow/scripts/phables_utils/genome_utils.py
 phables/workflow/scripts/phables_utils/output_utils.py
-phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv
-tests/test_phables.py
+phables/workflow/scripts/phables_utils/phrogs/phrog_annot.tsv
```

### Comparing `phables-1.0.0/setup.py` & `phables-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     author="Vijini Mallawaarachchi",
     author_email="viji.mallawaarachchi@gmail.com",
     data_files=data_files,
     py_modules=["phables"],
     install_requires=[
         "snakemake>=7.14.0",
         "pyyaml>=6.0",
-        "click>=8.1.3",
+        "click>=8.1.3"
     ],
     entry_points={"console_scripts": ["phables=phables.__main__:main"]},
     include_package_data=True,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

