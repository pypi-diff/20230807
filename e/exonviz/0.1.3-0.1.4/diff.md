# Comparing `tmp/exonviz-0.1.3.tar.gz` & `tmp/exonviz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exonviz-0.1.3.tar", last modified: Wed Jul 26 11:30:51 2023, max compression
+gzip compressed data, was "exonviz-0.1.4.tar", last modified: Mon Aug  7 07:42:00 2023, max compression
```

## Comparing `exonviz-0.1.3.tar` & `exonviz-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)    34523 2023-07-11 13:50:44.000000 exonviz-0.1.3/LICENSE
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3966 2023-07-26 11:30:51.212039 exonviz-0.1.3/PKG-INFO
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2960 2023-07-26 06:44:27.000000 exonviz-0.1.3/README.md
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       38 2023-07-26 11:30:51.212039 exonviz-0.1.3/setup.cfg
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2812 2023-07-26 11:30:04.000000 exonviz-0.1.3/setup.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/src/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.3/src/conftest.py
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/src/exonviz/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      166 2023-07-26 06:34:39.000000 exonviz-0.1.3/src/exonviz/__init__.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       61 2023-07-11 13:50:44.000000 exonviz-0.1.3/src/exonviz/__main__.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2542 2023-07-26 06:27:51.000000 exonviz-0.1.3/src/exonviz/cli.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     5895 2023-07-26 06:43:44.000000 exonviz-0.1.3/src/exonviz/draw.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3039 2023-07-11 13:50:44.000000 exonviz-0.1.3/src/exonviz/exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2056 2023-07-21 06:32:19.000000 exonviz-0.1.3/src/exonviz/mutalyzer.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:02:29.000000 exonviz-0.1.3/src/exonviz/py.typed
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/src/exonviz.egg-info/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3966 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/PKG-INFO
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      526 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/SOURCES.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/dependency_links.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       45 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/entry_points.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-26 05:36:45.000000 exonviz-0.1.3/src/exonviz.egg-info/not-zip-safe
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        7 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/requires.txt
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       17 2023-07-26 11:30:51.000000 exonviz-0.1.3/src/exonviz.egg-info/top_level.txt
-drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-07-26 11:30:51.212039 exonviz-0.1.3/tests/
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7408 2023-07-11 13:50:44.000000 exonviz-0.1.3/tests/test_Exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1090 2023-07-11 13:50:44.000000 exonviz-0.1.3/tests/test_cli.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1958 2023-07-11 13:50:44.000000 exonviz-0.1.3/tests/test_draw_exon.py
--rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1699 2023-07-11 13:50:44.000000 exonviz-0.1.3/tests/test_mutalyzer.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-08-07 07:42:00.772351 exonviz-0.1.4/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)    34523 2023-07-11 13:50:44.000000 exonviz-0.1.4/LICENSE
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     4446 2023-08-07 07:42:00.772351 exonviz-0.1.4/PKG-INFO
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3490 2023-08-07 07:34:40.000000 exonviz-0.1.4/README.md
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       38 2023-08-07 07:42:00.772351 exonviz-0.1.4/setup.cfg
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2783 2023-08-07 07:34:17.000000 exonviz-0.1.4/setup.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-08-07 07:42:00.768351 exonviz-0.1.4/src/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-11 13:50:44.000000 exonviz-0.1.4/src/conftest.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-08-07 07:42:00.768351 exonviz-0.1.4/src/exonviz/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      188 2023-08-07 06:07:51.000000 exonviz-0.1.4/src/exonviz/__init__.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       61 2023-07-11 13:50:44.000000 exonviz-0.1.4/src/exonviz/__main__.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3125 2023-08-07 07:05:00.000000 exonviz-0.1.4/src/exonviz/cli.py
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-08-07 07:42:00.768351 exonviz-0.1.4/src/exonviz/data/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)   165800 2023-08-07 06:07:51.000000 exonviz-0.1.4/src/exonviz/data/mane.txt.gz
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7018 2023-08-07 06:08:15.000000 exonviz-0.1.4/src/exonviz/draw.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     3039 2023-07-11 13:50:44.000000 exonviz-0.1.4/src/exonviz/exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     2197 2023-08-07 06:07:51.000000 exonviz-0.1.4/src/exonviz/mutalyzer.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        0 2023-07-21 06:02:29.000000 exonviz-0.1.4/src/exonviz/py.typed
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-08-07 07:42:00.768351 exonviz-0.1.4/src/exonviz.egg-info/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     4446 2023-08-07 07:42:00.000000 exonviz-0.1.4/src/exonviz.egg-info/PKG-INFO
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)      555 2023-08-07 07:42:00.000000 exonviz-0.1.4/src/exonviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-08-07 07:42:00.000000 exonviz-0.1.4/src/exonviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       45 2023-08-07 07:42:00.000000 exonviz-0.1.4/src/exonviz.egg-info/entry_points.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        1 2023-07-26 05:36:45.000000 exonviz-0.1.4/src/exonviz.egg-info/not-zip-safe
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)        7 2023-08-07 07:42:00.000000 exonviz-0.1.4/src/exonviz.egg-info/requires.txt
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)       17 2023-08-07 07:42:00.000000 exonviz-0.1.4/src/exonviz.egg-info/top_level.txt
+drwxrwxr-x   0 trijntje  (1000) trijntje  (1000)        0 2023-08-07 07:42:00.772351 exonviz-0.1.4/tests/
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     7408 2023-07-11 13:50:44.000000 exonviz-0.1.4/tests/test_Exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1090 2023-07-11 13:50:44.000000 exonviz-0.1.4/tests/test_cli.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1958 2023-07-11 13:50:44.000000 exonviz-0.1.4/tests/test_draw_exon.py
+-rw-rw-r--   0 trijntje  (1000) trijntje  (1000)     1699 2023-07-11 13:50:44.000000 exonviz-0.1.4/tests/test_mutalyzer.py
```

### Comparing `exonviz-0.1.3/LICENSE` & `exonviz-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.3/PKG-INFO` & `exonviz-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: exonviz
-Version: 0.1.3
+Version: 0.1.4
 Summary: Visualise exons and their reading frames
 Home-page: https://github.com/redmar-van-den-berg/exonviz
 Author: Redmar van den Berg
 Author-email: RedmarvandenBerg@lumc.nl
 License: AGPL-3.0
 Project-URL: Changelog, https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/redmar-van-den-berg/exonviz/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Continous integration](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml/badge.svg)](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
@@ -39,61 +38,70 @@
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
 
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
 ```
-usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding] [--gap GAP] transcript
+usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding]
+               [--gap GAP] [--color COLOR] [--exonnumber]
+               [--firstexon FIRSTEXON] [--lastexon LASTEXON]
+               transcript
 
 Description of command.
 
 positional arguments:
-  transcript       Transcript (with version) to visualise
+  transcript            Transcript (with version) to visualise
 
 optional arguments:
-  -h, --help       show this help message and exit
-  --width WIDTH    Maximum width of the figure (default: inf)
-  --height HEIGHT  Exon height (default: 20)
-  --noncoding      Show non coding regions (default: False)
-  --gap GAP        Gap between the exons (default: 5)
-  --color COLOR    Color for the exons (e.g. 'purple') (default: #4C72B7)
+  -h, --help            show this help message and exit
+  --width WIDTH         Maximum width of the figure (default: inf)
+  --height HEIGHT       Exon height (default: 20)
+  --noncoding           Show non coding regions (default: False)
+  --gap GAP             Gap between the exons (default: 5)
+  --color COLOR         Color for the exons (e.g. 'purple') (default: #4C72B7)
+  --exonnumber          Show exon number (default: False)
+  --firstexon FIRSTEXON
+                        The first exon to draw (default: 1)
+  --lastexon LASTEXON   The last exon to draw (default: inf)
 ```
 
 ## Examples
 ### SDHD
 Using the default settings, which does not include non-coding regions of the exon:
 
-`exonviz "NG_012337.3(NM_003002.4):c.274G>T" > SDHD.svg`
+`exonviz SDHD > SDHD.svg`
 
-![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/SDHD.svg)
+![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/SDHD.svg)
 
 ### DMD
-Since DMD has many exons, we specify a maximum width for the figure:
+For DMD, we explicitly specify the transcript we are interested in. We also set
+a maximum width for the figure, since DMD has many exons:
 
-`exonviz "NM_004006.3:c.=" --width 1024 --color purple > DMD.svg`
+`exonviz "NM_004006.3" --width 1024 --color purple --exonnumber > DMD.svg`
 
-![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/DMD.svg)
+![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/DMD.svg)
 
 
 # ATXN1
 Include the non coding exons, since most exons of ATXN1 are non coding. We
 limit the maximum width and increase the height of the picture. For clarity, we
 also increase the distance between the displayed exons:
 
 `exonviz ENST00000436367.6 --noncoding --width 4000 --height 150 --gap 50 > ATXN1.svg`
 
-![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/ATXN1.svg)
+![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/ATXN1.svg)
 
 ### PLP1
+You can also input a valid HGVS description on the transcript of interest. The variant will be ignored.
 Include the non coding regions and increase the height and distance between the exons:
 
-`exonviz "NM_000533.5" --noncoding --height 100 --gap 50 > PLP1.svg`
+`exonviz "NM_000533.5:c.100G>T" --noncoding --height 100 --gap 50 > PLP1.svg`
 
-![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/PLP1.svg)
+![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/PLP1.svg)
 
 ### NF1
 Set the maximum width of the figure to the approximate size of the largest exon:
 
 `exonviz "ENST00000358273.9" --noncoding --width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
 
-![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/NF1-202.svg)
+![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/NF1-202.svg)
```

### Comparing `exonviz-0.1.3/README.md` & `exonviz-0.1.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -14,61 +14,70 @@
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
 
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
 ```
-usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding] [--gap GAP] transcript
+usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding]
+               [--gap GAP] [--color COLOR] [--exonnumber]
+               [--firstexon FIRSTEXON] [--lastexon LASTEXON]
+               transcript
 
 Description of command.
 
 positional arguments:
-  transcript       Transcript (with version) to visualise
+  transcript            Transcript (with version) to visualise
 
 optional arguments:
-  -h, --help       show this help message and exit
-  --width WIDTH    Maximum width of the figure (default: inf)
-  --height HEIGHT  Exon height (default: 20)
-  --noncoding      Show non coding regions (default: False)
-  --gap GAP        Gap between the exons (default: 5)
-  --color COLOR    Color for the exons (e.g. 'purple') (default: #4C72B7)
+  -h, --help            show this help message and exit
+  --width WIDTH         Maximum width of the figure (default: inf)
+  --height HEIGHT       Exon height (default: 20)
+  --noncoding           Show non coding regions (default: False)
+  --gap GAP             Gap between the exons (default: 5)
+  --color COLOR         Color for the exons (e.g. 'purple') (default: #4C72B7)
+  --exonnumber          Show exon number (default: False)
+  --firstexon FIRSTEXON
+                        The first exon to draw (default: 1)
+  --lastexon LASTEXON   The last exon to draw (default: inf)
 ```
 
 ## Examples
 ### SDHD
 Using the default settings, which does not include non-coding regions of the exon:
 
-`exonviz "NG_012337.3(NM_003002.4):c.274G>T" > SDHD.svg`
+`exonviz SDHD > SDHD.svg`
 
-![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/SDHD.svg)
+![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/SDHD.svg)
 
 ### DMD
-Since DMD has many exons, we specify a maximum width for the figure:
+For DMD, we explicitly specify the transcript we are interested in. We also set
+a maximum width for the figure, since DMD has many exons:
 
-`exonviz "NM_004006.3:c.=" --width 1024 --color purple > DMD.svg`
+`exonviz "NM_004006.3" --width 1024 --color purple --exonnumber > DMD.svg`
 
-![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/DMD.svg)
+![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/DMD.svg)
 
 
 # ATXN1
 Include the non coding exons, since most exons of ATXN1 are non coding. We
 limit the maximum width and increase the height of the picture. For clarity, we
 also increase the distance between the displayed exons:
 
 `exonviz ENST00000436367.6 --noncoding --width 4000 --height 150 --gap 50 > ATXN1.svg`
 
-![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/ATXN1.svg)
+![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/ATXN1.svg)
 
 ### PLP1
+You can also input a valid HGVS description on the transcript of interest. The variant will be ignored.
 Include the non coding regions and increase the height and distance between the exons:
 
-`exonviz "NM_000533.5" --noncoding --height 100 --gap 50 > PLP1.svg`
+`exonviz "NM_000533.5:c.100G>T" --noncoding --height 100 --gap 50 > PLP1.svg`
 
-![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/PLP1.svg)
+![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/PLP1.svg)
 
 ### NF1
 Set the maximum width of the figure to the approximate size of the largest exon:
 
 `exonviz "ENST00000358273.9" --noncoding --width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
 
-![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/NF1-202.svg)
+![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/NF1-202.svg)
```

### Comparing `exonviz-0.1.3/setup.py` & `exonviz-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,39 +23,38 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="exonviz",
-    version="0.1.3",
+    version="0.1.4",
     license="AGPL-3.0",
     description="Visualise exons and their reading frames",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Redmar van den Berg",
     author_email="RedmarvandenBerg@lumc.nl",
     url="https://github.com/redmar-van-den-berg/exonviz",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
     include_package_data=True,
     package_data={
-        "exonviz": ["py.typed"]
+        "exonviz": ["py.typed", "data/mane.txt.gz"]
     },
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: Unix",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         # uncomment if you test on these interpreters:
         # 'Programming Language :: Python :: Implementation :: IronPython',
         # 'Programming Language :: Python :: Implementation :: Jython',
         # 'Programming Language :: Python :: Implementation :: Stackless',
@@ -64,15 +63,15 @@
     project_urls={
         "Changelog": "https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md",
         "Issue Tracker": "https://github.com/redmar-van-den-berg/exonviz/issues",
     },
     keywords=[
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     install_requires=[
         "svg.py",
         # eg: 'aspectlib==1.1.1', 'six>=1.7',
     ],
     extras_require={
         # eg:
         #   'rst': ['docutils>=0.11'],
```

### Comparing `exonviz-0.1.3/src/exonviz/cli.py` & `exonviz-0.1.4/src/exonviz/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,35 @@
 Module that contains the command line app, so we can still import __main__
 without executing side effects
 """
 
 import argparse
 import re
 import sys
-import math
+import gzip
+from importlib import resources
 
-from typing import List, Tuple
+from typing import List, Tuple, Dict
 from .draw import draw_exons
 from .exon import Exon
 from .mutalyzer import mutalyzer, extract_exons
 
 from .draw import _config
 
 
+def get_MANE() -> Dict[str, str]:
+    fname = str(resources.files("exonviz.data").joinpath("mane.txt.gz"))
+    with gzip.open(fname, "rt") as fin:
+        mane = dict()
+        for line in fin:
+            gene, transcript = line.strip("\n").split("\t")
+            mane[gene] = transcript
+    return mane
+
+
 def check_input(transcript: str) -> str:
     """Check the input from the user, and rewrite when needed"""
     # If it looks like there is no variant
     if re.match(r"^\w+\.\d+$", transcript):
         return f"{transcript}:c.="
 
     # If it looks like the user forgot the version number, there isn't much we can do
@@ -29,16 +40,22 @@
 
     return transcript
 
 
 def fetch_exons(transcript: str) -> Tuple[List[Exon], bool]:
     """Make or fetch the requested exons"""
 
-    # Does the transcript format make sense?
-    transcript = check_input(transcript)
+    # If the transcript is actually the gene name, substitute the MANE transcript
+    MANE = get_MANE()
+    transcript = MANE.get(transcript, transcript)
+    if transcript in MANE:
+        transcript = MANE[transcript]
+    else:
+        # Does the transcript format make sense?
+        transcript = check_input(transcript)
 
     payload = mutalyzer(transcript)
     if payload:
         return extract_exons(payload)
     else:
         return list(), False
```

### Comparing `exonviz-0.1.3/src/exonviz/draw.py` & `exonviz-0.1.4/src/exonviz/draw.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from typing import List, Union, Tuple, Optional, Any, Dict
 import svg
 from .exon import Exon, Region
 import math
+import textwrap
 
 
 # Options for drawing the figure. Used to create the cli parser and default dict
 _config = [
     ("width", math.inf, "Maximum width of the figure"),
     ("height", 20, "Exon height"),
     ("noncoding", False, "Show non coding regions"),
     ("gap", 5, "Gap between the exons"),
     ("color", "#4C72B7", "Color for the exons (e.g. 'purple')"),
+    ("exonnumber", False, "Show exon number"),
+    ("firstexon", 1, "The first exon to draw"),
+    ("lastexon", math.inf, "The last exon to draw"),
 ]
 
 config = {key: value for key, value, description in _config}
 
 
 def shift(
     points: List[Union[float, int]], x_offset: float, y_offset: float
@@ -25,31 +29,47 @@
 
 def draw_exons(
     exons: List[Exon],
     reverse: bool,
     config: Dict[str, Any],
     scale: int = 1,
 ) -> svg.SVG:
-    elements = list()
+    elements: List[Union[svg.Style, svg.Text]] = list()
 
+    # Set style for exonnumber, even if we don't need it
+    elements.append(
+        svg.Style(
+            text=textwrap.dedent(
+                f"""
+            .exonnr {{ text-anchor: middle; dominant-baseline: central; font: {config["height"]/2}px sans-serif; fill: white;}}
+            """
+            ),
+        )
+    )
     # The maximum width we have reached for this picture
     canvas_width: float = 0
 
     # These values will be updated as we draw the figure
     x_position: float = 10
     y_position: float = 0
 
-    for exon in exons:
+    # Get the first and last exon to draw
+    first = config["firstexon"]
+    last = int(min(config["lastexon"], len(exons)))
+    for i, exon in enumerate(exons[first - 1 : last], start=first):
         # The visual size of the exon depends on wether or not we draw the non-coding
         # regions
         if config["noncoding"]:
             exon_size = exon.size
         else:
             exon_size = exon.coding.size
 
+        # If there is nothing to draw, skip
+        if not exon_size:
+            continue
         # If we overflow the width, go to a new line
         if x_position + exon_size + config["height"] > config["width"] / scale:
             # If we are still at the start position for x, we dont start a new line
             # (this happens when the exon we want to draw is larger than
             # config["width"])
             if x_position == 10:
                 continue
@@ -67,14 +87,24 @@
             section = [x * scale for x in section]
 
             elements.append(
                 svg.Polygon(
                     points=section, stroke="red", fill=config["color"], stroke_width=0  # type: ignore
                 )
             )
+        # Put in the exon number
+        if config["exonnumber"]:
+            elements.append(
+                svg.Text(
+                    x=x_position + (exon_size / 2),
+                    y=y_position + 0.5 * config["height"],
+                    class_=["exonnr"],
+                    text=str(i),
+                )
+            )
         x_position = x_position + exon_size + config["gap"]
         canvas_width = max(x_position, canvas_width)
 
     return svg.SVG(width=canvas_width, height=y_position + config["height"], elements=elements)  # type: ignore
 
 
 def draw_non_coding(region: Region, height: float) -> List[float]:
```

### Comparing `exonviz-0.1.3/src/exonviz/exon.py` & `exonviz-0.1.4/src/exonviz/exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.3/src/exonviz/mutalyzer.py` & `exonviz-0.1.4/src/exonviz/mutalyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     try:
         response = urllib.request.urlopen(url)
     except HTTPError as e:
         msg = f"Fetching '{url}' returned {e}"
         raise RuntimeError(msg)
     else:
         js = json.loads(response.read())
+
+    if "selector_short" not in js:
+        msg = f"No exons found for {variant} (is it a genomic variant?)"
+        raise RuntimeError(msg)
     selector: Dict[str, Any] = js["selector_short"]
     return selector
 
 
 def convert_coding_positions(positions: List[List[str]]) -> Tuple[int, int]:
     start = int(positions[0][0])
     end = int(positions[0][1])
```

### Comparing `exonviz-0.1.3/src/exonviz.egg-info/PKG-INFO` & `exonviz-0.1.4/src/exonviz.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: exonviz
-Version: 0.1.3
+Version: 0.1.4
 Summary: Visualise exons and their reading frames
 Home-page: https://github.com/redmar-van-den-berg/exonviz
 Author: Redmar van den Berg
 Author-email: RedmarvandenBerg@lumc.nl
 License: AGPL-3.0
 Project-URL: Changelog, https://github.com/redmar-van-den-berg/exonviz/blob/main/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/redmar-van-den-berg/exonviz/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Continous integration](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml/badge.svg)](https://github.com/Redmar-van-den-Berg/exonviz/actions/workflows/ci.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
@@ -39,61 +38,70 @@
 ## Usage
 Pass either a transcript (with version!), or a valid HGVS description to exonviz to generate a figure.
 
 ### Options
 Since each gene is different, you will probably want to play around with the options to get the perfect figure for your favorite gene.
 
 ```
-usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding] [--gap GAP] transcript
+usage: exonviz [-h] [--width WIDTH] [--height HEIGHT] [--noncoding]
+               [--gap GAP] [--color COLOR] [--exonnumber]
+               [--firstexon FIRSTEXON] [--lastexon LASTEXON]
+               transcript
 
 Description of command.
 
 positional arguments:
-  transcript       Transcript (with version) to visualise
+  transcript            Transcript (with version) to visualise
 
 optional arguments:
-  -h, --help       show this help message and exit
-  --width WIDTH    Maximum width of the figure (default: inf)
-  --height HEIGHT  Exon height (default: 20)
-  --noncoding      Show non coding regions (default: False)
-  --gap GAP        Gap between the exons (default: 5)
-  --color COLOR    Color for the exons (e.g. 'purple') (default: #4C72B7)
+  -h, --help            show this help message and exit
+  --width WIDTH         Maximum width of the figure (default: inf)
+  --height HEIGHT       Exon height (default: 20)
+  --noncoding           Show non coding regions (default: False)
+  --gap GAP             Gap between the exons (default: 5)
+  --color COLOR         Color for the exons (e.g. 'purple') (default: #4C72B7)
+  --exonnumber          Show exon number (default: False)
+  --firstexon FIRSTEXON
+                        The first exon to draw (default: 1)
+  --lastexon LASTEXON   The last exon to draw (default: inf)
 ```
 
 ## Examples
 ### SDHD
 Using the default settings, which does not include non-coding regions of the exon:
 
-`exonviz "NG_012337.3(NM_003002.4):c.274G>T" > SDHD.svg`
+`exonviz SDHD > SDHD.svg`
 
-![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/SDHD.svg)
+![Figure of SDH exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/SDHD.svg)
 
 ### DMD
-Since DMD has many exons, we specify a maximum width for the figure:
+For DMD, we explicitly specify the transcript we are interested in. We also set
+a maximum width for the figure, since DMD has many exons:
 
-`exonviz "NM_004006.3:c.=" --width 1024 --color purple > DMD.svg`
+`exonviz "NM_004006.3" --width 1024 --color purple --exonnumber > DMD.svg`
 
-![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/DMD.svg)
+![Figure of DMD exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/DMD.svg)
 
 
 # ATXN1
 Include the non coding exons, since most exons of ATXN1 are non coding. We
 limit the maximum width and increase the height of the picture. For clarity, we
 also increase the distance between the displayed exons:
 
 `exonviz ENST00000436367.6 --noncoding --width 4000 --height 150 --gap 50 > ATXN1.svg`
 
-![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/ATXN1.svg)
+![Figure of ATXN1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/ATXN1.svg)
 
 ### PLP1
+You can also input a valid HGVS description on the transcript of interest. The variant will be ignored.
 Include the non coding regions and increase the height and distance between the exons:
 
-`exonviz "NM_000533.5" --noncoding --height 100 --gap 50 > PLP1.svg`
+`exonviz "NM_000533.5:c.100G>T" --noncoding --height 100 --gap 50 > PLP1.svg`
 
-![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/PLP1.svg)
+![Figure of PLP1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/PLP1.svg)
 
 ### NF1
 Set the maximum width of the figure to the approximate size of the largest exon:
 
 `exonviz "ENST00000358273.9" --noncoding --width 3600 --height 75 --gap 20 > examples/NF1-202.svg`
 
-![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/main/examples/NF1-202.svg)
+![Figure of NF1 exons](https://raw.githubusercontent.com/Redmar-van-den-Berg/exonviz/v0.1.4/examples/NF1-202.svg)
```

### Comparing `exonviz-0.1.3/src/exonviz.egg-info/SOURCES.txt` & `exonviz-0.1.4/src/exonviz.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 src/exonviz.egg-info/PKG-INFO
 src/exonviz.egg-info/SOURCES.txt
 src/exonviz.egg-info/dependency_links.txt
 src/exonviz.egg-info/entry_points.txt
 src/exonviz.egg-info/not-zip-safe
 src/exonviz.egg-info/requires.txt
 src/exonviz.egg-info/top_level.txt
+src/exonviz/data/mane.txt.gz
 tests/test_Exon.py
 tests/test_cli.py
 tests/test_draw_exon.py
 tests/test_mutalyzer.py
```

### Comparing `exonviz-0.1.3/tests/test_Exon.py` & `exonviz-0.1.4/tests/test_Exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.3/tests/test_cli.py` & `exonviz-0.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.3/tests/test_draw_exon.py` & `exonviz-0.1.4/tests/test_draw_exon.py`

 * *Files identical despite different names*

### Comparing `exonviz-0.1.3/tests/test_mutalyzer.py` & `exonviz-0.1.4/tests/test_mutalyzer.py`

 * *Files identical despite different names*

