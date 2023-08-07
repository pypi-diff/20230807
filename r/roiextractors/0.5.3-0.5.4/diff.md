# Comparing `tmp/roiextractors-0.5.3.tar.gz` & `tmp/roiextractors-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roiextractors-0.5.3.tar", last modified: Mon Jun 26 04:31:22 2023, max compression
+gzip compressed data, was "roiextractors-0.5.4.tar", last modified: Mon Aug  7 15:58:39 2023, max compression
```

## Comparing `roiextractors-0.5.3.tar` & `roiextractors-0.5.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-26 04:31:17.000000 roiextractors-0.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 04:31:17.000000 roiextractors-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-26 04:31:22.246183 roiextractors-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-06-26 04:31:17.000000 roiextractors-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-26 04:31:17.000000 roiextractors-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:31:22.246183 roiextractors-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 04:31:17.000000 roiextractors-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.238183 roiextractors-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/example_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/example_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/example_datasets/toy_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extraction_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractorlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/caiman/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/caiman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/caiman/caimansegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/hdf5imagingextractor/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/hdf5imagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/memmapextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/miniscopeimagingextractor/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/miniscopeimagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/numpyextractors/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/numpyextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/numpyextractors/numpyextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/nwbextractors/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/nwbextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/nwbextractors/nwbextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/sbximagingextractor/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/sbximagingextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/simaextractor/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/simaextractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/suite2p/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/suite2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/imagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/multiimagingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/multisegmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/segmentationextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-06-26 04:31:17.000000 roiextractors-0.5.3/src/roiextractors/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:31:22.246183 roiextractors-0.5.3/src/roiextractors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 04:31:22.000000 roiextractors-0.5.3/src/roiextractors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.322107 roiextractors-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-07 15:58:33.000000 roiextractors-0.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 15:58:33.000000 roiextractors-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-08-07 15:58:39.322107 roiextractors-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-08-07 15:58:33.000000 roiextractors-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-07 15:58:33.000000 roiextractors-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 15:58:39.322107 roiextractors-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-07 15:58:33.000000 roiextractors-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.314107 roiextractors-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/example_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/example_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/example_datasets/toy_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20217 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extraction_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractorlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/extractors/caiman/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/caiman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/caiman/caimansegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/extractors/hdf5imagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/hdf5imagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/extractors/memmapextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/memmapextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/memmapextractors/memmapextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/extractors/miniscopeimagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/miniscopeimagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/extractors/numpyextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/numpyextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/numpyextractors/numpyextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/extractors/nwbextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/nwbextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/nwbextractors/nwbextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors/extractors/sbximagingextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/sbximagingextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.322107 roiextractors-0.5.4/src/roiextractors/extractors/schnitzerextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/schnitzerextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.322107 roiextractors-0.5.4/src/roiextractors/extractors/simaextractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/simaextractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.322107 roiextractors-0.5.4/src/roiextractors/extractors/suite2p/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/suite2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.322107 roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/brukertiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/imagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/multiimagingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/multisegmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/segmentationextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-08-07 15:58:33.000000 roiextractors-0.5.4/src/roiextractors/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:58:39.318107 roiextractors-0.5.4/src/roiextractors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-08-07 15:58:39.000000 roiextractors-0.5.4/src/roiextractors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-07 15:58:39.000000 roiextractors-0.5.4/src/roiextractors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:58:39.000000 roiextractors-0.5.4/src/roiextractors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-07 15:58:39.000000 roiextractors-0.5.4/src/roiextractors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 15:58:39.000000 roiextractors-0.5.4/src/roiextractors.egg-info/top_level.txt
```

### Comparing `roiextractors-0.5.3/LICENSE.txt` & `roiextractors-0.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/PKG-INFO` & `roiextractors-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roiextractors
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python module for extracting optical physiology ROIs and traces for various file types and formats
 Home-page: https://github.com/catalystneuro/roiextractors
 Author: Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino
 Author-email: ben.dichter@gmail.com
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/roiextractors)
         ![Full Tests](https://github.com/catalystneuro/roiextractors/actions/workflows/testing.yml/badge.svg)
```

### Comparing `roiextractors-0.5.3/README.md` & `roiextractors-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/setup.py` & `roiextractors-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 gin_config_file_base = root / "base_gin_test_config.json"
 gin_config_file_local = root / "tests" / "gin_test_config.json"
 if not gin_config_file_local.exists():
     copy_file(src=gin_config_file_base, dst=gin_config_file_local)
 
 setup(
     name="roiextractors",
-    version="0.5.3",
+    version="0.5.4",
     author="Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino",
     author_email="ben.dichter@gmail.com",
     description="Python module for extracting optical physiology ROIs and traces for various file types and formats",
     url="https://github.com/catalystneuro/roiextractors",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
```

### Comparing `roiextractors-0.5.3/src/roiextractors/__init__.py` & `roiextractors-0.5.4/src/roiextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/example_datasets/toy_example.py` & `roiextractors-0.5.4/src/roiextractors/example_datasets/toy_example.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extraction_tools.py` & `roiextractors-0.5.4/src/roiextractors/extraction_tools.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractorlist.py` & `roiextractors-0.5.4/src/roiextractors/extractorlist.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,30 +11,32 @@
     ExtractSegmentationExtractor,
 )
 from .extractors.simaextractor import SimaSegmentationExtractor
 from .extractors.suite2p import Suite2pSegmentationExtractor
 from .extractors.tiffimagingextractors import (
     TiffImagingExtractor,
     ScanImageTiffImagingExtractor,
-    BrukerTiffImagingExtractor,
+    BrukerTiffMultiPlaneImagingExtractor,
+    BrukerTiffSinglePlaneImagingExtractor,
     MicroManagerTiffImagingExtractor,
 )
 from .extractors.sbximagingextractor import SbxImagingExtractor
 from .extractors.memmapextractors import NumpyMemmapImagingExtractor
 from .extractors.memmapextractors import MemmapImagingExtractor
 from .extractors.miniscopeimagingextractor import MiniscopeImagingExtractor
 from .multisegmentationextractor import MultiSegmentationExtractor
 from .multiimagingextractor import MultiImagingExtractor
 
 imaging_extractor_full_list = [
     NumpyImagingExtractor,
     Hdf5ImagingExtractor,
     TiffImagingExtractor,
     ScanImageTiffImagingExtractor,
-    BrukerTiffImagingExtractor,
+    BrukerTiffMultiPlaneImagingExtractor,
+    BrukerTiffSinglePlaneImagingExtractor,
     MicroManagerTiffImagingExtractor,
     MiniscopeImagingExtractor,
     NwbImagingExtractor,
     SbxImagingExtractor,
     NumpyMemmapImagingExtractor,
     MemmapImagingExtractor,
 ]
```

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/caiman/caimansegmentationextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/caiman/caimansegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/hdf5imagingextractor/hdf5imagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/memmapextractors.py` & `roiextractors-0.5.4/src/roiextractors/extractors/memmapextractors/memmapextractors.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/memmapextractors/numpymemampextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/miniscopeimagingextractor/miniscopeimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/numpyextractors/numpyextractors.py` & `roiextractors-0.5.4/src/roiextractors/extractors/numpyextractors/numpyextractors.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/nwbextractors/nwbextractors.py` & `roiextractors-0.5.4/src/roiextractors/extractors/nwbextractors/nwbextractors.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/sbximagingextractor/sbximagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/schnitzerextractor/cnmfesegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/schnitzerextractor/extractsegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/simaextractor/simasegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/suite2p/suite2psegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/micromanagertiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/scanimagetiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py` & `roiextractors-0.5.4/src/roiextractors/extractors/tiffimagingextractors/tiffimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/imagingextractor.py` & `roiextractors-0.5.4/src/roiextractors/imagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/multiimagingextractor.py` & `roiextractors-0.5.4/src/roiextractors/multiimagingextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/multisegmentationextractor.py` & `roiextractors-0.5.4/src/roiextractors/multisegmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/segmentationextractor.py` & `roiextractors-0.5.4/src/roiextractors/segmentationextractor.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors/testing.py` & `roiextractors-0.5.4/src/roiextractors/testing.py`

 * *Files identical despite different names*

### Comparing `roiextractors-0.5.3/src/roiextractors.egg-info/PKG-INFO` & `roiextractors-0.5.4/src/roiextractors.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roiextractors
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python module for extracting optical physiology ROIs and traces for various file types and formats
 Home-page: https://github.com/catalystneuro/roiextractors
 Author: Heberto Mayorquin, Szonja Weigl, Cody Baker, Ben Dichter, Alessio Buccino
 Author-email: ben.dichter@gmail.com
 License: UNKNOWN
 Description: [![PyPI version](https://badge.fury.io/py/roiextractors.svg)](https://badge.fury.io/py/roiextractors)
         ![Full Tests](https://github.com/catalystneuro/roiextractors/actions/workflows/testing.yml/badge.svg)
```

### Comparing `roiextractors-0.5.3/src/roiextractors.egg-info/SOURCES.txt` & `roiextractors-0.5.4/src/roiextractors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

