# Comparing `tmp/ExpoSeq-1.1.16.tar.gz` & `tmp/ExpoSeq-1.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.1.16.tar", last modified: Sat Jul 15 11:29:00 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.17.tar", last modified: Sun Jul 16 08:48:13 2023, max compression
```

## Comparing `ExpoSeq-1.1.16.tar` & `ExpoSeq-1.1.17.tar`

### file list

```diff
@@ -1,91 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.759494 ExpoSeq-1.1.16/
--rw-rw-rw-   0        0        0    11543 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/LICENSE
--rw-rw-rw-   0        0        0       59 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/MANIFEST.in
--rw-rw-rw-   0        0        0     4133 2023-07-15 11:29:00.759494 ExpoSeq-1.1.16/PKG-INFO
--rw-rw-rw-   0        0        0     3751 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 11:29:00.759494 ExpoSeq-1.1.16/setup.cfg
--rw-rw-rw-   0        0        0     1336 2023-07-15 11:28:40.000000 ExpoSeq-1.1.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.495241 ExpoSeq-1.1.16/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.526493 ExpoSeq-1.1.16/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.573915 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0     7915 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/mixcr_cl.py
--rw-rw-rw-   0        0        0    10625 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6814 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    19691 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10311 2023-07-15 11:21:27.000000 ExpoSeq-1.1.16/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    40754 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.620793 ExpoSeq-1.1.16/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3292 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4284 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3382 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1724 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1136 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2542 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.652117 ExpoSeq-1.1.16/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1890 2023-07-15 11:21:27.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      173 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.652117 ExpoSeq-1.1.16/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.683397 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    88335 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   213105 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    95440 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2634 2023-07-15 11:21:27.000000 ExpoSeq-1.1.16/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.728151 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.743782 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-07-15 11:20:54.000000 ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-07-15 11:29:00.526493 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     4133 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2971 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-15 11:29:00.000000 ExpoSeq-1.1.16/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:13.062381 ExpoSeq-1.1.17/
+-rw-rw-rw-   0        0        0    11543 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/MANIFEST.in
+-rw-rw-rw-   0        0        0     5527 2023-07-16 08:48:13.062381 ExpoSeq-1.1.17/PKG-INFO
+-rw-rw-rw-   0        0        0     5145 2023-07-15 16:34:55.000000 ExpoSeq-1.1.17/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 08:48:13.062381 ExpoSeq-1.1.17/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-07-16 08:47:58.000000 ExpoSeq-1.1.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.063291 ExpoSeq-1.1.17/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.228323 ExpoSeq-1.1.17/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.382409 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0    10625 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6814 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    19695 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10290 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    40816 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.649602 ExpoSeq-1.1.17/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3295 2023-07-16 08:45:22.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4284 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3382 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1724 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1134 2023-07-16 08:42:06.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2542 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.754157 ExpoSeq-1.1.17/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      173 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.794589 ExpoSeq-1.1.17/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.900318 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    88335 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   213105 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    95440 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.997740 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:13.062381 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-07-15 16:28:47.000000 ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:48:12.292604 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     5527 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2934 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 08:48:11.000000 ExpoSeq-1.1.17/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.1.16/LICENSE` & `ExpoSeq-1.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/PKG-INFO` & `ExpoSeq-1.1.17/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: ExpoSeq
-Version: 1.1.16
-Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
-Home-page: https://github.com/nilshof01/ExpoSeq
-Author: Nils Hofmann
-Author-email: n.hofmann.99@web.de
-License: Apache License 2.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Welcome to ExpoSeq
 
 ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
 
 ## Installation
 
 Open a virtual environment and type ```pip install ExpoSeq```. Ensure that you have python > 3.11 installed.
@@ -41,20 +29,41 @@
 If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
 ```import matplotlib.pyplot as plt```
 ```plt.xlabel("your_title")```
 If you would like to have details about the inputs and functions of the PlotManager call: ```help(plot)``` . You can also call ```help(plot.jaccard)```
 
 
+# Processing on a server with multithreading
+
+If you wish to process your data on a server to utilize multithreading, or to process on a screen in the background, use the scripts located in the `bash_processing` folder.
+
+Start by copying the folder and the directory with the `mixcr.jar` file to the corresponding directory. You can use the `run_mixcr.sh` script to generate a sequencing report, which is the input of the pipeline. The script requires certain inputs and can accept optional ones as well, such as the number of threads you wish to use. The inputs are listed below:
+
+### Required Inputs
+
+- `--fastq_directory`: Directory path to your fastq files.
+- `--path_to_mixcr`: Filepath (ending with .jar) to mixcr.
+
+### Optional Inputs
+
+- `--save_dir`: Directory where you would like to store the sequencing report (default is the working directory).
+- `--paired_end_sequencing`: Boolean indicating whether you have paired end sequencing data or not (default is `False`).
+- `--threads`: Number of threads you would like to utilize (default is `1`).
+- `--method`: Mixcr method to assemble and align your sequences (default is `milab-human-tcr-dna-multiplex-cdr3`).
+- `--trim_div_by`: Trims all sequences that are divisible by the integer you input (default is `3`).
+- `--trim_min_count`: Trims all sequences that are shorter than the given integer (default is `3`).
+
+
+
 ## References
 [1] Dmitriy A. Bolotin, Stanislav Poslavsky, Igor Mitrophanov, Mikhail Shugay, Ilgar Z. Mamedov, Ekaterina V. Putintseva, and Dmitriy M. Chudakov. "MiXCR: software for comprehensive adaptive immunity profiling." Nature methods 12, no. 5 (2015): 380-381.
 
 
-
-[2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908â€“911 (2017)
+[2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908–911 (2017)
 
 [3] (1, 2) Tareen A, Kinney JB (2019) Logomaker: beautiful sequence logos in Python. Bioinformatics btz921. bioRxiv doi:10.1101/635029.
```

### Comparing `ExpoSeq-1.1.16/README.md` & `ExpoSeq-1.1.17/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: ExpoSeq
+Version: 1.1.17
+Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
+Home-page: https://github.com/nilshof01/ExpoSeq
+Author: Nils Hofmann
+Author-email: n.hofmann.99@web.de
+License: Apache License 2.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Welcome to ExpoSeq
 
 ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](pictures_gen/expoSeq_overview.png)
 
 ## Installation
 
 Open a virtual environment and type ```pip install ExpoSeq```. Ensure that you have python > 3.11 installed.
@@ -29,20 +41,41 @@
 If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
 ```import matplotlib.pyplot as plt```
 ```plt.xlabel("your_title")```
 If you would like to have details about the inputs and functions of the PlotManager call: ```help(plot)``` . You can also call ```help(plot.jaccard)```
 
 
+# Processing on a server with multithreading
+
+If you wish to process your data on a server to utilize multithreading, or to process on a screen in the background, use the scripts located in the `bash_processing` folder.
+
+Start by copying the folder and the directory with the `mixcr.jar` file to the corresponding directory. You can use the `run_mixcr.sh` script to generate a sequencing report, which is the input of the pipeline. The script requires certain inputs and can accept optional ones as well, such as the number of threads you wish to use. The inputs are listed below:
+
+### Required Inputs
+
+- `--fastq_directory`: Directory path to your fastq files.
+- `--path_to_mixcr`: Filepath (ending with .jar) to mixcr.
+
+### Optional Inputs
+
+- `--save_dir`: Directory where you would like to store the sequencing report (default is the working directory).
+- `--paired_end_sequencing`: Boolean indicating whether you have paired end sequencing data or not (default is `False`).
+- `--threads`: Number of threads you would like to utilize (default is `1`).
+- `--method`: Mixcr method to assemble and align your sequences (default is `milab-human-tcr-dna-multiplex-cdr3`).
+- `--trim_div_by`: Trims all sequences that are divisible by the integer you input (default is `3`).
+- `--trim_min_count`: Trims all sequences that are shorter than the given integer (default is `3`).
+
+
+
 ## References
 [1] Dmitriy A. Bolotin, Stanislav Poslavsky, Igor Mitrophanov, Mikhail Shugay, Ilgar Z. Mamedov, Ekaterina V. Putintseva, and Dmitriy M. Chudakov. "MiXCR: software for comprehensive adaptive immunity profiling." Nature methods 12, no. 5 (2015): 380-381.
 
 
-
-[2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908–911 (2017)
+[2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908â€“911 (2017)
 
 [3] (1, 2) Tareen A, Kinney JB (2019) Logomaker: beautiful sequence logos in Python. Bioinformatics btz921. bioRxiv doi:10.1101/635029.
```

### Comparing `ExpoSeq-1.1.16/setup.py` & `ExpoSeq-1.1.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.1.16",
+    version = "1.1.17",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
     license = "Apache License 2.0",
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/mixcr_cl.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,249 @@
-import pandas as pd
 import os
+import sys
+from glob import glob
 import subprocess
+from ast import literal_eval
 import pickle
-from glob import glob
-import shutil
+import pandas as pd
 from ExpoSeq.augment_data.trimming import trimming
-#from .trimming import trimming
-
-#
-def remove_directories(directory_path):
-    # Iterate over all items in the directory
-    for item in os.listdir(directory_path):
-        shutil.rmtree(os.path.join(directory_path, item))
-
-
-def collect_fastq_files(fastq_directory):
+import pkg_resources
+try:
+    import tkinter as tk
+    from tkinter import filedialog
+except:
+    pass
+def add_fastq_files():
     filenames = []
-    path_to_files = os.path.abspath(fastq_directory)
-    filenames.extend(glob(os.path.join(path_to_files, "*.fastq")))
-    if len(filenames) == 0:
-       print(
-            "You have not chosen a directory with fastq files.")
-
-    else:
-        print("These are the files you chose:")
-        for i in filenames:
-            print(os.path.basename(i))
+    while True:
+        try:
+            while True:
+                path_to_files = filedialog.askdirectory()
+                if os.path.isdir(path_to_files) == True:
+                    break
+                else:
+                    pass
+            
+        except:
+            while True:
+                path_to_files = input("copy and paste the path to your directory")
+                if os.path.isdir(os.path.abspath(path_to_files)) == True:
+                    break
+                else:
+                    print("Please enter a valid directory. Dont add a \ to the end of the directory path")
+        path_to_files = os.path.abspath(path_to_files)
+        filenames.extend(glob(os.path.join(path_to_files, "*.fastq")))
+        if len(filenames) == 0:
+            user_choice = input("You have not chosen a directory with fastq files. If you want to try again press 1. If you want to cancel the analysis press 2")
+            if user_choice == str(1):
+                read_more_files = "Y"
+            else:
+                read_more_files = "N"
+        else:
+            print("These are the files you chose:")
+            for i in filenames:
+                print(os.path.basename(i))
+            while True:
+                read_more_files = input("do you want to add another folder? (Y/n)")
+                if read_more_files in ["Y" "y", "n", "N"]:
+                    break
+                else:
+                    pass
+        if read_more_files == "Y" or read_more_files == "y":
+            continue
+        else:
+            break
+    sorted(filenames)
 
     return filenames
 
 
-def mixcr_(fastq_directory, path_to_mixcr, save_dir, paired_end_sequencing, threads, method, trim_div_by, trim_min_count, testing = False):
+def process_mixcr(experiment, method, testing, paired_end_sequencing):
+    pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
+    module_dir = os.path.abspath("")
+    
     if not testing:
-        filenames = collect_fastq_files(fastq_directory)
+        print("Choose the directory where you store your fastq files")
+        while True:
+            filenames = add_fastq_files()
+            if len(filenames) == 0:
+                print("You have not added any fastq files the preprocessing is cancelled now.")
+            else:
+                break
+        if not os.path.isdir(os.path.join(module_dir, "my_experiments", experiment, "alignment_reports")):
+            os.mkdir(os.path.join(module_dir, "my_experiments", experiment, "alignment_reports"))
+
     else:
-        filenames = glob(os.path.join(r"C:\Users\nilsh\my_projects\ExpoSeq\tests", "*.fastq"))
-    if len(filenames) == 0:
-        print("You have not added any fastq files.")
-        return
-    print("Test Mixcr")
-    subprocess.run(["java",
-                    "-jar",
-                    path_to_mixcr,
-                    "--version"
-                    ])
-    confirmation = True
-    if confirmation == True:
-        if not os.path.isdir("temp"):
-            os.mkdir("temp")
-
-        module_dir = os.path.abspath("")
-        sequencing_report = pd.DataFrame([])
-        if paired_end_sequencing == True:
-            filenames_unique_reverse = [unique for unique in filenames if "2.fastq" in unique]
-            filenames_unique_forward = [unique for unique in filenames if "1.fastq" in unique]
-            combined_filenames = []
-            for i in filenames_unique_reverse:
-                file_one = i
-                basename = os.path.basename(os.path.splitext(file_one)[0])
-                basename = basename[:len(basename) - 2]
-                file_two = ""
-                for j in filenames_unique_forward:
-                    if basename in filenames_unique_forward:
-                        file_two = j
-                        break
-                if file_two == "":
-                    print("you are missing the the reverse strand for " + basename)
-                else:
-                    fastq_files = file_one + " " + file_two
-                    combined_filenames.append(fastq_files)
-            if len(combined_filenames) == 0:
-                print("the system couldnt find any forward reverse matches. Please check your given directory or continue with single-end analysis.")
-                return
-        else:
-            combined_filenames = filenames
-        for filename in combined_filenames:
-            try:
-                basename = os.path.basename(os.path.splitext(filename)[0])
-                basename = basename[:len(basename) - 2]
-                filename_base = basename
-                result = os.path.join(module_dir, "temp", filename_base + ".vdjca")
-                clones = os.path.join(module_dir, "temp", basename + "clones.clns")
-                subprocess.run(["java",
-                                "-jar",
-                                path_to_mixcr,
-                                "align",
-                                "-p " + method,
-                                filename,
-                                result,
-                                "--report",
-                                os.path.normpath(os.path.join(module_dir,
-                                                              filename_base + "_AlignmentReport.txt")),
-                                "--threads",
-                                str(threads)
-                                ])
 
-                subprocess.run(["java",
-                                "-jar",
-                                path_to_mixcr,
-                                "assemble",
-                                "-OseparateByC=true",
-                                "-OseparateByV=true",
-                                "-OseparateByJ=true",
-                                result,
-                                clones,
-                                "--threads",
-                                str(threads)
-                                ])
+        filenames = glob(os.path.join(pkg_path,"test_data","test_files", "*.fastq"))
+        print(filenames)
+        experiment = "test_directory"
+    
+    settings_dir = os.path.join(pkg_path,
+                                "settings",
+                                "global_vars.txt")
+    with open(settings_dir) as f:
+        data = f.read()
+    data = literal_eval(data)
+    path_to_mixcr = data["mixcr_path"]
+    if path_to_mixcr == "":
+        while True:
+            print("choose the mixcr java file with the file chooser")
+            try:
+                path_to_mixcr = filedialog.askopenfilename()
+            except:
+                path_to_mixcr = input("copy and paste the path to the mixcr jar file here.")
+                path_to_mixcr = os.path.normpath(path_to_mixcr)
+            if testing == True:
+                break
 
+            
+            try:
+                print("Test Mixcr")
                 subprocess.run(["java",
-                                "-jar",
-                                path_to_mixcr,
-                                "exportClones",
-                                "-cloneId",
-                                "-readCount",
-                                "-readFraction",
-                                "-lengthOf CDR3",
-                                "-nFeature CDR3",
-                                "-aaFeature CDR3",
-                                "-avrgFeatureQuality CDR3",
-                                clones,
-                                os.path.join(module_dir,
-                                             "temp",
-                                             basename + ".tsv"),
-                                "--threads",
-                                str(threads)
-                                ])
-
-                clones_sample = pd.read_table(os.path.join(module_dir,
-                                                           "temp",
-                                                           basename + "_IGH.tsv"))
-                clones_sample = clones_sample[["cloneId",
-                                               "readCount",
-                                               "readFraction",
-                                               "nSeqCDR3",
-                                               "aaSeqCDR3",
-                                               "minQualCDR3",
-                                               "lengthOfCDR3",
-                                               "meanQualCDR3"]]
-                new_fractions = clones_sample.groupby("nSeqCDR3")["readFraction"].sum().reset_index()
-                clones_sample = clones_sample.drop_duplicates(subset=["nSeqCDR3"], keep="first")
-                clones_sample = new_fractions.merge(clones_sample,
-                                                    how="left",
-                                                    on="nSeqCDR3")
-                clones_sample = clones_sample.sort_values(by="cloneId")
-                clones_sample = clones_sample.reset_index()
-                clones_sample = clones_sample.drop(columns=["readFraction_y", "index"])
-                clones_sample = clones_sample.rename(columns={"readFraction_x": "cloneFraction"})
-                clones_sample["Experiment"] = filename_base
-                clones_sample = trimming(clones_sample,
-                                         divisible_by=trim_div_by,
-                                         min_count=trim_min_count,
-                                         new_fraction="clonesFraction")
-                sequencing_report = pd.concat([sequencing_report, clones_sample])
-                files_to_remove = os.listdir(os.path.join(module_dir, "temp"))
-                for file in files_to_remove:
-                    os.remove(os.path.join(module_dir,
-                                           "temp",
-                                           file))
-                report_dir = os.path.join(save_dir,
-                                      "sequencing_report.txt")
-                sequencing_report.to_csv(report_dir)
+                                    "-jar",
+                                    path_to_mixcr,
+                                    "--version"
+                                    ])
+                confirmation = True
             except:
-                remove_directories(os.path.join(module_dir, "temp"))
-
+                print("Apparently you have not choosen the right path to the mixcr .jar file. Please try again")
+                confirmation = False
+            if confirmation == True:
+                path_to_mixcr = os.path.abspath(path_to_mixcr)
+                data["mixcr_path"] = path_to_mixcr
+                with open(settings_dir, "w") as f:
+                    f.write(str(data))
+                break
+    else:
+        pass
+    #kAligner2_4.0
+    #nebnext-human-bcr-cdr3
+    #milab-human-tcr-dna-multiplex-cdr3
+
+
+    sequencing_report = pd.DataFrame([])
+    if paired_end_sequencing == True:
+        filenames_unique_reverse = [unique for unique in filenames if "2.fastq" in unique]
+        filenames_unique_forward = [unique for unique in filenames if "1.fastq" in unique]
+        combined_filenames = []
+        for i in filenames_unique_reverse:
+            file_one = i
+            basename = os.path.basename(os.path.splitext(file_one)[0])
+            basename = basename[:len(basename) - 2]
+            file_two = ""
+            for j in filenames_unique_forward:
+                if basename in filenames_unique_forward:
+                    file_two = j
+                    break
+            if file_two == "":
+                print("you are missing the the reverse strand for " + basename)
+            else:
+                fastq_files = file_one + " " + file_two
+                combined_filenames.append(fastq_files)
+        if len(combined_filenames) == 0:
+            print("the system couldnt find any forward reverse matches. Please check your given directory or continue with single-end analysis.")
+            return
     else:
-        print("The path to the mixcr jar file is not correct or you are missing the licence")
+        combined_filenames = filenames
+
+    for filename in combined_filenames:
+        basename = os.path.basename(os.path.splitext(filename)[0])
+        basename = basename[:len(basename) - 2]
+        filename_base = basename
+        result = os.path.join(module_dir, "temp", filename_base + ".vdjca")
+        clones = os.path.join(module_dir, "temp", basename + "clones.clns")
+        subprocess.run(["java",
+                        "-jar",
+                        path_to_mixcr,
+                        "align",
+                        "-p " + method,
+                        os.path.normpath(filename),
+                        result,
+                        "--report",
+                        os.path.normpath(os.path.join(module_dir,
+                                           "my_experiments",
+                                           experiment,
+                                           "alignment_reports",
+                                           filename_base + "_AlignmentReport.txt"))
+                        ])
+
+        subprocess.run(["java",
+                        "-jar",
+                        path_to_mixcr,
+                        "assemble",
+                        "-OseparateByC=true",
+                        "-OseparateByV=true",
+                        "-OseparateByJ=true",
+                        result,
+                        clones
+                        ])
+
+        subprocess.run(["java",
+                        "-jar",
+                        path_to_mixcr,
+                        "exportClones",
+                        "-cloneId",
+                        "-readCount",
+                        "-readFraction",
+                        "-lengthOf CDR3",
+                        "-nFeature CDR3",
+                        "-aaFeature CDR3",
+                        "-avrgFeatureQuality CDR3",
+                        clones,
+                        os.path.join(module_dir,
+                                     "temp",
+                                     basename + ".tsv")
+                        ])
+
+        clones_sample = pd.read_table(os.path.join(module_dir,
+                                                   "temp",
+                                                   basename + "_IGH.tsv"))
+        clones_sample = clones_sample[["cloneId",
+                                        "readCount",
+                                        "readFraction",
+                                        "nSeqCDR3",
+                                        "aaSeqCDR3",
+                                        "minQualCDR3",
+                                        "lengthOfCDR3",
+                                        "meanQualCDR3"]]
+        new_fractions = clones_sample.groupby("nSeqCDR3")["readFraction"].sum().reset_index()
+        clones_sample = clones_sample.drop_duplicates(subset=["nSeqCDR3"], keep="first")
+        clones_sample = new_fractions.merge(clones_sample,
+                                            how = "left",
+                                            on = "nSeqCDR3")
+        clones_sample = clones_sample.sort_values(by="cloneId")
+        clones_sample = clones_sample.reset_index()
+        clones_sample = clones_sample.drop(columns = ["readFraction_y", "index"])
+        clones_sample = clones_sample.rename(columns={"readFraction_x": "cloneFraction"})
+        clones_sample["Experiment"] = filename_base
+        clones_sample = trimming(clones_sample,
+                                 divisible_by = 3,
+                                 min_count = 3,
+                                 new_fraction = "clonesFraction")
+        sequencing_report = pd.concat([sequencing_report, clones_sample])
+        files_to_remove = os.listdir(os.path.join(module_dir, "temp"))
+        for file in files_to_remove:
+            os.remove(os.path.join(module_dir,
+                                   "temp",
+                                   file))
+    if not testing:
+        report_dir = os.path.join(module_dir,
+                                  "my_experiments",
+                                  experiment,
+                                  "sequencing_report.csv")
+        sequencing_report.to_csv(report_dir)
+        data["last_experiment"] = experiment
+        glob_vars_dir = os.path.join(pkg_path,
+                                     "settings",
+                                     "global_vars.txt")
+        with open(glob_vars_dir, "w") as f:
+            f.write(str(data))
+        unique_experiments = sequencing_report["Experiment"].unique()
+        experiment_dic = {item: item for item in list(unique_experiments)}
+        exp_names_dir = os.path.join(module_dir,
+                                     "my_experiments",
+                                     experiment,
+                                     "experiment_names.pickle")
+        with open(exp_names_dir, "wb") as f:
+            pickle.dump(experiment_dic, f)
+
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/randomizer.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.1.17/src/ExpoSeq/augment_data/uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     return sequencing_report, all_alignment_reports, experiment
 
 def upload(testing=False, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1'):
    # module_dir = os.path.abspath("")
     module_dir = os.getcwd()
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     repo_path, last_experiment = check_last_exp(pkg_path, module_dir, testing)
-
+    
     if os.path.isfile(repo_path):
         continue_analysis = get_continue_analysis_input(last_experiment,
                                                         testing,
                                                         continue_analysis)
         if continue_analysis.lower() in ["n", "no"]:
             next_step = get_next_step_input(testing, choose_exp)
             if next_step == "1":
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/full_pipe.py` & `ExpoSeq-1.1.17/src/ExpoSeq/full_pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shutil
 import pkg_resources
 from ast import literal_eval
 
 def run_pipeline(antigens = None, usq_multiple = "n", pass_interrupt = True, test = False):
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     save_settings_path = os.path.join(pkg_path,
-                                      "settings",
+                 "settings",
                  "save_settings.txt")
     with open(save_settings_path, "r") as f:
         save_settings = f.read()
     save_settings = literal_eval(save_settings)
     original_path = save_settings["fname"]
     if antigens == True or antigens == False or antigens == None:
         pass
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.1.17/src/ExpoSeq/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,24 +70,25 @@
                                             "experiment_names.pickle")
             with open(experiment_path, "rb") as f:
                 self.unique_experiments = pickle.load(f)
             self.sequencing_report["Experiment"] = self.sequencing_report["Experiment"].map(self.unique_experiments)
             self.binding_data_dir = os.path.join(self.module_dir,
                     "my_experiments",
                     self.experiment,
-                    "sequencing_report.csv")
+                    "binding_data.csv")
             if not os.path.isfile(self.binding_data_dir):
                 self.add_binding = input("Do you have binding Data? Y/n")
                 if self.add_binding.lower() in ["Y", "y"]:
                     self.binding_data = collect_binding_data()
 
-                    self.binding_data.to_csv(self.binding_data_dir)
+                    self.binding_data.to_csv("binding_data.csv")
                 else:
                     self.binding_data = None
-                
+            else:
+                self.binding_data = pd.read_csv(self.binding_data_dir)
                 
         font_settings_path = os.path.join(self.pkg_path,
                                           "settings",
                                           "font_settings.txt")
         assert os.path.isfile(font_settings_path), "The font settings file does not exist in the given filepath"
         with open(font_settings_path, "r") as f:
             font_settings = f.read()
@@ -134,15 +135,15 @@
 
     def add_binding_data(self):
         """"
         :return: adds binding data to your analysis. You can add mutliple files with the filechooser or a given path to the file. For more information about the necessary file structure, check the supplementary information.
         """
         self.binding_data = collect_binding_data(binding_data = self.binding_data)
 
-        self.binding_data.to_csv(self.binding_data_dir)
+        self.binding_data.to_csv("binding_data.csv")
             
         
     def print_antigens(self):
         """
         :return: prints the antigens (columns) of your binding data
         """
         try:
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/length_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     ax.title.set_text(sample)
     ax.title.set_size(10)
     ax.set_ylabel("Read Count",
                     **font_settings)  # Y label
     ax.set_xlabel('Read Length',
                 **font_settings)  # X label
 
-    original_fontsize = font_settings["fontsize"]
-    font_settings["fontsize"] = 22
+#    original_fontsize = font_settings["fontsize"]
+ #   font_settings["fontsize"] = 22
     plt.title("Length Distribution of " + sample,
               pad=12,
               **font_settings)
-    font_settings["fontsize"] = original_fontsize
+  #  font_settings["fontsize"] = original_fontsize
 
 
 
 def length_distribution_multi(fig, sequencing_report, samples,num_cols, font_settings, test_version = False):
     if samples == "all":
         unique_experiments = sequencing_report["Experiment"].unique()
         unique_experiments = np.sort(unique_experiments)
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     ax.set_xlabel('Position on amino acid sequence', **font_settings)
     if protein == True:
         ax.set_ylabel('Relatvie Proportion of Amino Acid', **font_settings)
     else:
         ax.set_ylabel('Relatvie Proportion of Nucleotide', **font_settings)
 
 #    ax.set_xticks(rotation = 360)
-    plt.legend(**legend_settings)
+    ax.legend(**legend_settings)
     original_fontsize = font_settings["fontsize"]
     font_settings["fontsize"] = 22
     if protein == True:
         ax.set_title("Distribution of Aminoacids per Position for your sequences",pad = 12, **font_settings)
     else:
         ax.set_title("Distribution of Nucleotides per Position for your sequences",pad = 12, **font_settings)
-    ax.set_xticklabels(ax.get_xticklabels(), rotation=90, ha='center')
+    ax.set_xticklabels(ax.get_xticklabels(), rotation=0, ha='center')
     font_settings["fontsize"] = original_fontsize
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.1.17/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/reset.py` & `ExpoSeq-1.1.17/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.1.17/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.1.17/src/ExpoSeq/settings/change_save_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     pass
 class Change_save_settings():
     def __init__(self):
         self.pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
 
         self.save_settings_path = os.path.join(self.pkg_path,
                                           "settings",
-                                               "save_settings.txt")
+                                        "save_settings.txt")
         with open(self.save_settings_path, "r") as f:
             save_settings = f.read()
         self.save_settings = literal_eval(save_settings)
     def change_dpi(self, dpi):
         self.save_settings["dpi"] = dpi
         with open(self.save_settings_path, "w") as f:
             f.write(str(self.save_settings))
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.1.17/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-1.1.17/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-1.1.17/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/test_uploader.py` & `ExpoSeq-1.1.17/src/ExpoSeq/test_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     if not os.path.isdir(os.path.join(module_dir, "my_experiments")):
         os.mkdir(os.path.join(module_dir, "my_experiments"))
     if not os.path.isdir(os.path.join(module_dir, "temp")):
         os.mkdir(os.path.join(module_dir, "temp"))
     if not os.path.isdir(os.path.join(module_dir, "my_experiments", "test_directory")):
         new_dir = os.path.join(module_dir, "my_experiments", "test_directory")
         os.mkdir(new_dir)
-        source_seq_report = os.path.join(pkg_dir, "test_data", "test_files", "sequencing_report.csv")
+        source_seq_report = os.path.join(pkg_dir, "test_data","test_files", "sequencing_report.csv")
      #   source_align_report = os.path.join(pkg_dir, "test_data", "all_alignment_reports.pickle")
-        source_experiments = os.path.join(pkg_dir, "test_data", "test_files", "experiment_names.pickle")
+        source_experiments = os.path.join(pkg_dir, "test_data","test_files", "experiment_names.pickle")
         assert shutil.copy2(source_seq_report, new_dir), "could not copy sequencing report"
      #   shutil.copy2(source_align_report, new_dir)
         shutil.copy2(source_experiments, new_dir)
     else:
         pass
     
     #upload(testing=True, continue_analysis = "n", upload_type = "2", choose_exp = '1', paired_end_test = 'n', experiment_column = '1')
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.1.17/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.17/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.16
+Version: 1.1.17
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -41,19 +41,40 @@
 If you want to change the style of the plot you can use the PlotManager. If you called it ```plot``` you can do for instance the following: ```plot.style.title_xaxis("your_title")``` 
 If you want to implement further plot change you can also refer to the matplotlib.pyplot library and change it in the same way as following:
 ```import matplotlib.pyplot as plt```
 ```plt.xlabel("your_title")```
 If you would like to have details about the inputs and functions of the PlotManager call: ```help(plot)``` . You can also call ```help(plot.jaccard)```
 
 
+# Processing on a server with multithreading
+
+If you wish to process your data on a server to utilize multithreading, or to process on a screen in the background, use the scripts located in the `bash_processing` folder.
+
+Start by copying the folder and the directory with the `mixcr.jar` file to the corresponding directory. You can use the `run_mixcr.sh` script to generate a sequencing report, which is the input of the pipeline. The script requires certain inputs and can accept optional ones as well, such as the number of threads you wish to use. The inputs are listed below:
+
+### Required Inputs
+
+- `--fastq_directory`: Directory path to your fastq files.
+- `--path_to_mixcr`: Filepath (ending with .jar) to mixcr.
+
+### Optional Inputs
+
+- `--save_dir`: Directory where you would like to store the sequencing report (default is the working directory).
+- `--paired_end_sequencing`: Boolean indicating whether you have paired end sequencing data or not (default is `False`).
+- `--threads`: Number of threads you would like to utilize (default is `1`).
+- `--method`: Mixcr method to assemble and align your sequences (default is `milab-human-tcr-dna-multiplex-cdr3`).
+- `--trim_div_by`: Trims all sequences that are divisible by the integer you input (default is `3`).
+- `--trim_min_count`: Trims all sequences that are shorter than the given integer (default is `3`).
+
+
+
 ## References
 [1] Dmitriy A. Bolotin, Stanislav Poslavsky, Igor Mitrophanov, Mikhail Shugay, Ilgar Z. Mamedov, Ekaterina V. Putintseva, and Dmitriy M. Chudakov. "MiXCR: software for comprehensive adaptive immunity profiling." Nature methods 12, no. 5 (2015): 380-381.
 
 
-
 [2] Dmitriy A. Bolotin, Stanislav Poslavsky, Alexey N. Davydov, Felix E. Frenkel, Lorenzo Fanchi, Olga I. Zolotareva, Saskia Hemmers, Ekaterina V. Putintseva, Anna S. Obraztsova, Mikhail Shugay, Ravshan I. Ataullakhanov, Alexander Y. Rudensky, Ton N. Schumacher & Dmitriy M. Chudakov. "Antigen receptor repertoire profiling from RNA-seq data." Nature Biotechnology 35, 908â€“911 (2017)
 
 [3] (1, 2) Tareen A, Kinney JB (2019) Logomaker: beautiful sequence logos in Python. Bioinformatics btz921. bioRxiv doi:10.1101/635029.
```

### Comparing `ExpoSeq-1.1.16/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.1.17/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 src/ExpoSeq.egg-info/requires.txt
 src/ExpoSeq.egg-info/top_level.txt
 src/ExpoSeq/augment_data/__init__.py
 src/ExpoSeq/augment_data/binding_data.py
 src/ExpoSeq/augment_data/check_reports.py
 src/ExpoSeq/augment_data/load_data.py
 src/ExpoSeq/augment_data/loop_collect_reports.py
-src/ExpoSeq/augment_data/mixcr_cl.py
 src/ExpoSeq/augment_data/mixcr_nils.py
 src/ExpoSeq/augment_data/randomizer.py
 src/ExpoSeq/augment_data/read_raw_data.py
 src/ExpoSeq/augment_data/structure_files.py
 src/ExpoSeq/augment_data/trimming.py
 src/ExpoSeq/augment_data/uploader.py
 src/ExpoSeq/plots/__init__.py
```

