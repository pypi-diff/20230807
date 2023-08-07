# Comparing `tmp/DeepSlice-1.1.4.tar.gz` & `tmp/DeepSlice-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSlice-1.1.4.tar", last modified: Thu Aug  3 11:05:25 2023, max compression
+gzip compressed data, was "DeepSlice-1.1.5.tar", last modified: Mon Aug  7 15:09:13 2023, max compression
```

## Comparing `DeepSlice-1.1.4.tar` & `DeepSlice-1.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.189206 DeepSlice-1.1.4/DeepSlice/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.189206 DeepSlice-1.1.4/DeepSlice/coord_post_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/angle_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/depth_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.189206 DeepSlice-1.1.4/DeepSlice/coord_post_processing/plane_alignment_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/coord_post_processing/spacing_and_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/metadata/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/volumes/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/metadata/weights/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/metadata/weights/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/neural_network/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/neural_network/network_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/neural_network/neural_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/DeepSlice/read_and_write/
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/read_and_write/QuickNII_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/DeepSlice/read_and_write/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:05:25.189206 DeepSlice-1.1.4/DeepSlice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 11:05:25.000000 DeepSlice-1.1.4/DeepSlice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-08-03 11:05:09.000000 DeepSlice-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-03 11:05:25.193207 DeepSlice-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-03 11:05:10.000000 DeepSlice-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.934704 DeepSlice-1.1.5/DeepSlice/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/DeepSlice/coord_post_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/coord_post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/coord_post_processing/angle_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/coord_post_processing/depth_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/DeepSlice/coord_post_processing/plane_alignment_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/coord_post_processing/spacing_and_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/DeepSlice/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/metadata/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/DeepSlice/metadata/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/metadata/volumes/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/DeepSlice/metadata/weights/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/metadata/weights/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/DeepSlice/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/neural_network/network_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/neural_network/neural_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/DeepSlice/read_and_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/read_and_write/QuickNII_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/DeepSlice/read_and_write/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:09:13.934704 DeepSlice-1.1.5/DeepSlice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-08-07 15:09:13.000000 DeepSlice-1.1.5/DeepSlice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-07 15:09:13.000000 DeepSlice-1.1.5/DeepSlice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:09:13.000000 DeepSlice-1.1.5/DeepSlice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-07 15:09:13.000000 DeepSlice-1.1.5/DeepSlice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 15:09:13.000000 DeepSlice-1.1.5/DeepSlice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 15:09:13.938704 DeepSlice-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-07 15:09:01.000000 DeepSlice-1.1.5/setup.py
```

### Comparing `DeepSlice-1.1.4/DeepSlice/coord_post_processing/angle_methods.py` & `DeepSlice-1.1.5/DeepSlice/coord_post_processing/angle_methods.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice/coord_post_processing/depth_estimation.py` & `DeepSlice-1.1.5/DeepSlice/coord_post_processing/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py` & `DeepSlice-1.1.5/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice/coord_post_processing/spacing_and_indexing.py` & `DeepSlice-1.1.5/DeepSlice/coord_post_processing/spacing_and_indexing.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice/main.py` & `DeepSlice-1.1.5/DeepSlice/main.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice/metadata/config.json` & `DeepSlice-1.1.5/DeepSlice/metadata/config.json`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice/metadata/metadata_loader.py` & `DeepSlice-1.1.5/DeepSlice/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice/neural_network/neural_network.py` & `DeepSlice-1.1.5/DeepSlice/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice/read_and_write/QuickNII_functions.py` & `DeepSlice-1.1.5/DeepSlice/read_and_write/QuickNII_functions.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/DeepSlice.egg-info/PKG-INFO` & `DeepSlice-1.1.5/DeepSlice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.4
+Version: 1.1.5
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.4.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.5.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+
+[![DOI](https://zenodo.org/badge/274122364.svg)](https://zenodo.org/badge/latestdoi/274122364)
+
+
 ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
 DeepSlice is a python library which automatically aligns mouse histology with the allen brain atlas common coordinate framework.
 The alignments are viewable, and refinable, using the [QuickNII](https://www.nitrc.org/projects/quicknii "QuickNII") software package.
 DeepSlice requires no preprocessing and works on any stain, however we have found it performs best on brightfield images.
 At present one limitation is that it only works on Coronally cut sections, we will release an update in the future for sagittal and horizontally cut histology.
 ![Alt](docs/images/process.PNG) 
 DeepSlice automates the process of identifying exactly where in the brain a section lies, it can accomodate non-orthogonal cutting planes and will produce an image specific annotation for each section in your brain.
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.4 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.5 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.4.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.5.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
-LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
-DeepSlice is a python library which automatically aligns mouse histology with
-the allen brain atlas common coordinate framework. The alignments are viewable,
-and refinable, using the [QuickNII](https://www.nitrc.org/projects/quicknii
-"QuickNII") software package. DeepSlice requires no preprocessing and works on
-any stain, however we have found it performs best on brightfield images. At
-present one limitation is that it only works on Coronally cut sections, we will
-release an update in the future for sagittal and horizontally cut histology. !
-[Alt](docs/images/process.PNG) DeepSlice automates the process of identifying
-exactly where in the brain a section lies, it can accomodate non-orthogonal
-cutting planes and will produce an image specific annotation for each section
-in your brain. ## Workflow DeepSlice is fully integrated with the QUINT
-workflow. Quint helps you register, segment and quantify brain wide datasets!  
-ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use DeepSlice but
-don't need your own personal installation, check out [**DeepSlice Flask**]
-(https://www.DeepSlice.com.au), a fully functional web application which will
-allow you to upload your dataset and download the aligned results. The web
-interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
-[Installation: How to install DeepSlice](#installation) ## [Usage: How to align
-using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
+LICENSE [![DOI](https://zenodo.org/badge/274122364.svg)](https://zenodo.org/
+badge/latestdoi/274122364) ![Alt](docs/images/DeepSlice_github_banner.png
+"DeepSlice Banner") DeepSlice is a python library which automatically aligns
+mouse histology with the allen brain atlas common coordinate framework. The
+alignments are viewable, and refinable, using the [QuickNII](https://
+www.nitrc.org/projects/quicknii "QuickNII") software package. DeepSlice
+requires no preprocessing and works on any stain, however we have found it
+performs best on brightfield images. At present one limitation is that it only
+works on Coronally cut sections, we will release an update in the future for
+sagittal and horizontally cut histology. ![Alt](docs/images/process.PNG)
+DeepSlice automates the process of identifying exactly where in the brain a
+section lies, it can accomodate non-orthogonal cutting planes and will produce
+an image specific annotation for each section in your brain. ## Workflow
+DeepSlice is fully integrated with the QUINT_workflow. Quint helps you
+register, segment and quantify brain wide datasets!   ð­ð§ ð¬ð»ð¤ ##
+Web Application If you would like to use DeepSlice but don't need your own
+personal installation, check out [**DeepSlice Flask**](https://
+www.DeepSlice.com.au), a fully functional web application which will allow you
+to upload your dataset and download the aligned results. The web interface was
+developed by [Michael Pegios](https://github.com/ThermoDev/). ## [Installation:
+How to install DeepSlice](#installation) ## [Usage: How to align using
+DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
 (examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ****** Installation ******
 ***** From PIP *****
 This is the easy and recommended way to install DeepSlice. Make sure your env
 has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
 you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
 project/DeepSlice/)
```

### Comparing `DeepSlice-1.1.4/DeepSlice.egg-info/SOURCES.txt` & `DeepSlice-1.1.5/DeepSlice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/LICENSE` & `DeepSlice-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.4/PKG-INFO` & `DeepSlice-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.4
+Version: 1.1.5
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.4.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.5.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
+
+[![DOI](https://zenodo.org/badge/274122364.svg)](https://zenodo.org/badge/latestdoi/274122364)
+
+
 ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
 DeepSlice is a python library which automatically aligns mouse histology with the allen brain atlas common coordinate framework.
 The alignments are viewable, and refinable, using the [QuickNII](https://www.nitrc.org/projects/quicknii "QuickNII") software package.
 DeepSlice requires no preprocessing and works on any stain, however we have found it performs best on brightfield images.
 At present one limitation is that it only works on Coronally cut sections, we will release an update in the future for sagittal and horizontally cut histology.
 ![Alt](docs/images/process.PNG) 
 DeepSlice automates the process of identifying exactly where in the brain a section lies, it can accomodate non-orthogonal cutting planes and will produce an image specific annotation for each section in your brain.
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.4 Summary: A package to
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.5 Summary: A package to
 align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
 DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.4.tar.gz Author: DeepSlice Team Author-email:
+tags/1.1.5.tar.gz Author: DeepSlice Team Author-email:
 harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
 histology,brain,atlas,alignment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
 Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
-LICENSE ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
-DeepSlice is a python library which automatically aligns mouse histology with
-the allen brain atlas common coordinate framework. The alignments are viewable,
-and refinable, using the [QuickNII](https://www.nitrc.org/projects/quicknii
-"QuickNII") software package. DeepSlice requires no preprocessing and works on
-any stain, however we have found it performs best on brightfield images. At
-present one limitation is that it only works on Coronally cut sections, we will
-release an update in the future for sagittal and horizontally cut histology. !
-[Alt](docs/images/process.PNG) DeepSlice automates the process of identifying
-exactly where in the brain a section lies, it can accomodate non-orthogonal
-cutting planes and will produce an image specific annotation for each section
-in your brain. ## Workflow DeepSlice is fully integrated with the QUINT
-workflow. Quint helps you register, segment and quantify brain wide datasets!  
-ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use DeepSlice but
-don't need your own personal installation, check out [**DeepSlice Flask**]
-(https://www.DeepSlice.com.au), a fully functional web application which will
-allow you to upload your dataset and download the aligned results. The web
-interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
-[Installation: How to install DeepSlice](#installation) ## [Usage: How to align
-using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
+LICENSE [![DOI](https://zenodo.org/badge/274122364.svg)](https://zenodo.org/
+badge/latestdoi/274122364) ![Alt](docs/images/DeepSlice_github_banner.png
+"DeepSlice Banner") DeepSlice is a python library which automatically aligns
+mouse histology with the allen brain atlas common coordinate framework. The
+alignments are viewable, and refinable, using the [QuickNII](https://
+www.nitrc.org/projects/quicknii "QuickNII") software package. DeepSlice
+requires no preprocessing and works on any stain, however we have found it
+performs best on brightfield images. At present one limitation is that it only
+works on Coronally cut sections, we will release an update in the future for
+sagittal and horizontally cut histology. ![Alt](docs/images/process.PNG)
+DeepSlice automates the process of identifying exactly where in the brain a
+section lies, it can accomodate non-orthogonal cutting planes and will produce
+an image specific annotation for each section in your brain. ## Workflow
+DeepSlice is fully integrated with the QUINT_workflow. Quint helps you
+register, segment and quantify brain wide datasets!   ð­ð§ ð¬ð»ð¤ ##
+Web Application If you would like to use DeepSlice but don't need your own
+personal installation, check out [**DeepSlice Flask**](https://
+www.DeepSlice.com.au), a fully functional web application which will allow you
+to upload your dataset and download the aligned results. The web interface was
+developed by [Michael Pegios](https://github.com/ThermoDev/). ## [Installation:
+How to install DeepSlice](#installation) ## [Usage: How to align using
+DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
 (examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ****** Installation ******
 ***** From PIP *****
 This is the easy and recommended way to install DeepSlice. Make sure your env
 has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
 you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
 project/DeepSlice/)
```

### Comparing `DeepSlice-1.1.4/README.md` & `DeepSlice-1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+
+
+[![DOI](https://zenodo.org/badge/274122364.svg)](https://zenodo.org/badge/latestdoi/274122364)
+
+
 ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
 DeepSlice is a python library which automatically aligns mouse histology with the allen brain atlas common coordinate framework.
 The alignments are viewable, and refinable, using the [QuickNII](https://www.nitrc.org/projects/quicknii "QuickNII") software package.
 DeepSlice requires no preprocessing and works on any stain, however we have found it performs best on brightfield images.
 At present one limitation is that it only works on Coronally cut sections, we will release an update in the future for sagittal and horizontally cut histology.
 ![Alt](docs/images/process.PNG) 
 DeepSlice automates the process of identifying exactly where in the brain a section lies, it can accomodate non-orthogonal cutting planes and will produce an image specific annotation for each section in your brain.
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner") DeepSlice is
-a python library which automatically aligns mouse histology with the allen
-brain atlas common coordinate framework. The alignments are viewable, and
-refinable, using the [QuickNII](https://www.nitrc.org/projects/quicknii
-"QuickNII") software package. DeepSlice requires no preprocessing and works on
-any stain, however we have found it performs best on brightfield images. At
-present one limitation is that it only works on Coronally cut sections, we will
-release an update in the future for sagittal and horizontally cut histology. !
-[Alt](docs/images/process.PNG) DeepSlice automates the process of identifying
-exactly where in the brain a section lies, it can accomodate non-orthogonal
-cutting planes and will produce an image specific annotation for each section
-in your brain. ## Workflow DeepSlice is fully integrated with the QUINT
-workflow. Quint helps you register, segment and quantify brain wide datasets!  
-ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use DeepSlice but
-don't need your own personal installation, check out [**DeepSlice Flask**]
-(https://www.DeepSlice.com.au), a fully functional web application which will
-allow you to upload your dataset and download the aligned results. The web
-interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
-[Installation: How to install DeepSlice](#installation) ## [Usage: How to align
-using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
+ [![DOI](https://zenodo.org/badge/274122364.svg)](https://zenodo.org/badge/
+latestdoi/274122364) ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice
+Banner") DeepSlice is a python library which automatically aligns mouse
+histology with the allen brain atlas common coordinate framework. The
+alignments are viewable, and refinable, using the [QuickNII](https://
+www.nitrc.org/projects/quicknii "QuickNII") software package. DeepSlice
+requires no preprocessing and works on any stain, however we have found it
+performs best on brightfield images. At present one limitation is that it only
+works on Coronally cut sections, we will release an update in the future for
+sagittal and horizontally cut histology. ![Alt](docs/images/process.PNG)
+DeepSlice automates the process of identifying exactly where in the brain a
+section lies, it can accomodate non-orthogonal cutting planes and will produce
+an image specific annotation for each section in your brain. ## Workflow
+DeepSlice is fully integrated with the QUINT_workflow. Quint helps you
+register, segment and quantify brain wide datasets!   ð­ð§ ð¬ð»ð¤ ##
+Web Application If you would like to use DeepSlice but don't need your own
+personal installation, check out [**DeepSlice Flask**](https://
+www.DeepSlice.com.au), a fully functional web application which will allow you
+to upload your dataset and download the aligned results. The web interface was
+developed by [Michael Pegios](https://github.com/ThermoDev/). ## [Installation:
+How to install DeepSlice](#installation) ## [Usage: How to align using
+DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
 (examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ****** Installation ******
 ***** From PIP *****
 This is the easy and recommended way to install DeepSlice. Make sure your env
 has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
 you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
 project/DeepSlice/)
```

### Comparing `DeepSlice-1.1.4/setup.py` & `DeepSlice-1.1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,39 +6,40 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='DeepSlice',
     packages=find_packages(),
-    version='1.1.4',
+    version='1.1.5',
     license='GPL-3.0',
     description='A package to align histology to 3D brain atlases',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepSlice Team',
     package_data={'DeepSlice': ['metadata/volumes/placeholder.txt', 'metadata/config.json','metadata/weights/*.txt']},
     include_package_data=True,
     author_email='harry.carey@medisin.uio.no',
     url='https://github.com/PolarBean/DeepSlice',
-    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.4.tar.gz',
+    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.5.tar.gz',
     keywords=['histology', 'brain', 'atlas', 'alignment'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scikit-image',
         'tensorflow==1.15.0',
         'h5py==2.10.0',
         'typing',
         'pandas==1.3.5',
         'requests',
-        'protobuf==3.20'
+        'protobuf==3.20',
+        'lxml'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.7',
     ],
 
-)   
+)
```

