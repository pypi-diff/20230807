# Comparing `tmp/pedl-1.0.0.tar.gz` & `tmp/pedl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pedl-1.0.0.tar", last modified: Fri Jun  2 13:28:26 2023, max compression
+gzip compressed data, was "pedl-1.0.1.tar", last modified: Mon Aug  7 12:23:52 2023, max compression
```

## Comparing `pedl-1.0.0.tar` & `pedl-1.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.607981 pedl-1.0.0/
--rw-r--r--   0 leon       (501) staff       (20)     5929 2023-06-02 13:28:26.607852 pedl-1.0.0/PKG-INFO
--rw-r--r--   0 leon       (501) staff       (20)     5637 2023-06-02 13:25:24.000000 pedl-1.0.0/README.md
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.586580 pedl-1.0.0/pedl/
--rw-r--r--   0 leon       (501) staff       (20)       22 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/__init__.py
--rw-r--r--   0 leon       (501) staff       (20)     4898 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/bert_for_distant_supervision.py
--rw-r--r--   0 leon       (501) staff       (20)     4242 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/build_training_set.py
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.587725 pedl-1.0.0/pedl/configs/
--rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/__init__.py
--rw-r--r--   0 leon       (501) staff       (20)      501 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/build_training_set.yaml
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.587920 pedl-1.0.0/pedl/configs/database/
--rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/database/__init__.py
--rw-r--r--   0 leon       (501) staff       (20)      452 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/database/default.yaml
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.588018 pedl-1.0.0/pedl/configs/elastic/
--rw-r--r--   0 leon       (501) staff       (20)       67 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/elastic/default.yaml
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.588201 pedl-1.0.0/pedl/configs/entities/
--rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/entities/__init__.py
--rw-r--r--   0 leon       (501) staff       (20)       96 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/entities/default.yaml
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.588295 pedl-1.0.0/pedl/configs/hydra/
--rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/hydra/__init__.py
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.588867 pedl-1.0.0/pedl/configs/hydra/help/
--rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/hydra/help/__init__.py
--rw-r--r--   0 leon       (501) staff       (20)      967 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/build_training_set_help.yaml
--rw-r--r--   0 leon       (501) staff       (20)     1109 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/excel_summarize_help.yaml
--rw-r--r--   0 leon       (501) staff       (20)     1549 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/predict_help.yaml
--rw-r--r--   0 leon       (501) staff       (20)      745 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/pubtator_elasticsearch_help.yaml
--rw-r--r--   0 leon       (501) staff       (20)      823 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/rebuild_pubtator_index_help.yaml
--rw-r--r--   0 leon       (501) staff       (20)      858 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/predict.yaml
--rw-r--r--   0 leon       (501) staff       (20)      116 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/pubtator_elaticsearch.yaml
--rw-r--r--   0 leon       (501) staff       (20)      503 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/rebuild_pubtator_index.yaml
--rw-r--r--   0 leon       (501) staff       (20)      849 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/summarize.yaml
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.589144 pedl-1.0.0/pedl/configs/type/
--rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/type/__init__.py
--rw-r--r--   0 leon       (501) staff       (20)      556 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/type/drug_protein.yaml
--rw-r--r--   0 leon       (501) staff       (20)      476 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/type/protein_protein.yaml
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.605622 pedl-1.0.0/pedl/data/
--rw-r--r--   0 leon       (501) staff       (20) 18171360 2022-12-02 15:16:45.000000 pedl-1.0.0/pedl/data/HOM_AllOrganism.rpt
--rw-r--r--   0 leon       (501) staff       (20)  5179646 2022-12-02 15:16:45.000000 pedl-1.0.0/pedl/data/geneid_to_name.json
--rw-r--r--   0 leon       (501) staff       (20)   716415 2022-12-02 15:16:45.000000 pedl-1.0.0/pedl/data/uniprot2geneid.json
--rw-r--r--   0 leon       (501) staff       (20)    18740 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/data_getter.py
--rw-r--r--   0 leon       (501) staff       (20)     1634 2022-12-02 15:16:45.000000 pedl-1.0.0/pedl/database.py
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.606782 pedl-1.0.0/pedl/datasets/
--rw-r--r--   0 leon       (501) staff       (20)        0 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/datasets/__init__.py
--rw-r--r--   0 leon       (501) staff       (20)     5473 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/datasets/pedl_dataset.py
--rw-r--r--   0 leon       (501) staff       (20)     7997 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/predict.py
--rw-r--r--   0 leon       (501) staff       (20)     8640 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/pubtator_elasticsearch.py
--rw-r--r--   0 leon       (501) staff       (20)     1112 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/rebuild_pubtator_index.py
--rw-r--r--   0 leon       (501) staff       (20)    13091 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/summarize.py
--rw-r--r--   0 leon       (501) staff       (20)    18176 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/utils.py
-drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.587167 pedl-1.0.0/pedl.egg-info/
--rw-r--r--   0 leon       (501) staff       (20)     5929 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/PKG-INFO
--rw-r--r--   0 leon       (501) staff       (20)     1362 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/SOURCES.txt
--rw-r--r--   0 leon       (501) staff       (20)        1 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/dependency_links.txt
--rw-r--r--   0 leon       (501) staff       (20)      246 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/entry_points.txt
--rw-r--r--   0 leon       (501) staff       (20)      161 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/requires.txt
--rw-r--r--   0 leon       (501) staff       (20)        5 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/top_level.txt
--rw-r--r--   0 leon       (501) staff       (20)       38 2023-06-02 13:28:26.608040 pedl-1.0.0/setup.cfg
--rw-r--r--   0 leon       (501) staff       (20)     1304 2023-06-02 13:27:53.000000 pedl-1.0.0/setup.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.147140 pedl-1.0.1/
+-rw-r--r--   0 leon       (501) staff       (20)     6836 2023-08-07 12:23:52.147026 pedl-1.0.1/PKG-INFO
+-rw-r--r--   0 leon       (501) staff       (20)     6543 2023-06-03 08:48:49.000000 pedl-1.0.1/README.md
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.132525 pedl-1.0.1/pedl/
+-rw-r--r--   0 leon       (501) staff       (20)       22 2023-08-07 12:22:08.000000 pedl-1.0.1/pedl/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)     4898 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/bert_for_distant_supervision.py
+-rw-r--r--   0 leon       (501) staff       (20)     4242 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/build_training_set.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.133959 pedl-1.0.1/pedl/configs/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-08-07 12:22:08.000000 pedl-1.0.1/pedl/configs/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)      501 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/build_training_set.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.134186 pedl-1.0.1/pedl/configs/database/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-08-07 12:22:08.000000 pedl-1.0.1/pedl/configs/database/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)      452 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/database/default.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.134302 pedl-1.0.1/pedl/configs/elastic/
+-rw-r--r--   0 leon       (501) staff       (20)       67 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/elastic/default.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.134517 pedl-1.0.1/pedl/configs/entities/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-08-07 12:22:08.000000 pedl-1.0.1/pedl/configs/entities/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)       96 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/entities/default.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.134614 pedl-1.0.1/pedl/configs/hydra/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-08-07 12:22:08.000000 pedl-1.0.1/pedl/configs/hydra/__init__.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.135200 pedl-1.0.1/pedl/configs/hydra/help/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-08-07 12:22:08.000000 pedl-1.0.1/pedl/configs/hydra/help/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)      967 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/hydra/help/build_training_set_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)     1109 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/hydra/help/excel_summarize_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)     1549 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/hydra/help/predict_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      745 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/hydra/help/pubtator_elasticsearch_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      823 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/hydra/help/rebuild_pubtator_index_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      858 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/predict.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      116 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/pubtator_elaticsearch.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      503 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/rebuild_pubtator_index.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      849 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/summarize.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.135472 pedl-1.0.1/pedl/configs/type/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-08-07 12:22:08.000000 pedl-1.0.1/pedl/configs/type/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)      556 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/type/drug_protein.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      476 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/configs/type/protein_protein.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.146377 pedl-1.0.1/pedl/data/
+-rw-r--r--   0 leon       (501) staff       (20) 18171360 2022-12-02 15:16:45.000000 pedl-1.0.1/pedl/data/HOM_AllOrganism.rpt
+-rw-r--r--   0 leon       (501) staff       (20)  5179646 2022-12-02 15:16:45.000000 pedl-1.0.1/pedl/data/geneid_to_name.json
+-rw-r--r--   0 leon       (501) staff       (20)   716415 2022-12-02 15:16:45.000000 pedl-1.0.1/pedl/data/uniprot2geneid.json
+-rw-r--r--   0 leon       (501) staff       (20)    18816 2023-08-07 10:11:11.000000 pedl-1.0.1/pedl/data_getter.py
+-rw-r--r--   0 leon       (501) staff       (20)     1634 2022-12-02 15:16:45.000000 pedl-1.0.1/pedl/database.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.146867 pedl-1.0.1/pedl/datasets/
+-rw-r--r--   0 leon       (501) staff       (20)        0 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/datasets/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)     5473 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/datasets/pedl_dataset.py
+-rw-r--r--   0 leon       (501) staff       (20)     7971 2023-08-07 12:11:44.000000 pedl-1.0.1/pedl/predict.py
+-rw-r--r--   0 leon       (501) staff       (20)     8640 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/pubtator_elasticsearch.py
+-rw-r--r--   0 leon       (501) staff       (20)     1112 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/rebuild_pubtator_index.py
+-rw-r--r--   0 leon       (501) staff       (20)    13091 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/summarize.py
+-rw-r--r--   0 leon       (501) staff       (20)    18176 2023-05-15 11:13:55.000000 pedl-1.0.1/pedl/utils.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-08-07 12:23:52.133212 pedl-1.0.1/pedl.egg-info/
+-rw-r--r--   0 leon       (501) staff       (20)     6836 2023-08-07 12:23:52.000000 pedl-1.0.1/pedl.egg-info/PKG-INFO
+-rw-r--r--   0 leon       (501) staff       (20)     1362 2023-08-07 12:23:52.000000 pedl-1.0.1/pedl.egg-info/SOURCES.txt
+-rw-r--r--   0 leon       (501) staff       (20)        1 2023-08-07 12:23:52.000000 pedl-1.0.1/pedl.egg-info/dependency_links.txt
+-rw-r--r--   0 leon       (501) staff       (20)      246 2023-08-07 12:23:52.000000 pedl-1.0.1/pedl.egg-info/entry_points.txt
+-rw-r--r--   0 leon       (501) staff       (20)      161 2023-08-07 12:23:52.000000 pedl-1.0.1/pedl.egg-info/requires.txt
+-rw-r--r--   0 leon       (501) staff       (20)        5 2023-08-07 12:23:52.000000 pedl-1.0.1/pedl.egg-info/top_level.txt
+-rw-r--r--   0 leon       (501) staff       (20)       38 2023-08-07 12:23:52.147177 pedl-1.0.1/setup.cfg
+-rw-r--r--   0 leon       (501) staff       (20)     1304 2023-08-07 12:22:08.000000 pedl-1.0.1/setup.py
```

### Comparing `pedl-1.0.0/PKG-INFO` & `pedl-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-Metadata-Version: 2.1
-Name: pedl
-Version: 1.0.0
-Summary: Search the biomedical literature for protein interactions andprotein associations.
-Home-page: https://github.com/leonweber/pedl
-Author: Leon Weber
-Author-email: leonweber@posteo.de
-License: MIT
-Description-Content-Type: text/markdown
-
 # PEDL: Protein-Drug and Protein-Protein Association Extraction
 
 PEDL is a powerful framework designed to extract protein-protein and drug-protein associations from biomedical literature. By searching over 30 million abstracts of biomedical publications and more than 4 million full texts using [PubTatorCentral](https://www.ncbi.nlm.nih.gov/research/pubtator/), PEDL leverages state-of-the-art machine reading models to predict association types between proteins, supported by literature evidence.
 
 PEDL is capable of detecting the following association types:
 
 - **Protein-Protein**: controls-phosphorylation-of, controls-state-change-of, controls-transport-of, controls-expression-of, in-complex-with, interacts-with, and catalysis-precedes 
 - **Drug-Protein**: antagonist, agonist, agonist-inihibitor, direct-regulator, activator, inhibitor, indirect-downregulator, indirect-upregulator, part-of, product-of, substrate, and substrate\_product-of
 
 For example usage with expected results, see [this notebook](https://github.com/leonweber/pedl/blob/master/example_usage.ipynb).
 
+### README Contents
+- [Installation](#installation)
+- [Usage](#usage)
+- [FAQ](#faq)
+
 ## Installation
 
 Install PEDL via pip:
 
 ```
 pip install pedl
 ```
@@ -136,7 +131,16 @@
 ```
 
 To only use high-confidence extractions, use the `threshold` parameter:
 
 ```bash
 pedl-summarize input=PEDL_extractions output=summary threshold=0.9
 ```
+
+  ## FAQ
+  - **On which platforms does PEDL work?**
+    - We have thoroughly tested PEDL on Linux and MacOS and verified that its basic functionality works on Windows. We strongly recommend using [mambaforge](https://github.com/conda-forge/miniforge#mambaforge) or [anaconda](https://www.anaconda.com/products/individual) as your Python environment.
+  - **How can I perform a clean uninstall of PEDL?**
+    1. Uninstall the package: `pip uninstall pedl`
+    2. Delete the PEDL cache folder. You can typically find it under `~/.cache/pedl`. So you can delete it by running `rm -rf ~/.cache/pedl`.
+  - **I am running into issues with PEDL. What can I do?**
+    - Try to perform a clean uninstall and reinstall of PEDL. If the issue persists, please open an issue on GitHub and we will try to help you as soon as possible.
```

### Comparing `pedl-1.0.0/README.md` & `pedl-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,33 @@
+Metadata-Version: 2.1
+Name: pedl
+Version: 1.0.1
+Summary: Search the biomedical literature for protein interactions andprotein associations.
+Home-page: https://github.com/leonweber/pedl
+Author: Leon Weber
+Author-email: leonweber@posteo.de
+License: MIT
+Description-Content-Type: text/markdown
+
 # PEDL: Protein-Drug and Protein-Protein Association Extraction
 
 PEDL is a powerful framework designed to extract protein-protein and drug-protein associations from biomedical literature. By searching over 30 million abstracts of biomedical publications and more than 4 million full texts using [PubTatorCentral](https://www.ncbi.nlm.nih.gov/research/pubtator/), PEDL leverages state-of-the-art machine reading models to predict association types between proteins, supported by literature evidence.
 
 PEDL is capable of detecting the following association types:
 
 - **Protein-Protein**: controls-phosphorylation-of, controls-state-change-of, controls-transport-of, controls-expression-of, in-complex-with, interacts-with, and catalysis-precedes 
 - **Drug-Protein**: antagonist, agonist, agonist-inihibitor, direct-regulator, activator, inhibitor, indirect-downregulator, indirect-upregulator, part-of, product-of, substrate, and substrate\_product-of
 
 For example usage with expected results, see [this notebook](https://github.com/leonweber/pedl/blob/master/example_usage.ipynb).
 
+### README Contents
+- [Installation](#installation)
+- [Usage](#usage)
+- [FAQ](#faq)
+
 ## Installation
 
 Install PEDL via pip:
 
 ```
 pip install pedl
 ```
@@ -126,7 +141,16 @@
 ```
 
 To only use high-confidence extractions, use the `threshold` parameter:
 
 ```bash
 pedl-summarize input=PEDL_extractions output=summary threshold=0.9
 ```
+
+  ## FAQ
+  - **On which platforms does PEDL work?**
+    - We have thoroughly tested PEDL on Linux and MacOS and verified that its basic functionality works on Windows. We strongly recommend using [mambaforge](https://github.com/conda-forge/miniforge#mambaforge) or [anaconda](https://www.anaconda.com/products/individual) as your Python environment.
+  - **How can I perform a clean uninstall of PEDL?**
+    1. Uninstall the package: `pip uninstall pedl`
+    2. Delete the PEDL cache folder. You can typically find it under `~/.cache/pedl`. So you can delete it by running `rm -rf ~/.cache/pedl`.
+  - **I am running into issues with PEDL. What can I do?**
+    - Try to perform a clean uninstall and reinstall of PEDL. If the issue persists, please open an issue on GitHub and we will try to help you as soon as possible.
```

### Comparing `pedl-1.0.0/pedl/bert_for_distant_supervision.py` & `pedl-1.0.1/pedl/bert_for_distant_supervision.py`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/build_training_set.py` & `pedl-1.0.1/pedl/build_training_set.py`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/configs/hydra/help/build_training_set_help.yaml` & `pedl-1.0.1/pedl/configs/hydra/help/build_training_set_help.yaml`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/configs/hydra/help/excel_summarize_help.yaml` & `pedl-1.0.1/pedl/configs/hydra/help/excel_summarize_help.yaml`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/configs/hydra/help/predict_help.yaml` & `pedl-1.0.1/pedl/configs/hydra/help/predict_help.yaml`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/configs/hydra/help/pubtator_elasticsearch_help.yaml` & `pedl-1.0.1/pedl/configs/hydra/help/pubtator_elasticsearch_help.yaml`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/configs/hydra/help/rebuild_pubtator_index_help.yaml` & `pedl-1.0.1/pedl/configs/hydra/help/rebuild_pubtator_index_help.yaml`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/configs/predict.yaml` & `pedl-1.0.1/pedl/configs/predict.yaml`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/configs/summarize.yaml` & `pedl-1.0.1/pedl/configs/summarize.yaml`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/configs/type/drug_protein.yaml` & `pedl-1.0.1/pedl/configs/type/drug_protein.yaml`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/data/HOM_AllOrganism.rpt` & `pedl-1.0.1/pedl/data/HOM_AllOrganism.rpt`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/data/geneid_to_name.json` & `pedl-1.0.1/pedl/data/geneid_to_name.json`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/data/uniprot2geneid.json` & `pedl-1.0.1/pedl/data/uniprot2geneid.json`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/data_getter.py` & `pedl-1.0.1/pedl/data_getter.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,15 @@
                 len_ent2 = entity2_lengths[j]
                 sentence = self.get_sentence(
                     passage=passage,
                     offset_ent1=loc_ent1,
                     offset_ent2=loc_ent2,
                     len_ent1=len_ent1,
                     len_ent2=len_ent2,
-                    pmid=document.id,
+                    pmid=get_pmid(document)[0],
                 )
                 if sentence:
                     sentences.append(sentence)
 
         return sentences
 
     def get_pmids(self, entity: Entity) -> Set[str]:
@@ -351,14 +351,16 @@
         pmid_to_pmcid = self.maybe_map_to_pmcid(uncached_pmids)
 
         pmids_to_retreive = [i for i in uncached_pmids if i not in pmid_to_pmcid]
         pmcids_to_retreive = [
             pmid_to_pmcid[i] for i in uncached_pmids if i in pmid_to_pmcid
         ]
 
+        pmcid_to_pmid = {v: k for k, v in pmid_to_pmcid.items()}
+
         for pmid_chunk in list(chunks(pmids_to_retreive, self.CHUNK_SIZE)):
 
             result = requests.get(
                 service_root, params={"pmids": ",".join(pmid_chunk), "concepts": "gene,chemical"}
             )
             collection = bioc.loads(result.content.decode())
             yield collection.documents
```

### Comparing `pedl-1.0.0/pedl/database.py` & `pedl-1.0.1/pedl/database.py`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/datasets/pedl_dataset.py` & `pedl-1.0.1/pedl/datasets/pedl_dataset.py`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/predict.py` & `pedl-1.0.1/pedl/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,16 +138,16 @@
     with (Path(cfg.out) / f"{PREFIX_PROCESSED_PAIRS}_{uuid.uuid4()}").open("w") as f_pairs_processed:
         for datapoint in tqdm(dataloader, desc="Reading"):
             head, tail = datapoint["pair"]
             if "sentences" not in datapoint:
                 f_pairs_processed.write(f"{head}\t{tail}\n")
                 continue
 
-            name1 = geneid_to_name.get(head.cuid, head.cuid)
-            name2 = geneid_to_name.get(tail.cuid, tail.cuid)
+            name1 = head.cuid.replace(":", "_")
+            name2 = tail.cuid.replace(":", "_")
 
             file_out = Path(cfg.out) / f"{name1}-_-{name2}.txt"
 
             if head == tail:
                 f_pairs_processed.write(f"{head}\t{tail}\n")
                 continue
```

### Comparing `pedl-1.0.0/pedl/pubtator_elasticsearch.py` & `pedl-1.0.1/pedl/pubtator_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/rebuild_pubtator_index.py` & `pedl-1.0.1/pedl/rebuild_pubtator_index.py`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/summarize.py` & `pedl-1.0.1/pedl/summarize.py`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl/utils.py` & `pedl-1.0.1/pedl/utils.py`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/pedl.egg-info/PKG-INFO` & `pedl-1.0.1/pedl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pedl
-Version: 1.0.0
+Version: 1.0.1
 Summary: Search the biomedical literature for protein interactions andprotein associations.
 Home-page: https://github.com/leonweber/pedl
 Author: Leon Weber
 Author-email: leonweber@posteo.de
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -15,14 +15,19 @@
 PEDL is capable of detecting the following association types:
 
 - **Protein-Protein**: controls-phosphorylation-of, controls-state-change-of, controls-transport-of, controls-expression-of, in-complex-with, interacts-with, and catalysis-precedes 
 - **Drug-Protein**: antagonist, agonist, agonist-inihibitor, direct-regulator, activator, inhibitor, indirect-downregulator, indirect-upregulator, part-of, product-of, substrate, and substrate\_product-of
 
 For example usage with expected results, see [this notebook](https://github.com/leonweber/pedl/blob/master/example_usage.ipynb).
 
+### README Contents
+- [Installation](#installation)
+- [Usage](#usage)
+- [FAQ](#faq)
+
 ## Installation
 
 Install PEDL via pip:
 
 ```
 pip install pedl
 ```
@@ -136,7 +141,16 @@
 ```
 
 To only use high-confidence extractions, use the `threshold` parameter:
 
 ```bash
 pedl-summarize input=PEDL_extractions output=summary threshold=0.9
 ```
+
+  ## FAQ
+  - **On which platforms does PEDL work?**
+    - We have thoroughly tested PEDL on Linux and MacOS and verified that its basic functionality works on Windows. We strongly recommend using [mambaforge](https://github.com/conda-forge/miniforge#mambaforge) or [anaconda](https://www.anaconda.com/products/individual) as your Python environment.
+  - **How can I perform a clean uninstall of PEDL?**
+    1. Uninstall the package: `pip uninstall pedl`
+    2. Delete the PEDL cache folder. You can typically find it under `~/.cache/pedl`. So you can delete it by running `rm -rf ~/.cache/pedl`.
+  - **I am running into issues with PEDL. What can I do?**
+    - Try to perform a clean uninstall and reinstall of PEDL. If the issue persists, please open an issue on GitHub and we will try to help you as soon as possible.
```

### Comparing `pedl-1.0.0/pedl.egg-info/SOURCES.txt` & `pedl-1.0.1/pedl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pedl-1.0.0/setup.py` & `pedl-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name='pedl',
-    version='1.0.0',
+    version='1.0.1',
     description='Search the biomedical literature for protein interactions and'
                 'protein associations.',
     url='https://github.com/leonweber/pedl',
     author='Leon Weber',
     author_email='leonweber@posteo.de',
     license='MIT',
     packages=find_packages(),
```

