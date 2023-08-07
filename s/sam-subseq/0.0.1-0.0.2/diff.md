# Comparing `tmp/sam_subseq-0.0.1.tar.gz` & `tmp/sam_subseq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_subseq-0.0.1.tar", last modified: Thu Jun  8 16:12:34 2023, max compression
+gzip compressed data, was "sam_subseq-0.0.2.tar", last modified: Mon Aug  7 11:59:20 2023, max compression
```

## Comparing `sam_subseq-0.0.1.tar` & `sam_subseq-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-06-08 16:12:34.127262 sam_subseq-0.0.1/
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     1056 2023-06-08 15:02:58.000000 sam_subseq-0.0.1/LICENSE
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     6823 2023-06-08 16:12:34.127262 sam_subseq-0.0.1/PKG-INFO
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     6377 2023-06-08 16:07:51.000000 sam_subseq-0.0.1/README.md
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)      602 2023-06-08 15:48:53.000000 sam_subseq-0.0.1/pyproject.toml
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)       38 2023-06-08 16:12:34.127262 sam_subseq-0.0.1/setup.cfg
-drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-06-08 16:12:34.127262 sam_subseq-0.0.1/src/
-drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-06-08 16:12:34.127262 sam_subseq-0.0.1/src/sam_subseq/
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     8088 2023-05-29 22:08:48.000000 sam_subseq-0.0.1/src/sam_subseq/IndexMap.py
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     1547 2023-05-29 20:41:39.000000 sam_subseq-0.0.1/src/sam_subseq/SamRefAlignment.py
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)        0 2023-05-31 19:58:07.000000 sam_subseq-0.0.1/src/sam_subseq/__init__.py
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     3922 2023-06-01 13:04:14.000000 sam_subseq-0.0.1/src/sam_subseq/io.py
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     5270 2023-06-08 15:17:55.000000 sam_subseq-0.0.1/src/sam_subseq/main.py
-drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-06-08 16:12:34.127262 sam_subseq-0.0.1/src/sam_subseq.egg-info/
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     6823 2023-06-08 16:12:34.000000 sam_subseq-0.0.1/src/sam_subseq.egg-info/PKG-INFO
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)      428 2023-06-08 16:12:34.000000 sam_subseq-0.0.1/src/sam_subseq.egg-info/SOURCES.txt
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)        1 2023-06-08 16:12:34.000000 sam_subseq-0.0.1/src/sam_subseq.egg-info/dependency_links.txt
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)       60 2023-06-08 16:12:34.000000 sam_subseq-0.0.1/src/sam_subseq.egg-info/entry_points.txt
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)       11 2023-06-08 16:12:34.000000 sam_subseq-0.0.1/src/sam_subseq.egg-info/top_level.txt
-drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-06-08 16:12:34.127262 sam_subseq-0.0.1/tests/
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     2825 2023-05-29 22:11:41.000000 sam_subseq-0.0.1/tests/test_index_map.py
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)      705 2023-06-08 15:36:58.000000 sam_subseq-0.0.1/tests/test_main.py
--rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     3194 2023-05-29 21:59:43.000000 sam_subseq-0.0.1/tests/test_ref_alignment.py
+drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-08-07 11:59:20.294048 sam_subseq-0.0.2/
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     1056 2023-06-08 15:02:58.000000 sam_subseq-0.0.2/LICENSE
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     6853 2023-08-07 11:59:20.294048 sam_subseq-0.0.2/PKG-INFO
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     6385 2023-08-07 11:38:25.000000 sam_subseq-0.0.2/README.md
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)      627 2023-08-07 11:47:25.000000 sam_subseq-0.0.2/pyproject.toml
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)       38 2023-08-07 11:59:20.294048 sam_subseq-0.0.2/setup.cfg
+drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-08-07 11:59:20.294048 sam_subseq-0.0.2/src/
+drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-08-07 11:59:20.294048 sam_subseq-0.0.2/src/sam_subseq/
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     8088 2023-05-29 22:08:48.000000 sam_subseq-0.0.2/src/sam_subseq/IndexMap.py
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     1547 2023-05-29 20:41:39.000000 sam_subseq-0.0.2/src/sam_subseq/SamRefAlignment.py
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)        0 2023-05-31 19:58:07.000000 sam_subseq-0.0.2/src/sam_subseq/__init__.py
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     3922 2023-06-01 13:04:14.000000 sam_subseq-0.0.2/src/sam_subseq/io.py
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     5278 2023-08-07 11:35:46.000000 sam_subseq-0.0.2/src/sam_subseq/main.py
+drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-08-07 11:59:20.294048 sam_subseq-0.0.2/src/sam_subseq.egg-info/
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     6853 2023-08-07 11:59:20.000000 sam_subseq-0.0.2/src/sam_subseq.egg-info/PKG-INFO
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)      428 2023-08-07 11:59:20.000000 sam_subseq-0.0.2/src/sam_subseq.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)        1 2023-08-07 11:59:20.000000 sam_subseq-0.0.2/src/sam_subseq.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)       60 2023-08-07 11:59:20.000000 sam_subseq-0.0.2/src/sam_subseq.egg-info/entry_points.txt
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)       11 2023-08-07 11:59:20.000000 sam_subseq-0.0.2/src/sam_subseq.egg-info/top_level.txt
+drwxrwxr-x   0 thomaso   (1001) thomaso   (1001)        0 2023-08-07 11:59:20.294048 sam_subseq-0.0.2/tests/
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     2825 2023-05-29 22:11:41.000000 sam_subseq-0.0.2/tests/test_index_map.py
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)      705 2023-06-08 15:36:58.000000 sam_subseq-0.0.2/tests/test_main.py
+-rw-rw-r--   0 thomaso   (1001) thomaso   (1001)     3194 2023-05-29 21:59:43.000000 sam_subseq-0.0.2/tests/test_ref_alignment.py
```

### Comparing `sam_subseq-0.0.1/LICENSE` & `sam_subseq-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_subseq-0.0.1/PKG-INFO` & `sam_subseq-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sam_subseq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extract subsequences corresponding to annotated reference features from aligned reads in a SAM file
 Author-email: Oliver Thomas <thomaso@ie-freiburg.mpg.de>
 Project-URL: Repository, https://www.github.com/osthomas/sam_subseq
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sam_subseq - Extract GFF Features From Aligned Reads
 
 `sam_subseq` takes two inputs:
 
@@ -47,15 +48,15 @@
              80        180        290
                        |---CDS----|
              |----exon------------|
 REF:  -------------------------------
 QRY:         xxxxxxxxxxyyyyyyy--z
 
 The reference has an exon annotation from position 80-290.
-Extracting this feature from the query will yield: xxxxxxxxxx
+Extracting this feature from the query will yield: xxxxxxxxxxyyyyyyyz
 The CDS in the query shows a deletion and is incompletely represented.
 Extracting the CDS from 180-290 will yield yyyyyyyz.
 
 Some information from the gff file is written into the header of each
 output sequence. Coordinates conform to Python conventions, ie.
 zero-based and end-exclusive.
 
@@ -125,15 +126,15 @@
 **GFF input**
 ```
 ##gff-version 3
 ##sequence-region ref1 1 67
 ref1	.	gene	1	67	.	+	.	ID=ref1
 ref1	.	exon	10	62	.	+	.	ID=ref1:exon;=ref1-exon;Parent=ref1
 ref1	.	CDS	20	62	.	+	0	ID=ref1:CDS;Name=ref1-cds;Parent=ref1
-##sequence-region ref1 1 67
+##sequence-region ref2 1 67
 ref2	.	gene	1	67	.	+	.	ID=ref2
 ref2	.	exon	10	62	.	+	.	ID=ref2:exon;=ref2-exon;Parent=ref2
 ref2	.	CDS	20	62	.	+	0	ID=ref2:CDS;Name=ref2-cds;Parent=ref2
 ```
 
 
 **FASTA output**
```

### Comparing `sam_subseq-0.0.1/README.md` & `sam_subseq-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
              80        180        290
                        |---CDS----|
              |----exon------------|
 REF:  -------------------------------
 QRY:         xxxxxxxxxxyyyyyyy--z
 
 The reference has an exon annotation from position 80-290.
-Extracting this feature from the query will yield: xxxxxxxxxx
+Extracting this feature from the query will yield: xxxxxxxxxxyyyyyyyz
 The CDS in the query shows a deletion and is incompletely represented.
 Extracting the CDS from 180-290 will yield yyyyyyyz.
 
 Some information from the gff file is written into the header of each
 output sequence. Coordinates conform to Python conventions, ie.
 zero-based and end-exclusive.
 
@@ -114,15 +114,15 @@
 **GFF input**
 ```
 ##gff-version 3
 ##sequence-region ref1 1 67
 ref1	.	gene	1	67	.	+	.	ID=ref1
 ref1	.	exon	10	62	.	+	.	ID=ref1:exon;=ref1-exon;Parent=ref1
 ref1	.	CDS	20	62	.	+	0	ID=ref1:CDS;Name=ref1-cds;Parent=ref1
-##sequence-region ref1 1 67
+##sequence-region ref2 1 67
 ref2	.	gene	1	67	.	+	.	ID=ref2
 ref2	.	exon	10	62	.	+	.	ID=ref2:exon;=ref2-exon;Parent=ref2
 ref2	.	CDS	20	62	.	+	0	ID=ref2:CDS;Name=ref2-cds;Parent=ref2
 ```
 
 
 **FASTA output**
```

### Comparing `sam_subseq-0.0.1/src/sam_subseq/IndexMap.py` & `sam_subseq-0.0.2/src/sam_subseq/IndexMap.py`

 * *Files identical despite different names*

### Comparing `sam_subseq-0.0.1/src/sam_subseq/SamRefAlignment.py` & `sam_subseq-0.0.2/src/sam_subseq/SamRefAlignment.py`

 * *Files identical despite different names*

### Comparing `sam_subseq-0.0.1/src/sam_subseq/io.py` & `sam_subseq-0.0.2/src/sam_subseq/io.py`

 * *Files identical despite different names*

### Comparing `sam_subseq-0.0.1/src/sam_subseq/main.py` & `sam_subseq-0.0.2/src/sam_subseq/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                      80        180        290
                                |---CDS----|
                      |----exon------------|
         REF:  -------------------------------
         QRY:         xxxxxxxxxxyyyyyyy--z
 
         The reference has an exon annotation from position 80-290.
-        Extracting this feature from the query will yield: xxxxxxxxxx
+        Extracting this feature from the query will yield: xxxxxxxxxxyyyyyyyz
         The CDS in the query shows a deletion and is incompletely represented.
         Extracting the CDS from 180-290 will yield yyyyyyyz.
 
         Some information from the gff file is written into the header of each
         output sequence. Coordinates conform to Python conventions, ie.
         zero-based and end-exclusive.
```

### Comparing `sam_subseq-0.0.1/src/sam_subseq.egg-info/PKG-INFO` & `sam_subseq-0.0.2/src/sam_subseq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sam-subseq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Extract subsequences corresponding to annotated reference features from aligned reads in a SAM file
 Author-email: Oliver Thomas <thomaso@ie-freiburg.mpg.de>
 Project-URL: Repository, https://www.github.com/osthomas/sam_subseq
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+Requires-Python: >3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sam_subseq - Extract GFF Features From Aligned Reads
 
 `sam_subseq` takes two inputs:
 
@@ -47,15 +48,15 @@
              80        180        290
                        |---CDS----|
              |----exon------------|
 REF:  -------------------------------
 QRY:         xxxxxxxxxxyyyyyyy--z
 
 The reference has an exon annotation from position 80-290.
-Extracting this feature from the query will yield: xxxxxxxxxx
+Extracting this feature from the query will yield: xxxxxxxxxxyyyyyyyz
 The CDS in the query shows a deletion and is incompletely represented.
 Extracting the CDS from 180-290 will yield yyyyyyyz.
 
 Some information from the gff file is written into the header of each
 output sequence. Coordinates conform to Python conventions, ie.
 zero-based and end-exclusive.
 
@@ -125,15 +126,15 @@
 **GFF input**
 ```
 ##gff-version 3
 ##sequence-region ref1 1 67
 ref1	.	gene	1	67	.	+	.	ID=ref1
 ref1	.	exon	10	62	.	+	.	ID=ref1:exon;=ref1-exon;Parent=ref1
 ref1	.	CDS	20	62	.	+	0	ID=ref1:CDS;Name=ref1-cds;Parent=ref1
-##sequence-region ref1 1 67
+##sequence-region ref2 1 67
 ref2	.	gene	1	67	.	+	.	ID=ref2
 ref2	.	exon	10	62	.	+	.	ID=ref2:exon;=ref2-exon;Parent=ref2
 ref2	.	CDS	20	62	.	+	0	ID=ref2:CDS;Name=ref2-cds;Parent=ref2
 ```
 
 
 **FASTA output**
```

### Comparing `sam_subseq-0.0.1/tests/test_index_map.py` & `sam_subseq-0.0.2/tests/test_index_map.py`

 * *Files identical despite different names*

### Comparing `sam_subseq-0.0.1/tests/test_main.py` & `sam_subseq-0.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `sam_subseq-0.0.1/tests/test_ref_alignment.py` & `sam_subseq-0.0.2/tests/test_ref_alignment.py`

 * *Files identical despite different names*

