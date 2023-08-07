# Comparing `tmp/cellmaps_image_embedding-0.1.0a8.tar.gz` & `tmp/cellmaps_image_embedding-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_image_embedding-0.1.0a8.tar", last modified: Wed Aug  2 01:47:59 2023, max compression
+gzip compressed data, was "dist/cellmaps_image_embedding-0.1.0a9.tar", last modified: Mon Aug  7 21:51:37 2023, max compression
```

## Comparing `cellmaps_image_embedding-0.1.0a8.tar` & `cellmaps_image_embedding-0.1.0a9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.617403 cellmaps_image_embedding-0.1.0a8/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-07-17 19:14:35.000000 cellmaps_image_embedding-0.1.0a8/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3731 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-18 23:31:36.000000 cellmaps_image_embedding-0.1.0a8/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6446 2023-08-02 01:47:59.617558 cellmaps_image_embedding-0.1.0a8/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4360 2023-07-26 17:56:48.000000 cellmaps_image_embedding-0.1.0a8/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.606394 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/
--rw-r--r--   0 churas     (504) staff       (20)      312 2023-08-02 01:47:05.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     6564 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     5706 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/dataset.py
--rw-r--r--   0 churas     (504) staff       (20)      143 2023-03-30 21:25:53.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     7602 2023-05-16 19:18:42.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/models.py
--rw-r--r--   0 churas     (504) staff       (20)    20431 2023-08-02 01:47:05.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.607975 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6446 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1207 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      121 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       25 2023-08-02 01:47:59.000000 cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.614837 cellmaps_image_embedding-0.1.0a8/docs/
--rw-r--r--   0 churas     (504) staff       (20)      625 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.601784 cellmaps_image_embedding-0.1.0a8/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.601870 cellmaps_image_embedding-0.1.0a8/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.616062 cellmaps_image_embedding-0.1.0a8/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a8/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a8/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a8/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1234 2023-05-18 23:15:22.000000 cellmaps_image_embedding-0.1.0a8/docs/cellmaps_image_embedding.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6131 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      292 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      849 2023-07-26 17:56:48.000000 cellmaps_image_embedding-0.1.0a8/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1254 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      472 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      822 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       83 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4424 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      794 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      739 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      407 2023-08-02 01:47:59.618089 cellmaps_image_embedding-0.1.0a8/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2463 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a8/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-02 01:47:59.617179 cellmaps_image_embedding-0.1.0a8/tests/
--rw-r--r--   0 churas     (504) staff       (20)       79 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1630 2023-05-08 16:58:10.000000 cellmaps_image_embedding-0.1.0a8/tests/test_cellmaps_image_embeddingcmd.py
--rw-r--r--   0 churas     (504) staff       (20)     1394 2023-05-15 20:45:32.000000 cellmaps_image_embedding-0.1.0a8/tests/test_cellmaps_image_embeddingrunner.py
--rw-r--r--   0 churas     (504) staff       (20)      821 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a8/tests/test_integration_cellmaps_image_embedding.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-07 21:51:37.687672 cellmaps_image_embedding-0.1.0a9/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-07-17 19:14:35.000000 cellmaps_image_embedding-0.1.0a9/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3731 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-18 23:31:36.000000 cellmaps_image_embedding-0.1.0a9/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6446 2023-08-07 21:51:37.687816 cellmaps_image_embedding-0.1.0a9/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4360 2023-07-26 17:56:48.000000 cellmaps_image_embedding-0.1.0a9/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-07 21:51:37.679970 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/
+-rw-r--r--   0 churas     (504) staff       (20)      312 2023-08-07 21:20:42.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     6399 2023-08-07 21:20:42.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     5706 2023-06-15 20:35:46.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/dataset.py
+-rw-r--r--   0 churas     (504) staff       (20)      143 2023-03-30 21:25:53.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)     7602 2023-05-16 19:18:42.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/models.py
+-rw-r--r--   0 churas     (504) staff       (20)    24926 2023-08-07 21:27:14.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-07 21:51:37.681536 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6446 2023-08-07 21:51:37.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1207 2023-08-07 21:51:37.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-07 21:51:37.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-07 21:51:37.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      130 2023-08-07 21:51:37.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       25 2023-08-07 21:51:37.000000 cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-07 21:51:37.685703 cellmaps_image_embedding-0.1.0a9/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      625 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-07 21:51:37.676094 cellmaps_image_embedding-0.1.0a9/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-07 21:51:37.676184 cellmaps_image_embedding-0.1.0a9/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-07 21:51:37.686444 cellmaps_image_embedding-0.1.0a9/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a9/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a9/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_image_embedding-0.1.0a9/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1234 2023-05-18 23:15:22.000000 cellmaps_image_embedding-0.1.0a9/docs/cellmaps_image_embedding.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6131 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      292 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      849 2023-07-26 17:56:48.000000 cellmaps_image_embedding-0.1.0a9/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1254 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      472 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      822 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       83 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4424 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      794 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      739 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      407 2023-08-07 21:51:37.688464 cellmaps_image_embedding-0.1.0a9/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2491 2023-08-07 21:20:42.000000 cellmaps_image_embedding-0.1.0a9/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-07 21:51:37.687461 cellmaps_image_embedding-0.1.0a9/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       79 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1630 2023-05-08 16:58:10.000000 cellmaps_image_embedding-0.1.0a9/tests/test_cellmaps_image_embeddingcmd.py
+-rw-r--r--   0 churas     (504) staff       (20)     4480 2023-08-07 21:20:42.000000 cellmaps_image_embedding-0.1.0a9/tests/test_cellmaps_image_embeddingrunner.py
+-rw-r--r--   0 churas     (504) staff       (20)      821 2023-03-30 21:19:36.000000 cellmaps_image_embedding-0.1.0a9/tests/test_integration_cellmaps_image_embedding.py
```

### Comparing `cellmaps_image_embedding-0.1.0a8/CONTRIBUTING.rst` & `cellmaps_image_embedding-0.1.0a9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/LICENSE` & `cellmaps_image_embedding-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/PKG-INFO` & `cellmaps_image_embedding-0.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_image_embedding
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: A tool to generate embeddings from HPA IF images
 Home-page: https://github.com/idekerlab/cellmaps_image_embedding
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: =============================================
         Cell Maps ImmunoFluorescent Image Embedder
```

### Comparing `cellmaps_image_embedding-0.1.0a8/README.rst` & `cellmaps_image_embedding-0.1.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py` & `cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/cellmaps_image_embeddingcmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,16 @@
     parser = argparse.ArgumentParser(description=desc,
                                      formatter_class=constants.ArgParseFormatter)
     parser.add_argument('outdir', help='Output directory')
     parser.add_argument('--inputdir', required=True,
                         help='Directory with rocrate where blue, red, '
                              'yellow, and green image directories reside')
     parser.add_argument('--model_path', type=str,
-                        help='Path to model file. A model file to download '
-                             'is here: '
-                             'https://github.com/'
-                             'CellProfiling/densenet/releases/download/'
-                             'v0.1.0/external_crop512_focal_slov_hardlog'
-                             '_class_densenet121_dropout_i768_aug2_5folds'
-                             '_fold0_final.pth')
+                        default='https://github.com/CellProfiling/densenet/releases/download/v0.1.0/external_crop512_focal_slov_hardlog_class_densenet121_dropout_i768_aug2_5folds_fold0_final.pth',
+                        help='URL or path to model file for image embedding')
     parser.add_argument('--name',
                         help='Name of this run, needed for FAIRSCAPE. If '
                              'unset, name value from specified '
                              'by --inputdir directory will be used')
     parser.add_argument('--organization_name',
                         help='Name of organization running this tool, needed '
                              'for FAIRSCAPE. If unset, organization name specified '
```

### Comparing `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/dataset.py` & `cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/dataset.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/models.py` & `cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/models.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding/runner.py` & `cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #! /usr/bin/env python
 
 import os
 import sys
 import time
 from datetime import date
-import numpy as np
 import logging
+import shutil
 import csv
 import random
 import warnings
+import requests
 import torch
 from torch.autograd import Variable
 from torch.nn import DataParallel
 from torch.utils.data import DataLoader
 from torch.utils.data.sampler import SequentialSampler
 from tqdm import tqdm
 from cellmaps_utils import constants
@@ -63,14 +64,15 @@
     network embeddings
     """
     def __init__(self, dimensions=1024):
         """
         Constructor
         """
         self._dimensions = dimensions
+        self._fairscape_dataset_tuples = []
 
     def get_dimensions(self):
         """
         Gets number of dimensions this embedding will generate
 
         :return: number of dimensions aka vector length
         :rtype: int
@@ -84,14 +86,23 @@
 
         :raises: NotImplementedError: Subclasses should implement this
         :return: Embedding
         :rtype: list
         """
         raise NotImplementedError('Subclasses should implement')
 
+    def get_datasets_that_need_to_be_registered(self):
+        """
+        Gets any datasets that need to be registered with FAIRSCAPE
+
+        :return: list of tuples in format of (dict, filepath as str)
+        :rtype: list
+        """
+        return self._fairscape_dataset_tuples
+
 
 class FakeEmbeddingGenerator(EmbeddingGenerator):
     """
     Fakes image embedding
     """
     def __init__(self, inputdir, dimensions=1024,
                  suffix='.jpg', img_emd_translator=None):
@@ -146,15 +157,15 @@
         :raises: NotImplementedError: Subclasses should implement this
         :return: Embedding
         :rtype: list
         """
         for image_id in self._get_image_id_list():
             if image_id not in self._img_emd_translator.get_name_mapping():
                 continue
-            g =  self._img_emd_translator.get_name_mapping()[image_id]
+            g = self._img_emd_translator.get_name_mapping()[image_id]
 
             row = [g]
             row.extend(np.random.normal(size=self.get_dimensions()))  # sample normal distribution
             prob = [g]
             prob.extend([random.random() for x in range(0, len(ABB_LABEL_INDEX.keys()))])  # might need to add to one
             yield row, prob
 
@@ -168,15 +179,15 @@
     code and no memory leaks
 
     """
     def __init__(self, inputdir, dimensions=1024,
                  outdir=None,
                  model_path=None,
                  suffix='.jpg',
-                 fold = 1,
+                 fold=1,
                  img_emd_translator=None):
         """
         Constructor
 
         :param inputdir: Directory where red, blue, green, and yellow
                          image directories reside
         :type inputdir: str
@@ -200,23 +211,24 @@
         self._inputdir = inputdir
         self.fold = fold
         self._gpus = ''
         self._image_size = 1536
         self._crop_size = 1024
         self._device = 'cpu'
         self._cuda_available = False
-        self._model_path = os.path.abspath(model_path)
+        self._model_path = model_path
         self._suffix = suffix
         self._channels = 4
         self._num_classes = 28
         self._seeds = [0]
         self._augments = ['default']
-        self._model = self._initialize_model()
-        self._dataset = self._initialize_dataset()
-        self._dataloader = self._initialize_dataloader()
+        self._model = None
+        self._dataset = None
+        self._dataloader = None
+
         if img_emd_translator is None:
             self._img_emd_translator = ImageEmbeddingFilterAndNameTranslator(image_downloaddir=inputdir,
                                                                              fold=fold)
 
     def _initialize_model(self):
         """
 
@@ -255,21 +267,78 @@
             batch_size=1,
             drop_last=False,
             num_workers=0,
             pin_memory=False,
         )
         return dataloader
 
+    def _download_model(self, model_path):
+        """
+        If model_path is a URL attempt to download it
+        to pipeline directory, otherwise return as is
+
+        :param model_path: URL or file path to model file needed
+                           for image embedding
+        :type model_path: str
+        :return: path to model file
+        :rtype: str
+        """
+        dest_file = os.path.abspath(os.path.join(self._outdir, 'model.pth'))
+        self._update_fairscape_dataset_tuples(dest_model=dest_file,
+                                              src_url=model_path)
+        if os.path.isfile(model_path):
+            shutil.copy(model_path, dest_file)
+            return dest_file
+
+        with requests.get(model_path,
+                          stream=True) as r:
+            content_size = int(r.headers.get('content-length', 0))
+            tqdm_bar = tqdm(desc='Downloading ' + os.path.basename(model_path),
+                            total=content_size,
+                            unit='B', unit_scale=True,
+                            unit_divisor=1024)
+            logger.debug('Downloading ' + str(model_path) +
+                         ' of size ' + str(content_size) +
+                         'b to ' + dest_file)
+            try:
+                r.raise_for_status()
+                with open(dest_file, 'wb') as f:
+                    for chunk in r.iter_content(chunk_size=8192):
+                        f.write(chunk)
+                        tqdm_bar.update(len(chunk))
+            finally:
+                tqdm_bar.close()
+        return dest_file
+
+    def _update_fairscape_dataset_tuples(self, dest_model=None, src_url=None):
+        """
+        Registers model.pth file with create as a dataset
+
+        """
+        data_dict = {'name': 'Densenet model file',
+                     'description': 'Trained Densenet model used for classification of IF images'
+                                    ' from ' + str(src_url),
+                     'data-format': 'pth',
+                     'author': cellmaps_image_embedding.__name__,
+                     'version': cellmaps_image_embedding.__version__,
+                     'date-published': date.today().strftime('%m-%d-%Y')}
+        self._fairscape_dataset_tuples.append((data_dict, dest_model))
+
     def get_next_embedding(self):
         """
         Generator method for getting next embedding.
 
         :return: Embedding vector with 1st element
         :rtype: list
         """
+        self._model_path = self._download_model(self._model_path)
+        self._model = self._initialize_model()
+        self._dataset = self._initialize_dataset()
+        self._dataloader = self._initialize_dataloader()
+
         for seed in self._seeds:
             for augment in self._augments:
                 np.random.seed(seed)
                 torch.manual_seed(seed)
                 # eg. augment_default
                 transform = eval("augment_%s" % augment)
                 self._dataloader.dataset.set_transform(transform=transform)
@@ -286,38 +355,55 @@
                         else:
                             images = Variable(images)
                         logits, features = self._model(images)
 
                         image_id = image_ids[iter_index] + '_'
                         if image_id not in self._img_emd_translator.get_name_mapping():
                             continue
-                        g =  self._img_emd_translator.get_name_mapping()[image_id]
+                        g = self._img_emd_translator.get_name_mapping()[image_id]
                         # probabilities
                         probs = F.sigmoid(logits)
                         prob_list = [g]
                         prob_list.extend(probs.cpu().data.numpy().tolist()[0])
 
                         # features
                         features = features.cpu().data.numpy().tolist()
                         row = [g]
                         row.extend(features[0])
                         del features
                         del logits
                         yield row, prob_list
 
+    def get_datasets_that_need_to_be_registered(self):
+        """
+        Gets model.pth dataset that needs to be registered with FAIRSCAPE.
+
+        .. warning::
+
+            Must not be called before invocation of :meth:`~cellmaps_image_embedding.runner.DensenetEmbeddingGenerator.get_next_embedding`
+
+        :raises CellMapsImageEmbeddingError: If this method is called before at least one
+                                             invocation of :meth:`~cellmaps_image_embedding.runner.DensenetEmbeddingGenerator.get_next_embedding`
+        :return: list of tuples in format of (dict, filepath as str)
+        :rtype: list
+        """
+        if len(self._fairscape_dataset_tuples) == 0:
+            raise CellMapsImageEmbeddingError('get_next_embedding must be called at least '
+                                              'once before invoking this method')
+        return self._fairscape_dataset_tuples
 
 
 class ImageEmbeddingFilterAndNameTranslator(object):
     """
     Converts image embedding names and filters keeping only
     one per gene
 
     """
 
-    def __init__(self, image_downloaddir=None, fold = 1):
+    def __init__(self, image_downloaddir=None, fold=1):
         """
         Constructor
         """
         self._id_to_gene_mapping = self._gen_filtered_mapping(os.path.join(image_downloaddir, str(fold) + '_' +
                                                                            constants.IMAGE_GENE_NODE_ATTR_FILE))
 
     def _gen_filtered_mapping(self, image_gene_node_attrs_file):
@@ -328,25 +414,27 @@
         :return:
         """
         mapping_dict = {}
         with open(image_gene_node_attrs_file, 'r') as f:
             reader = csv.DictReader(f, delimiter='\t')
             for row in reader:
                 mapping_dict[row['filename'].split(',')[0]] = row['name']
+        if logger.isEnabledFor(logging.DEBUG):
+            logger.debug('Mapping dict: ' + str(mapping_dict))
         return mapping_dict
 
     def get_name_mapping(self):
         """
         Gets mapping of old name to new name
 
         :return: mapping of old name to new name
         :rtype: dict
         """
         return self._id_to_gene_mapping
-                        
+
                         
 class CellmapsImageEmbedder(object):
     """
     Class to run algorithm
     """
     def __init__(self, outdir=None,
                  inputdir=None,
@@ -384,15 +472,15 @@
         self._name = name
         self._project_name = project_name
         self._organization_name = organization_name
         self._provenance_utils = provenance_utils
         self._embedding_generator = embedding_generator
         self._softwareid = None
         self._input_data_dict = input_data_dict
-        self._image_embedding = None
+        self._generated_dataset_ids = []
      
     def _create_rocrate(self):
         """
         Creates rocrate for output directory
 
         :raises CellMapsProvenanceError: If there is an error
         """
@@ -458,31 +546,45 @@
         self._provenance_utils.register_computation(self._outdir,
                                                     name=cellmaps_image_embedding.__name__ + ' computation',
                                                     run_by=str(self._provenance_utils.get_login()),
                                                     command=str(self._input_data_dict),
                                                     description='run of ' + cellmaps_image_embedding.__name__,
                                                     used_software=[self._softwareid],
                                                     used_dataset=[input_dataset_id],
-                                                    generated=[self._image_embedding])
+                                                    generated=self._generated_dataset_ids)
 
     def _register_image_embedding_file(self):
         """
         Registers image_gene_node_attributes.tsv file with create as a dataset
 
         """
         data_dict = {'name': cellmaps_image_embedding.__name__ + ' output file',
                      'description': 'Image gene node attributes file',
                      'data-format': 'tsv',
                      'author': cellmaps_image_embedding.__name__,
                      'version': cellmaps_image_embedding.__version__,
                      'date-published': date.today().strftime('%m-%d-%Y')}
-        self._image_embedding = self._provenance_utils.register_dataset(self._outdir,
-                                                                        source_file=self.get_image_embedding_file(),
-                                                                        data_dict=data_dict,
-                                                                        skip_copy=True)
+        dset_id = self._provenance_utils.register_dataset(self._outdir,
+                                                          source_file=self.get_image_embedding_file(),
+                                                          data_dict=data_dict,
+                                                          skip_copy=True)
+        self._generated_dataset_ids.append(dset_id)
+
+    def _register_embedding_generator_datasets(self):
+        """
+
+        :return:
+        """
+        for dset_tuple in self._embedding_generator.get_datasets_that_need_to_be_registered():
+            dset_id = self._provenance_utils.register_dataset(self._outdir,
+                                                              source_file=dset_tuple[1],
+                                                              data_dict=dset_tuple[0],
+                                                              skip_copy=True)
+            logger.debug('Adding embedding_generator dataset to fairscape: ' + str(dset_tuple))
+            self._generated_dataset_ids.append(dset_id)
 
     def get_image_embedding_file(self):
         """
         Gets image embedding file
         :return:
         """
         return os.path.join(self._outdir, constants.IMAGE_EMBEDDING_FILE)
@@ -542,14 +644,15 @@
                     prob_writer.writerow(header_line_prob)
                     for row, prob_list in self._embedding_generator.get_next_embedding():
                         writer.writerow(row)
                         raw_embeddings.append(row)
                         prob_writer.writerow(prob_list)
  
             self._register_image_embedding_file()
+            self._register_embedding_generator_datasets()
 
             self._register_computation()
             exitcode = 0
         finally:
             logutils.write_task_finish_json(outdir=self._outdir,
                                             start_time=self._start_time,
                                             status=exitcode)
```

### Comparing `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/PKG-INFO` & `cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-image-embedding
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: A tool to generate embeddings from HPA IF images
 Home-page: https://github.com/idekerlab/cellmaps_image_embedding
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: =============================================
         Cell Maps ImmunoFluorescent Image Embedder
```

### Comparing `cellmaps_image_embedding-0.1.0a8/cellmaps_image_embedding.egg-info/SOURCES.txt` & `cellmaps_image_embedding-0.1.0a9/cellmaps_image_embedding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/Makefile` & `cellmaps_image_embedding-0.1.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/cellmaps_image_embedding.rst` & `cellmaps_image_embedding-0.1.0a9/docs/cellmaps_image_embedding.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/conf.py` & `cellmaps_image_embedding-0.1.0a9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/index.rst` & `cellmaps_image_embedding-0.1.0a9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/installation.rst` & `cellmaps_image_embedding-0.1.0a9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/make.bat` & `cellmaps_image_embedding-0.1.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/newrelease.rst` & `cellmaps_image_embedding-0.1.0a9/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/pypircfile.rst` & `cellmaps_image_embedding-0.1.0a9/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/usage.rst` & `cellmaps_image_embedding-0.1.0a9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/docs/versioningscheme.rst` & `cellmaps_image_embedding-0.1.0a9/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/setup.py` & `cellmaps_image_embedding-0.1.0a9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
 requirements = ['cellmaps_utils',
+                'requests',
                 'tqdm',
                 'numpy',
                 'pandas>0.23.1',
                 'torch',
                 'torchvision',
                 'opencv-python',
                 'mlcrate',
```

### Comparing `cellmaps_image_embedding-0.1.0a8/tests/test_cellmaps_image_embeddingcmd.py` & `cellmaps_image_embedding-0.1.0a9/tests/test_cellmaps_image_embeddingcmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_image_embedding-0.1.0a8/tests/test_integration_cellmaps_image_embedding.py` & `cellmaps_image_embedding-0.1.0a9/tests/test_integration_cellmaps_image_embedding.py`

 * *Files identical despite different names*

