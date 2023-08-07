# Comparing `tmp/kmergenetyper-1.0.9.tar.gz` & `tmp/kmergenetyper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmergenetyper-1.0.9.tar", last modified: Mon May  1 12:23:23 2023, max compression
+gzip compressed data, was "kmergenetyper-1.1.0.tar", last modified: Mon Aug  7 07:04:23 2023, max compression
```

## Comparing `kmergenetyper-1.0.9.tar` & `kmergenetyper-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-05-01 12:23:23.551486 kmergenetyper-1.0.9/
--rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-03-22 07:59:26.000000 kmergenetyper-1.0.9/LICENSE
--rw-r--r--   0 malhal     (502) staff       (20)      645 2023-05-01 12:23:23.551356 kmergenetyper-1.0.9/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      361 2023-04-13 12:04:26.000000 kmergenetyper-1.0.9/README.md
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-05-01 12:23:23.549758 kmergenetyper-1.0.9/bin/
--rwxr-xr-x   0 malhal     (502) staff       (20)     1693 2023-04-05 08:34:47.000000 kmergenetyper-1.0.9/bin/kmergenetyper
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-05-01 12:23:23.550786 kmergenetyper-1.0.9/kmergenetyper/
--rw-r--r--   0 malhal     (502) staff       (20)        0 2023-03-22 09:30:11.000000 kmergenetyper-1.0.9/kmergenetyper/__init__.py
--rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-03-22 08:43:08.000000 kmergenetyper-1.0.9/kmergenetyper/kma.py
--rw-r--r--   0 malhal     (502) staff       (20)     4303 2023-05-01 12:22:54.000000 kmergenetyper-1.0.9/kmergenetyper/realignConsensus.py
--rw-r--r--   0 malhal     (502) staff       (20)     2339 2023-04-05 08:36:09.000000 kmergenetyper-1.0.9/kmergenetyper/typeGenes.py
--rw-r--r--   0 malhal     (502) staff       (20)       21 2023-05-01 12:23:10.000000 kmergenetyper-1.0.9/kmergenetyper/version.py
-drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-05-01 12:23:23.551204 kmergenetyper-1.0.9/kmergenetyper.egg-info/
--rw-r--r--   0 malhal     (502) staff       (20)      645 2023-05-01 12:23:23.000000 kmergenetyper-1.0.9/kmergenetyper.egg-info/PKG-INFO
--rw-r--r--   0 malhal     (502) staff       (20)      325 2023-05-01 12:23:23.000000 kmergenetyper-1.0.9/kmergenetyper.egg-info/SOURCES.txt
--rw-r--r--   0 malhal     (502) staff       (20)        1 2023-05-01 12:23:23.000000 kmergenetyper-1.0.9/kmergenetyper.egg-info/dependency_links.txt
--rw-r--r--   0 malhal     (502) staff       (20)       14 2023-05-01 12:23:23.000000 kmergenetyper-1.0.9/kmergenetyper.egg-info/top_level.txt
--rw-r--r--   0 malhal     (502) staff       (20)       38 2023-05-01 12:23:23.551529 kmergenetyper-1.0.9/setup.cfg
--rw-r--r--   0 malhal     (502) staff       (20)      710 2023-04-21 07:49:49.000000 kmergenetyper-1.0.9/setup.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-08-07 07:04:23.926922 kmergenetyper-1.1.0/
+-rw-r--r--   0 malhal     (502) staff       (20)    11357 2023-05-25 12:32:15.000000 kmergenetyper-1.1.0/LICENSE
+-rw-r--r--   0 malhal     (502) staff       (20)      682 2023-08-07 07:04:23.926769 kmergenetyper-1.1.0/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      361 2023-05-25 12:32:15.000000 kmergenetyper-1.1.0/README.md
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-08-07 07:04:23.925104 kmergenetyper-1.1.0/bin/
+-rwxr-xr-x   0 malhal     (502) staff       (20)     2135 2023-07-25 08:39:46.000000 kmergenetyper-1.1.0/bin/kmergenetyper
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-08-07 07:04:23.926155 kmergenetyper-1.1.0/kmergenetyper/
+-rw-r--r--   0 malhal     (502) staff       (20)        0 2023-05-25 12:32:15.000000 kmergenetyper-1.1.0/kmergenetyper/__init__.py
+-rw-r--r--   0 malhal     (502) staff       (20)     1007 2023-05-25 12:32:15.000000 kmergenetyper-1.1.0/kmergenetyper/kma.py
+-rw-r--r--   0 malhal     (502) staff       (20)     5048 2023-07-10 15:52:27.000000 kmergenetyper-1.1.0/kmergenetyper/realignConsensus.py
+-rw-r--r--   0 malhal     (502) staff       (20)     2772 2023-07-25 08:40:00.000000 kmergenetyper-1.1.0/kmergenetyper/typeGenes.py
+-rw-r--r--   0 malhal     (502) staff       (20)       22 2023-08-07 07:04:12.000000 kmergenetyper-1.1.0/kmergenetyper/version.py
+drwxr-xr-x   0 malhal     (502) staff       (20)        0 2023-08-07 07:04:23.926593 kmergenetyper-1.1.0/kmergenetyper.egg-info/
+-rw-r--r--   0 malhal     (502) staff       (20)      682 2023-08-07 07:04:23.000000 kmergenetyper-1.1.0/kmergenetyper.egg-info/PKG-INFO
+-rw-r--r--   0 malhal     (502) staff       (20)      325 2023-08-07 07:04:23.000000 kmergenetyper-1.1.0/kmergenetyper.egg-info/SOURCES.txt
+-rw-r--r--   0 malhal     (502) staff       (20)        1 2023-08-07 07:04:23.000000 kmergenetyper-1.1.0/kmergenetyper.egg-info/dependency_links.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       14 2023-08-07 07:04:23.000000 kmergenetyper-1.1.0/kmergenetyper.egg-info/top_level.txt
+-rw-r--r--   0 malhal     (502) staff       (20)       38 2023-08-07 07:04:23.926970 kmergenetyper-1.1.0/setup.cfg
+-rw-r--r--   0 malhal     (502) staff       (20)      710 2023-05-25 12:32:15.000000 kmergenetyper-1.1.0/setup.py
```

### Comparing `kmergenetyper-1.0.9/LICENSE` & `kmergenetyper-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.9/PKG-INFO` & `kmergenetyper-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: kmergenetyper
-Version: 1.0.9
+Version: 1.1.0
 Summary: kmergenetyper - K-mer Gene Typer
 Home-page: https://https://github.com/MBHallgren/kmergenetyper
 Author: Malte B. Hallgren
 Author-email: malhal@food.dtu.dk
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kmergenetyper (k-mer gene typer)
 
 # Installation
 
@@ -20,7 +22,9 @@
 `conda activate kmergenetyper`
 
 `pip install kmergenetyper`
 
 # Usage
 
 `kmergenetyper -h`
+
+
```

### Comparing `kmergenetyper-1.0.9/bin/kmergenetyper` & `kmergenetyper-1.1.0/bin/kmergenetyper`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,24 @@
                   ' Illumina and Nanopore sequencing data.'
 
     parser = argparse.ArgumentParser(description=description)
     parser.add_argument('-illumina', action="store", type=str, dest='illumina', nargs="+",
                         default=[], help='Illumina input files. Must be paired-end.')
     parser.add_argument('-nanopore', action="store", type=str, dest='nanopore', nargs="+",
                         default=[], help='Nanopore input files.')
-    parser.add_argument('-md', action="store", type=int, default=5, dest='md',
-                        help='Minimum depth. Default: 5')
+    parser.add_argument('-fasta', action="store", type=str, dest='fasta', nargs="+",
+                        default=[], help='fasta input files.')
+    parser.add_argument('-md', action="store", type=float, default=5.0, dest='md',
+                        help='Minimum depth. Default: 5.0')
+    parser.add_argument('-t', action="store", type=int, default=4, dest='threads',
+                        help='Number of threads. Default: 4')
     parser.add_argument('-t_db', action="store", type=str, dest='t_db', help='KMA indexed database')
     parser.add_argument('-o', action="store", type=str, dest='output', help='Output directory')
+    parser.add_argument('-q', action="store", type=int, default=8, dest='q_score',
+                        help='Minimum q-score. Default: 8')
     parser.add_argument('-keep', action="store_true", dest='keep', help='Keep intermediate gene files.')
     parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
 
     args = parser.parse_args()
 
     if args.illumina != []:
         check_illumina_pe(args.illumina)
```

### Comparing `kmergenetyper-1.0.9/kmergenetyper/kma.py` & `kmergenetyper-1.1.0/kmergenetyper/kma.py`

 * *Files identical despite different names*

### Comparing `kmergenetyper-1.0.9/kmergenetyper.egg-info/PKG-INFO` & `kmergenetyper-1.1.0/kmergenetyper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: kmergenetyper
-Version: 1.0.9
+Version: 1.1.0
 Summary: kmergenetyper - K-mer Gene Typer
 Home-page: https://https://github.com/MBHallgren/kmergenetyper
 Author: Malte B. Hallgren
 Author-email: malhal@food.dtu.dk
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kmergenetyper (k-mer gene typer)
 
 # Installation
 
@@ -20,7 +22,9 @@
 `conda activate kmergenetyper`
 
 `pip install kmergenetyper`
 
 # Usage
 
 `kmergenetyper -h`
+
+
```

### Comparing `kmergenetyper-1.0.9/setup.py` & `kmergenetyper-1.1.0/setup.py`

 * *Files identical despite different names*

