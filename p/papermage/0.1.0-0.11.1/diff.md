# Comparing `tmp/papermage-0.1.0.tar.gz` & `tmp/papermage-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papermage-0.1.0.tar", last modified: Wed Aug  2 04:58:56 2023, max compression
+gzip compressed data, was "papermage-0.11.1.tar", last modified: Mon Aug  7 17:22:13 2023, max compression
```

## Comparing `papermage-0.1.0.tar` & `papermage-0.11.1.tar`

### file list

```diff
@@ -1,69 +1,109 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.027852 papermage-0.1.0/
--rw-r--r--   0 lucas      (502) staff       (20)    11358 2023-08-02 01:44:14.000000 papermage-0.1.0/LICENSE
--rw-r--r--   0 lucas      (502) staff       (20)     7545 2023-08-02 04:58:56.027721 papermage-0.1.0/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     6328 2023-08-02 01:44:14.000000 papermage-0.1.0/README.md
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.014024 papermage-0.1.0/examples/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/examples/__init__.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.014128 papermage-0.1.0/papermage/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/__init__.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.015619 papermage-0.1.0/papermage/parsers/
--rw-r--r--   0 lucas      (502) staff       (20)      102 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/parsers/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)      593 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/parsers/parser.py
--rw-r--r--   0 lucas      (502) staff       (20)    18967 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/parsers/pdfplumber_parser.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.016143 papermage-0.1.0/papermage/predictors/
--rw-r--r--   0 lucas      (502) staff       (20)      149 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/predictors/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1444 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/predictors/base_predictor.py
--rw-r--r--   0 lucas      (502) staff       (20)    15068 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/predictors/entity_classification_predictor.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.016455 papermage-0.1.0/papermage/rasterizers/
--rw-r--r--   0 lucas      (502) staff       (20)      105 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/rasterizers/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     2047 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/rasterizers/rasterizer.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.016703 papermage-0.1.0/papermage/trainers/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/trainers/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)    20509 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/trainers/entity_classification_predictor_trainer.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.018215 papermage-0.1.0/papermage/types/
--rw-r--r--   0 lucas      (502) staff       (20)      930 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     2544 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/annotation.py
--rw-r--r--   0 lucas      (502) staff       (20)     4542 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/box.py
--rw-r--r--   0 lucas      (502) staff       (20)     4057 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/document.py
--rw-r--r--   0 lucas      (502) staff       (20)     2880 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/entity.py
--rw-r--r--   0 lucas      (502) staff       (20)     3947 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/image.py
--rw-r--r--   0 lucas      (502) staff       (20)     3061 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/indexer.py
--rw-r--r--   0 lucas      (502) staff       (20)    15532 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/metadata.py
--rw-r--r--   0 lucas      (502) staff       (20)     5341 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/types/span.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.018399 papermage-0.1.0/papermage/visualizers/
--rw-r--r--   0 lucas      (502) staff       (20)     1810 2023-08-02 01:44:14.000000 papermage-0.1.0/papermage/visualizers/visualizer.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.014776 papermage-0.1.0/papermage.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)     7545 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     1643 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)      516 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)       43 2023-08-02 04:58:56.000000 papermage-0.1.0/papermage.egg-info/top_level.txt
--rw-r--r--   0 lucas      (502) staff       (20)     3900 2023-08-02 04:58:01.000000 papermage-0.1.0/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       21 2023-08-02 01:44:14.000000 papermage-0.1.0/requirements.txt
--rw-r--r--   0 lucas      (502) staff       (20)       38 2023-08-02 04:58:56.027896 papermage-0.1.0/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.018561 papermage-0.1.0/tests/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/__init__.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.018784 papermage-0.1.0/tests/test_parsers/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_parsers/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     8969 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_parsers/test_pdf_plumber_parser.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.019196 papermage-0.1.0/tests/test_predictors/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_predictors/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     3180 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_predictors/test_entity_classification_predictor.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.019593 papermage-0.1.0/tests/test_rasterizers/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_rasterizers/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1053 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_rasterizers/test_pdf2image_rasterizer.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.019820 papermage-0.1.0/tests/test_trainers/
--rw-r--r--   0 lucas      (502) staff       (20)     7861 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_trainers/test_entity_classification_predictor_trainer.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.027033 papermage-0.1.0/tests/test_types/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)     1438 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_annotation.py
--rw-r--r--   0 lucas      (502) staff       (20)     4926 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_box.py
--rw-r--r--   0 lucas      (502) staff       (20)     2685 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_document.py
--rw-r--r--   0 lucas      (502) staff       (20)     3222 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_entity.py
--rw-r--r--   0 lucas      (502) staff       (20)     2668 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_image.py
--rw-r--r--   0 lucas      (502) staff       (20)     1950 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_indexer.py
--rw-r--r--   0 lucas      (502) staff       (20)     1851 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_metadata.py
--rw-r--r--   0 lucas      (502) staff       (20)     4133 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_types/test_span.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-02 04:58:56.027472 papermage-0.1.0/tests/test_visualizers/
--rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_visualizers/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)      927 2023-08-02 01:44:14.000000 papermage-0.1.0/tests/test_visualizers/test_visualizer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.371209 papermage-0.11.1/
+-rw-r--r--   0 lucas      (502) staff       (20)    11358 2023-08-02 01:44:14.000000 papermage-0.11.1/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)     7590 2023-08-07 17:22:13.371063 papermage-0.11.1/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     6339 2023-08-04 22:55:13.000000 papermage-0.11.1/README.md
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.354168 papermage-0.11.1/examples/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.11.1/examples/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.354661 papermage-0.11.1/papermage/
+-rw-r--r--   0 lucas      (502) staff       (20)       93 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.357567 papermage-0.11.1/papermage/magelib/
+-rw-r--r--   0 lucas      (502) staff       (20)     1808 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/magelib/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3393 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/magelib/annotation.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5054 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/magelib/box.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7010 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/magelib/document.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3453 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/magelib/entity.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3932 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/magelib/image.py
+-rw-r--r--   0 lucas      (502) staff       (20)     6299 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/magelib/indexer.py
+-rw-r--r--   0 lucas      (502) staff       (20)    15532 2023-08-04 22:55:13.000000 papermage-0.11.1/papermage/magelib/metadata.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5676 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/magelib/span.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.358488 papermage-0.11.1/papermage/parsers/
+-rw-r--r--   0 lucas      (502) staff       (20)      102 2023-08-02 01:44:14.000000 papermage-0.11.1/papermage/parsers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    14885 2023-08-07 06:40:08.000000 papermage-0.11.1/papermage/parsers/grobid_parser.py
+-rw-r--r--   0 lucas      (502) staff       (20)      595 2023-08-05 17:10:16.000000 papermage-0.11.1/papermage/parsers/parser.py
+-rw-r--r--   0 lucas      (502) staff       (20)    18459 2023-08-06 21:31:13.000000 papermage-0.11.1/papermage/parsers/pdfplumber_parser.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.359142 papermage-0.11.1/papermage/predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)      847 2023-08-06 21:31:11.000000 papermage-0.11.1/papermage/predictors/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.359552 papermage-0.11.1/papermage/predictors/api_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-04 22:55:13.000000 papermage-0.11.1/papermage/predictors/api_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3889 2023-08-07 04:50:04.000000 papermage-0.11.1/papermage/predictors/api_predictors/span_qa_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1452 2023-08-07 04:50:04.000000 papermage-0.11.1/papermage/predictors/base_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.360845 papermage-0.11.1/papermage/predictors/hf_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)       58 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/predictors/hf_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    16941 2023-08-07 04:50:04.000000 papermage-0.11.1/papermage/predictors/hf_predictors/bio_tagger_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8928 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/predictors/hf_predictors/vila_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1701 2023-08-07 04:50:04.000000 papermage-0.11.1/papermage/predictors/hf_predictors/whitespace_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.361088 papermage-0.11.1/papermage/predictors/lp_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-04 22:55:13.000000 papermage-0.11.1/papermage/predictors/lp_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3516 2023-08-07 04:50:04.000000 papermage-0.11.1/papermage/predictors/lp_predictors/block_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.361362 papermage-0.11.1/papermage/predictors/sklearn_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-06 21:31:11.000000 papermage-0.11.1/papermage/predictors/sklearn_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    22808 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/predictors/sklearn_predictors/word_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.361677 papermage-0.11.1/papermage/predictors/spacy_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-06 21:31:11.000000 papermage-0.11.1/papermage/predictors/spacy_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4871 2023-08-07 10:29:00.000000 papermage-0.11.1/papermage/predictors/spacy_predictors/sentence_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-06 21:31:13.000000 papermage-0.11.1/papermage/py.typed
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.362240 papermage-0.11.1/papermage/rasterizers/
+-rw-r--r--   0 lucas      (502) staff       (20)      105 2023-08-02 01:44:14.000000 papermage-0.11.1/papermage/rasterizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2049 2023-08-04 22:55:13.000000 papermage-0.11.1/papermage/rasterizers/rasterizer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.362875 papermage-0.11.1/papermage/recipes/
+-rw-r--r--   0 lucas      (502) staff       (20)       84 2023-08-04 22:55:13.000000 papermage-0.11.1/papermage/recipes/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     6127 2023-08-07 11:11:56.000000 papermage-0.11.1/papermage/recipes/core_recipe.py
+-rw-r--r--   0 lucas      (502) staff       (20)      314 2023-08-04 22:55:13.000000 papermage-0.11.1/papermage/recipes/recipe.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.363128 papermage-0.11.1/papermage/trainers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.11.1/papermage/trainers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    20816 2023-08-06 21:31:13.000000 papermage-0.11.1/papermage/trainers/bio_tagger_predictor_trainer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.363923 papermage-0.11.1/papermage/utils/
+-rw-r--r--   0 lucas      (502) staff       (20)      171 2023-08-07 07:22:25.000000 papermage-0.11.1/papermage/utils/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1961 2023-08-07 10:06:17.000000 papermage-0.11.1/papermage/utils/annotate.py
+-rw-r--r--   0 lucas      (502) staff       (20)      307 2023-08-07 06:00:30.000000 papermage-0.11.1/papermage/utils/text.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1025 2023-08-06 21:31:13.000000 papermage-0.11.1/papermage/utils/version.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.364196 papermage-0.11.1/papermage/visualizers/
+-rw-r--r--   0 lucas      (502) staff       (20)       83 2023-08-07 11:11:56.000000 papermage-0.11.1/papermage/visualizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1812 2023-08-04 22:55:13.000000 papermage-0.11.1/papermage/visualizers/visualizer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.355406 papermage-0.11.1/papermage.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     7590 2023-08-07 17:22:13.000000 papermage-0.11.1/papermage.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     2959 2023-08-07 17:22:13.000000 papermage-0.11.1/papermage.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2023-08-07 17:22:13.000000 papermage-0.11.1/papermage.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      589 2023-08-07 17:22:13.000000 papermage-0.11.1/papermage.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       43 2023-08-07 17:22:13.000000 papermage-0.11.1/papermage.egg-info/top_level.txt
+-rw-r--r--   0 lucas      (502) staff       (20)     4033 2023-08-07 07:22:25.000000 papermage-0.11.1/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       21 2023-08-02 01:44:14.000000 papermage-0.11.1/requirements.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.364681 papermage-0.11.1/scripts/
+-rw-r--r--   0 lucas      (502) staff       (20)     5076 2023-08-07 06:40:08.000000 papermage-0.11.1/scripts/evaluation.py
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2023-08-07 17:22:13.371249 papermage-0.11.1/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.364942 papermage-0.11.1/tests/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.11.1/tests/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.366598 papermage-0.11.1/tests/test_magelib/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_magelib/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1440 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_magelib/test_annotation.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4929 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_magelib/test_box.py
+-rw-r--r--   0 lucas      (502) staff       (20)    10590 2023-08-07 06:40:08.000000 papermage-0.11.1/tests/test_magelib/test_document.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3206 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_magelib/test_entity.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2535 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_magelib/test_image.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4376 2023-08-05 20:44:51.000000 papermage-0.11.1/tests/test_magelib/test_indexer.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1853 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_magelib/test_metadata.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4137 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_magelib/test_span.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.366836 papermage-0.11.1/tests/test_parsers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.11.1/tests/test_parsers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8971 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_parsers/test_pdf_plumber_parser.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.368803 papermage-0.11.1/tests/test_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.11.1/tests/test_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2859 2023-08-07 06:40:08.000000 papermage-0.11.1/tests/test_predictors/test_entity_classification_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1771 2023-08-07 04:50:04.000000 papermage-0.11.1/tests/test_predictors/test_lp_predictors.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3314 2023-08-07 06:41:31.000000 papermage-0.11.1/tests/test_predictors/test_sentence_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3898 2023-08-07 06:40:08.000000 papermage-0.11.1/tests/test_predictors/test_span_qa_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2659 2023-08-07 06:40:08.000000 papermage-0.11.1/tests/test_predictors/test_vila_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2222 2023-08-07 06:40:08.000000 papermage-0.11.1/tests/test_predictors/test_whitespace_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4975 2023-08-06 21:31:11.000000 papermage-0.11.1/tests/test_predictors/test_word_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.369171 papermage-0.11.1/tests/test_rasterizers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.11.1/tests/test_rasterizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1055 2023-08-07 06:40:08.000000 papermage-0.11.1/tests/test_rasterizers/test_pdf2image_rasterizer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.370073 papermage-0.11.1/tests/test_recipes/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_recipes/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)   243222 2023-08-04 22:55:13.000000 papermage-0.11.1/tests/test_recipes/core_recipe_fixtures.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1580 2023-08-07 07:22:25.000000 papermage-0.11.1/tests/test_recipes/test_core_recipe.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.370347 papermage-0.11.1/tests/test_trainers/
+-rw-r--r--   0 lucas      (502) staff       (20)     7658 2023-08-07 06:40:08.000000 papermage-0.11.1/tests/test_trainers/test_entity_classification_predictor_trainer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-08-07 17:22:13.370757 papermage-0.11.1/tests/test_visualizers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-08-02 01:44:14.000000 papermage-0.11.1/tests/test_visualizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      890 2023-08-05 17:10:20.000000 papermage-0.11.1/tests/test_visualizers/test_visualizer.py
```

### Comparing `papermage-0.1.0/LICENSE` & `papermage-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `papermage-0.1.0/PKG-INFO` & `papermage-0.11.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: papermage
-Version: 0.1.0
+Version: 0.11.1
 Summary: Papermage. Casting magic over scientific PDFs.
 Author-email: Kyle Lo <kylel@allenai.org>, Luca Soldaini <luca@soldaini.net>, Shannon Zejiang Shen <zejiangshen@gmail.com>, Ben Newman <blnewman@stanford.edu>, Russell Authur <russell.authur@gmail.com>, Stefan Candra <stefanc@allenai.org>, Yoganand Chandrasekhar <yogic@allenai.org>, Regan Huff <reganh@allenai.org>, Amanpreet Singh <amans@allenai.org>, Chris Wilhelm <chrisw@allenai.org>, Angele Zamarron <angelez@allenai.org>
 Maintainer-email: Kyle Lo <kylel@allenai.org>, Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://www.github.com/allenai/papermage
 Project-URL: Repository, https://www.github.com/allenai/papermage
 Project-URL: Bug Tracker, https://www.github.com/allenai/papermage/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: visualizers
 Provides-Extra: predictors
+Provides-Extra: production
 License-File: LICENSE
 
 # papermage
 
 ### Setup
 
 ```python
-conda create -n papermage python=3.11
+conda create -n papermage python=3.9
 conda activate papermage
-pip install -e '.[dev,predictors]'
+pip install -e '.[dev,predictors,visualizers]'
 ```
 
 If you're on MacOSX, you'll also want to run:
 ```
 conda install poppler
 ```
```

### Comparing `papermage-0.1.0/README.md` & `papermage-0.11.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # papermage
 
 ### Setup
 
 ```python
-conda create -n papermage python=3.11
+conda create -n papermage python=3.9
 conda activate papermage
-pip install -e '.[dev,predictors]'
+pip install -e '.[dev,predictors,visualizers]'
 ```
 
 If you're on MacOSX, you'll also want to run:
 ```
 conda install poppler
 ```
```

### Comparing `papermage-0.1.0/papermage/parsers/parser.py` & `papermage-0.11.1/papermage/parsers/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @kylel, shannons, bnewm0609
 
 """
 
 from abc import abstractmethod
 from typing import Protocol
 
-from papermage.types import Document
+from papermage.magelib import Document
 
 
 class Parser(Protocol):
     @abstractmethod
     def parse(self, input_pdf_path: str, **kwargs) -> Document:
         """Given an input PDF return a Document with at least symbols
```

### Comparing `papermage-0.1.0/papermage/parsers/pdfplumber_parser.py` & `papermage-0.11.1/papermage/parsers/pdfplumber_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 try:
     # pdfplumber >= 0.8.0
     import pdfplumber.utils.text as ppu
 except:
     # pdfplumber <= 0.7.6
     import pdfplumber.utils as ppu
 
-from papermage.parsers.parser import Parser
-from papermage.types import (
+from papermage.magelib import (
     Box,
     Document,
     EntitiesFieldName,
     Entity,
     Metadata,
     PagesFieldName,
     RowsFieldName,
     Span,
     SymbolsFieldName,
     TokensFieldName,
 )
+from papermage.parsers.parser import Parser
+from papermage.utils.text import maybe_normalize
 
 _TOL = Union[int, float]
 
 
 class WordExtractorWithFontInfo(ppu.WordExtractor):
     """Override WordExtractor methods to append additional char-level info."""
 
@@ -206,15 +207,15 @@
                     fine_tokens=[f["text"] for f in fine_tokens],
                 )
                 assert len(word_ids_of_fine_tokens) == len(fine_tokens)
                 # 4) normalize / clean tokens & boxes
                 fine_tokens = [
                     {
                         "text": token["text"],
-                        "fontname": token["fontname"],
+                        "fontname": maybe_normalize(token["fontname"]),
                         "size": token["size"],
                         "bbox": Box.from_xy_coordinates(
                             x1=float(token["x0"]),
                             y1=float(token["top"]),
                             x2=float(token["x1"]),
                             y2=float(token["bottom"]),
                             page_width=float(page.width),
@@ -245,23 +246,14 @@
                 token_dicts=all_tokens,
                 word_ids=all_word_ids,
                 row_ids=all_row_ids,
                 page_ids=all_page_ids,
                 dims=all_page_dims,
             )
             doc = Document.from_json(doc_json)
-
-            # now set ids for all of the attributes that were added
-            # NOTE: to set an `id` for an entity, it needs to have a `doc` attribute. These do not have to
-            # explicitly be set here because `Document.from_json` will set the `doc` attribute.
-            # All that's left is to set the `id` attribute.
-            added_entities = [TokensFieldName, RowsFieldName, PagesFieldName]
-            for entity_name in added_entities:
-                for entity_i, entity in enumerate(getattr(doc, entity_name)):
-                    entity.id = entity_i
             return doc
 
     def _convert_nested_text_to_doc_json(
         self,
         token_dicts: List[dict],
         word_ids: List[int],
         row_ids: List[int],
```

### Comparing `papermage-0.1.0/papermage/predictors/base_predictor.py` & `papermage-0.11.1/papermage/predictors/base_predictor.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @shannons, @kylel
 
 """
 
 from abc import abstractmethod
 from typing import Any, Dict, List, Union
 
-from papermage.types import Annotation, Document
+from papermage.magelib import Annotation, Document
 
 
 class BasePredictor:
     @property
     @abstractmethod
     def REQUIRED_BACKENDS(self):
         raise NotImplementedError
@@ -40,9 +40,9 @@
         """For all the predictors, the input is a document object, and
         the output is a list of annotations.
         """
         self._doc_field_checker(doc)
         return self._predict(doc=doc)
 
     @abstractmethod
-    def _predict(doc: Document) -> List[Annotation]:
+    def _predict(self, doc: Document) -> List[Annotation]:
         raise NotImplementedError
```

### Comparing `papermage-0.1.0/papermage/predictors/entity_classification_predictor.py` & `papermage-0.11.1/papermage/predictors/hf_predictors/bio_tagger_predictor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 
 @kylel, benjaminn
 
 """
 
 from collections import defaultdict
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 import transformers
 from smashed.interfaces.simple import (
     FixedBatchSizeMapper,
     FromTokenizerListCollatorMapper,
     Python2TorchMapper,
     TokenizerMapper,
     UnpackingMapper,
 )
 
+from papermage.magelib import Annotation, Box, Document, Entity, Metadata, Span
 from papermage.predictors.base_predictor import BasePredictor
-from papermage.types import Annotation, Document, Entity, Metadata, Span
 
 
-class EntityClassificationBatch:
+class BIOBatch:
     def __init__(
         self,
         input_ids: List[List[int]],
         attention_mask: List[List[int]],
         entity_ids: List[List[Optional[int]]],
         context_id: List[int],
     ):
@@ -43,23 +43,23 @@
 
         self.input_ids = input_ids
         self.attention_mask = attention_mask
         self.entity_ids = entity_ids
         self.context_id = context_id
 
 
-class EntityClassificationPrediction:
+class BIOPrediction:
     def __init__(self, context_id: int, entity_id: int, label: str, score: float):
         self.context_id = context_id
         self.entity_id = entity_id
         self.label = label
         self.score = score
 
 
-class EntityClassificationPredictor(BasePredictor):
+class HFBIOTaggerPredictor(BasePredictor):
     """
     This is a generic wrapper around Huggingface Token Classification models.
 
     First, we need an `entity_name` which defines the Document field that we will
     receive a prediction. For example, if `entity_name` is 'tokens', then we expect
     to classify every Document.token.  But technically, `entity_name` could be anything,
     such as `words` or `rows` or any Entity.
@@ -99,15 +99,17 @@
     ):
         self.model = model
         self.config = config
         self.tokenizer = tokenizer
         self.entity_name = entity_name
         self.context_name = context_name
         self.batch_size = batch_size
-        self.device = device
+
+        # move model to device
+        self.model.to(device)
 
         # For some reason, the roberta max_position_embeddings is larger than the actual model context window
         # so use the model_max_length instead. (We can't replace model_max_length with max_position_embeddings
         # in general, because model_max_legnth will be set to a very large number if the model length is not
         # explicitly included in the tokenizer (like in the case of alleani/scibert). As a compromise, check
         # if the model_max_legnth is big, and it's too big, then use the max_position_embeddings as the context
         # window size.
@@ -151,18 +153,30 @@
             pad_to_length=None,  # keeping this `None` is best because of dynamic padding
             fields_pad_ids={
                 self._HF_RESERVED_WORD_IDS: self._HF_RESERVED_WORD_PAD_VALUE,
                 "labels": -100,
             },
         )
         # this casts python Dict[List] into tensors.  if using GPU, would do `device='gpu'`
-        self.python_to_torch_mapper = Python2TorchMapper(device=device)
+        self.python_to_torch_mapper = Python2TorchMapper(device=self.model.device)
         # combining everything
         self.preprocess_mapper = self.tokenizer_mapper >> self.unpacking_mapper >> self.batch_size_mapper
 
+    @property
+    def device(self) -> torch.device:
+        device = self.model.device
+        device = torch.device(device) if isinstance(device, str) else device
+        return device
+
+    @device.setter
+    def device(self, device: Union[torch.device, str]) -> None:
+        device = torch.device(device) if isinstance(device, str) else device
+        self.model.to(device)
+        self.python_to_torch_mapper.device = device
+
     @classmethod
     def from_pretrained(
         cls,
         model_name_or_path: str,
         entity_name: str,
         context_name: str,
         batch_size: Optional[int] = 2,
@@ -200,15 +214,15 @@
         )
         return predictor
 
     @property
     def REQUIRED_DOCUMENT_FIELDS(self) -> List[str]:
         return [self.context_name, self.entity_name]
 
-    def preprocess(self, doc: Document, context_name: str) -> List[EntityClassificationBatch]:
+    def preprocess(self, doc: Document, context_name: str) -> List[BIOBatch]:
         """Processes document into whatever makes sense for the Huggingface model"""
         # (1) get it into a dictionary format that Smashed expects
 
         dataset = [
             {
                 self._INPUT_FIELD_NAME: [entity.text for entity in getattr(context, self.entity_name)],
                 self._CONTEXT_ID: i,
@@ -219,94 +233,124 @@
         # (2) apply Smashed
         batch_dicts = self.preprocess_mapper.map(dataset=dataset)
 
         # (3) convert dicts to objects
         return [
             # slightly annoying, but the names `input_ids`, `attention_mask` and `word_ids` are
             # reserved and produced after tokenization, which is why hard-coded here.
-            EntityClassificationBatch(
+            BIOBatch(
                 input_ids=batch_dict[self._HF_RESERVED_INPUT_IDS],
                 attention_mask=batch_dict[self._HF_RESERVED_ATTN_MASK],
                 entity_ids=batch_dict[self._HF_RESERVED_WORD_IDS],
                 context_id=batch_dict[self._CONTEXT_ID],
             )
             for batch_dict in batch_dicts
         ]
 
-    def postprocess(
-        self, doc: Document, context_name: str, preds: List[EntityClassificationPrediction]
-    ) -> List[Annotation]:
+    def combine_annotations(self, annotations: List[Entity]) -> Annotation:
+        # import pytest; pytest.set_trace()
+        label = annotations[0].metadata.label[2:]  # remove the B-
+        scores = [annotation.metadata.score for annotation in annotations]
+        span = Span.create_enclosing_span([span for annotation in annotations for span in annotation.spans])
+        smaller_boxes = [box for annotation in annotations for box in annotation.boxes]
+        box = [Box.create_enclosing_box(smaller_boxes)] if smaller_boxes else []
+        return Entity(
+            spans=[span],
+            boxes=box,
+            metadata=Metadata(label=label, score=np.mean(scores)),
+        )
+
+    def postprocess(self, doc: Document, context_name: str, preds: List[BIOPrediction]) -> List[Annotation]:
         """This function handles a bunch of nonsense that happens with Huggingface models &
         how we processed the data.  Namely:
 
         Because Huggingface might drop tokens during the course of tokenization
         we need to organize our predictions into a Lookup <dict> and cross-reference
         with the original input SpanGroups to make sure they all got classified.
         """
         # (1) organize predictions into a Lookup at the (Context, SpanGroup) level.
-        context_id_to_entity_id_to_pred: Dict[int, Dict[int, EntityClassificationPrediction]] = defaultdict(dict)
+        context_id_to_entity_id_to_pred: Dict[int, Dict[int, BIOPrediction]] = defaultdict(dict)
         for prediction in preds:
             context_id_to_entity_id_to_pred[prediction.context_id][prediction.entity_id] = prediction
 
         # (2) iterate through original data to check against that Lookup
         annotations: List[Annotation] = []
+        field_annotations: List[Entity] = []
         for i, context in enumerate(getattr(doc, context_name)):
             for j, entity in enumerate(getattr(context, self.entity_name)):
-                pred: Optional[EntityClassificationPrediction] = context_id_to_entity_id_to_pred[i].get(j, None)
+                pred: Optional[BIOPrediction] = context_id_to_entity_id_to_pred[i].get(j, None)
                 # TODO: double-check whether this deepcopy is needed...
                 new_metadata = Metadata.from_json(entity.metadata.to_json())
                 if pred is not None:
                     new_metadata.label = pred.label
                     new_metadata.score = pred.score
                 else:
                     new_metadata.label = None
                     new_metadata.score = None
                 new_entity = Entity(
                     spans=entity.spans,
                     boxes=entity.boxes,
                     metadata=new_metadata,
                 )
-                annotations.append(new_entity)
+
+                if new_entity.metadata.label.startswith("B"):
+                    # end the last annotation
+                    if field_annotations:
+                        annotations.append(self.combine_annotations(field_annotations))
+                    field_annotations = [new_entity]
+                elif new_entity.metadata.label == "O":
+                    # end the last annotation
+                    if field_annotations:
+                        annotations.append(self.combine_annotations(field_annotations))
+                    field_annotations = []
+                else:
+                    # Either "I", so we're in the same field or "None", so we're in the same word-piece
+                    field_annotations.append(new_entity)
+                # annotations.append(new_entity)
+        if field_annotations:
+            annotations.append(self.combine_annotations(field_annotations))
+
         return annotations
 
     def _predict(self, doc: Document) -> List[Annotation]:
         # (1) Make batches
-        batches: List[EntityClassificationBatch] = self.preprocess(doc=doc, context_name=self.context_name)
+        batches: List[BIOBatch] = self.preprocess(doc=doc, context_name=self.context_name)
 
         # (2) Predict each batch.
-        preds: List[EntityClassificationPrediction] = []
+        preds: List[BIOPrediction] = []
         for batch in batches:
             for pred in self._predict_batch(batch=batch):
                 preds.append(pred)
 
         # (3) Postprocess into proper Annotations
         annotations = self.postprocess(doc=doc, context_name=self.context_name, preds=preds)
         return annotations
 
     def _predict_batch(
         self,
-        batch: EntityClassificationBatch,
-        device: str = "cpu",
-    ) -> List[EntityClassificationPrediction]:
+        batch: BIOBatch,
+        device: Union[None, str, torch.device] = None
+    ) -> List[BIOPrediction]:
         #
         #   preprocessing!!  (padding & tensorification)
         #
         pytorch_batch = self.python_to_torch_mapper.transform(
             data=self.list_collator_mapper.transform(
                 data={
                     self._HF_RESERVED_INPUT_IDS: batch.input_ids,
                     self._HF_RESERVED_ATTN_MASK: batch.attention_mask,
                 }
             )
         )
+        # change device if needed
+        if device:
+            pytorch_batch = {k: v.to(device) for k, v in pytorch_batch.items()}
         #
         #   inference!! (preferably on gpu)
         #
-        # TODO: add something here for gpu migration
-        pytorch_batch = {k: v.to(device) for k, v in pytorch_batch.items()}
         self.model.eval()
         with torch.no_grad():
             pytorch_output = self.model(**pytorch_batch)
         scores_tensor = torch.softmax(pytorch_output.logits, dim=2)
         token_scoresss = [
             [token_scores for token_scores, yn in zip(token_scoress, yns) if yn == 1]
             for token_scoress, yns in zip(scores_tensor.tolist(), batch.attention_mask)
@@ -321,15 +365,15 @@
             for word_id, token_scores, is_valid_pred in zip(
                 word_ids, token_scoress, self._token_pooling_strategy_mask(word_ids=word_ids)
             ):
                 if word_id is None or is_valid_pred is False:
                     continue
                 else:
                     label_id = np.argmax(token_scores)
-                    pred = EntityClassificationPrediction(
+                    pred = BIOPrediction(
                         context_id=context_id,
                         entity_id=word_id,
                         label=self.config.id2label[label_id],
                         score=token_scores[label_id],
                     )
                     preds.append(pred)
         return preds
```

### Comparing `papermage-0.1.0/papermage/rasterizers/rasterizer.py` & `papermage-0.11.1/papermage/rasterizers/rasterizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 @shannons, @kylel
 
 """
 
 from typing import Iterable, List, Protocol
 
-from papermage.types import Document, Image, PagesFieldName
+from papermage.magelib import Document, Image, PagesFieldName
 
 try:
     import pdf2image
 except ImportError:
     pass
```

### Comparing `papermage-0.1.0/papermage/trainers/entity_classification_predictor_trainer.py` & `papermage-0.11.1/papermage/trainers/bio_tagger_predictor_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 import transformers
 from omegaconf import DictConfig
 from pytorch_lightning.callbacks import LearningRateMonitor, ModelCheckpoint
 from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-from papermage.predictors import EntityClassificationPredictor
-from papermage.types import Box, Document, Entity, Span
+from papermage.magelib import Box, Document, Entity, Span
+from papermage.predictors import HFBIOTaggerPredictor
 
 
-class EntityClassificationPredictorWrapper(pl.LightningModule):
-    def __init__(self, predictor: EntityClassificationPredictor):
+class HFBioTaggerPredictorWrapper(pl.LightningModule):
+    def __init__(self, predictor: HFBIOTaggerPredictor):
         super().__init__()
         self.predictor = predictor
         self.learning_rate = None  # this will be set by the trainer
         self.warmup_steps = None  # this will be set by the trainer
         self.num_training_steps = None  # this will be set by the trainer
 
     def training_step(self, batch, batch_idx) -> Optional[STEP_OUTPUT]:
@@ -53,14 +53,26 @@
         )
         return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
     def preprocess(self, doc: Document, context_name: str = "pages") -> List:
         # is this the default context we should use?
         return self.predictor.preprocess(doc, context_name)
 
+    def on_train_start(self) -> None:
+        self.predictor.device = self.device
+        return super().on_train_start()
+
+    def on_validation_start(self) -> None:
+        self.predictor.device = self.device
+        return super().on_validation_start()
+
+    def on_test_start(self) -> None:
+        self.predictor.device = self.device
+        return super().on_test_start()
+
     def __getattr__(self, name):
         """Allow access to the predictor's attributes if the wrapper doesn't have them."""
         if name not in self.__dict__:
             return getattr(self.predictor, name)
 
 
 class HFCheckpoint(pl.Callback):
@@ -80,23 +92,23 @@
         pl_module.predictor.tokenizer.save_pretrained(self.save_dir)
 
         # don't want to save the state twice bc it might be big. But not saving it might cause issues if we want
         # to load the model later, that's a TODO for now.
         # del checkpoint["state_dict"]
 
 
-class EntityClassificationPredictorTrainer:
+class HFBIOTaggerPredictorTrainer:
     CACHE_PATH = Path(os.environ.get("PAPERMAGE_CACHE_DIR", Path.home() / ".cache/papermage"))
 
-    def __init__(self, predictor: EntityClassificationPredictor, config: DictConfig):
+    def __init__(self, predictor: HFBIOTaggerPredictor, config: DictConfig):
         if not self.CACHE_PATH.exists():
             self.CACHE_PATH.mkdir(parents=True)
 
         transformers.set_seed(config.seed)
-        self.predictor = EntityClassificationPredictorWrapper(predictor)
+        self.predictor = HFBioTaggerPredictorWrapper(predictor)
         self.predictor.learning_rate = config.learning_rate
         self.predictor.warmup_steps = config.warmup_steps
 
         self.config = config
         if self.config.accelerator == "auto":
             self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         else:
@@ -389,15 +401,15 @@
         print(clf_report_token)
         print("Results saved to:", (self.config.default_root_dir / "results"))
 
         # return all_gold_labels, all_pred_labels, all_extracted_text
 
 
 @springs.dataclass
-class EntityClassificationTrainConfig:
+class HFBIOTaggerPredictorTrainConfig:
     """Stores the default training args"""
 
     data_path: Path  # Path to the data to train on. Should be a jsonl file where each row is a doc.
     label_field: str  # The field in the document to use as the labels for the tokens.
     # label_fields: List[str]  # The fields in the document to use as labels for the tokens.
     entity_name: str = "tokens"  # The field in the document to use as the unit of prediction.
     context_name: str = "pages"  # The field in the document to use as the input example to the model.
@@ -423,16 +435,16 @@
     log_every_n_steps: int = 1
     val_check_interval: Union[float, int] = 1.0
     # Args for development/testing
     fast_dev_run: bool = False
     overfit_batches: bool = False
 
 
-@springs.cli(EntityClassificationTrainConfig)
-def main(config: EntityClassificationTrainConfig):
+@springs.cli(HFBIOTaggerPredictorTrainConfig)
+def main(config: HFBIOTaggerPredictorTrainConfig):
     """Launch a training run.
 
     For now, the simplest way to do this is to just pass the data. We can abstract this later and add some way to
     configure the training run.
     """
 
     # parse out the label fields:
@@ -445,16 +457,16 @@
     kwargs = {"num_labels": len(id2label), "id2label": id2label, "label2id": label2id}
 
     if "roberta" in config.model_name_or_path:
         kwargs["add_prefix_space"] = True
         # kwargs["max_position_embeddings"] = 512  # This is set to 514 for some reason...
 
     # Initialize the trainer
-    trainer = EntityClassificationPredictorTrainer(
-        predictor=EntityClassificationPredictor.from_pretrained(
+    trainer = HFBIOTaggerPredictorTrainer(
+        predictor=HFBIOTaggerPredictor.from_pretrained(
             model_name_or_path=config.model_name_or_path,
             entity_name=config.entity_name,
             context_name=config.context_name,
             **kwargs,
         ),
         config=config,
     )
```

### Comparing `papermage-0.1.0/papermage/types/annotation.py` & `papermage-0.11.1/papermage/magelib/annotation.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 in a document; representing it as an Annotation data type would allow you to access the
 Document object directly from within the Entity itself.
 
 @kylel
 
 """
 
-import logging
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 if TYPE_CHECKING:
-    # from papermage.types.document import Document
-    pass
+    from .document import Document
 
 
 class Annotation:
     """Represent a "unit" (e.g. highlighted span, drawn boxes) layered on a Document."""
 
     @abstractmethod
     def __init__(self) -> None:
@@ -62,15 +60,36 @@
 
     @classmethod
     @abstractmethod
     def from_json(cls, annotation_json: Union[Dict, List]) -> "Annotation":
         pass
 
     def __getattr__(self, field: str) -> List["Annotation"]:
-        """This method allows you to access overlapping Annotations within the Document"""
+        """This Overloading is convenient syntax since the `entity.layer` operation is intuitive for folks."""
+        try:
+            return self.find_by_span(field=field)
+        except ValueError:
+            # maybe users just want some attribute of the Annotation object
+            return self.__getattribute__(field)
+
+    def find_by_span(self, field: str) -> List["Annotation"]:
+        """This method allows you to access overlapping Annotations
+        within the Document based on Span"""
         if self.doc is None:
             raise ValueError("This annotation is not attached to a document")
 
         if field in self.doc.fields:
-            return self.doc.find_span_overlap_entities(self, field)
+            return self.doc.find_by_span(self, field)
+        else:
+            raise ValueError(f"Field {field} not found in Document")
+
+    def find_by_box(self, field: str) -> List["Annotation"]:
+        """This method allows you to access overlapping Annotations
+        within the Document based on Box"""
 
-        return self.__getattribute__(field)
+        if self.doc is None:
+            raise ValueError("This annotation is not attached to a document")
+
+        if field in self.doc.fields:
+            return self.doc.find_by_box(self, field)
+        else:
+            raise ValueError(f"Field {field} not found in Document")
```

### Comparing `papermage-0.1.0/papermage/types/box.py` & `papermage-0.11.1/papermage/magelib/box.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,31 @@
 Rectangular region on a document.
 
 @kylel
 
 """
 
 import logging
-from typing import Dict, List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 
-from papermage.types import Span
+from .span import Span
+
+
+class _BoxSpan(Span):
+    def __init__(self, start: float, end: float):
+        self.start = start  # type: ignore
+        self.end = end  # type: ignore
 
 
 class Box:
+
+    __slots__ = ["l", "t", "w", "h", "page"]
+
     def __init__(self, l: float, t: float, w: float, h: float, page: int):
         assert w >= 0.0, "Box width cant be negative"
         assert h >= 0.0, "Box height cant be negative"
         self.l = float(l)
         self.t = float(t)
         self.w = float(w)
         self.h = float(h)
@@ -69,14 +78,25 @@
 
         return Box(l=_x1, t=_y1, w=_x2 - _x1, h=_y2 - _y1, page=page)
 
     @property
     def xy_coordinates(self) -> Tuple[float, float, float, float]:
         return self.l, self.t, self.l + self.w, self.t + self.h
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Box):
+            return False
+        return (
+            self.l == other.l
+            and self.t == other.t
+            and self.w == other.w
+            and self.h == other.h
+            and self.page == other.page
+        )
+
     def to_relative(self, page_width: float, page_height: float) -> "Box":
         """Get the relative coordinates of self based on page_width, page_height."""
         return self.__class__(
             l=float(self.l) / page_width,
             t=float(self.t) / page_height,
             w=float(self.w) / page_width,
             h=float(self.h) / page_height,
@@ -103,22 +123,22 @@
         if self.page != other.page:
             return False
 
         self_x1, self_y1, self_x2, self_y2 = self.xy_coordinates
         other_x1, other_y1, other_x2, other_y2 = other.xy_coordinates
 
         # check x-axis
-        span_x_self = Span(start=self_x1, end=self_x2)
-        span_x_other = Span(start=other_x1, end=other_x2)
+        span_x_self = _BoxSpan(start=self_x1, end=self_x2)
+        span_x_other = _BoxSpan(start=other_x1, end=other_x2)
         if not span_x_self.is_overlap(span_x_other):
             return False
 
         # check y-axis
-        span_y_self = Span(start=self_y1, end=self_y2)
-        span_y_other = Span(start=other_y1, end=other_y2)
+        span_y_self = _BoxSpan(start=self_y1, end=self_y2)
+        span_y_other = _BoxSpan(start=other_y1, end=other_y2)
         if not span_y_self.is_overlap(span_y_other):
             return False
 
         return True
 
     @classmethod
     def create_enclosing_box(cls, boxes: List["Box"]) -> "Box":
```

### Comparing `papermage-0.1.0/papermage/types/entity.py` & `papermage-0.11.1/papermage/magelib/entity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 
 An annotated "unit" on a Document.
 
 """
 
-from typing import TYPE_CHECKING, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
-from papermage.types import Annotation, Box, Image, Metadata, Span
-
-if TYPE_CHECKING:
-    from papermage.types.document import Document
+from .annotation import Annotation
+from .box import Box
+from .image import Image
+from .metadata import Metadata
+from .span import Span
 
 
 class Entity(Annotation):
     def __init__(
         self,
         spans: Optional[List[Span]] = None,
         boxes: Optional[List[Box]] = None,
@@ -25,18 +26,17 @@
         self.spans = spans if spans else []
         self.boxes = boxes if boxes else []
         self.images = images if images else []
         self.metadata = metadata if metadata else Metadata()
         super().__init__()
 
     def __repr__(self):
-        if self.doc and self.spans:
-            symbols: List[str] = [self.doc.symbols[span.start : span.end] for span in self.spans]
-            return f"Entity\tSymbols\t{symbols}"
-        return f"Entity{self.to_json()}"
+        if self.doc:
+            return f"Annotated Entity:\tSpans: {True if self.spans else False}\tBoxes: {True if self.boxes else False}\nText: {self.text}"
+        return f"Unannotated Entity: {self.to_json()}"
 
     def to_json(self) -> Dict:
         entity_dict = dict(
             spans=[span.to_json() for span in self.spans],
             boxes=[box.to_json() for box in self.boxes],
             metadata=self.metadata.to_json(),
         )
@@ -56,26 +56,41 @@
         return min([span.start for span in self.spans]) if len(self.spans) > 0 else float("-inf")
 
     @property
     def end(self) -> Union[int, float]:
         return max([span.end for span in self.spans]) if len(self.spans) > 0 else float("inf")
 
     @property
-    def symbols(self) -> List[str]:
+    def symbols_from_spans(self) -> List[str]:
         if self.doc is not None:
             return [self.doc.symbols[span.start : span.end] for span in self.spans]
         else:
             return []
 
     @property
+    def symbols_from_boxes(self) -> List[str]:
+        if self.doc is not None:
+            matched_tokens = self.doc.find_by_box(query=self, field_name="tokens")
+            return [self.doc.symbols[span.start : span.end] for t in matched_tokens for span in t.spans]
+        else:
+            return []
+
+    @property
     def text(self) -> str:
+        # return stored metadata
         maybe_text = self.metadata.get("text", None)
-        if maybe_text is None:
-            return " ".join(self.symbols)
-        return maybe_text
+        if maybe_text:
+            return maybe_text
+        # return derived from symbols
+        if self.symbols_from_spans:
+            return " ".join(self.symbols_from_spans)
+        # return derived from boxes and tokens
+        if self.symbols_from_boxes:
+            return " ".join(self.symbols_from_boxes)
+        return ""
 
     @text.setter
     def text(self, text: Union[str, None]) -> None:
         self.metadata.text = text
 
     def __iter__(self):
         """By default, iterate over the spans"""
```

### Comparing `papermage-0.1.0/papermage/types/image.py` & `papermage-0.11.1/papermage/magelib/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Monkey patch the PIL.Image methods to add base64 conversion
 
 @kylel, adapted some prior code from @shannons
 
 """
 
 import base64
-import logging
 import os
 from io import BytesIO
 
 import numpy as np
 from PIL import Image as pilimage_module
 from PIL import ImageChops as pilimagechops_module
 from PIL.Image import Image as PILImageClass
```

### Comparing `papermage-0.1.0/papermage/types/metadata.py` & `papermage-0.11.1/papermage/magelib/metadata.py`

 * *Files identical despite different names*

### Comparing `papermage-0.1.0/papermage/types/span.py` & `papermage-0.11.1/papermage/magelib/span.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 A (start, end) interval that references some string. For example, span (0, 4)
 represents the word 'This' in the string 'This is a document.'
 
 @kylel, @egork
 
 """
 
-from typing import List, Optional, Dict, Tuple, List
+from typing import List, Dict, List
 
 from collections import defaultdict
 
 
 class Span:
+    __slots__ = ['start', 'end']
+
     def __init__(self, start: int, end: int):
         self.start = start
         self.end = end
 
     def to_json(self) -> List[int]:
         """Returns whatever representation is JSON compatible"""
         return [self.start, self.end]
@@ -25,29 +27,36 @@
     def from_json(cls, span_json: List) -> "Span":
         """Recreates the object from the JSON serialization"""
         return Span(start=span_json[0], end=span_json[-1])
 
     def __repr__(self):
         return f'Span{self.to_json()}'
 
-    def __eq__(self, other):
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, Span):
+            return False
         return self.start == other.start and self.end == other.end
 
     def __lt__(self, other: 'Span'):
         """Useful for sort(). Orders according to the start index.
         If ties, then order according to the end index."""
         if self.start == other.start:
             return self.end < other.end
         return self.start < other.start
 
+    def __hash__(self) -> int:
+        return hash((self.start, self.end))
+
     def is_overlap(self, other: 'Span') -> bool:
         """Whether self overlaps with the other Span object."""
-        return self.start <= other.start < self.end or \
-               other.start <= self.start < other.end or \
-               self == other
+        return (
+            self.start <= other.start < self.end
+            or other.start <= self.start < other.end
+            or self == other
+        )
 
     @classmethod
     def create_enclosing_span(cls, spans: List['Span']) -> 'Span':
         """Create the narrowest Span that completely encloses all the input Spans."""
         if not spans:
             raise ValueError(f'`spans` should be non-empty.')
         start = spans[0].start
@@ -101,28 +110,30 @@
 
     @property
     def clusters(self) -> List[List[Span]]:
         if not self._clusters:
             self._clusters = self._cluster(spans=self.spans)
         return self._clusters
 
-    def _build_graph(self, spans: List[Span], index_distance: int) -> defaultdict(list):
+    @staticmethod
+    def _is_neighboring_spans(span1: Span, span2: Span, index_distance: int) -> bool:
+        """Whether two spans are considered neighboring"""
+        return min(
+            abs(span1.start - span2.end), abs(span1.end - span2.start)
+        ) <= index_distance
+
+    def _build_graph(self, spans: List[Span], index_distance: int) -> Dict[int, List[int]]:
         """
         Build graph, each node is the position within the input list of spans.
         Spans are considered overlapping if they are index_distance apart
         """
-        is_neighboring_spans = (
-            lambda span1, span2: min(
-                abs(span1.start - span2.end), abs(span1.end - span2.start)
-            ) <= index_distance
-        )
         graph = defaultdict(list)
         for i, span_i in enumerate(spans):
             for j in range(i + 1, len(spans)):
-                if is_neighboring_spans(span_i, spans[j]):
+                if self._is_neighboring_spans(span1=span_i, span2=spans[j], index_distance=index_distance):
                     graph[i].append(j)
                     graph[j].append(i)
         return graph
 
     def _cluster(self, spans: List[Span]) -> List[List[Span]]:
         """Cluster nodes (i.e. spans) by finding connected components"""
         if len(spans) == 0:
```

### Comparing `papermage-0.1.0/papermage/visualizers/visualizer.py` & `papermage-0.11.1/papermage/visualizers/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from typing import Dict, List, Optional, Union
 
 import layoutparser.elements as lpe
 import layoutparser.visualization as lpv
 
-from papermage.types import Entity, Image
+from papermage.magelib import Entity, Image
 
 
 def plot_entities_on_page(
     page_image: Image,
     entities: List[Entity],
     box_width: Optional[Union[List[int], int]] = None,
     box_alpha: Optional[Union[List[float], float]] = None,
```

### Comparing `papermage-0.1.0/papermage.egg-info/PKG-INFO` & `papermage-0.11.1/papermage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: papermage
-Version: 0.1.0
+Version: 0.11.1
 Summary: Papermage. Casting magic over scientific PDFs.
 Author-email: Kyle Lo <kylel@allenai.org>, Luca Soldaini <luca@soldaini.net>, Shannon Zejiang Shen <zejiangshen@gmail.com>, Ben Newman <blnewman@stanford.edu>, Russell Authur <russell.authur@gmail.com>, Stefan Candra <stefanc@allenai.org>, Yoganand Chandrasekhar <yogic@allenai.org>, Regan Huff <reganh@allenai.org>, Amanpreet Singh <amans@allenai.org>, Chris Wilhelm <chrisw@allenai.org>, Angele Zamarron <angelez@allenai.org>
 Maintainer-email: Kyle Lo <kylel@allenai.org>, Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://www.github.com/allenai/papermage
 Project-URL: Repository, https://www.github.com/allenai/papermage
 Project-URL: Bug Tracker, https://www.github.com/allenai/papermage/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: visualizers
 Provides-Extra: predictors
+Provides-Extra: production
 License-File: LICENSE
 
 # papermage
 
 ### Setup
 
 ```python
-conda create -n papermage python=3.11
+conda create -n papermage python=3.9
 conda activate papermage
-pip install -e '.[dev,predictors]'
+pip install -e '.[dev,predictors,visualizers]'
 ```
 
 If you're on MacOSX, you'll also want to run:
 ```
 conda install poppler
 ```
```

### Comparing `papermage-0.1.0/pyproject.toml` & `papermage-0.11.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [project]
 name = 'papermage'
-version = '0.1.0'
+version = '0.11.1'
 description = 'Papermage. Casting magic over scientific PDFs.'
 license = {text = 'Apache-2.0'}
 readme = 'README.md'
-requires-python = '>=3.8'
+requires-python = '>=3.8,<3.11'
 dependencies = [
         'tqdm',
         'pdf2image',
         'pdfplumber==0.7.4',
         'requests',
         'numpy>=1.23.2',
         'scipy>=1.9.0',
         'pandas<2',
         'ncls==0.0.66',
         'necessary>=0.3.2',
-        'unidecode>=1.3.4'
+        'grobid-client-python==0.0.5',
+        'charset-normalizer',
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Typing :: Typed",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
@@ -88,23 +89,24 @@
 
 [tool.setuptools.packages.find]
 where = ['.',]
 
 [tool.setuptools.package-data]
 papermage = [
     '../requirements.txt',
+    'py.typed',
 ]
 
 [build-system]
 build-backend = 'setuptools.build_meta'
 requires = [
     'setuptools >= 61.0.0',
     'pip >= 21.0.0',
     'wheel',
-    'cython'
+    'Cython==0.29.36'
 ]
 
 [project.optional-dependencies]
 dev = [
     'pytest',
     'pytest-xdist',
     'pytest-cov',
@@ -113,28 +115,32 @@
 visualizers = [
     'layoutparser==0.3.4'
 ]
 predictors = [
     'thefuzz[speedup]',
     'scikit-learn==1.1.2',
     'xgboost==1.6.2',
-    'spacy==3.3.1',
+    'spacy==3.4.1',
     'pysbd==0.3.4',
     'tokenizers==0.13.1',
     'torch==1.12.1',
     'torchvision==0.13.1',
     'layoutparser==0.3.4',
     'transformers',
     'smashed==0.1.10',
-    'optimum[onnxruntime]==1.4.0',
     'pytorch-lightning==2.0.5',
     'springs==1.12.3',
     'wandb==0.15.7',
     'seqeval==1.2.2',
-    'effdet==0.3.0'
+    'effdet==0.3.0',
+    'decontext==0.1.5',
+    'vila==0.5.0'
+]
+production = [
+    'optimum[onnxruntime]==1.4.0'
 ]
 
 [tool.pytest.ini_options]
 addopts = '-n auto --cov=.'
 testpaths = ['tests/']
 pythonpath = [
   '.', 'src',
```

### Comparing `papermage-0.1.0/tests/test_parsers/test_pdf_plumber_parser.py` & `papermage-0.11.1/tests/test_parsers/test_pdf_plumber_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import os
 import pathlib
 import re
 import unittest
 
 import numpy as np
 
+from papermage.magelib import Box, Document, Entity, Span
 from papermage.parsers import PDFPlumberParser
-from papermage.types import Box, Document, Entity, Span
 
 
 class TestPDFPlumberParser(unittest.TestCase):
     def setUp(self) -> None:
         self.fixture_path = pathlib.Path(__file__).parent.parent / "fixtures"
         self.parser = PDFPlumberParser()
         self.doc = self.parser.parse(input_pdf_path=str(self.fixture_path / "2304.02623v1.pdf"))
```

### Comparing `papermage-0.1.0/tests/test_predictors/test_entity_classification_predictor.py` & `papermage-0.11.1/tests/test_predictors/test_entity_classification_predictor.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,54 +4,51 @@
 
 """
 
 import json
 import pathlib
 import unittest
 
+from papermage.magelib import Document, Entity, Span
 from papermage.parsers import PDFPlumberParser
-from papermage.predictors import EntityClassificationPredictor
-from papermage.types import Document, Entity, Span
+from papermage.predictors import HFBIOTaggerPredictor
 
 TEST_SCIBERT_WEIGHTS = "allenai/scibert_scivocab_uncased"
-# TEST_BIB_PARSER_WEIGHTS = '/Users/kylel/ai2/mmda/stefans/'
 
 
 class TestEntityClassificationPredictor(unittest.TestCase):
     def setUp(self):
         self.fixture_path = pathlib.Path(__file__).parent.parent / "fixtures"
         with open(self.fixture_path / "entity_classification_predictor_test_doc_papermage.json", "r") as f:
             test_doc_json = json.load(f)
         self.doc = Document.from_json(doc_json=test_doc_json)
         ent1 = Entity(spans=[Span(start=86, end=456)])
         ent2 = Entity(spans=[Span(start=457, end=641)])
         self.doc.annotate_entity(field_name="bibs", entities=[ent1, ent2])
-        ent1.id = 0
-        ent2.id = 1
 
-        self.predictor = EntityClassificationPredictor.from_pretrained(
+        self.predictor = HFBIOTaggerPredictor.from_pretrained(
             model_name_or_path=TEST_SCIBERT_WEIGHTS, entity_name="tokens", context_name="pages"
         )
 
     def test_predict_pages_tokens(self):
-        predictor = EntityClassificationPredictor.from_pretrained(
+        predictor = HFBIOTaggerPredictor.from_pretrained(
             model_name_or_path=TEST_SCIBERT_WEIGHTS, entity_name="tokens", context_name="pages"
         )
         token_tags = predictor.predict(doc=self.doc)
-        assert len(token_tags) == len([token for page in self.doc.pages for token in page.tokens])
+        assert len(token_tags) == 1
 
         self.doc.annotate_entity(field_name="token_tags", entities=token_tags)
         for token_tag in token_tags:
             assert isinstance(token_tag.metadata.label, str)
             assert isinstance(token_tag.metadata.score, float)
 
     def test_predict_bibs_tokens(self):
         self.predictor.context_name = "bibs"
         token_tags = self.predictor.predict(doc=self.doc)
-        assert len(token_tags) == len([token for bib in self.doc.bibs for token in bib.tokens])
+        assert len(token_tags) == 1
 
     def test_missing_fields(self):
         self.predictor.entity_name = "OHNO"
         with self.assertRaises(AssertionError) as e:
             self.predictor.predict(doc=self.doc)
             assert "OHNO" in e.exception
 
@@ -60,20 +57,20 @@
         with self.assertRaises(AssertionError) as e:
             self.predictor.predict(doc=self.doc)
             assert "BLABLA" in e.exception
 
         self.predictor.context_name = "pages"
 
     def test_predict_pages_tokens_roberta(self):
-        predictor = EntityClassificationPredictor.from_pretrained(
+        predictor = HFBIOTaggerPredictor.from_pretrained(
             model_name_or_path="roberta-base",
             entity_name="tokens",
             context_name="pages",
             add_prefix_space=True,  # Needed for roberta
         )
         token_tags = predictor.predict(doc=self.doc)
-        assert len(token_tags) == len([token for page in self.doc.pages for token in page.tokens])
+        assert len(token_tags) == 1
 
         self.doc.annotate_entity(field_name="token_tags", entities=token_tags)
         for token_tag in token_tags:
             assert isinstance(token_tag.metadata.label, str)
             assert isinstance(token_tag.metadata.score, float)
```

### Comparing `papermage-0.1.0/tests/test_rasterizers/test_pdf2image_rasterizer.py` & `papermage-0.11.1/tests/test_rasterizers/test_pdf2image_rasterizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 import json
 import os
 import pathlib
 import re
 import unittest
 
+from papermage.magelib import Document, Entity, Image, Span
 from papermage.rasterizers import PDF2ImageRasterizer
-from papermage.types import Document, Entity, Image, Span
 
 
 class TestPDF2ImageRasterizer(unittest.TestCase):
     def setUp(cls) -> None:
         cls.fixture_path = pathlib.Path(__file__).parent.parent / "fixtures"
 
     def test_raseterize(self):
```

### Comparing `papermage-0.1.0/tests/test_trainers/test_entity_classification_predictor_trainer.py` & `papermage-0.11.1/tests/test_trainers/test_entity_classification_predictor_trainer.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,60 +8,57 @@
 import unittest
 from pathlib import Path
 
 import springs
 import torch
 import transformers
 
-from papermage.parsers import PDFPlumberParser
-from papermage.predictors import EntityClassificationPredictor
-from papermage.trainers.entity_classification_predictor_trainer import (
-    EntityClassificationPredictorTrainer,
-    EntityClassificationTrainConfig,
+from papermage.magelib import Document, Entity, Span
+from papermage.predictors import HFBIOTaggerPredictor
+from papermage.trainers.bio_tagger_predictor_trainer import (
+    HFBIOTaggerPredictorTrainConfig,
+    HFBIOTaggerPredictorTrainer,
 )
-from papermage.types import Document, Entity, Span
 
 TEST_SCIBERT_WEIGHTS = "allenai/scibert_scivocab_uncased"
 
 
 class TestEntityClassificationPredictorTrainer(unittest.TestCase):
     def setUp(self):
         transformers.set_seed(407)
         self.fixture_path = Path("tests/fixtures")
         with open(self.fixture_path / "entity_classification_predictor_test_doc_papermage.json", "r") as f:
             test_doc_json = json.load(f)
         self.doc = Document.from_json(doc_json=test_doc_json)
         ent1 = Entity(spans=[Span(start=86, end=456)])
         ent2 = Entity(spans=[Span(start=457, end=641)])
         self.doc.annotate_entity(field_name="bibs", entities=[ent1, ent2])
-        ent1.id = 0
-        ent2.id = 1
 
-        self.predictor = EntityClassificationPredictor.from_pretrained(
+        self.predictor = HFBIOTaggerPredictor.from_pretrained(
             model_name_or_path=TEST_SCIBERT_WEIGHTS,
             entity_name="tokens",
             context_name="pages",
             num_labels=3,
             id2label={0: "O", 1: "B_Title", 2: "I_Title"},
             label2id={"O": 0, "B_Title": 1, "I_Title": 2},
         )
 
-        config = springs.from_dataclass(EntityClassificationTrainConfig)
+        config = springs.from_dataclass(HFBIOTaggerPredictorTrainConfig)
         config = springs.merge(
             config,
             springs.from_dict(
                 {
                     "data_path": self.fixture_path / "predictor_training_docs_tiny.jsonl",
                     "label_field": "words_starting_with_td",
                     "max_steps": 1,
                     "seed": 407,
                 }
             ),
         )
-        self.trainer = EntityClassificationPredictorTrainer(
+        self.trainer = HFBIOTaggerPredictorTrainer(
             predictor=self.predictor,
             config=config,
         )
 
     def test_train(self) -> None:
         if (self.trainer.CACHE_PATH / self.trainer.data_id / "inputs.pt").exists():
             (self.trainer.CACHE_PATH / self.trainer.data_id / "inputs.pt").unlink()
@@ -77,24 +74,24 @@
             annotations_entity_names=["words_starting_with_td"],
         )
 
         # check that the cache file exists
         assert (self.trainer.CACHE_PATH / self.trainer.data_id / "inputs.pt").exists()
 
         # check that we can load in the trained model and run it on the test doc (`self.doc`)
-        new_predictor = EntityClassificationPredictor.from_pretrained(
+        new_predictor = HFBIOTaggerPredictor.from_pretrained(
             model_name_or_path=self.trainer.config.default_root_dir / "checkpoints",
             entity_name=self.predictor.entity_name,
             context_name=self.predictor.context_name,
             id2label=id2label,
             label2id=label2id,
         )
 
         token_tags = new_predictor.predict(doc=self.doc)
-        assert len(token_tags) == len([token for page in self.doc.pages for token in page.tokens])
+        assert len(token_tags) == 20
 
     def test_preprocess(self):
         self.trainer.predictor.predictor.config.id2label = {
             0: "O",
             1: "B-words_starting_with_td",
             2: "I-words_starting_with_td",
         }
```

### Comparing `papermage-0.1.0/tests/test_types/test_annotation.py` & `papermage-0.11.1/tests/test_magelib/test_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 @kylel
 
 """
 
 import unittest
 
-from papermage.types import Annotation
+from papermage.magelib import Annotation
 
 
 class DummyAnnotation(Annotation):
     pass
 
 
 class DummyDoc:
```

### Comparing `papermage-0.1.0/tests/test_types/test_box.py` & `papermage-0.11.1/tests/test_magelib/test_box.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
 @kylel
 
 """
 
 import unittest
-from papermage.types import Box
+
+from papermage.magelib import Box
 
 
 class TestBox(unittest.TestCase):
     def test_create(self):
         with self.assertRaises(AssertionError):
             Box(l=0.2, t=0.09, w=-0.095, h=0.017, page=3)
         with self.assertRaises(AssertionError):
```

### Comparing `papermage-0.1.0/tests/test_types/test_entity.py` & `papermage-0.11.1/tests/test_magelib/test_entity.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 
 @kylel
 
 """
 
 import unittest
-from papermage.types import Entity, Span, Box, Metadata
+
+from papermage.magelib import Box, Entity, Metadata, Span
+
 
 class TestEntity(unittest.TestCase):
     def test_create_empty(self):
         with self.assertRaises(ValueError):
             e = Entity()
         # both nones not OK
         with self.assertRaises(ValueError):
@@ -55,34 +57,38 @@
     def test_to_from_json(self):
         spans = [Span(0, 1), Span(2, 3)]
         boxes = [Box(0, 0, 0, 0, 0), Box(1, 1, 1, 1, 1)]
         metadata = Metadata(x=123, y=456)
 
         #  spans only
         entity = Entity(spans=spans)
-        self.assertEqual(entity.to_json(), {'spans': [[0, 1], [2, 3]]})
+        self.assertEqual(entity.to_json(), {"spans": [[0, 1], [2, 3]]})
         entity2 = Entity.from_json(entity.to_json())
         self.assertDictEqual(entity2.to_json(), entity.to_json())
 
         #  boxes only
         entity = Entity(boxes=boxes)
-        self.assertEqual(entity.to_json(),
-                         {'boxes': [[0.0, 0.0, 0.0, 0.0, 0], [1.0, 1.0, 1.0, 1.0, 1]]})
+        self.assertEqual(entity.to_json(), {"boxes": [[0.0, 0.0, 0.0, 0.0, 0], [1.0, 1.0, 1.0, 1.0, 1]]})
         entity2 = Entity.from_json(entity.to_json())
         self.assertDictEqual(entity2.to_json(), entity.to_json())
 
         # both
         entity = Entity(spans=spans, boxes=boxes)
-        self.assertEqual(entity.to_json(),
-                         {'spans': [[0, 1], [2, 3]],
-                          'boxes': [[0.0, 0.0, 0.0, 0.0, 0], [1.0, 1.0, 1.0, 1.0, 1]]})
+        self.assertEqual(
+            entity.to_json(),
+            {"spans": [[0, 1], [2, 3]], "boxes": [[0.0, 0.0, 0.0, 0.0, 0], [1.0, 1.0, 1.0, 1.0, 1]]},
+        )
         entity2 = Entity.from_json(entity.to_json())
         self.assertDictEqual(entity2.to_json(), entity.to_json())
 
         # incl metadata
         entity = Entity(spans=spans, boxes=boxes, metadata=metadata)
-        self.assertEqual(entity.to_json(),
-                         {'spans': [[0, 1], [2, 3]],
-                          'boxes': [[0.0, 0.0, 0.0, 0.0, 0], [1.0, 1.0, 1.0, 1.0, 1]],
-                          'metadata': {'x': 123, 'y': 456}})
+        self.assertEqual(
+            entity.to_json(),
+            {
+                "spans": [[0, 1], [2, 3]],
+                "boxes": [[0.0, 0.0, 0.0, 0.0, 0], [1.0, 1.0, 1.0, 1.0, 1]],
+                "metadata": {"x": 123, "y": 456},
+            },
+        )
         entity2 = Entity.from_json(entity.to_json())
         self.assertDictEqual(entity2.to_json(), entity.to_json())
```

### Comparing `papermage-0.1.0/tests/test_types/test_image.py` & `papermage-0.11.1/tests/test_magelib/test_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 
 @kylel
 
 """
 
+import os
 import unittest
-from papermage.types import Image
 
-import os
 import numpy as np
 
+from papermage.magelib import Image
+
 
 class TestImage(unittest.TestCase):
     def test_to_from_array(self):
-        imarray = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]],
-                            [[11, 12, 13], [14, 15, 16], [17, 18, 19]]])
+        imarray = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]], [[11, 12, 13], [14, 15, 16], [17, 18, 19]]])
         image = Image.from_array(imarray=imarray)
         imarray2 = image.to_array()
         self.assertListEqual(imarray.tolist(), imarray2.tolist())
 
     def test_to_from_array_dimensions(self):
         # wrong number of color channel
         with self.assertRaises(ValueError):
@@ -26,44 +26,42 @@
             image = Image.from_array(imarray=imarray)
         # missing some dimension
         with self.assertRaises(ValueError):
             imarray = np.array([[1, 2, 4, 5, 7, 8], [11, 12, 14, 15, 17, 18]])
             image = Image.from_array(imarray=imarray)
 
     def test_eq(self):
-        imarray = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]],
-                            [[11, 12, 13], [14, 15, 16], [17, 18, 19]]])
+        imarray = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]], [[11, 12, 13], [14, 15, 16], [17, 18, 19]]])
         image1 = Image.from_array(imarray=imarray)
         image2 = Image.from_array(imarray=imarray)
         self.assertEqual(image1, image2)
 
-        imarray2 = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]],
-                            [[11, 12, 13], [14, 15, 16], [17, 18, 20]]])
+        imarray2 = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]], [[11, 12, 13], [14, 15, 16], [17, 18, 20]]])
         image3 = Image.from_array(imarray=imarray2)
         self.assertNotEqual(image1, image3)
 
     def test_greyscale(self):
-        imarray = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]],
-                            [[11, 12, 13], [14, 15, 16], [17, 18, 19]]])
+        imarray = np.array([[[1, 2, 3], [4, 5, 6], [7, 8, 9]], [[11, 12, 13], [14, 15, 16], [17, 18, 19]]])
         image = Image.from_array(imarray=imarray)
         image_grey = image.convert_to_greyscale()
-        self.assertListEqual(image_grey.to_array().tolist(),
-                             [[[2, 2, 2], [5, 5, 5], [8, 8, 8]],
-                              [[12, 12, 12], [15, 15, 15], [18, 18, 18]]])
+        self.assertListEqual(
+            image_grey.to_array().tolist(),
+            [[[2, 2, 2], [5, 5, 5], [8, 8, 8]], [[12, 12, 12], [15, 15, 15], [18, 18, 18]]],
+        )
         self.assertNotEqual(image, image_grey)
-        self.assertEqual(image_grey.mode, 'RGB')
+        self.assertEqual(image_grey.mode, "RGB")
 
     def test_save_open(self):
         # open
-        imagefile = os.path.join(os.path.dirname(__file__), '../fixtures/white_page.png')
+        imagefile = os.path.join(os.path.dirname(__file__), "../fixtures/white_page.png")
         image = Image.open(imagefile)
         # save
-        imagefile = imagefile.replace('white_page.png', 'temp_123_white_page.png')
+        imagefile = imagefile.replace("white_page.png", "temp_123_white_page.png")
         image.save(imagefile)
         # clean
         os.remove(imagefile)
 
     def test_create_rgb_all_white(self):
         image = Image.create_rgb_all_white(width=600, height=800)
-        imagefile = os.path.join(os.path.dirname(__file__), '../fixtures/white_page.png')
+        imagefile = os.path.join(os.path.dirname(__file__), "../fixtures/white_page.png")
         image2 = Image.open(imagefile)
         self.assertEqual(image, image2)
```

### Comparing `papermage-0.1.0/tests/test_types/test_metadata.py` & `papermage-0.11.1/tests/test_magelib/test_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,70 +2,70 @@
 
 Tests for Metadata
 
 @lucas
 
 """
 
-from copy import deepcopy
 import unittest
+from copy import deepcopy
 
-from papermage.types import Metadata
+from papermage.magelib import Metadata
 
 
 class TestMetadata(unittest.TestCase):
     def test_add_keys(self):
         metadata = Metadata()
 
-        metadata['foo'] = 1
+        metadata["foo"] = 1
         self.assertEqual(metadata.foo, 1)
 
         metadata.bar = 2
         self.assertEqual(metadata.bar, 2)
 
-        metadata.set('baz', 3)
+        metadata.set("baz", 3)
         self.assertEqual(metadata.baz, 3)
 
     def test_access_keys(self):
         metadata = Metadata()
         metadata.foo = "bar"
 
         self.assertEqual(metadata.foo, "bar")
         self.assertEqual(metadata.get("foo"), "bar")
         self.assertTrue(metadata["foo"])
         self.assertIsNone(metadata.get("bar"))
 
     def test_json_transform(self):
-        metadata = Metadata.from_json({'foo': 'bar'})
+        metadata = Metadata.from_json({"foo": "bar"})
 
-        self.assertEqual(metadata.to_json(), {'foo': 'bar'})
+        self.assertEqual(metadata.to_json(), {"foo": "bar"})
         self.assertEqual(Metadata.from_json(metadata.to_json()), metadata)
 
     def test_len(self):
-        metadata = Metadata.from_json({f'k{i}': i for i in range(10)})
+        metadata = Metadata.from_json({f"k{i}": i for i in range(10)})
         self.assertEqual(len(metadata), 10)
 
-        metadata.pop('k0')
+        metadata.pop("k0")
         self.assertEqual(len(metadata), 9)
 
         del metadata.k1
         self.assertEqual(len(metadata), 8)
 
     def test_valid_names(self):
         metadata = Metadata()
 
         # this should work fine
-        metadata.set('foo', 'bar')
-        self.assertEqual(metadata.foo, 'bar')
+        metadata.set("foo", "bar")
+        self.assertEqual(metadata.foo, "bar")
 
         # this should fail because `1foo` is not a valid python variable name
         with self.assertRaises(ValueError):
-            metadata.set('1foo', 'bar')
+            metadata.set("1foo", "bar")
 
     def test_deep_copy(self):
-        metadata = Metadata.from_json({'foo': 1, 'bar': 2, 'baz': 3})
+        metadata = Metadata.from_json({"foo": 1, "bar": 2, "baz": 3})
         metadata2 = deepcopy(metadata)
         self.assertEqual(metadata, metadata2)
 
     def test_get_unknown_key(self):
         metadata = Metadata()
         self.assertIsNone(metadata.text)
```

### Comparing `papermage-0.1.0/tests/test_types/test_span.py` & `papermage-0.11.1/tests/test_magelib/test_span.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 @kylel
 
 """
 
 
 import unittest
-from papermage.types import Span
-from papermage.types.span import MergeClusterSpans
 
+from papermage.magelib import Span
+from papermage.magelib.span import MergeClusterSpans
 
-class TestSpan(unittest.TestCase):
 
+class TestSpan(unittest.TestCase):
     def test_to_from_json(self):
         span = Span(start=0, end=0)
         self.assertEqual(span.to_json(), [0, 0])
 
         span2 = Span.from_json(span.to_json())
         self.assertEqual(span2.start, 0)
         self.assertEqual(span2.end, 0)
```

### Comparing `papermage-0.1.0/tests/test_visualizers/test_visualizer.py` & `papermage-0.11.1/tests/test_visualizers/test_visualizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,25 @@
 import os
 import pathlib
 import re
 import unittest
 
 import numpy as np
 
+from papermage.magelib import Box, Document, Entity, Span
 from papermage.parsers import PDFPlumberParser
 from papermage.rasterizers import PDF2ImageRasterizer
-from papermage.types import Box, Document, Entity, Span
 
 
 class TestVisualizer(unittest.TestCase):
     def setUp(self) -> None:
         self.fixture_path = pathlib.Path(__file__).parent.parent / "fixtures"
         with open(self.fixture_path / "2304.02623v1.json") as f_in:
             doc_dict = json.load(f_in)
             self.doc = Document.from_json(doc_dict)
 
         rasterizer = PDF2ImageRasterizer()
-        images = rasterizer.rasterize(
-            input_pdf_path="/Users/kylel/ai2/papermage/tests/fixtures/2304.02623v1.pdf", dpi=72
-        )
+        images = rasterizer.rasterize(input_pdf_path=str(self.fixture_path / "2304.02623v1.pdf"), dpi=72)
         rasterizer.attach_images(images=images, doc=self.doc)
         page = self.doc.pages[0]
         page_image = page.images[0]
         entities_on_page = page.tokens
```

