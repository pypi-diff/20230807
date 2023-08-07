# Comparing `tmp/DAJIN2-0.2.4.tar.gz` & `tmp/DAJIN2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DAJIN2-0.2.4.tar", last modified: Tue Jun 13 04:33:34 2023, max compression
+gzip compressed data, was "DAJIN2-0.3.0.tar", last modified: Mon Aug  7 00:20:39 2023, max compression
```

## Comparing `DAJIN2-0.2.4.tar` & `DAJIN2-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,73 @@
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:34.150776 DAJIN2-0.2.4/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.4/LICENSE
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.4/MANIFEST.in
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3767 2023-06-13 04:33:34.147775 DAJIN2-0.2.4/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3199 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/README.md
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-13 04:33:34.150776 DAJIN2-0.2.4/setup.cfg
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1150 2023-06-13 04:32:42.000000 DAJIN2-0.2.4/setup.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.471855 DAJIN2-0.2.4/src/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.739585 DAJIN2-0.2.4/src/DAJIN2/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:26:28.000000 DAJIN2-0.2.4/src/DAJIN2/__init__.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.950507 DAJIN2-0.2.4/src/DAJIN2/core/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/__init__.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.060284 DAJIN2-0.2.4/src/DAJIN2/core/classification/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/classification/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/classification/classify.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/classification/detect_sv.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.246900 DAJIN2-0.2.4/src/DAJIN2/core/clustering/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/clustering.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/make_score.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/merge_clusters.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3824 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/return_labels.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.396723 DAJIN2-0.2.4/src/DAJIN2/core/consensus/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      409 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/consensus/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5930 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/consensus/consensus.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2513 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/consensus/extract_mutation_loci_by_labels.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/consensus/subset.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11018 2023-06-12 07:18:55.000000 DAJIN2-0.2.4/src/DAJIN2/core/core_execute.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.740810 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      367 2023-06-12 07:12:52.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5418 2023-06-12 07:18:55.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/call_midsv.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      917 2023-06-12 07:02:39.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/check_caches.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6116 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_knockin_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7157 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_mutation_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4437 2023-06-08 03:17:27.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/format_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/mappy_align.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/replace_NtoD.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.927117 DAJIN2-0.2.4/src/DAJIN2/core/report/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       86 2023-06-07 21:49:16.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5125 2023-06-08 04:18:39.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/remove_microhomology.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     8324 2023-06-12 07:18:55.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/report_bam.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/report_files.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1565 2023-06-07 21:55:43.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/reverse_sam.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2883 2023-06-05 08:39:04.000000 DAJIN2-0.2.4/src/DAJIN2/gui.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11137 2023-06-12 07:09:09.000000 DAJIN2-0.2.4/src/DAJIN2/main.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.992717 DAJIN2-0.2.4/src/DAJIN2/postprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/postprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/postprocess/report.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:34.053552 DAJIN2-0.2.4/src/DAJIN2/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:06:47.000000 DAJIN2-0.2.4/src/DAJIN2/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5440 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/preprocess/validate_inputs.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.557038 DAJIN2-0.2.4/src/DAJIN2/static/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:34.086588 DAJIN2-0.2.4/src/DAJIN2/static/css/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/static/css/style.css
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/template_igvjs.html
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:34.121250 DAJIN2-0.2.4/src/DAJIN2/templates/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/templates/index.html
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/view.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.890881 DAJIN2-0.2.4/src/DAJIN2.egg-info/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3767 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1746 2023-06-13 04:33:32.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/SOURCES.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/dependency_links.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       47 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/entry_points.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      237 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/requires.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/top_level.txt
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:39.588317 DAJIN2-0.3.0/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.3.0/LICENSE
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.3.0/MANIFEST.in
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5915 2023-08-07 00:20:39.582008 DAJIN2-0.3.0/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5336 2023-08-06 02:01:50.000000 DAJIN2-0.3.0/README.md
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-08-07 00:20:39.589328 DAJIN2-0.3.0/setup.cfg
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1161 2023-08-07 00:17:12.000000 DAJIN2-0.3.0/setup.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:37.687403 DAJIN2-0.3.0/src/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:37.926381 DAJIN2-0.3.0/src/DAJIN2/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:26:28.000000 DAJIN2-0.3.0/src/DAJIN2/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:38.138250 DAJIN2-0.3.0/src/DAJIN2/core/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.3.0/src/DAJIN2/core/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:38.252281 DAJIN2-0.3.0/src/DAJIN2/core/classification/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       65 2023-08-05 10:09:24.000000 DAJIN2-0.3.0/src/DAJIN2/core/classification/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1510 2023-08-06 23:34:58.000000 DAJIN2-0.3.0/src/DAJIN2/core/classification/classify.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.3.0/src/DAJIN2/core/classification/tmp_detect_sv.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:38.493978 DAJIN2-0.3.0/src/DAJIN2/core/clustering/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      233 2023-06-16 07:46:39.000000 DAJIN2-0.3.0/src/DAJIN2/core/clustering/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5690 2023-08-04 00:44:58.000000 DAJIN2-0.3.0/src/DAJIN2/core/clustering/clustering.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2804 2023-07-08 21:57:57.000000 DAJIN2-0.3.0/src/DAJIN2/core/clustering/make_kmer.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4258 2023-07-08 02:22:32.000000 DAJIN2-0.3.0/src/DAJIN2/core/clustering/make_score.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.3.0/src/DAJIN2/core/clustering/merge_clusters.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7617 2023-07-27 03:17:07.000000 DAJIN2-0.3.0/src/DAJIN2/core/clustering/return_labels.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:38.655359 DAJIN2-0.3.0/src/DAJIN2/core/consensus/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      409 2023-06-12 03:47:36.000000 DAJIN2-0.3.0/src/DAJIN2/core/consensus/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     8358 2023-08-06 00:07:29.000000 DAJIN2-0.3.0/src/DAJIN2/core/consensus/consensus.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2700 2023-08-04 00:52:14.000000 DAJIN2-0.3.0/src/DAJIN2/core/consensus/extract_mutation_loci_by_labels.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.3.0/src/DAJIN2/core/consensus/subset.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12428 2023-08-05 22:37:31.000000 DAJIN2-0.3.0/src/DAJIN2/core/core_execute.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:39.164806 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      539 2023-08-03 20:56:29.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4691 2023-08-03 21:20:43.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/align.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5635 2023-08-03 09:34:03.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/call_midsv.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      917 2023-06-12 07:02:39.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/check_caches.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7298 2023-07-13 05:01:37.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1259 2023-08-03 20:56:30.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/extract_knockin_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11512 2023-08-04 02:31:12.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/extract_mutation_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5542 2023-08-04 01:01:01.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/format_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    14012 2023-08-06 06:11:48.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/generate_insertion_fasta.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3855 2023-08-03 20:56:31.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/get_index_mapping.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12144 2023-07-13 04:33:49.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/tmp_extract_errors_in_knockin_loci.py.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     9969 2023-07-13 04:33:52.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/tmp_extract_mutation_loci_with_indexmapping.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    13952 2023-08-05 11:25:00.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/tmp_generate_truncated_fasta.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.3.0/src/DAJIN2/core/preprocess/tmp_replace_NtoD.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:39.371231 DAJIN2-0.3.0/src/DAJIN2/core/report/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      133 2023-07-21 02:12:00.000000 DAJIN2-0.3.0/src/DAJIN2/core/report/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5125 2023-06-08 04:18:39.000000 DAJIN2-0.3.0/src/DAJIN2/core/report/remove_microhomology.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10543 2023-08-03 05:45:41.000000 DAJIN2-0.3.0/src/DAJIN2/core/report/report_bam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1773 2023-08-06 00:05:58.000000 DAJIN2-0.3.0/src/DAJIN2/core/report/report_files.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6877 2023-08-04 01:06:17.000000 DAJIN2-0.3.0/src/DAJIN2/core/report/report_mutation.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1565 2023-06-07 21:55:43.000000 DAJIN2-0.3.0/src/DAJIN2/core/report/reverse_sam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2883 2023-06-05 08:39:04.000000 DAJIN2-0.3.0/src/DAJIN2/gui.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11134 2023-08-06 23:49:55.000000 DAJIN2-0.3.0/src/DAJIN2/main.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:39.429740 DAJIN2-0.3.0/src/DAJIN2/postprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.3.0/src/DAJIN2/postprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2279 2023-07-21 02:12:19.000000 DAJIN2-0.3.0/src/DAJIN2/postprocess/report.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:39.488495 DAJIN2-0.3.0/src/DAJIN2/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:06:47.000000 DAJIN2-0.3.0/src/DAJIN2/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5196 2023-07-13 07:16:36.000000 DAJIN2-0.3.0/src/DAJIN2/preprocess/validate_inputs.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:37.757101 DAJIN2-0.3.0/src/DAJIN2/static/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:39.524495 DAJIN2-0.3.0/src/DAJIN2/static/css/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.3.0/src/DAJIN2/static/css/style.css
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.3.0/src/DAJIN2/template_igvjs.html
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:39.554496 DAJIN2-0.3.0/src/DAJIN2/templates/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.3.0/src/DAJIN2/templates/index.html
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.3.0/src/DAJIN2/view.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-08-07 00:20:38.078924 DAJIN2-0.3.0/src/DAJIN2.egg-info/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5915 2023-08-07 00:20:37.000000 DAJIN2-0.3.0/src/DAJIN2.egg-info/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2134 2023-08-07 00:20:37.000000 DAJIN2-0.3.0/src/DAJIN2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-08-07 00:20:37.000000 DAJIN2-0.3.0/src/DAJIN2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       47 2023-08-07 00:20:37.000000 DAJIN2-0.3.0/src/DAJIN2.egg-info/entry_points.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      254 2023-08-07 00:20:37.000000 DAJIN2-0.3.0/src/DAJIN2.egg-info/requires.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-08-07 00:20:37.000000 DAJIN2-0.3.0/src/DAJIN2.egg-info/top_level.txt
```

### Comparing `DAJIN2-0.2.4/LICENSE` & `DAJIN2-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/setup.py` & `DAJIN2-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as requirements_file:
     install_requirements = requirements_file.read().splitlines()
 
 setuptools.setup(
     name="DAJIN2",
-    version="0.2.4",
+    version="0.3.0",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
-    description="One-step genotyping tools for Targeted long-read sequencing",
+    description="One-step genotyping tools for targeted long-read sequencing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/DAJIN2",
     install_requires=install_requirements,
     packages=setuptools.find_packages(
         where="src",
     ),
     package_dir={"": "src"},
     entry_points={"console_scripts": ["DAJIN2=DAJIN2.main:execute"]},
     include_package_data=True,
     classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
+        "Development Status :: 3 - Alpha",
+        "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX",
-        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Science/Research",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
 )
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/clustering/merge_clusters.py` & `DAJIN2-0.3.0/src/DAJIN2/core/clustering/merge_clusters.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/consensus/consensus.py` & `DAJIN2-0.3.0/src/DAJIN2/core/consensus/consensus.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,60 @@
 from __future__ import annotations
 
 import re
+import pickle
+from pathlib import Path
 from collections import defaultdict
 from itertools import groupby
 
+###########################################################
+# call position weight matrix (cons_pergentage)
+###########################################################
+
+
+def _count_consecutive_n(cons_percentage: list[dict[str, float]]) -> tuple(int, int):
+    seq = "".join(max(c, key=c.get) for c in cons_percentage)
+    n_left = len(re.match(r"^N*", seq)[0]) if re.match(r"^N*", seq) else 0
+    n_right = len(seq) - len(re.match(r"N*$", seq)[0]) if re.match(r"N*$", seq) else len(seq)
+    return n_left, n_right
+
+
+def _remove_nonconsecutive_n(cons_percentage: list[dict[str, float]]) -> list[dict[str, float]]:
+    """remove nonconsecutive N"""
+    cons_percentage_remove_n = []
+    n_left, n_right = _count_consecutive_n(cons_percentage)
+    for i, cons_per in enumerate(cons_percentage):
+        if i < n_left or i >= n_right:
+            cons_percentage_remove_n.append(cons_per)
+            continue
+        if not cons_per == {"N": 100}:
+            cons_per.pop("N", None)
+        cons_percentage_remove_n.append(cons_per)
+    return cons_percentage_remove_n
+
+
+def _update_percentage(cons_percentage: list[dict[str, float]]) -> list[dict[str, float]]:
+    """replace sequence error as distributing according to proportion of cs tags"""
+    cons_percentage_update = []
+    for cons_per in cons_percentage:
+        if "SEQERROR" not in cons_per:
+            cons_percentage_update.append(cons_per)
+            continue
+        if len(cons_per) == 1 and cons_per["SEQERROR"]:
+            cons_percentage_update.append({"N": 100})
+            continue
+        cons_per_update = dict()
+        div = 100 / (sum(cons_per.values()) - cons_per["SEQERROR"])
+        for key, val in cons_per.items():
+            if key == "SEQERROR":
+                continue
+            cons_per_update[key] = val * div
+        cons_percentage_update.append(cons_per_update)
+    return cons_percentage_update
+
 
 def _call_percentage(cssplits: list[str], mutation_loci) -> list[dict[str, float]]:
     """call position weight matrix in defferent loci.
     - non defferent loci are annotated to "Match" or "Unknown(N)"
     - sequence errors are annotated to "SEQERROR"
     """
     cssplits_transposed = [list(cs) for cs in zip(*cssplits)]
@@ -15,66 +62,59 @@
     cons_percentage = []
     for cs_transposed, mut_loci in zip(cssplits_transposed, mutation_loci):
         count_cs = defaultdict(float)
         for cs in cs_transposed:
             if cs[0] in {"+", "-", "*"} and cs[0] not in mut_loci:
                 cs = "SEQERROR"
             count_cs[cs] += 1 / coverage * 100
-        count_cs_sorted = dict(sorted(count_cs.items(), key=lambda x: x[1], reverse=True))
-        cons_percentage.append(count_cs_sorted)
+        cons_percentage.append(count_cs)
+    cons_percentage = _remove_nonconsecutive_n(cons_percentage)
+    cons_percentage = _update_percentage(cons_percentage)
     return cons_percentage
 
 
-def _replace_percentage(cons_percentage: list[dict[str, float]]) -> list[dict[str, float]]:
-    """replace sequence error as distributing according to proportion of cs tags"""
-    cons_percentage_updated = []
-    for dict_percentage in cons_percentage:
-        if "SEQERROR" not in dict_percentage:
-            cons_percentage_updated.append(dict_percentage)
-            continue
-        if len(dict_percentage) == 1 and dict_percentage["SEQERROR"]:
-            cons_percentage_updated.append({"N": 100})
-            continue
-        dict_percentage_update = dict()
-        div = 100 / (100 - dict_percentage["SEQERROR"])
-        for key, val in dict_percentage.items():
-            if key == "SEQERROR":
-                continue
-            dict_percentage_update[key] = round(val * div, 5)
-        cons_percentage_updated.append(dict_percentage_update)
-    return cons_percentage_updated
+###########################################################
+# Call sequence
+###########################################################
+
+
+def _process_base(cons: str) -> str:
+    if cons.startswith("="):  # match
+        return cons.replace("=", "")
+    elif cons.startswith("-"):  # deletion
+        return ""
+    elif cons.startswith("*"):  # substitution
+        return cons[-1]
+    elif cons.startswith("+"):  # insertion
+        cons_ins = cons.split("|")
+        if cons_ins[-1].startswith("="):  # match after insertion
+            cons = cons.replace("=", "")
+        elif cons_ins[-1].startswith("-"):  # deletion after insertion
+            cons = "".join(cons_ins[:-1])
+        elif cons_ins[-1].startswith("*"):  # substitution after insertion
+            cons = "".join([*cons_ins[:-1], cons_ins[-1][-1]])
+        return cons.replace("+", "").replace("|", "")
+    return cons
 
 
 def _call_sequence(cons_percentage: list[dict[str, float]]) -> str:
     consensus_sequence = []
-    for cons_per in cons_percentage:
-        cons = max(cons_per, key=cons_per.get)
-        if cons.startswith("="):
-            cons = cons.replace("=", "")
-        elif cons.startswith("-"):
-            continue
-        elif cons.startswith("*"):
-            cons = cons[-1]
-        elif cons.startswith("+"):
-            cons_ins = cons.split("|")
-            if cons_ins[-1].startswith("="):
-                cons = cons.replace("=", "")
-            elif cons_ins[-1].startswith("-"):
-                cons = "".join(cons_ins[:-1])
-            elif cons_ins[-1].startswith("*"):
-                cons = "".join([*cons_ins[:-1], cons_ins[-1][-1]])
-            cons = cons.replace("+", "")
-            cons = cons.replace("|", "")
-        consensus_sequence.append(cons)
+    n_left, n_right = _count_consecutive_n(cons_percentage)
+    for i, cons_per in enumerate(cons_percentage):
+        if i < n_left or i >= n_right:
+            consensus_sequence.append("N")
+        else:
+            cons = max(cons_per, key=cons_per.get)
+            consensus_sequence.append(_process_base(cons))
     return "".join(consensus_sequence)
 
 
-def _detect_sv(cons_percentage: defaultdict[list], threshold: int = 50) -> list[bool]:
+def _detect_sv(cons_percentages: defaultdict[list], threshold: int = 50) -> list[bool]:
     exists_sv = []
-    for cons_per in cons_percentage.values():
+    for cons_per in cons_percentages.values():
         cons_cssplits = []
         for cssplit in cons_per:
             seq = max(cssplit, key=cssplit.get)
             cons_cssplits.append(seq)
         cons_cssplits = "".join(cons_cssplits)
         if "N" * threshold in cons_cssplits:
             exists_sv.append(True)
@@ -92,43 +132,61 @@
 
 
 ###########################################################
 # main
 ###########################################################
 
 
-def call_consensus(clust_sample: list[dict], MUTATION_LOCI_LABELS) -> tuple[defaultdict[list], defaultdict[str]]:
-    cons_percentage = defaultdict(list)
-    cons_sequence = defaultdict(str)
+def call_consensus(
+    TEMPDIR: Path, SAMPLE_NAME: str, clust_sample: list[dict]
+) -> tuple[defaultdict[list], defaultdict[str]]:
+    cons_percentages = defaultdict(list)
+    cons_sequences = defaultdict(str)
     clust_sample.sort(key=lambda x: x["LABEL"])
     for label, group in groupby(clust_sample, key=lambda x: x["LABEL"]):
         clust = list(group)
-        keys = (
-            clust[0]["ALLELE"],
-            clust[0]["LABEL"],
-            clust[0]["PERCENT"],
-        )
-        # mutation_loci = MUTATION_LOCI_ALLELES[clust[0]["ALLELE"]]
-        mutation_loci = MUTATION_LOCI_LABELS[label]
+        allele = clust[0]["ALLELE"]
+        keys = (allele, label, clust[0]["PERCENT"])
+        with open(Path(TEMPDIR, SAMPLE_NAME, "mutation_loci", f"{allele}.pickle"), "rb") as p:
+            mutation_loci = pickle.load(p)
         cssplits = [cs["CSSPLIT"].split(",") for cs in clust]
-        cons_per = _call_percentage(cssplits, mutation_loci)
-        cons_per = _replace_percentage(cons_per)
-        cons_seq = _call_sequence(cons_per)
-        cons_percentage[keys] = cons_per
-        cons_sequence[keys] = cons_seq
-    return cons_percentage, cons_sequence
+        cons_percentage = _call_percentage(cssplits, mutation_loci)
+        # cons_percentage = _replace_percentage(cons_percentage)
+        cons_percentages[keys] = cons_percentage
+        cons_sequences[keys] = _call_sequence(cons_percentage)
+    return cons_percentages, cons_sequences
+
+
+# def call_consensus(clust_sample: list[dict], MUTATION_LOCI_LABELS) -> tuple[defaultdict[list], defaultdict[str]]:
+#     cons_percentages = defaultdict(list)
+#     cons_sequences = defaultdict(str)
+#     clust_sample.sort(key=lambda x: x["LABEL"])
+#     for label, group in groupby(clust_sample, key=lambda x: x["LABEL"]):
+#         clust = list(group)
+#         keys = (
+#             clust[0]["ALLELE"],
+#             clust[0]["LABEL"],
+#             clust[0]["PERCENT"],
+#         )
+#         mutation_loci = MUTATION_LOCI_LABELS[label]
+#         cssplits = [cs["CSSPLIT"].split(",") for cs in clust]
+#         cons_percentage = _call_percentage(cssplits, mutation_loci)
+#         cons_percentage = _replace_percentage(cons_percentage)
+#         cons_percentages[keys] = cons_percentage
+#         cons_sequences[keys] = _call_sequence(cons_percentage)
+#     return cons_percentages, cons_sequences
 
 
 def call_allele_name(
-    cons_sequence: defaultdict[dict], cons_percentage: defaultdict[list], FASTA_ALLELES: dict
+    cons_sequences: defaultdict[dict], cons_percentages: defaultdict[list], FASTA_ALLELES: dict
 ) -> dict[int, str]:
-    exists_sv = _detect_sv(cons_percentage)
-    label_digits = len(str(len(cons_percentage)))
+    exists_sv = _detect_sv(cons_percentages)
+    label_digits = len(str(len(cons_percentages)))
     allele_names = {}
-    for is_sv, (keys, cons_seq) in zip(exists_sv, cons_sequence.items()):
+    for is_sv, (keys, cons_seq) in zip(exists_sv, cons_sequences.items()):
         ALLELE, LABEL, PERCENT = keys
         label_format = f"{LABEL:0{label_digits}}"
         allele_name = f"allele{label_format}_{ALLELE}"
         if cons_seq == FASTA_ALLELES[ALLELE]:
             allele_name += "_intact"
         elif is_sv:
             allele_name += "_sv"
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/consensus/extract_mutation_loci_by_labels.py` & `DAJIN2-0.3.0/src/DAJIN2/core/consensus/extract_mutation_loci_by_labels.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,46 +7,49 @@
 from DAJIN2.core.preprocess.extract_mutation_loci import (
     discard_errors_in_homopolymer,
     call_coverage_on_each_base,
     count_indels,
     normalize_indels,
     split_kmer,
     extract_dissimilar_loci,
+    extract_anomal_loci,
+    merge_loci,
+    add_knockin_loci,
     transpose_mutation_loci,
+    merge_index_of_consecutive_insertions,
 )
 from DAJIN2.core.preprocess.extract_errors_in_homopolymer import extract_errors_in_homopolymer
 
 
-def _extract_errors_in_homopolymer(indels_sample, indels_control, sequence, dissimilar_loci) -> dict[str, set]:
-    errors_in_homopolymer = dict()
-    for mut in ["+", "-", "*"]:
-        indels_sample_mut = indels_sample[mut]
-        indels_control_mut = indels_control[mut]
-        candidate_loci = dissimilar_loci[mut]
-        error_loci: set = extract_errors_in_homopolymer(indels_sample_mut, indels_control_mut, sequence, candidate_loci)
-        errors_in_homopolymer[mut] = error_loci
-    return errors_in_homopolymer
-
-
-def extract_mutation_loci_by_labels(clust_sample, TEMPDIR, FASTA_ALLELES, CONTROL_NAME):
+def extract_mutation_loci_by_labels(clust_sample, TEMPDIR, FASTA_ALLELES, CONTROL_NAME, SAMPLE_NAME):
     MUTATION_LOCI_LABELS = dict()
     clust_sample.sort(key=lambda x: [x["ALLELE"], x["LABEL"]])
     for (allele, label), group in groupby(clust_sample, key=lambda x: [x["ALLELE"], x["LABEL"]]):
         sequence = FASTA_ALLELES[allele]
         group = list(group)
         coverages_sample = call_coverage_on_each_base(group, sequence)
-        indels_sample = count_indels(group, len(sequence))
+        indels_sample = count_indels(group, sequence)
         indels_sample_normalized = normalize_indels(indels_sample, coverages_sample)
-        indels_kmer_sample = split_kmer(indels_sample_normalized, kmer=10)
-        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_normalized.pkl"), "rb") as f:
+        indels_kmer_sample = split_kmer(indels_sample_normalized, kmer=11)
+        with open(Path(TEMPDIR, CONTROL_NAME, "mutation_loci", f"{allele}_normalized.pickle"), "rb") as f:
             indels_control_normalized = pickle.load(f)
-        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_kmer.pkl"), "rb") as f:
+        with open(Path(TEMPDIR, CONTROL_NAME, "mutation_loci", f"{allele}_kmer.pickle"), "rb") as f:
             indels_kmer_control = pickle.load(f)
-        dissimilar_loci: dict = extract_dissimilar_loci(indels_kmer_sample, indels_kmer_control)
+        # Calculate dissimilar loci
+        dissimilar_loci = extract_dissimilar_loci(indels_kmer_sample, indels_kmer_control)
+        anomal_loci = extract_anomal_loci(indels_sample_normalized, indels_control_normalized)
+        candidate_loci = merge_loci(dissimilar_loci, anomal_loci)
         # Extract error loci in homopolymer regions
-        errors_in_homopolymer = _extract_errors_in_homopolymer(
-            indels_sample_normalized, indels_control_normalized, sequence, dissimilar_loci
+        errors_in_homopolymer = extract_errors_in_homopolymer(
+            sequence, indels_sample_normalized, indels_control_normalized, candidate_loci
         )
-        mutation_loci = discard_errors_in_homopolymer(dissimilar_loci, errors_in_homopolymer)
-        mutation_loci_transposed = transpose_mutation_loci(mutation_loci, len(sequence))
+        mutation_loci = discard_errors_in_homopolymer(candidate_loci, errors_in_homopolymer)
+        # Add all mutations into knockin loci
+        path_knockin = Path(TEMPDIR, SAMPLE_NAME, "knockin_loci", f"{allele}.pickle")
+        if path_knockin.exists():
+            with open(path_knockin, "rb") as p:
+                knockin_loci = pickle.load(p)
+            mutation_loci = add_knockin_loci(mutation_loci, knockin_loci)
+        mutation_loci = merge_index_of_consecutive_insertions(mutation_loci)
+        mutation_loci_transposed = transpose_mutation_loci(mutation_loci, sequence)
         MUTATION_LOCI_LABELS[label] = mutation_loci_transposed
     return MUTATION_LOCI_LABELS
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/core_execute.py` & `DAJIN2-0.3.0/src/DAJIN2/core/core_execute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,90 @@
 from __future__ import annotations
 
 import os
 import sys
-import json
 import pickle
 import resource
 import shutil
 from datetime import datetime
 from pathlib import Path
 
 import midsv
 
+from collections import defaultdict
 from DAJIN2.core import classification, clustering, consensus, preprocess, report
 
 # limit max memory usage
 mem_bytes = os.sysconf("SC_PAGE_SIZE") * os.sysconf("SC_PHYS_PAGES")
 resource.setrlimit(resource.RLIMIT_DATA, (int(mem_bytes * 9 / 10), -1))
 
 
 def _parse_arguments(arguments: dict):
     SAMPLE: str = arguments["sample"]
     CONTROL: str = arguments["control"]
     ALLELE: str = arguments["allele"]
     NAME: str = arguments["name"]
     THREADS: int = arguments["threads"]
+    GENOME_URLS = defaultdict(str)
     if "genome" in arguments:
-        GENOME: str = arguments["genome"]
-        URL_UCSC = arguments["ucsc"]
-        URL_GOLDENPATH = arguments["goldenpath"]
-    else:
-        GENOME = ""
-        URL_UCSC = ""
-        URL_GOLDENPATH = ""
-    return SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME, URL_UCSC, URL_GOLDENPATH
+        GENOME_URLS["genome"] = arguments["genome"]
+        GENOME_URLS["blat"] = arguments["blat"]
+        GENOME_URLS["goldenpath"] = arguments["goldenpath"]
+    return SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME_URLS
 
 
 def _format_inputs(arguments: dict):
-    SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME, URL_UCSC, URL_GOLDENPATH = _parse_arguments(arguments)
+    SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME_URLS = _parse_arguments(arguments)
     SAMPLE = preprocess.format_inputs.convert_to_posix_path(SAMPLE)
     CONTROL = preprocess.format_inputs.convert_to_posix_path(CONTROL)
     ALLELE = preprocess.format_inputs.convert_to_posix_path(ALLELE)
 
     SAMPLE_NAME: str = preprocess.format_inputs.extract_basename(SAMPLE)
     CONTROL_NAME: str = preprocess.format_inputs.extract_basename(CONTROL)
     FASTA_ALLELES: dict = preprocess.format_inputs.dictionize_allele(ALLELE)
 
     TEMPDIR = Path("DAJINResults", ".tempdir", NAME)
-    SUBDIRS = ["cache", "fasta", "sam", "midsv", "clustering", "report", "result", "mutation_loci"]
-    SUBDIRS_REPORT = ["HTML", "FASTA", "BAM", ".igvjs"]
-    preprocess.format_inputs.make_directories(TEMPDIR, SUBDIRS, SUBDIRS_REPORT, SAMPLE_NAME, CONTROL_NAME)
+    Path(TEMPDIR, "cache", ".igvjs", CONTROL_NAME).mkdir(parents=True, exist_ok=True)
 
     IS_CACHE_CONTROL = preprocess.check_caches.exists_cached_control(CONTROL, TEMPDIR)
-    IS_CACHE_GENOME = preprocess.check_caches.exists_cached_genome(GENOME, TEMPDIR, IS_CACHE_CONTROL)
-    if GENOME:
+    IS_CACHE_GENOME = preprocess.check_caches.exists_cached_genome(GENOME_URLS["genome"], TEMPDIR, IS_CACHE_CONTROL)
+
+    GENOME_COODINATES = {
+        "genome": GENOME_URLS["genome"],
+        "chrom_size": 0,
+        "chr": "control",
+        "start": 0,
+        "end": len(FASTA_ALLELES["control"]) - 1,
+        "strand": "+",
+    }
+    if GENOME_URLS["genome"]:
         if not IS_CACHE_GENOME:
-            GENOME_COODINATES = preprocess.format_inputs.fetch_coordinate(GENOME, URL_UCSC, FASTA_ALLELES["control"])
-            CHROME_SIZE = preprocess.format_inputs.fetch_chrom_size(GENOME_COODINATES["chr"], GENOME, URL_GOLDENPATH)
-            preprocess.format_inputs.cache_coodinates_and_chromsize(TEMPDIR, GENOME, GENOME_COODINATES, CHROME_SIZE)
+            GENOME_COODINATES = preprocess.format_inputs.fetch_coordinate(
+                GENOME_COODINATES, GENOME_URLS, FASTA_ALLELES["control"]
+            )
+            GENOME_COODINATES = preprocess.format_inputs.fetch_chrom_size(GENOME_COODINATES, GENOME_URLS)
+            midsv.write_jsonl([GENOME_COODINATES], Path(TEMPDIR, "cache", "genome_coodinates.jsonl"))
         else:
-            GENOME_COODINATES = json.loads(Path(TEMPDIR, "cache", "genome_coodinates.jsonl").read_text())
-            CHROME_SIZE = int(Path(TEMPDIR, "cache", "chrome_size.txt").read_text())
-    return SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, CHROME_SIZE, THREADS
+            GENOME_COODINATES = midsv.read_jsonl(Path(TEMPDIR, "cache", "genome_coodinates.jsonl"))
+    return SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, THREADS
 
 
 def _dtnow() -> str:
     return datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
 
 def execute_control(arguments: dict):
     print(f"{_dtnow()}: {arguments['control']} is now processing...", file=sys.stderr)
     ###########################################################
     # Preprocess
     ###########################################################
-    SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME, _, _ = _parse_arguments(arguments)
-    _, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, CHROME_SIZE, THREADS = _format_inputs(arguments)
+    SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME_URLS = _parse_arguments(arguments)
+    SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, THREADS = _format_inputs(arguments)
+    preprocess.format_inputs.make_directories(TEMPDIR, CONTROL_NAME, is_control=True)
+    preprocess.format_inputs.make_report_directories(TEMPDIR, CONTROL_NAME, is_control=True)
     ###########################################################
     # Check caches
     ###########################################################
     if Path(TEMPDIR, "report", "BAM", CONTROL_NAME, f"{CONTROL_NAME}.bam").exists():
         print(
             f"{arguments['control']} is already preprocessed and reuse the results for the current run...",
             file=sys.stderr,
@@ -86,120 +93,138 @@
     print(f"{_dtnow()}: Preprocess {arguments['control']}...", file=sys.stderr)
     ###########################################################
     # Mapping
     ###########################################################
     # ============================================================
     # Export fasta files as single-FASTA format
     # ============================================================
-    for identifier, sequence in FASTA_ALLELES.items():
-        contents = "\n".join([">" + identifier, sequence]) + "\n"
-        output_fasta = Path(TEMPDIR, "fasta", f"{identifier}.fasta")
-        output_fasta.write_text(contents)
+    preprocess.format_inputs.export_fasta_files(TEMPDIR, FASTA_ALLELES, CONTROL_NAME)
     # ============================================================
     # Mapping using mappy
     # ============================================================
-    for path_fasta in Path(TEMPDIR, "fasta").glob("*.fasta"):
-        name_fasta = path_fasta.stem
-        preprocess.mappy_align.output_sam(TEMPDIR, path_fasta, name_fasta, CONTROL, CONTROL_NAME, threads=THREADS)
-        preprocess.mappy_align.output_sam(
-            TEMPDIR, path_fasta, name_fasta, CONTROL, CONTROL_NAME, preset="splice", threads=THREADS
-        )
+    paths_fasta = Path(TEMPDIR, CONTROL_NAME, "fasta").glob("*.fasta")
+    preprocess.align.generate_sam(TEMPDIR, paths_fasta, CONTROL, CONTROL_NAME, THREADS)
     ###########################################################
     # MIDSV conversion
     ###########################################################
     preprocess.call_midsv(TEMPDIR, FASTA_ALLELES, CONTROL_NAME)
     ###########################################################
+    # Prepare data to `extract mutaion loci`
+    ###########################################################
+    # preprocess.save_index_mapping(TEMPDIR)
+    preprocess.extract_mutation_loci(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME, CONTROL_NAME, is_control=True)
+    ###########################################################
     # Output BAM
     ###########################################################
     print(f"{_dtnow()}: Output BAM files of {arguments['control']}...", file=sys.stderr)
-    report.report_bam.output_bam_control(TEMPDIR, CONTROL_NAME, GENOME, GENOME_COODINATES, CHROME_SIZE, THREADS)
+    report.report_bam.output_bam(TEMPDIR, CONTROL_NAME, GENOME_COODINATES, THREADS, is_control=True)
     ###########################################################
     # Finish call
     ###########################################################
     print(f"{_dtnow()}: \N{teacup without handle} {arguments['control']} is finished!", file=sys.stderr)
 
 
 def execute_sample(arguments: dict):
     print(f"{_dtnow()}: {arguments['sample']} is now processing...", file=sys.stderr)
     ###########################################################
     # Preprocess
     ###########################################################
-    SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME, _, _ = _parse_arguments(arguments)
-    SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, CHROME_SIZE, THREADS = _format_inputs(
-        arguments
-    )
+    SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME_URLS = _parse_arguments(arguments)
+    SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, THREADS = _format_inputs(arguments)
+    preprocess.format_inputs.make_directories(TEMPDIR, SAMPLE_NAME)
+    preprocess.format_inputs.make_report_directories(TEMPDIR, SAMPLE_NAME)
+
     print(f"{_dtnow()}: Preprocess {arguments['sample']}...", file=sys.stderr)
+
+    for path_fasta in Path(TEMPDIR, CONTROL_NAME, "fasta").glob("*.fasta"):
+        shutil.copy(path_fasta, Path(TEMPDIR, SAMPLE_NAME, "fasta"))
     # ============================================================
     # Mapping with mappy
     # ============================================================
-    for path_fasta in Path(TEMPDIR, "fasta").glob("*.fasta"):
-        name_fasta = path_fasta.stem
-        preprocess.mappy_align.output_sam(TEMPDIR, path_fasta, name_fasta, SAMPLE, SAMPLE_NAME, threads=THREADS)
-        preprocess.mappy_align.output_sam(
-            TEMPDIR, path_fasta, name_fasta, SAMPLE, SAMPLE_NAME, preset="splice", threads=THREADS
-        )
+    paths_fasta = Path(TEMPDIR, SAMPLE_NAME, "fasta").glob("*.fasta")
+    preprocess.align.generate_sam(TEMPDIR, paths_fasta, SAMPLE, SAMPLE_NAME, THREADS)
     # ============================================================
     # MIDSV conversion
     # ============================================================
     preprocess.call_midsv(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME)
     # ============================================================
     # Extract mutation loci
     # ============================================================
-    MUTATION_LOCI_ALLELES = preprocess.extract_mutation_loci(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME, CONTROL_NAME)
-    KNOCKIN_LOCI_ALLELES = preprocess.extract_knockin_loci(TEMPDIR)
-    with open(Path(TEMPDIR, "mutation_loci", f"{SAMPLE_NAME}.plk"), "wb") as p:
-        pickle.dump(MUTATION_LOCI_ALLELES, p)
+    preprocess.extract_knockin_loci(TEMPDIR, SAMPLE_NAME)
+    preprocess.extract_mutation_loci(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME, CONTROL_NAME)
+    # ============================================================
+    # Detect and align insertion alleles
+    # ============================================================
+    paths_predifined_allele = {str(p) for p in Path(TEMPDIR, SAMPLE_NAME, "fasta").glob("*.fasta")}
+    preprocess.generate_insertion_fasta(TEMPDIR, SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES)
+    paths_insertion = {str(p) for p in Path(TEMPDIR, SAMPLE_NAME, "fasta").glob("insertion*.fasta")}
+    paths_insertion -= paths_predifined_allele
+    if paths_insertion:
+        # mapping to insertion alleles
+        preprocess.align.generate_sam(TEMPDIR, paths_insertion, CONTROL, CONTROL_NAME, THREADS)
+        preprocess.align.generate_sam(TEMPDIR, paths_insertion, SAMPLE, SAMPLE_NAME, THREADS)
+        # add insertions to FASTA_ALLELES
+        for path_fasta in paths_insertion:
+            allele, seq = Path(path_fasta).read_text().strip().split("\n")
+            allele = allele.replace(">", "")
+            FASTA_ALLELES[allele] = seq
+        # MIDSV conversion
+        preprocess.call_midsv(TEMPDIR, FASTA_ALLELES, CONTROL_NAME)
+        preprocess.call_midsv(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME)
+        # Reculculate mutation loci
+        preprocess.extract_mutation_loci(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME, CONTROL_NAME, is_control=True)
+        preprocess.extract_knockin_loci(TEMPDIR, SAMPLE_NAME)
+        preprocess.extract_mutation_loci(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME, CONTROL_NAME)
     ########################################################################
     # Classify alleles
     ########################################################################
     print(f"{_dtnow()}: Classify {arguments['sample']}...", file=sys.stderr)
     classif_sample = classification.classify_alleles(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME)
+    with open(Path(TEMPDIR, SAMPLE_NAME, "classif_sample.pickle"), "wb") as p:
+        pickle.dump(classif_sample, p)
     ########################################################################
     # Clustering
     ########################################################################
     print(f"{_dtnow()}: Clustering {arguments['sample']}...", file=sys.stderr)
-    clust_sample = clustering.add_labels(
-        classif_sample, TEMPDIR, SAMPLE_NAME, CONTROL_NAME, MUTATION_LOCI_ALLELES, KNOCKIN_LOCI_ALLELES, THREADS
-    )
+    clust_sample = clustering.add_labels(classif_sample, TEMPDIR, SAMPLE_NAME, CONTROL_NAME, THREADS)
     clust_sample = clustering.add_readnum(clust_sample)
     clust_sample = clustering.add_percent(clust_sample)
     clust_sample = clustering.update_labels(clust_sample)
-    with open(Path(TEMPDIR, "clustering", f"{SAMPLE_NAME}.plk"), "wb") as p:
+    with open(Path(TEMPDIR, SAMPLE_NAME, "clust_sample.pickle"), "wb") as p:
         pickle.dump(clust_sample, p)
     ########################################################################
     # Consensus call
     ########################################################################
     print(f"{_dtnow()}: Consensus calling of {arguments['sample']}...", file=sys.stderr)
     # Downsampling to 1000 reads in each LABEL
+    # MUTATION_LOCI_LABELS = consensus.extract_mutation_loci_by_labels(
+    #     clust_sample, TEMPDIR, FASTA_ALLELES, CONTROL_NAME, SAMPLE_NAME
+    # )
     clust_subset_sample = consensus.subset_clust(clust_sample, 1000)
-    MUTATION_LOCI_LABELS = consensus.extract_mutation_loci_by_labels(clust_sample, TEMPDIR, FASTA_ALLELES, CONTROL_NAME)
-    cons_percentage, cons_sequence = consensus.call_consensus(clust_subset_sample, MUTATION_LOCI_LABELS)
+    cons_percentage, cons_sequence = consensus.call_consensus(TEMPDIR, SAMPLE_NAME, clust_subset_sample)
+    # cons_percentage, cons_sequence = consensus.call_consensus(clust_subset_sample, MUTATION_LOCI_LABELS)
     allele_names = consensus.call_allele_name(cons_sequence, cons_percentage, FASTA_ALLELES)
     cons_percentage = consensus.update_key_by_allele_name(cons_percentage, allele_names)
     cons_sequence = consensus.update_key_by_allele_name(cons_sequence, allele_names)
     RESULT_SAMPLE = consensus.add_key_by_allele_name(clust_sample, allele_names)
     RESULT_SAMPLE.sort(key=lambda x: x["LABEL"])
     ########################################################################
     # Output Report：RESULT/FASTA/HTML/BAM
     ########################################################################
     print(f"{_dtnow()}: Output reports of {arguments['sample']}...", file=sys.stderr)
     # RESULT
     midsv.write_jsonl(RESULT_SAMPLE, Path(TEMPDIR, "result", f"{SAMPLE_NAME}.jsonl"))
     # FASTA
-    for header, cons_seq in cons_sequence.items():
-        cons_fasta = report.report_files.to_fasta(header, cons_seq)
-        Path(TEMPDIR, "report", "FASTA", SAMPLE_NAME, f"{SAMPLE_NAME}_{header}.fasta").write_text(cons_fasta)
+    report.report_files.to_fasta(TEMPDIR, SAMPLE_NAME, cons_sequence)
     # HTML
-    for header, cons_per in cons_percentage.items():
-        cons_html = report.report_files.to_html(header, cons_per)
-        Path(TEMPDIR, "report", "HTML", SAMPLE_NAME, f"{SAMPLE_NAME}_{header}.html").write_text(cons_html)
+    report.report_files.to_html(TEMPDIR, SAMPLE_NAME, cons_percentage)
+    # CSV (Allele Info)
+    report.report_mutation.to_csv(TEMPDIR, SAMPLE_NAME, GENOME_COODINATES, cons_percentage)
     # BAM
-    report.report_bam.output_bam_sample(
-        TEMPDIR, RESULT_SAMPLE, SAMPLE_NAME, GENOME, GENOME_COODINATES, CHROME_SIZE, THREADS
-    )
+    report.report_bam.output_bam(TEMPDIR, SAMPLE_NAME, GENOME_COODINATES, THREADS, RESULT_SAMPLE)
     for path_bam_igvjs in Path(TEMPDIR, "cache", ".igvjs").glob(f"{CONTROL_NAME}_control.bam*"):
         shutil.copy(path_bam_igvjs, Path(TEMPDIR, "report", ".igvjs", SAMPLE_NAME))
     # VCF
     # working in progress
     ###########################################################
     # Finish call
     ###########################################################
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/call_midsv.py` & `DAJIN2-0.3.0/src/DAJIN2/core/preprocess/call_midsv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import json
+# import json
 import re
 from itertools import chain, groupby
 from pathlib import Path
 from typing import Generator
 
 import midsv
 
@@ -81,22 +81,22 @@
             if alignment[0] in qname_of_map_ont:
                 yield alignment
         else:
             if alignment[0] not in qname_of_map_ont:
                 yield alignment
 
 
-def midsv_transform(sam: Generator[list[str]]) -> Generator[list[str]]:
-    for midsv_sample in midsv.transform(sam, midsv=False, cssplit=True, qscore=False):
+def midsv_transform(sam: Generator[list[str]]) -> Generator[list[dict]]:
+    for midsv_sample in midsv.transform(sam, midsv=False, cssplit=True, qscore=False, keep=set(["FLAG"])):
         yield midsv_sample
 
 
-def replaceNtoD(midsv_sample: Generator[list[str]], sequence: str) -> Generator[dict[str, str]]:
+def replace_n_to_d(midsv_sample: Generator[list[dict]], sequence: str) -> Generator[list[dict]]:
+    """Replace contiguous N with D, but not contiguous from both ends"""
     for samp in midsv_sample:
-        qname = samp["QNAME"]
         cssplits = samp["CSSPLIT"].split(",")
         # extract right/left index of the end of sequential Ns
         left_idx_n = 0
         for cs in cssplits:
             if cs != "N":
                 break
             left_idx_n += 1
@@ -106,34 +106,46 @@
                 break
             right_idx_n += 1
         right_idx_n = len(cssplits) - right_idx_n - 1
         # replace sequential Ns within the sequence
         for j, (cs, seq) in enumerate(zip(cssplits, sequence)):
             if left_idx_n <= j <= right_idx_n and cs == "N":
                 cssplits[j] = f"-{seq}"
-        yield {"QNAME": qname, "CSSPLIT": ",".join(cssplits)}
+        samp["CSSPLIT"] = ",".join(cssplits)
+        yield samp
+
+
+def convert_flag_to_strand(midsv_sample: Generator[list[str]]) -> Generator[list[dict]]:
+    """Convert FLAG to STRAND (+ or -)"""
+    for samp in midsv_sample:
+        flag = samp["FLAG"]
+        strand = "-" if flag & 16 else "+"
+        samp["STRAND"] = strand
+        del samp["FLAG"]
+        yield samp
 
 
 ###########################################################
 # main
 ###########################################################
 
 
-def call_midsv(TEMPDIR: Path | str, FASTA_ALLELES: dict, SAMPLE_NAME: str) -> None:
+def call_midsv(TEMPDIR: Path | str, FASTA_ALLELES: dict, NAME: str) -> None:
     for allele, sequence in FASTA_ALLELES.items():
-        path_ont = Path(TEMPDIR, "sam", f"{SAMPLE_NAME}_map-ont_{allele}.sam")
-        path_splice = Path(TEMPDIR, "sam", f"{SAMPLE_NAME}_splice_{allele}.sam")
+        path_output = Path(TEMPDIR, NAME, "midsv", f"{allele}.json")
+        if path_output.exists():
+            continue
+        path_ont = Path(TEMPDIR, NAME, "sam", f"map-ont_{allele}.sam")
+        path_splice = Path(TEMPDIR, NAME, "sam", f"splice_{allele}.sam")
         sam_ont = remove_overlapped_reads(list(midsv.read_sam(path_ont)))
         sam_splice = remove_overlapped_reads(list(midsv.read_sam(path_splice)))
         qname_of_map_ont = extract_qname_of_map_ont(sam_ont, sam_splice)
         sam_of_map_ont = extract_sam(sam_ont, qname_of_map_ont, preset="map-ont")
         sam_of_splice = extract_sam(sam_splice, qname_of_map_ont, preset="splice")
-        # qname_of_map_ont = extract_qname_of_map_ont(midsv.read_sam(path_ont), midsv.read_sam(path_splice))
-        # sam_of_map_ont = extract_sam(midsv.read_sam(path_ont), qname_of_map_ont, preset="map-ont")
-        # sam_of_splice = extract_sam(midsv.read_sam(path_splice), qname_of_map_ont, preset="splice")
         sam_chained = chain(sam_of_map_ont, sam_of_splice)
         midsv_chaind = midsv_transform(sam_chained)
-        midsv_sample = replaceNtoD(midsv_chaind, sequence)
-        filepath = Path(TEMPDIR, "midsv", f"{SAMPLE_NAME}_{allele}.json")
-        with open(filepath, "wt", encoding="utf-8") as f:
-            for data in midsv_sample:
-                f.write(json.dumps(data) + "\n")
+        midsv_sample = replace_n_to_d(midsv_chaind, sequence)
+        midsv_sample = convert_flag_to_strand(midsv_sample)
+        midsv.write_jsonl(midsv_sample, path_output)
+        # with open(path_output, "wt", encoding="utf-8") as f:
+        #     for data in midsv_sample:
+        #         f.write(json.dumps(data) + "\n")
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/check_caches.py` & `DAJIN2-0.3.0/src/DAJIN2/core/preprocess/check_caches.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py` & `DAJIN2-0.3.0/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 import re
 from collections import defaultdict
 import numpy as np
 import scipy
 from statsmodels.nonparametric.smoothers_lowess import lowess as sm_lowess
 
 
-def get_repeat_regions(sequence: str, candidate_loci: set(int)) -> list[tuple[int, int]]:
+def get_repeat_regions(sequence: str, loci: set[int]) -> list[tuple[int, int]]:
     """
     Find homopolymers in the sequence but discard them that
     are adjacent to candidate mutation loci because they are
     likely to be covered by the real mutations
     """
     pattern = r"A{4,}|C{4,}|G{4,}|T{4,}|N{4,}"
     repeat_regions = []
     for start, end in (match.span() for match in re.finditer(pattern, sequence)):
-        if not (start - 1 in candidate_loci and end + 1 in candidate_loci):
+        if not (start - 1 in loci and end + 1 in loci):
             repeat_regions.append((start, end))
     return repeat_regions
 
 
-def get_counts_homopolymer(indels_sample_mut, indels_control_mut, repeat_regions):
+def get_counts_homopolymer(
+    indels_sample_mut, indels_control_mut, repeat_regions
+) -> tuple[dict[int, list[float]], list[tuple[int, int, np.array]]]:
     # Initialize default dictionaries to hold counts
     mutation_counts = defaultdict(list)
     mutation_counts_regions = []
     # Iterate through each repeat region
     for start, end in repeat_regions:
         # Calculate mutations for each sample and control
         sample_mutations = np.array(indels_sample_mut[start:end])
@@ -118,17 +120,42 @@
 
 
 ###########################################################
 # main
 ###########################################################
 
 
-def extract_errors_in_homopolymer(indels_sample_mut, indels_control_mut, sequence, candidate_loci) -> set(int):
-    repeat_regions = get_repeat_regions(sequence, candidate_loci)
-    if repeat_regions == []:
-        return set()
-    mutation_counts, mutation_counts_regions = get_counts_homopolymer(
-        indels_sample_mut, indels_control_mut, repeat_regions
-    )
-    thresholds = return_thresholds(mutation_counts)
-    errors_in_homopolyer = get_errors_in_homopolyer(mutation_counts_regions, thresholds)
-    return errors_in_homopolyer
+def extract_errors_in_homopolymer(
+    sequence, indels_sample, indels_control, candidate_loci: dict[set]
+) -> dict[str, set(int)]:
+    errors_in_homopolymer = dict()
+    for mut in ["+", "-", "*"]:
+        repeat_regions = get_repeat_regions(sequence, candidate_loci[mut])
+        if repeat_regions == []:
+            errors_in_homopolymer[mut] = set()
+            continue
+        mutation_counts, mutation_counts_regions = get_counts_homopolymer(
+            indels_sample[mut], indels_control[mut], repeat_regions
+        )
+        thresholds = return_thresholds(mutation_counts)
+        errors_in_homopolymer[mut] = get_errors_in_homopolyer(mutation_counts_regions, thresholds)
+    return errors_in_homopolymer
+
+
+# def _extract_errors_in_homopolymer(sequence, indels_sample_mut, indels_control_mut, candidate_loci) -> set(int):
+#     repeat_regions = get_repeat_regions(sequence, candidate_loci)
+#     if repeat_regions == []:
+#         return set()
+#     mutation_counts, mutation_counts_regions = get_counts_homopolymer(
+#         indels_sample_mut, indels_control_mut, repeat_regions
+#     )
+#     thresholds = return_thresholds(mutation_counts)
+#     errors_in_homopolyer = get_errors_in_homopolyer(mutation_counts_regions, thresholds)
+#     return errors_in_homopolyer
+
+
+# def extract_errors_in_homopolymer(sequence, indels_sample, indels_control, candidate_loci) -> dict[str, set]:
+#     errors_in_homopolymer = dict()
+#     for mut in ["+", "-", "*"]:
+#         error_loci: set = _extract_errors_in_homopolymer(sequence, indels_sample[mut], indels_control[mut], candidate_loci[mut])
+#         errors_in_homopolymer[mut] = error_loci
+#     return errors_in_homopolymer
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_mutation_loci.py` & `DAJIN2-0.3.0/src/DAJIN2/core/preprocess/tmp_extract_mutation_loci_with_indexmapping.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,29 +16,33 @@
 
 def read_midsv(filepath) -> Generator[dict[str, str]]:
     with open(filepath, "r") as f:
         for line in f:
             yield json.loads(line)
 
 
-def call_coverage_on_each_base(midsv_sample: Generator[dict], sequence: str) -> list[int]:
+def call_coverage_on_each_base(midsv_sample: Generator[dict], sequence: str, index_mapping: dict) -> list[int]:
     coverages = [1] * len(sequence)
-    for cont in midsv_sample:
-        cssplits = cont["CSSPLIT"].split(",")
-        for i, cssplit in enumerate(cssplits):
-            if cssplit == "N":
+    for samp in midsv_sample:
+        for i, cs in enumerate(samp["CSSPLIT"].split(",")):
+            if i not in index_mapping:
                 continue
-            coverages[i] += 1
+            if cs == "N":
+                continue
+            coverages[index_mapping[i]] += 1
     return coverages
 
 
-def count_indels(midsv_sample, len_sequence: int) -> dict[str, list[int]]:
+def count_indels(midsv_sample, sequence: str, index_mapping: dict) -> dict[str, list[int]]:
+    len_sequence = len(sequence)
     count = {"+": [0] * len_sequence, "-": [0] * len_sequence, "*": [0] * len_sequence}
     for samp in midsv_sample:
         for i, cs in enumerate(samp["CSSPLIT"].split(",")):
+            if i not in index_mapping:
+                continue
             if cs.startswith("=") or cs == "N" or re.search(r"a|c|g|t|n", cs):
                 continue
             if cs.startswith("+"):
                 # count["+"][i] += len(cs.split("|"))
                 count["+"][i] += 1
             elif cs.startswith("-"):
                 count["-"][i] += 1
@@ -52,15 +56,15 @@
     coverages = np.array(coverages)
     for mut in count:
         counts = np.array(count[mut])
         count_normalized[mut] = counts / coverages
     return count_normalized
 
 
-def split_kmer(indels: dict[str, np.array], kmer: int = 10) -> dict[str, np.array]:
+def split_kmer(indels: dict[str, np.array], kmer: int = 11) -> dict[str, np.array]:
     results = defaultdict(list)
     center = kmer // 2
     for mut, value in indels.items():
         for i in range(len(value)):
             if center <= i <= len(value) - center:
                 start = i - center
                 if kmer % 2 == 0:
@@ -69,91 +73,142 @@
                     end = i + center + 1
                 results[mut].append(value[start:end])
             else:
                 results[mut].append(np.array([0] * kmer))
     return results
 
 
+def merge_peaks(indels_sample_normalized, mutation, peaks, hight):
+    """Values higher than 75% quantile of the control values and the surrouings are peaks, merge it as a peak"""
+    values_sample = indels_sample_normalized[mutation]
+    for i, value in enumerate(values_sample):
+        if i not in peaks and value > hight:
+            for j in range(i - 5, i + 6):
+                if j in peaks:
+                    peaks.add(i)
+                    break
+    return peaks
+
+
 def extract_dissimilar_loci(indels_kmer_sample: dict, indels_kmer_control: dict) -> dict[str, set]:
     """
-    Comparing Sample and Control, the 1. 'high similarity',  2. 'similar mean' and
-    3. 'similar variance' are considered as sequence errors.
+    Comparing Sample and Control, the 'similar mean' and
+    'similar variance' are considered as sequence errors.
     """
     results = dict()
     for mut in indels_kmer_sample:
         values_sample = indels_kmer_sample[mut]
         values_control = indels_kmer_control[mut]
-        # Calculate cosine similarity: 1 means exactly same, 0 means completely different.
-        # When calculating cossim, uint32 returns inaccurate results so convert to float64
-        cossim = [1 - distance.cosine(x, y) for x, y in zip(values_sample, values_control)]
+        """
+        Calculate cosine similarity: 1 means exactly same, 0 means completely different.
+        Zero vector does not return correct value, so add epsilon (1e-10).
+        example: distance.cosine([0,0,0], [1,2,3]) retuns 0.
+        """
+        cossims = [1 - distance.cosine(x + 1e-10, y + 1e-10) for x, y in zip(values_sample, values_control)]
         # Perform T-test: nan means exactly same, p > 0.05 means similar in average.
         t_pvalues = [stats.ttest_ind(x, y, equal_var=False)[1] for x, y in zip(values_sample, values_control)]
         t_pvalues = [1 if np.isnan(t) else t for t in t_pvalues]
         # Perform F-test: p > 0.05 means similar in variance.
         f_pvalues = [stats.bartlett(x, y)[1] for x, y in zip(values_sample, values_control)]
         # if pvalue == nan or pval > 0.05, samples and controls are similar.
         dissimilar_loci = set()
-        for i, (sim, t_pval, f_pval) in enumerate(zip(cossim, t_pvalues, f_pvalues)):
-            if not (sim > 0.90 and t_pval > 0.05 and f_pval > 0.05):
+        for i, (cossim, t_pval, f_pval) in enumerate(zip(cossims, t_pvalues, f_pvalues)):
+            # deletion may be the similar cossim, but t_val < 0.05. Others should be dissimilar.
+            if (cossim > 0.9 and t_pval < 0.05) or (cossim < 0.9 and (t_pval < 0.05 or f_pval < 0.05)):
                 dissimilar_loci.add(i)
         results[mut] = dissimilar_loci
     return results
 
 
 def discard_errors_in_homopolymer(dissimilar_loci, errors_in_homopolymer) -> dict[str, set]:
     mutation_loci = dict()
     for mut in ["+", "-", "*"]:
         error_loci = errors_in_homopolymer[mut]
         mutation_loci[mut] = dissimilar_loci[mut] - error_loci
     return mutation_loci
 
 
-def transpose_mutation_loci(mutation_loci: set[int], len_sequence: int) -> list[set]:
-    mutation_loci_transposed = [set() for _ in range(len_sequence)]
+def transpose_mutation_loci(mutation_loci: set[int], sequence: str) -> list[set]:
+    mutation_loci_transposed = [set() for _ in range(len(sequence))]
     for mut, idx_mutation in mutation_loci.items():
         for i, loci in enumerate(mutation_loci_transposed):
             if i in idx_mutation:
                 loci.add(mut)
     return mutation_loci_transposed
 
 
 ###########################################################
 # main
 ###########################################################
 
 
-def extract_mutation_loci(
-    TEMPDIR: Path, FASTA_ALLELES: dict, SAMPLE_NAME: str, CONTROL_NAME: str
-) -> dict[str, list[set[str]]]:
+def process_mutation_loci(TEMPDIR: Path, FASTA_ALLELES: dict, CONTROL_NAME: str) -> None:
+    with open(Path(TEMPDIR, "mutation_loci", "index_mapping..pickle"), "rb") as f:
+        INDEX_MAPPING = pickle.load(f)
+    for allele, sequence in FASTA_ALLELES.items():
+        index_mapping = INDEX_MAPPING.get(allele, {i: i for i in range(len(sequence))})
+        index_mapping = {v: k for k, v in index_mapping.items()}
+        filepath_control = Path(TEMPDIR, "midsv", f"{CONTROL_NAME}_{allele}.json")
+        indels_control = count_indels(read_midsv(filepath_control), sequence, index_mapping)
+        coverages_control = call_coverage_on_each_base(read_midsv(filepath_control), sequence, index_mapping)
+        indels_control_normalized = normalize_indels(indels_control, coverages_control)
+        indels_kmer_control = split_kmer(indels_control_normalized, kmer=11)
+        # Save indels_control_normalized and indels_kmer_control as pickle to reuse in consensus calling
+        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_normalized..pickle"), "wb") as f:
+            pickle.dump(indels_control_normalized, f)
+        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_kmer..pickle"), "wb") as f:
+            pickle.dump(indels_kmer_control, f)
+
+
+def update_mutation_loci(MUTATION_LOCI_ALLELES, INDEX_MAPPING) -> dict[str, list]:
+    """
+    Filter mutations that exists both in control and other alleles
+    """
+    mutation_loci_control = MUTATION_LOCI_ALLELES["control"]
+    for allele in MUTATION_LOCI_ALLELES:
+        if allele == "control":
+            continue
+        index_mapping = INDEX_MAPPING[allele]
+        for i, mut_control in enumerate(mutation_loci_control):
+            corresponded_mutation = mut_control & MUTATION_LOCI_ALLELES[allele][index_mapping[i]]
+            if corresponded_mutation:
+                MUTATION_LOCI_ALLELES[allele][i] = corresponded_mutation
+            else:
+                MUTATION_LOCI_ALLELES["control"][i] = set()
+                MUTATION_LOCI_ALLELES[allele][index_mapping[i]] = set()
+    return MUTATION_LOCI_ALLELES
+
+
+def extract_mutation_loci(TEMPDIR: Path, FASTA_ALLELES: dict, SAMPLE_NAME: str, CONTROL_NAME: str) -> dict[str, list]:
+    with open(Path(TEMPDIR, "mutation_loci", "index_mapping..pickle"), "rb") as f:
+        INDEX_MAPPING = pickle.load(f)
     MUTATION_LOCI_ALLELES = dict()
     for allele, sequence in FASTA_ALLELES.items():
         filepath_sample = Path(TEMPDIR, "midsv", f"{SAMPLE_NAME}_{allele}.json")
-        filepath_control = Path(TEMPDIR, "midsv", f"{CONTROL_NAME}_{allele}.json")
-        indels_sample = count_indels(read_midsv(filepath_sample), len(sequence))
-        indels_control = count_indels(read_midsv(filepath_control), len(sequence))
-        coverages_sample = call_coverage_on_each_base(read_midsv(filepath_sample), sequence)
-        coverages_control = call_coverage_on_each_base(read_midsv(filepath_control), sequence)
+        index_mapping = INDEX_MAPPING.get(allele, {i: i for i in range(len(sequence))})
+        index_mapping = {v: k for k, v in index_mapping.items()}
+        indels_sample = count_indels(read_midsv(filepath_sample), sequence, index_mapping)
+        coverages_sample = call_coverage_on_each_base(read_midsv(filepath_sample), sequence, index_mapping)
         indels_sample_normalized = normalize_indels(indels_sample, coverages_sample)
-        indels_control_normalized = normalize_indels(indels_control, coverages_control)
-        indels_kmer_sample = split_kmer(indels_sample_normalized, kmer=10)
-        indels_kmer_control = split_kmer(indels_control_normalized, kmer=10)
-        # anomaly_loci = _extract_anomaly_loci(indels_kmer_sample, indels_kmer_control)
+        indels_kmer_sample = split_kmer(indels_sample_normalized, kmer=11)
+        # Load indels_control_normalized and indels_kmer_control
+        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_normalized..pickle"), "rb") as f:
+            indels_control_normalized = pickle.load(f)
+        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_kmer..pickle"), "rb") as f:
+            indels_kmer_control = pickle.load(f)
+        # Calculate dissimilar loci
         dissimilar_loci = extract_dissimilar_loci(indels_kmer_sample, indels_kmer_control)
         # Extract error loci in homopolymer regions
         errors_in_homopolymer = dict()
         for mut in ["+", "-", "*"]:
             indels_sample_mut = indels_sample_normalized[mut]
             indels_control_mut = indels_control_normalized[mut]
             candidate_loci = dissimilar_loci[mut]
             # candidate_loci = anomaly_loci[mut] & dissimilar_loci[mut]
             errors_in_homopolymer[mut] = extract_errors_in_homopolymer(
                 indels_sample_mut, indels_control_mut, sequence, candidate_loci
             )
         mutation_loci = discard_errors_in_homopolymer(dissimilar_loci, errors_in_homopolymer)
-        mutation_loci_transposed = transpose_mutation_loci(mutation_loci, len(sequence))
+        mutation_loci_transposed = transpose_mutation_loci(mutation_loci, sequence)
         MUTATION_LOCI_ALLELES[allele] = mutation_loci_transposed
-        # Save indels_control_normalized and indels_kmer_control as pickle to reuse in consensus calling
-        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_normalized.pkl"), "wb") as f:
-            pickle.dump(indels_control_normalized, f)
-        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_kmer.pkl"), "wb") as f:
-            pickle.dump(indels_kmer_control, f)
+    MUTATION_LOCI_ALLELES = update_mutation_loci(MUTATION_LOCI_ALLELES, INDEX_MAPPING)
     return MUTATION_LOCI_ALLELES
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/format_inputs.py` & `DAJIN2-0.3.0/src/DAJIN2/core/preprocess/format_inputs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 from __future__ import annotations
 
-import os
 import re
 from pathlib import Path
 from urllib.request import urlopen
 
 import mappy
-import midsv
 import wslPath
 
 ########################################################################
 # Make directories
 ########################################################################
 
 
-def make_directories(TEMPDIR: Path, SUBDIRS: list[str], SUBDIRS_REPORT: list[str], SAMPLE_NAME: str, CONTROL_NAME: str):
+def make_directories(TEMPDIR: Path, NAME: str, is_control=False) -> None:
+    Path(TEMPDIR, "result").mkdir(parents=True, exist_ok=True)
+    if is_control:
+        SUBDIRS = ["fasta", "sam", "midsv", "mutation_loci", "clustering"]
+    else:
+        SUBDIRS = [
+            "fasta",
+            "sam",
+            "midsv",
+            "mutation_loci",
+            "knockin_loci",
+            "classification",
+            "clustering",
+            "consensus",
+        ]
     for subdir in SUBDIRS:
-        Path(TEMPDIR, subdir).mkdir(parents=True, exist_ok=True)
+        Path(TEMPDIR, NAME, subdir).mkdir(parents=True, exist_ok=True)
+
+
+def make_report_directories(TEMPDIR: Path, NAME: str, is_control=False) -> None:
+    if is_control:
+        Path(TEMPDIR, "report", "BAM", NAME).mkdir(parents=True, exist_ok=True)
+        return
+    SUBDIRS_REPORT = ["HTML", "FASTA", "BAM", "MUTATION_INFO", ".igvjs"]
     for reportdir in SUBDIRS_REPORT:
-        Path(TEMPDIR, "report", reportdir, SAMPLE_NAME).mkdir(parents=True, exist_ok=True)
-    Path(TEMPDIR, "report", "BAM", CONTROL_NAME).mkdir(parents=True, exist_ok=True)
-    Path(TEMPDIR, "cache", ".igvjs").mkdir(parents=True, exist_ok=True)
+        if reportdir == "MUTATION_INFO":
+            Path(TEMPDIR, "report", reportdir).mkdir(parents=True, exist_ok=True)
+        else:
+            Path(TEMPDIR, "report", reportdir, NAME).mkdir(parents=True, exist_ok=True)
 
 
 ########################################################################
 # Convert Path
 ########################################################################
 
 
@@ -70,49 +90,66 @@
 
 
 ########################################################################
 # Fetch genome coodinate and chrom size
 ########################################################################
 
 
-def fetch_coordinate(genome: str, ucsc_url: str, seq: str) -> dict:
-    def _fetch_seq(seq: str):
-        url_blat = f"{ucsc_url}/cgi-bin/hgBlat?db={genome}&type=BLAT&userSeq={seq}"
+def fetch_coordinate(GENOME_COODINATES: dict, GENOME_URLS: dict, seq: str) -> dict:
+    def _fetch_seq(genome: str, seq: str, blat: str):
+        url_blat = f"{blat}?db={genome}&type=BLAT&userSeq={seq}"
         request = urlopen(url_blat).read().decode("utf8").split("\n")
         matches = [x for x in request if "100.0%" in x]
         if not matches:
             raise AttributeError(f"{seq} is not found in {genome}")
         return matches[0].split()[-5:-1]
 
+    genome = GENOME_COODINATES["genome"]
+    blat = GENOME_URLS["blat"]
     seq_start, seq_end = seq[:1000], seq[-1000:]
-    coordinate_start, coordinate_end = _fetch_seq(seq_start), _fetch_seq(seq_end)
+    coordinate_start = _fetch_seq(genome, seq_start, blat)
+    coordinate_end = _fetch_seq(genome, seq_end, blat)
 
     chromosome, strand = coordinate_start[0], coordinate_start[1]
     if strand == "+":
         start, end = int(coordinate_start[2]), int(coordinate_end[3])
     else:
         start, end = int(coordinate_end[2]), int(coordinate_start[3])
 
-    return {"chr": chromosome, "start": start, "end": end, "strand": strand}
+    GENOME_COODINATES["chr"] = chromosome
+    GENOME_COODINATES["start"] = start
+    GENOME_COODINATES["end"] = end
+    GENOME_COODINATES["strand"] = strand
+    return GENOME_COODINATES
 
 
-def fetch_chrom_size(chrom: str, genome: str, goldenpath_url: str) -> int:
-    url = f"{goldenpath_url}/{genome}/bigZips/{genome}.chrom.sizes"
+def fetch_chrom_size(GENOME_COODINATES: dict, GENOME_URLS: dict) -> int:
+    chrom = GENOME_COODINATES["chr"]
+    genome = GENOME_COODINATES["genome"]
+    url_goldenpath = GENOME_URLS["goldenpath"]
+    url = f"{url_goldenpath}/{genome}/bigZips/{genome}.chrom.sizes"
     request = urlopen(url).read().decode("utf8").split("\n")
     for req in request:
         req = req.split("\t")
         if chrom == req[0]:
             chrom_size = int(req[1])
-    return chrom_size
+    GENOME_COODINATES["chrom_size"] = chrom_size
+    return GENOME_COODINATES
+
 
+########################################################################
+# Export fasta files as single-FASTA format
+########################################################################
 
-def cache_coodinates_and_chromsize(TEMPDIR, GENOME, GENOME_COODINATES, CHROME_SIZE) -> None:
+
+def export_fasta_files(TEMPDIR: Path, FASTA_ALLELES: dict, NAME: str) -> None:
     """
-    Save (1) genome_symbol.txt, (2) genome_coodinates.jsonl, (3) chrome_size.txt
+    This function exports FASTA files in single-FASTA format.
+
+    :param TEMPDIR: Temporary directory Path object where the output files will be saved.
+    :param FASTA_ALLELES: Dictionary containing identifier and sequence pairs.
+    :param NAME: Name to be included in the output path.
     """
-    # Save info to the cache directory
-    Path(TEMPDIR, "cache", "genome_symbol.txt").write_text(GENOME + "\n")
-    midsv.write_jsonl([GENOME_COODINATES], Path(TEMPDIR, "cache", "genome_coodinates.jsonl"))
-    Path(TEMPDIR, "cache", "chrome_size.txt").write_text(str(CHROME_SIZE))
-    # Save info to the .igvjs directory
-    Path(TEMPDIR, "report", ".igvjs", "genome_symbol.txt").write_text(GENOME + "\n")
-    midsv.write_jsonl([GENOME_COODINATES], Path(TEMPDIR, "report", ".igvjs", "genome_coodinates.jsonl"))
+    for identifier, sequence in FASTA_ALLELES.items():
+        contents = "\n".join([">" + identifier, sequence]) + "\n"
+        output_fasta = Path(TEMPDIR, NAME, "fasta", f"{identifier}.fasta")
+        output_fasta.write_text(contents)
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/mappy_align.py` & `DAJIN2-0.3.0/src/DAJIN2/core/preprocess/align.py`

 * *Files 21% similar despite different names*

```diff
@@ -82,28 +82,47 @@
             alignment = [str(a) for a in alignment]
             SAM.append("\t".join(alignment))
     for record in SAM:
         yield record
 
 
 def output_sam(
-    tmpdir: Path,
+    TEMPDIR: Path,
     path_fasta: str | Path,
     name_fasta: str,
     path_fastq: str | Path,
     name_fastq: str,
     preset: str = "map-ont",
     threads: int = 1,
 ):
     sam = to_sam(path_fasta, path_fastq, preset=preset, threads=threads)
-    output_sam = Path(tmpdir, "sam", f"{name_fastq}_{preset}_{name_fasta}.sam")
+    output_sam = Path(TEMPDIR, name_fastq, "sam", f"{preset}_{name_fasta}.sam")
     output_sam.write_text("\n".join(sam))
 
 
 ########################################################################
+# main
+########################################################################
+
+
+def generate_sam(TEMPDIR, paths_fasta, path_fastq, name_fastq, THREADS) -> None:
+    for path_fasta in paths_fasta:
+        path_fasta = Path(path_fasta)
+        output_sam(TEMPDIR, path_fasta, path_fasta.stem, path_fastq, name_fastq, preset="map-ont", threads=THREADS)
+        output_sam(TEMPDIR, path_fasta, path_fasta.stem, path_fastq, name_fastq, preset="splice", threads=THREADS)
+
+
+# def generate_sam(TEMPDIR, CONTROL, CONTROL_NAME, THREADS) -> None:
+#     for path_fasta in Path(TEMPDIR, CONTROL_NAME, "fasta").glob("*.fasta"):
+#         name_fasta = path_fasta.stem
+#         output_sam(TEMPDIR, path_fasta, name_fasta, CONTROL, CONTROL_NAME, threads=THREADS)
+#         output_sam(TEMPDIR, path_fasta, name_fasta, CONTROL, CONTROL_NAME, preset="splice", threads=THREADS)
+
+
+########################################################################
 # Create faidx
 ########################################################################
 
 
 def make_faidx(path_fasta: Path | str) -> str:
     fasta = Path(path_fasta).read_text().split()
     name = fasta[0].strip(">")
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/replace_NtoD.py` & `DAJIN2-0.3.0/src/DAJIN2/core/preprocess/tmp_replace_NtoD.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/report/remove_microhomology.py` & `DAJIN2-0.3.0/src/DAJIN2/core/report/remove_microhomology.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2/core/report/reverse_sam.py` & `DAJIN2-0.3.0/src/DAJIN2/core/report/reverse_sam.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2/gui.py` & `DAJIN2-0.3.0/src/DAJIN2/gui.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2/main.py` & `DAJIN2-0.3.0/src/DAJIN2/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import wslPath
 
 from DAJIN2 import gui, view
 from DAJIN2.core import core_execute
 from DAJIN2.postprocess import report
 from DAJIN2.preprocess.validate_inputs import validate_files, validate_genome_and_fetch_urls
 
-VERSION = "0.2.4"
+VERSION = "0.3.0"
 
 # prevent BLAS from using all cores
 os.environ["OMP_NUM_THREADS"] = "1"
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["VECLIB_MAXIMUM_THREADS"] = "1"
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
@@ -66,15 +66,15 @@
     iterator = iter(iterable)
     chunk = tuple(islice(iterator, chunk_size))
     while chunk:
         yield chunk
         chunk = tuple(islice(iterator, chunk_size))
 
 
-def _run_multiprocess(function, arguments: list, num_workers: int = 1) -> None:
+def run_multiprocess(function, arguments: list, num_workers: int = 1) -> None:
     arguments_batched = _batched(arguments, num_workers)
     for args in arguments_batched:
         jobs = []
         for arg in args:
             p = multiprocessing.Process(target=function, args=(arg,))
             jobs.append(p)
             p.start()
@@ -154,29 +154,29 @@
             args["sample"] = args["control"]
             if len(groups) > 1:
                 args["threads"] = 1
             if "genome" in args:
                 args.update(URLS_GENOME[args["genome"]])
             contents_control.append(args)
         contents_control_unique = _extract_unique_contents(contents_control)
-        _run_multiprocess(core_execute.execute_control, contents_control_unique, num_workers)
+        run_multiprocess(core_execute.execute_control, contents_control_unique, num_workers)
         # ------------------------------
         # Handle samples
         # ------------------------------
         contents_sample = []
         for group in groups:
             args = {h: g for h, g in zip(columns, group)}
             if args["sample"] == args["control"]:
                 continue
             if "threads" not in args:
                 args["threads"] = 1
             args.update(URLS_GENOME[args["genome"]])
             contents_sample.append(args)
         contents_sample_unique = _extract_unique_contents(contents_sample)
-        _run_multiprocess(core_execute.execute_sample, contents_sample_unique, num_workers)
+        run_multiprocess(core_execute.execute_sample, contents_sample_unique, num_workers)
         report.report(name)
         print(
             f"\N{party popper} Finished! Open DAJINResults/{name} to see the report.",
             file=sys.stderr,
         )
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/postprocess/report.py` & `DAJIN2-0.3.0/src/DAJIN2/postprocess/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,13 @@
     except ValueError:
         pass
 
 
 def report(name: str):
     report_directory = Path("DAJINResults", name)
     report_directory.mkdir(exist_ok=True, parents=True)
-    for directory in Path("DAJINResults", ".tempdir", name, "report").iterdir():
-        shutil.copytree(directory, Path(report_directory, directory.stem), dirs_exist_ok=True)
+    shutil.copytree(Path("DAJINResults", ".tempdir", name, "report"), report_directory, dirs_exist_ok=True)
     df_all = extract_all_info(Path("DAJINResults", ".tempdir", name, "result"))
     df_all.to_csv(Path(report_directory, "read_all.csv"), index=False)
     df_summary = summarize_info(df_all)
     df_summary.to_csv(Path(report_directory, "read_summary.csv"), index=False)
     output_plot(df_summary, report_directory)
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/preprocess/validate_inputs.py` & `DAJIN2-0.3.0/src/DAJIN2/preprocess/validate_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -64,87 +64,86 @@
 
 
 ########################################################################
 # Check Cache
 ########################################################################
 
 
-def exists_cached_control(CONTROL: str, TEMPDIR: Path) -> bool:
-    PATH_CACHE_HASH = Path(TEMPDIR, "cache", "control_hash.txt")
-    EXISTS_CACHE_CONTROL = False
-    if PATH_CACHE_HASH.exists():
-        current_hash = hashlib.sha256(Path(CONTROL).read_bytes()).hexdigest()
-        cashed_hash = PATH_CACHE_HASH.read_text()
+def exists_cached_control(control: str, tempdir: Path) -> bool:
+    path_cache_hash = Path(tempdir, "cache", "control_hash.txt")
+    if path_cache_hash.exists():
+        current_hash = hashlib.sha256(Path(control).read_bytes()).hexdigest()
+        cashed_hash = path_cache_hash.read_text()
         if current_hash == cashed_hash:
-            EXISTS_CACHE_CONTROL = True
-    return EXISTS_CACHE_CONTROL
+            return True
+    return False
 
 
-def exists_cached_genome(GENOME: str, TEMPDIR: Path, EXISTS_CACHE_CONTROL: bool) -> bool:
-    PATH_CACHE_GENOME = Path(TEMPDIR, "cache", "genome_symbol.txt")
-    EXISTS_CACHE_GENOME = False
-    if GENOME and EXISTS_CACHE_CONTROL and PATH_CACHE_GENOME.exists():
-        cashed_genome = PATH_CACHE_GENOME.read_text()
-        if GENOME == cashed_genome:
-            EXISTS_CACHE_GENOME = True
-    return EXISTS_CACHE_GENOME
+def exists_cached_genome(genome: str, tempdir: Path, exists_cache_control: bool) -> bool:
+    path_cache_genome = Path(tempdir, "cache", "genome_symbol.txt")
+    if genome and exists_cache_control and path_cache_genome.exists():
+        cashed_genome = path_cache_genome.read_text()
+        if genome == cashed_genome:
+            return True
+    return False
 
 
 ########################################################################
 # Check genome and UCSC server
 ########################################################################
 
 
-def _check_url_availabilities(urls: list[str]) -> list[bool]:
-    availabilities = []
-    for url in urls:
-        try:
-            _ = urlopen(url, timeout=10)
-        except TimeoutError:
-            availabilities.append(False)
-        else:
-            availabilities.append(True)
-    return availabilities
-
-
-def _extract_available_urls(urls: list[str], availabilities: list[bool]) -> list[str]:
-    available_urls = []
-    for url, flag in zip(urls, availabilities):
-        if flag:
-            available_urls.append(url)
-    return available_urls
+def _check_url_availability(url: str) -> bool:
+    try:
+        _ = urlopen(url, timeout=10)
+        return True
+    except (URLError, TimeoutError):
+        return False
 
 
-def _is_genome_listed_in_UCSC(genome: str, ucsc_url: str) -> None:
+def get_first_available_url(urls: list[str]) -> str | None:
+    return next((url for url in urls if _check_url_availability(url)), None)
+
+
+def is_genome_listed_in_UCSC(genome: str, ucsc_url: str) -> bool:
     url = f"{ucsc_url}/cgi-bin/das/{genome}/dna?segment=1:1,10"
-    response = urlopen(url, timeout=10)
-    content = response.read()
-    response.close()
-    if not content:
-        raise AttributeError(
-            f"{genome} is not listed in UCSC genome browser. Available genomes are listed in {ucsc_url}/cgi-bin/das/dsn"
-        )
+    try:
+        response = urlopen(url, timeout=10)
+        return bool(response.read())
+    except (URLError, TimeoutError):
+        return False
 
 
-def validate_genome_and_fetch_urls(GENOME: str) -> dict[str, str]:
-    # Check UCSC Server is available
-    URLS_UCSC = [
-        "https://genome.ucsc.edu/",
-        "https://genome-asia.ucsc.edu/",
-        "https://genome-euro.ucsc.edu/",
+def validate_genome_and_fetch_urls(genome: str) -> dict[str, str]:
+    ucsc_blat_servers = [
+        "https://genome.ucsc.edu/cgi-bin/hgBlat",
+        "https://genome-asia.ucsc.edu/cgi-bin/hgBlat",
+        "https://genome-euro.ucsc.edu/cgi-bin/hgBlat",
     ]
-    url_availabilities = _check_url_availabilities(URLS_UCSC)
-    if not any(url_availabilities):
-        raise URLError("All servers of UCSC Genome Browsers are currently down. Please wait for a while and try again.")
-    URL_UCSC_AVAILABLE = _extract_available_urls(URLS_UCSC, url_availabilities)[0]
-    # Check UCSC Download Server is available
-    URLS_GOLDENPATH = [
+    ucsc_das_servers = [
+        "https://genome.ucsc.edu/cgi-bin/das/dsn/",
+        "https://genome-asia.ucsc.edu/cgi-bin/das/dsn/",
+        "https://genome-euro.ucsc.edu/cgi-bin/das/dsn",
+    ]
+    goldenpath_servers = [
         "https://hgdownload.cse.ucsc.edu/goldenPath",
         "http://hgdownload-euro.soe.ucsc.edu/goldenPath",
     ]
-    url_availabilities = _check_url_availabilities(URLS_UCSC)
-    if not any(url_availabilities):
-        raise URLError("All servers of UCSC GoldenPath are currently down. Please wait for a while and try again.")
-    URL_GOLDENPATH_AVAILABLE = _extract_available_urls(URLS_GOLDENPATH, url_availabilities)[0]
-    # Check input genome is listed in UCSC
-    _is_genome_listed_in_UCSC(GENOME, URL_UCSC_AVAILABLE)
-    return {"ucsc": URL_UCSC_AVAILABLE, "goldenpath": URL_GOLDENPATH_AVAILABLE}
+    available_servers = {
+        "blat": get_first_available_url(ucsc_blat_servers),
+        "das": get_first_available_url(ucsc_das_servers),
+        "goldenpath": get_first_available_url(goldenpath_servers),
+    }
+
+    if not available_servers["blat"]:
+        raise URLError("All UCSC blat servers are currently down. Please wait for a while and try again.")
+
+    if not available_servers["goldenpath"]:
+        raise URLError("All UCSC GoldenPath servers are currently down. Please wait for a while and try again.")
+
+    if not available_servers["das"]:
+        raise URLError("All UCSC DAS servers are currently down. Please wait for a while and try again.")
+
+    if not is_genome_listed_in_UCSC(genome, available_servers["das"]):
+        raise AttributeError(f"{genome} is not listed. Available genomes are in {available_servers['das']}")
+
+    return available_servers
```

### Comparing `DAJIN2-0.2.4/src/DAJIN2/template_igvjs.html` & `DAJIN2-0.3.0/src/DAJIN2/template_igvjs.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2/templates/index.html` & `DAJIN2-0.3.0/src/DAJIN2/templates/index.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2/view.py` & `DAJIN2-0.3.0/src/DAJIN2/view.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.4/src/DAJIN2.egg-info/SOURCES.txt` & `DAJIN2-0.3.0/src/DAJIN2.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,37 +13,44 @@
 src/DAJIN2.egg-info/entry_points.txt
 src/DAJIN2.egg-info/requires.txt
 src/DAJIN2.egg-info/top_level.txt
 src/DAJIN2/core/__init__.py
 src/DAJIN2/core/core_execute.py
 src/DAJIN2/core/classification/__init__.py
 src/DAJIN2/core/classification/classify.py
-src/DAJIN2/core/classification/detect_sv.py
+src/DAJIN2/core/classification/tmp_detect_sv.py
 src/DAJIN2/core/clustering/__init__.py
 src/DAJIN2/core/clustering/clustering.py
+src/DAJIN2/core/clustering/make_kmer.py
 src/DAJIN2/core/clustering/make_score.py
 src/DAJIN2/core/clustering/merge_clusters.py
 src/DAJIN2/core/clustering/return_labels.py
 src/DAJIN2/core/consensus/__init__.py
 src/DAJIN2/core/consensus/consensus.py
 src/DAJIN2/core/consensus/extract_mutation_loci_by_labels.py
 src/DAJIN2/core/consensus/subset.py
 src/DAJIN2/core/preprocess/__init__.py
+src/DAJIN2/core/preprocess/align.py
 src/DAJIN2/core/preprocess/call_midsv.py
 src/DAJIN2/core/preprocess/check_caches.py
 src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
 src/DAJIN2/core/preprocess/extract_knockin_loci.py
 src/DAJIN2/core/preprocess/extract_mutation_loci.py
 src/DAJIN2/core/preprocess/format_inputs.py
-src/DAJIN2/core/preprocess/mappy_align.py
-src/DAJIN2/core/preprocess/replace_NtoD.py
+src/DAJIN2/core/preprocess/generate_insertion_fasta.py
+src/DAJIN2/core/preprocess/get_index_mapping.py
+src/DAJIN2/core/preprocess/tmp_extract_errors_in_knockin_loci.py.py
+src/DAJIN2/core/preprocess/tmp_extract_mutation_loci_with_indexmapping.py
+src/DAJIN2/core/preprocess/tmp_generate_truncated_fasta.py
+src/DAJIN2/core/preprocess/tmp_replace_NtoD.py
 src/DAJIN2/core/report/__init__.py
 src/DAJIN2/core/report/remove_microhomology.py
 src/DAJIN2/core/report/report_bam.py
 src/DAJIN2/core/report/report_files.py
+src/DAJIN2/core/report/report_mutation.py
 src/DAJIN2/core/report/reverse_sam.py
 src/DAJIN2/postprocess/__init__.py
 src/DAJIN2/postprocess/report.py
 src/DAJIN2/preprocess/__init__.py
 src/DAJIN2/preprocess/validate_inputs.py
 src/DAJIN2/static/css/style.css
 src/DAJIN2/templates/index.html
```

