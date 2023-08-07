# Comparing `tmp/AnkiChinese-1.1.0.tar.gz` & `tmp/AnkiChinese-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnkiChinese-1.1.0.tar", last modified: Sat Aug  5 21:13:58 2023, max compression
+gzip compressed data, was "AnkiChinese-1.3.0.tar", last modified: Mon Aug  7 19:17:32 2023, max compression
```

## Comparing `AnkiChinese-1.1.0.tar` & `AnkiChinese-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 21:13:58.254444 AnkiChinese-1.1.0/
--rw-rw-rw-   0        0        0     1086 2023-08-05 21:12:48.000000 AnkiChinese-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2142 2023-08-05 21:13:58.254444 AnkiChinese-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-08-05 21:12:48.000000 AnkiChinese-1.1.0/README.md
--rw-rw-rw-   0        0        0       88 2023-08-05 21:12:48.000000 AnkiChinese-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      870 2023-08-05 21:13:58.256439 AnkiChinese-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 21:13:58.218617 AnkiChinese-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 21:13:58.250455 AnkiChinese-1.1.0/src/AnkiChinese.egg-info/
--rw-rw-rw-   0        0        0     2142 2023-08-05 21:13:58.000000 AnkiChinese-1.1.0/src/AnkiChinese.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-08-05 21:13:58.000000 AnkiChinese-1.1.0/src/AnkiChinese.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 21:13:58.000000 AnkiChinese-1.1.0/src/AnkiChinese.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-05 21:13:58.000000 AnkiChinese-1.1.0/src/AnkiChinese.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-08-05 21:13:58.000000 AnkiChinese-1.1.0/src/AnkiChinese.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-05 21:13:58.000000 AnkiChinese-1.1.0/src/AnkiChinese.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 21:13:58.253446 AnkiChinese-1.1.0/src/scrape/
--rw-rw-rw-   0        0        0        0 2023-08-05 20:55:38.000000 AnkiChinese-1.1.0/src/scrape/__init__.py
--rw-rw-rw-   0        0        0     4229 2023-08-05 21:12:15.000000 AnkiChinese-1.1.0/src/scrape/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.364717 AnkiChinese-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.364717 AnkiChinese-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.384719 AnkiChinese-1.3.0/card_template/
+-rw-r--r--   0 runner    (1001) docker     (123) 17321876 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/card_template/CNstrokeorder-0.0.4.7.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/card_template/back.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/card_template/front.html
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/card_template/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/input.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.364717 AnkiChinese-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-07 19:17:32.000000 AnkiChinese-1.3.0/src/AnkiChinese.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:32.388720 AnkiChinese-1.3.0/src/scrape/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/src/scrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/src/scrape/scrape_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-08-07 19:17:18.000000 AnkiChinese-1.3.0/src/scrape/scraper.py
```

### Comparing `AnkiChinese-1.1.0/LICENSE.txt` & `AnkiChinese-1.3.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Luke Tao
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Luke Tao
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `AnkiChinese-1.1.0/PKG-INFO` & `AnkiChinese-1.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,72 @@
-Metadata-Version: 2.1
-Name: AnkiChinese
-Version: 1.1.0
-Summary: An ArchChinese scraper for Anki
-Home-page: https://github.com/autoelk/AnkiChinese
-Author: Luke Tao
-Author-email: luketao68@gmail.com
-Project-URL: Bug Tracker, https://github.com/autoelk/AnkiChinese/issues
-Project-URL: repository, https://github.com/autoelk/AnkiChinese
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# AnkiChinese
-
-This program scrapes the ArchChinese dictionary to generate Anki flashcards.
-
-## 1. Installation
-
-    pip install ankichinese
-
-## 2. Usage
-
-    ankichinese
-
-    -i, --input                 Input file (default: input.txt)
-    -o, --output                Output file (default: output.csv)
-    -d, --numDefs               Number of definitions to include (default: 5)
-    -e, --numExamples           Number of examples to include (default: 3)
-MIT License
-
-Copyright (c) 2023 Luke Tao
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Metadata-Version: 2.1
+Name: AnkiChinese
+Version: 1.3.0
+Summary: An ArchChinese scraper for Anki
+Home-page: https://github.com/autoelk/AnkiChinese
+Author: Luke Tao
+Author-email: luketao68@gmail.com
+Project-URL: Repository, https://github.com/autoelk/AnkiChinese
+Project-URL: Bug Tracker, https://github.com/autoelk/AnkiChinese/issues
+Project-URL: Changelog, https://github.com/autoelk/AnkiChinese/releases
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# AnkiChinese
+
+Scrape the ArchChinese dictionary to generate Anki flashcards with:
+1. Pinyin & Audio
+2. Definitions
+3. Common examples
+4. Stroke order diagrams
+5. HSK level
+
+## 1. Installation
+
+    pip install ankichinese
+
+## 2. Usage
+
+    ankichinese
+
+    -h, --help                  Show help message and exit 
+
+    --input, -i INPUT           Input file with characters to scrape (default: input.txt)
+    --output, -o OUTPUT         Name of output file (do not include extension) 
+                                (default: ankichinese_output)
+    --type, -t {anki,csv}       Output file type (default: anki)
+
+    --defs, -d NUM              Number of definitions to scrape per character (default: 5)
+    --examples, -e NUM          Number of example words to scrape per character (default: 3)
+
+## Credits
+Online stroke order diagrams: https://hanziwriter.org/
+Offline stroke order font: https://rtega.be/chmn/index.php?subpage=68
+
+Chinese audio:
+1. https://yoyochinese.com/chinese-learning-tools/Mandarin-Chinese-pronunciation-lesson/pinyin-chart-table
+2. https://www.purpleculture.net/chinese_pinyin_chart/
+MIT License
+
+Copyright (c) 2023 Luke Tao
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `AnkiChinese-1.1.0/setup.cfg` & `AnkiChinese-1.3.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2041 6e6b 6943 6869 6e65 7365 0d0a   = AnkiChinese..
-00000020: 7665 7273 696f 6e20 3d20 312e 312e 300d  version = 1.1.0.
-00000030: 0a61 7574 686f 7220 3d20 4c75 6b65 2054  .author = Luke T
-00000040: 616f 0d0a 6175 7468 6f72 5f65 6d61 696c  ao..author_email
-00000050: 203d 206c 756b 6574 616f 3638 4067 6d61   = luketao68@gma
-00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
-00000070: 696f 6e20 3d20 416e 2041 7263 6843 6869  ion = An ArchChi
-00000080: 6e65 7365 2073 6372 6170 6572 2066 6f72  nese scraper for
-00000090: 2041 6e6b 690d 0a6c 6f6e 675f 6465 7363   Anki..long_desc
-000000a0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-000000b0: 5245 4144 4d45 2e6d 642c 204c 4943 454e  README.md, LICEN
-000000c0: 5345 2e74 7874 0d0a 6c6f 6e67 5f64 6573  SE.txt..long_des
-000000d0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-000000e0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-000000f0: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000110: 6175 746f 656c 6b2f 416e 6b69 4368 696e  autoelk/AnkiChin
-00000120: 6573 650d 0a70 726f 6a65 6374 5f75 726c  ese..project_url
-00000130: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000140: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-00000150: 6875 622e 636f 6d2f 6175 746f 656c 6b2f  hub.com/autoelk/
-00000160: 416e 6b69 4368 696e 6573 652f 6973 7375  AnkiChinese/issu
-00000170: 6573 0d0a 0972 6570 6f73 6974 6f72 7920  es...repository 
-00000180: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000190: 2e63 6f6d 2f61 7574 6f65 6c6b 2f41 6e6b  .com/autoelk/Ank
-000001a0: 6943 6869 6e65 7365 0d0a 636c 6173 7369  iChinese..classi
-000001b0: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
-000001c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-000001e0: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-000001f0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-00000200: 4c69 6365 6e73 650d 0a09 4f70 6572 6174  License...Operat
-00000210: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000220: 2049 6e64 6570 656e 6465 6e74 0d0a 0d0a   Independent....
-00000230: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-00000240: 6765 5f64 6972 203d 200d 0a09 3d20 7372  ge_dir = ...= sr
-00000250: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
-00000260: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
-00000270: 6972 6573 203d 203e 3d33 2e38 0d0a 696e  ires = >=3.8..in
-00000280: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000290: 200d 0a09 6273 340d 0a09 6c78 6d6c 0d0a   ...bs4...lxml..
-000002a0: 0961 696f 6d65 7465 720d 0a09 706c 6179  .aiometer...play
-000002b0: 7772 6967 6874 0d0a 0970 616e 6461 730d  wright...pandas.
-000002c0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000002d0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-000002e0: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
-000002f0: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
-00000300: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
-00000310: 7473 203d 200d 0a09 616e 6b69 6368 696e  ts = ...ankichin
-00000320: 6573 6520 3d20 7363 7261 7065 2e73 6372  ese = scrape.scr
-00000330: 6170 6572 3a63 6c69 0d0a 0d0a 5b65 6767  aper:cli....[egg
-00000340: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000350: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000360: 2030 0d0a 0d0a                            0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 416e 6b69 4368 696e 6573 650a 6175  = AnkiChinese.au
+00000020: 7468 6f72 203d 204c 756b 6520 5461 6f0a  thor = Luke Tao.
+00000030: 6175 7468 6f72 5f65 6d61 696c 203d 206c  author_email = l
+00000040: 756b 6574 616f 3638 4067 6d61 696c 2e63  uketao68@gmail.c
+00000050: 6f6d 0a64 6573 6372 6970 7469 6f6e 203d  om.description =
+00000060: 2041 6e20 4172 6368 4368 696e 6573 6520   An ArchChinese 
+00000070: 7363 7261 7065 7220 666f 7220 416e 6b69  scraper for Anki
+00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000090: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000a0: 2e6d 642c 204c 4943 454e 5345 2e74 7874  .md, LICENSE.txt
+000000b0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000c0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+000000d0: 2074 6578 742f 6d61 726b 646f 776e 0a75   text/markdown.u
+000000e0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+000000f0: 6875 622e 636f 6d2f 6175 746f 656c 6b2f  hub.com/autoelk/
+00000100: 416e 6b69 4368 696e 6573 650a 7072 6f6a  AnkiChinese.proj
+00000110: 6563 745f 7572 6c73 203d 200a 0952 6570  ect_urls = ..Rep
+00000120: 6f73 6974 6f72 7920 3d20 6874 7470 733a  ository = https:
+00000130: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7574  //github.com/aut
+00000140: 6f65 6c6b 2f41 6e6b 6943 6869 6e65 7365  oelk/AnkiChinese
+00000150: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
+00000160: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000170: 6f6d 2f61 7574 6f65 6c6b 2f41 6e6b 6943  om/autoelk/AnkiC
+00000180: 6869 6e65 7365 2f69 7373 7565 730a 0943  hinese/issues..C
+00000190: 6861 6e67 656c 6f67 203d 2068 7474 7073  hangelog = https
+000001a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6175  ://github.com/au
+000001b0: 746f 656c 6b2f 416e 6b69 4368 696e 6573  toelk/AnkiChines
+000001c0: 652f 7265 6c65 6173 6573 0a63 6c61 7373  e/releases.class
+000001d0: 6966 6965 7273 203d 200a 0950 726f 6772  ifiers = ..Progr
+000001e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0a09  :: Python :: 3..
+00000200: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000210: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000220: 6963 656e 7365 0a09 4f70 6572 6174 696e  icense..Operatin
+00000230: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000240: 6e64 6570 656e 6465 6e74 0a0a 5b6f 7074  ndependent..[opt
+00000250: 696f 6e73 5d0a 7061 636b 6167 655f 6469  ions].package_di
+00000260: 7220 3d20 0a09 3d20 7372 630a 7061 636b  r = ..= src.pack
+00000270: 6167 6573 203d 2066 696e 643a 0a70 7974  ages = find:.pyt
+00000280: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000290: 3d33 2e38 0a69 6e73 7461 6c6c 5f72 6571  =3.8.install_req
+000002a0: 7569 7265 7320 3d20 0a09 6273 340a 0968  uires = ..bs4..h
+000002b0: 746d 6c35 6c69 620a 0961 696f 6d65 7465  tml5lib..aiomete
+000002c0: 720a 0970 6c61 7977 7269 6768 740a 0970  r..playwright..p
+000002d0: 616e 6461 730a 0967 656e 616e 6b69 0a09  andas..genanki..
+000002e0: 7471 646d 0a0a 5b6f 7074 696f 6e73 2e70  tqdm..[options.p
+000002f0: 6163 6b61 6765 732e 6669 6e64 5d0a 7768  ackages.find].wh
+00000300: 6572 6520 3d20 7372 630a 0a5b 6f70 7469  ere = src..[opti
+00000310: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
+00000320: 5d0a 636f 6e73 6f6c 655f 7363 7269 7074  ].console_script
+00000330: 7320 3d20 0a09 616e 6b69 6368 696e 6573  s = ..ankichines
+00000340: 6520 3d20 7363 7261 7065 2e73 6372 6170  e = scrape.scrap
+00000350: 6572 3a63 6c69 0a0a 5b65 6767 5f69 6e66  er:cli..[egg_inf
+00000360: 6f5d 0a74 6167 5f62 7569 6c64 203d 200a  o].tag_build = .
+00000370: 7461 675f 6461 7465 203d 2030 0a0a       tag_date = 0..
```

### Comparing `AnkiChinese-1.1.0/src/AnkiChinese.egg-info/PKG-INFO` & `AnkiChinese-1.3.0/src/AnkiChinese.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,72 @@
-Metadata-Version: 2.1
-Name: AnkiChinese
-Version: 1.1.0
-Summary: An ArchChinese scraper for Anki
-Home-page: https://github.com/autoelk/AnkiChinese
-Author: Luke Tao
-Author-email: luketao68@gmail.com
-Project-URL: Bug Tracker, https://github.com/autoelk/AnkiChinese/issues
-Project-URL: repository, https://github.com/autoelk/AnkiChinese
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# AnkiChinese
-
-This program scrapes the ArchChinese dictionary to generate Anki flashcards.
-
-## 1. Installation
-
-    pip install ankichinese
-
-## 2. Usage
-
-    ankichinese
-
-    -i, --input                 Input file (default: input.txt)
-    -o, --output                Output file (default: output.csv)
-    -d, --numDefs               Number of definitions to include (default: 5)
-    -e, --numExamples           Number of examples to include (default: 3)
-MIT License
-
-Copyright (c) 2023 Luke Tao
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Metadata-Version: 2.1
+Name: AnkiChinese
+Version: 1.3.0
+Summary: An ArchChinese scraper for Anki
+Home-page: https://github.com/autoelk/AnkiChinese
+Author: Luke Tao
+Author-email: luketao68@gmail.com
+Project-URL: Repository, https://github.com/autoelk/AnkiChinese
+Project-URL: Bug Tracker, https://github.com/autoelk/AnkiChinese/issues
+Project-URL: Changelog, https://github.com/autoelk/AnkiChinese/releases
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# AnkiChinese
+
+Scrape the ArchChinese dictionary to generate Anki flashcards with:
+1. Pinyin & Audio
+2. Definitions
+3. Common examples
+4. Stroke order diagrams
+5. HSK level
+
+## 1. Installation
+
+    pip install ankichinese
+
+## 2. Usage
+
+    ankichinese
+
+    -h, --help                  Show help message and exit 
+
+    --input, -i INPUT           Input file with characters to scrape (default: input.txt)
+    --output, -o OUTPUT         Name of output file (do not include extension) 
+                                (default: ankichinese_output)
+    --type, -t {anki,csv}       Output file type (default: anki)
+
+    --defs, -d NUM              Number of definitions to scrape per character (default: 5)
+    --examples, -e NUM          Number of example words to scrape per character (default: 3)
+
+## Credits
+Online stroke order diagrams: https://hanziwriter.org/
+Offline stroke order font: https://rtega.be/chmn/index.php?subpage=68
+
+Chinese audio:
+1. https://yoyochinese.com/chinese-learning-tools/Mandarin-Chinese-pronunciation-lesson/pinyin-chart-table
+2. https://www.purpleculture.net/chinese_pinyin_chart/
+MIT License
+
+Copyright (c) 2023 Luke Tao
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

