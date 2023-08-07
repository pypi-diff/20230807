# Comparing `tmp/phone_gen-2.3.5.tar.gz` & `tmp/phone_gen-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phone_gen-2.3.5.tar", last modified: Sun Jul 23 14:53:33 2023, max compression
+gzip compressed data, was "phone_gen-2.3.6.tar", last modified: Mon Aug  7 15:34:03 2023, max compression
```

## Comparing `phone_gen-2.3.5.tar` & `phone_gen-2.3.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:53:33.276693 phone_gen-2.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:53:33.272693 phone_gen-2.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:53:33.276693 phone_gen-2.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-23 14:53:20.000000 phone_gen-2.3.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-23 14:53:20.000000 phone_gen-2.3.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-23 14:53:20.000000 phone_gen-2.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-23 14:53:20.000000 phone_gen-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-23 14:53:33.276693 phone_gen-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-23 14:53:20.000000 phone_gen-2.3.5/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-23 14:53:20.000000 phone_gen-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:53:33.276693 phone_gen-2.3.5/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-07-23 14:53:20.000000 phone_gen-2.3.5/dev_tools/patterns_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-23 14:53:20.000000 phone_gen-2.3.5/dev_tools/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:53:33.276693 phone_gen-2.3.5/phone_gen/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-23 14:53:20.000000 phone_gen-2.3.5/phone_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-23 14:53:33.000000 phone_gen-2.3.5/phone_gen/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-23 14:53:20.000000 phone_gen-2.3.5/phone_gen/_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-23 14:53:20.000000 phone_gen-2.3.5/phone_gen/alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-23 14:53:20.000000 phone_gen-2.3.5/phone_gen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-23 14:53:20.000000 phone_gen-2.3.5/phone_gen/country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-07-23 14:53:20.000000 phone_gen-2.3.5/phone_gen/iso3.py
--rw-r--r--   0 runner    (1001) docker     (123)    87940 2023-07-23 14:53:20.000000 phone_gen-2.3.5/phone_gen/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:53:33.276693 phone_gen-2.3.5/phone_gen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-23 14:53:33.000000 phone_gen-2.3.5/phone_gen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-23 14:53:33.000000 phone_gen-2.3.5/phone_gen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 14:53:33.000000 phone_gen-2.3.5/phone_gen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-23 14:53:33.000000 phone_gen-2.3.5/phone_gen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-23 14:53:33.000000 phone_gen-2.3.5/phone_gen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-23 14:53:33.276693 phone_gen-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-23 14:53:20.000000 phone_gen-2.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 14:53:33.276693 phone_gen-2.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-23 14:53:20.000000 phone_gen-2.3.5/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-23 14:53:20.000000 phone_gen-2.3.5/tests/test_alt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-23 14:53:20.000000 phone_gen-2.3.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-23 14:53:20.000000 phone_gen-2.3.5/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-23 14:53:20.000000 phone_gen-2.3.5/tests/test_load_alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-23 14:53:20.000000 phone_gen-2.3.5/tests/test_phone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:34:03.641402 phone_gen-2.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:34:03.637402 phone_gen-2.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:34:03.637402 phone_gen-2.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-07 15:33:52.000000 phone_gen-2.3.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-07 15:33:52.000000 phone_gen-2.3.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-07 15:33:52.000000 phone_gen-2.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-07 15:33:52.000000 phone_gen-2.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-07 15:34:03.641402 phone_gen-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-07 15:33:52.000000 phone_gen-2.3.6/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-08-07 15:33:52.000000 phone_gen-2.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:34:03.641402 phone_gen-2.3.6/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-08-07 15:33:52.000000 phone_gen-2.3.6/dev_tools/patterns_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-07 15:33:52.000000 phone_gen-2.3.6/dev_tools/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:34:03.641402 phone_gen-2.3.6/phone_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-07 15:33:52.000000 phone_gen-2.3.6/phone_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-07 15:34:03.000000 phone_gen-2.3.6/phone_gen/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-08-07 15:33:52.000000 phone_gen-2.3.6/phone_gen/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-07 15:33:52.000000 phone_gen-2.3.6/phone_gen/alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-07 15:33:52.000000 phone_gen-2.3.6/phone_gen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-08-07 15:33:52.000000 phone_gen-2.3.6/phone_gen/country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-08-07 15:33:52.000000 phone_gen-2.3.6/phone_gen/iso3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88003 2023-08-07 15:33:52.000000 phone_gen-2.3.6/phone_gen/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:34:03.641402 phone_gen-2.3.6/phone_gen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-07 15:34:03.000000 phone_gen-2.3.6/phone_gen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-07 15:34:03.000000 phone_gen-2.3.6/phone_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 15:34:03.000000 phone_gen-2.3.6/phone_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-07 15:34:03.000000 phone_gen-2.3.6/phone_gen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-07 15:34:03.000000 phone_gen-2.3.6/phone_gen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-07 15:34:03.641402 phone_gen-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-07 15:33:52.000000 phone_gen-2.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 15:34:03.641402 phone_gen-2.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-07 15:33:52.000000 phone_gen-2.3.6/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-07 15:33:52.000000 phone_gen-2.3.6/tests/test_alt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-07 15:33:52.000000 phone_gen-2.3.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-07 15:33:52.000000 phone_gen-2.3.6/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-07 15:33:52.000000 phone_gen-2.3.6/tests/test_load_alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-08-07 15:33:52.000000 phone_gen-2.3.6/tests/test_phone.py
```

### Comparing `phone_gen-2.3.5/.github/workflows/python-package.yml` & `phone_gen-2.3.6/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.17
+          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.18
           python -m pip install -e .
       - name: Flake8
         run: |
           flake8 phone_gen
       - name: Black
         run: |
           black --check phone_gen
```

### Comparing `phone_gen-2.3.5/.github/workflows/python-publish.yml` & `phone_gen-2.3.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/.gitignore` & `phone_gen-2.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/LICENSE` & `phone_gen-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/PKG-INFO` & `phone_gen-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_gen
-Version: 2.3.5
+Version: 2.3.6
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.3.5/README.md` & `phone_gen-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/dev_tools/patterns_generator.py` & `phone_gen-2.3.6/dev_tools/patterns_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/dev_tools/update.py` & `phone_gen-2.3.6/dev_tools/update.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/phone_gen/__init__.py` & `phone_gen-2.3.6/phone_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/phone_gen/_generator.py` & `phone_gen-2.3.6/phone_gen/_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/phone_gen/alt_patterns.py` & `phone_gen-2.3.6/phone_gen/alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/phone_gen/cli.py` & `phone_gen-2.3.6/phone_gen/cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/phone_gen/country_name.py` & `phone_gen-2.3.6/phone_gen/country_name.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/phone_gen/iso3.py` & `phone_gen-2.3.6/phone_gen/iso3.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/phone_gen/patterns.py` & `phone_gen-2.3.6/phone_gen/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-Auto-generated file 2023-07-23 14:45:42 UTC
-Resource: https://github.com/google/libphonenumber v8.13.17
+Auto-generated file 2023-08-07 15:24:18 UTC
+Resource: https://github.com/google/libphonenumber v8.13.18
 """
 
 
 PATTERNS = {
-    "info": "libphonenumber v8.13.17",
+    "info": "libphonenumber v8.13.18",
     "data": {
         "AC": {
             "code": "247",
             "pattern": "((6[2-467][\\d]{3}))",
             "mobile": "((4[\\d]{4}))",
         },
         "AD": {
@@ -116,16 +116,16 @@
         "BG": {
             "code": "359",
             "pattern": "((2[\\d]{5:7})|((43[1-6])|(70[1-9])[\\d]{4:5})|(([36][\\d])|(4[124-7])|([57][1-9])|(8[1-6])|(9[1-7])[\\d]{5:6}))",
             "mobile": "(((43[07-9])|(99[69][\\d])[\\d]{5})|((8[7-9])|(98)[\\d]{7}))",
         },
         "BH": {
             "code": "973",
-            "pattern": "(((1(3[1356])|(6[0156])|(7[\\d])[\\d])|(6(1[16][\\d])|(500)|(6(0[\\d])|(3[12])|(44)|(7[7-9])|(88))|(9[69][69]))|(7(1(11)|(78))|(7[\\d][\\d]))[\\d]{4}))",
-            "mobile": "(((3([1-79][\\d])|(8[0-47-9])[\\d])|(6(3(00)|(33)|(6[16]))|(6(3[03-9])|([69][\\d])|(7[0-6])))[\\d]{4}))",
+            "pattern": "(((1(3[1356])|(6[0156])|(7[\\d])[\\d])|(6(1[16][\\d])|(500)|(6(0[\\d])|(3[12])|(44)|(7[7-9])|(88))|(9[69][69]))|(7([07][\\d][\\d])|(1(11)|(78)))[\\d]{4}))",
+            "mobile": "(((3([0-79][\\d])|(8[0-57-9])[\\d])|(6(3(00)|(33)|(6[16]))|(441)|(6(3[03-9])|([69][\\d])|(7[0-6])))[\\d]{4}))",
         },
         "BI": {
             "code": "257",
             "pattern": "(((22)|(31)[\\d]{6}))",
             "mobile": "(((29)|([67][125-9])[\\d]{6}))",
         },
         "BJ": {
@@ -252,15 +252,15 @@
             "code": "506",
             "pattern": "((210[7-9][\\d]{4})|(2([024-7][\\d])|(1[1-9])[\\d]{5}))",
             "mobile": "(((3005[\\d])|(6500[01])[\\d]{3})|((5[07])|(6[0-4])|(7[0-3])|(8[3-9])[\\d]{6}))",
         },
         "CU": {
             "code": "53",
             "pattern": "(((3[23])|(4[89])[\\d]{4:6})|((31)|(4[36])|(8(0[25])|(78)[\\d])[\\d]{6})|((2[1-4])|(4[1257])|(7[\\d])[\\d]{5:6}))",
-            "mobile": "((5[\\d]{7}))",
+            "mobile": "(((5[\\d])|(63)[\\d]{6}))",
         },
         "CV": {
             "code": "238",
             "pattern": "((2(2[1-7])|(3[0-8])|(4[12])|(5[1256])|(6[\\d])|(7[1-3])|(8[1-5])[\\d]{4}))",
             "mobile": "(((36)|(5[1-389])|(9[\\d])[\\d]{5}))",
         },
         "CW": {
@@ -392,15 +392,15 @@
             "code": "1",
             "pattern": "((473(2(3[0-2])|(69))|(3(2[89])|(86))|(4([06]8)|(3[5-9])|(4[0-49])|(5[5-79])|(73)|(90))|(63[68])|(7(58)|(84))|(800)|(938)[\\d]{4}))",
             "mobile": "((473(4(0[2-79])|(1[04-9])|(2[0-5])|(58))|(5(2[01])|(3[3-8]))|(901)[\\d]{4}))",
         },
         "GE": {
             "code": "995",
             "pattern": "(((3([256][\\d])|(4[124-9])|(7[0-4]))|(4(1[\\d])|(2[2-7])|(3[1-79])|(4[2-8])|(7[239])|(9[1-7]))[\\d]{6}))",
-            "mobile": "((5(((0555)|(1([17]77)|(555))[5-9])|(757(7[7-9])|(8[01]))[\\d])|(22252[0-4])[\\d][\\d])|((5(00(0[\\d])|(44)|(5[05])|(77)|(88)|(99))|(1(1(00)|([124][\\d])|(3[01]))|(4[\\d][\\d]))|((44)|(68)[\\d][\\d])|(5([0157-9][\\d][\\d])|(200))|(7([0147-9][\\d][\\d])|(5(00)|([57]5)))|(8(0([01][\\d])|(2[0-4]))|(58[89])|(8(55)|(88)))|(9(090)|([1-35-9][\\d][\\d])))|(790[\\d][\\d])[\\d]{4})|(5(0(070)|(505))|(1(0[01]0)|(1(07)|(33)|(51)))|(2(0[02]0)|(2[25]2))|(3(0[03]0)|(3[35]3))|((40[04])|(900)0)|(5222)[0-4][\\d]{3}))",
+            "mobile": "((5(((0555)|(1([17]77)|(555))[5-9])|(757(7[7-9])|(8[01]))[\\d])|(22252[0-4])[\\d][\\d])|((5(00(0[\\d])|(11)|(22)|(33)|(44)|(5[05])|(77)|(88)|(99))|(1(1(00)|([124][\\d])|(3[01]))|(4[\\d][\\d]))|((44)|(68)[\\d][\\d])|(5([0157-9][\\d][\\d])|(200))|(7([0147-9][\\d][\\d])|(5(00)|([57]5)))|(8(0([01][\\d])|(2[0-4]))|(58[89])|(8(55)|(88)))|(9(090)|([1-35-9][\\d][\\d])))|(790[\\d][\\d])[\\d]{4})|(5(0(070)|(505))|(1(0[01]0)|(1(07)|(33)|(51)))|(2(0[02]0)|(2[25]2))|(3(0[03]0)|(3[35]3))|((40[04])|(900)0)|(5222)[0-4][\\d]{3}))",
         },
         "GF": {
             "code": "594",
             "pattern": "((594([02-49][\\d])|([16][0-3])|(5[6-9])|(80)[\\d]{4}))",
             "mobile": "((694([0-249][\\d])|(3[0-8])[\\d]{4}))",
         },
         "GG": {
@@ -416,15 +416,15 @@
         "GI": {
             "code": "350",
             "pattern": "((2190[0-2][\\d]{3})|(2(0([02][\\d])|(3[01]))|(16[24-9])|(2[2-5][\\d])[\\d]{4}))",
             "mobile": "((5251[0-4][\\d]{3})|((5([146-8][\\d][\\d])|(250))|(60(1[01])|(6[\\d]))[\\d]{4}))",
         },
         "GL": {
             "code": "299",
-            "pattern": "(((19)|(3[1-7])|(6[14689])|(70)|(8[14-79])|(9[\\d])[\\d]{4}))",
+            "pattern": "(((19)|(3[1-7])|([68][1-9])|(70)|(9[\\d])[\\d]{4}))",
             "mobile": "(([245][\\d]{5}))",
         },
         "GM": {
             "code": "220",
             "pattern": "(((4([23][\\d][\\d])|(4(1[024679])|([6-9][\\d])))|(5(5(3[\\d])|(4[0-7]))|(6[67][\\d])|(7(1[04])|(2[035])|(3[58])|(48)))|(8[\\d]{3})[\\d]{3}))",
             "mobile": "((([23679][\\d])|(5[0-489])[\\d]{5}))",
         },
@@ -502,15 +502,15 @@
             "code": "353",
             "pattern": "(((1[\\d])|(21)[\\d]{6:7})|((2[24-9])|(4(0[24])|(5[\\d])|(7))|(5(0[45])|(1[\\d])|(8))|(6(1[\\d])|([237-9]))|(9(1[\\d])|([35-9]))[\\d]{5})|((23)|(4([1-469])|(8[\\d]))|(5[23679])|(6[4-6])|(7[14])|(9[04])[\\d]{7}))",
             "mobile": "((8(22)|([35-9][\\d])[\\d]{6}))",
         },
         "IL": {
             "code": "972",
             "pattern": "((153[\\d]{8:9})|(29[1-9][\\d]{5})|((2[0-8])|([3489][\\d])[\\d]{6}))",
-            "mobile": "((55410[\\d]{4})|(5(([02368][\\d])|([19][2-9])|(4[1-9])[\\d])|(5(01)|(1[79])|(2[2-9])|(3[0-3])|(4[34])|(5[015689])|(6[6-8])|(7[0-267])|(8[7-9])|(9[1-9]))[\\d]{5}))",
+            "mobile": "((55410[\\d]{4})|(5(([02368][\\d])|([19][2-9])|(4[1-9])[\\d])|(5(01)|(1[79])|(2[2-9])|(3[0-3])|(4[34])|(5[0-25689])|(6[6-8])|(7[0-267])|(8[7-9])|(9[1-9]))[\\d]{5}))",
         },
         "IM": {
             "code": "44",
             "pattern": "((1624(230)|([5-8][\\d][\\d])[\\d]{3}))",
             "mobile": "((76245[06][\\d]{4})|(7(4576)|([59]24[\\d])|(624[0-4689])[\\d]{5}))",
         },
         "IN": {
@@ -834,15 +834,15 @@
             "code": "683",
             "pattern": "(([47][\\d]{3}))",
             "mobile": "((888[4-9][\\d]{3}))",
         },
         "NZ": {
             "code": "64",
             "pattern": "((24099[\\d]{3})|((3[2-79])|([49][2-9])|(6[235-9])|(7[2-57-9])[\\d]{6}))",
-            "mobile": "((2[0-27-9][\\d]{7:8})|(2(1[\\d])|(75)[\\d]{5}))",
+            "mobile": "((2([0-27-9][\\d])|(6)[\\d]{6:7})|(2(1[\\d])|(75)[\\d]{5}))",
         },
         "OM": {
             "code": "968",
             "pattern": "((2[1-6][\\d]{6}))",
             "mobile": "((1505[\\d]{4})|((7([1289][\\d])|(69)|(7[0-5]))|(9(0[1-9])|([1-9][\\d]))[\\d]{5}))",
         },
         "PA": {
@@ -964,15 +964,15 @@
             "code": "46",
             "pattern": "(((([12][136])|(3[356])|(4[0246])|(6[03])|(8[\\d])[\\d])|(90[1-9])[\\d]{4:6})|((1(2[0-35])|(4[0-4])|(5[0-25-9])|(7[13-6])|([89][\\d]))|(2(2[0-7])|(4[0136-8])|(5[0138])|(7[018])|(8[01])|(9[0-57]))|(3(0[0-4])|(1[\\d])|(2[0-25])|(4[056])|(7[0-2])|(8[0-3])|(9[023]))|(4(1[013-8])|(3[0135])|(5[14-79])|(7[0-246-9])|(8[0156])|(9[0-689]))|(5(0[0-6])|([15][0-5])|(2[0-68])|(3[0-4])|(4[\\d])|(6[03-5])|(7[013])|(8[0-79])|(9[01]))|(6(1[1-3])|(2[0-4])|(4[02-57])|(5[0-37])|(6[0-3])|(7[0-2])|(8[0247])|(9[0-356]))|(9(1[0-68])|(2[\\d])|(3[02-5])|(4[0-3])|(5[0-4])|([68][01])|(7[0135-8]))[\\d]{5:6}))",
             "mobile": "((7[02369][\\d]{7}))",
         },
         "SG": {
             "code": "65",
             "pattern": "((662[0-24-9][\\d]{4})|(6([0-578][\\d])|(6[013-57-9])|(9[0-35-9])[\\d]{5}))",
-            "mobile": "((8(07[01])|(95[0-2])[\\d]{4})|((8(0[1-6])|([1-8][\\d])|(9[0-4]))|(9[0-8][\\d])[\\d]{5}))",
+            "mobile": "((8(08[01])|(95[0-2])[\\d]{4})|((8(0[1-7])|([1-8][\\d])|(9[0-4]))|(9[0-8][\\d])[\\d]{5}))",
         },
         "SH": {
             "code": "290",
             "pattern": "((2([0-57-9][\\d])|(6[4-9])[\\d][\\d]))",
             "mobile": "(([56][\\d]{4}))",
         },
         "SI": {
@@ -1125,30 +1125,30 @@
             "code": "380",
             "pattern": "(((3[1-8])|(4[13-8])|(5[1-7])|(6[12459])[\\d]{7}))",
             "mobile": "(((39)|(50)|(6[36-8])|(7[1-3])|(9[1-9])[\\d]{7}))",
         },
         "UG": {
             "code": "256",
             "pattern": "((20((240)|(30[67])[\\d])|(6(00[0-2])|(30[0-4]))[\\d]{3})|((20([017][\\d])|(2[5-9])|(32)|(5[0-4])|(6[15-9]))|([34][\\d]{3})[\\d]{5}))",
-            "mobile": "((726[01][\\d]{5})|(7([01578][\\d])|(20)|(36)|([46][0-4])|(9[89])[\\d]{6}))",
+            "mobile": "((726[01][\\d]{5})|(7([01578][\\d])|(20)|(36)|(4[0-4])|(6[0-5])|(9[89])[\\d]{6}))",
         },
         "US": {
             "code": "1",
             "pattern": "((5056([0-35-9][\\d])|(4[46])[\\d]{4})|((4722)|(505[2-57-9])[\\d]{6})|((2(0[1-35-9])|(1[02-9])|(2[03-589])|(3[149])|(4[08])|(5[1-46])|(6[0279])|(7[0269])|(8[13]))|(3(0[1-57-9])|(1[02-9])|(2[01356])|(3[0-24679])|(4[167])|(5[0-2])|(6[014])|(8[056]))|(4(0[124-9])|(1[02-579])|(2[3-5])|(3[0245])|(4[023578])|(58)|(6[349])|(7[0589])|(8[04]))|(5(0[1-47-9])|(1[0235-8])|(20)|(3[0149])|(4[01])|(5[179])|(6[1-47])|(7[0-5])|(8[0256]))|(6(0[1-35-9])|(1[024-9])|(2[03689])|([34][016])|(5[01679])|(6[0-279])|(78)|(8[0-29]))|(7(0[1-46-8])|(1[2-9])|(2[04-7])|(3[1247])|(4[037])|(5[47])|(6[02359])|(7[0-59])|(8[156]))|(8(0[1-68])|(1[02-8])|(2[068])|(3[0-2589])|(4[03578])|(5[046-9])|(6[02-5])|(7[028]))|(9(0[1346-9])|(1[02-9])|(2[0589])|(3[0146-8])|(4[01357-9])|(5[12469])|(7[0-389])|(8[04-69]))[2-9][\\d]{6}))",
             "mobile": "((5056([0-35-9][\\d])|(4[46])[\\d]{4})|((4722)|(505[2-57-9])[\\d]{6})|((2(0[1-35-9])|(1[02-9])|(2[03-589])|(3[149])|(4[08])|(5[1-46])|(6[0279])|(7[0269])|(8[13]))|(3(0[1-57-9])|(1[02-9])|(2[01356])|(3[0-24679])|(4[167])|(5[0-2])|(6[014])|(8[056]))|(4(0[124-9])|(1[02-579])|(2[3-5])|(3[0245])|(4[023578])|(58)|(6[349])|(7[0589])|(8[04]))|(5(0[1-47-9])|(1[0235-8])|(20)|(3[0149])|(4[01])|(5[179])|(6[1-47])|(7[0-5])|(8[0256]))|(6(0[1-35-9])|(1[024-9])|(2[03689])|([34][016])|(5[01679])|(6[0-279])|(78)|(8[0-29]))|(7(0[1-46-8])|(1[2-9])|(2[04-7])|(3[1247])|(4[037])|(5[47])|(6[02359])|(7[0-59])|(8[156]))|(8(0[1-68])|(1[02-8])|(2[068])|(3[0-2589])|(4[03578])|(5[046-9])|(6[02-5])|(7[028]))|(9(0[1346-9])|(1[02-9])|(2[0589])|(3[0146-8])|(4[01357-9])|(5[12469])|(7[0-389])|(8[04-69]))[2-9][\\d]{6}))",
         },
         "UY": {
             "code": "598",
             "pattern": "(((1(770)|(987))|((2[\\d])|(4[2-7])[\\d][\\d])[\\d]{4}))",
             "mobile": "((9[1-9][\\d]{6}))",
         },
         "UZ": {
             "code": "998",
             "pattern": "(((55[\\d][\\d])|(6(1(22)|(3[124])|(4[1-4])|(5[1-3578])|(64))|(2(22)|(3[0-57-9])|(41))|(5(22)|(3[3-7])|(5[024-8]))|(6[\\d][\\d])|(7([23][\\d])|(7[69]))|(9(22)|(4[1-8])|(6[135])))|(7(0(5[4-9])|(6[0146])|(7[124-6])|(9[135-8]))|((1[12])|(8[\\d])[\\d])|(2(22)|(3[13-57-9])|(4[1-3579])|(5[14]))|(3(2[\\d])|(3[1578])|(4[1-35-7])|(5[1-57])|(61))|(4(2[\\d])|(3[1-579])|(7[1-79]))|(5(22)|(5[1-9])|(6[1457]))|(6(22)|(3[12457])|(4[13-8]))|(9(22)|(5[1-9])))[\\d]{5}))",
-            "mobile": "((((33)|(50)|(88)|(9[0-57-9])[\\d]{3})|(6(1(2(2[01])|(98))|(35[0-4])|(50[\\d])|(61[23])|(7([01][017])|(4[\\d])|(55)|(9[5-9])))|(2((11)|(7[\\d])[\\d])|(2([12]1)|(9[01379]))|(5([126][\\d])|(3[0-4])))|(5(19[01])|(2(27)|(9[26]))|((30)|(59)|(7[\\d])[\\d]))|(6(2(1[5-9])|(2[0367])|(38)|(41)|(52)|(60))|((3[79])|(9[0-3])[\\d])|(4(56)|(83))|(7([07][\\d])|(1[017])|(3[07])|(4[047])|(5[057])|(67)|(8[0178])|(9[79])))|(7(2(24)|(3[237])|(4[5-9])|(7[15-8]))|(5(7[12])|(8[0589]))|(7(0[\\d])|([39][07]))|(9(0[\\d])|(7[079])))|(9(2(1[1267])|(3[01])|(5[\\d])|(7[0-4]))|((5[67])|(7[\\d])[\\d])|(6(2[0-26])|(8[\\d]))))|(7([07][\\d]{3})|(1(13[01])|(6(0[47])|(1[67])|(66))|(71[3-69])|(98[\\d]))|(2(2(2[79])|(95))|(3(2[5-9])|(6[0-6]))|(57[\\d])|(7(0[\\d])|(1[17])|(2[27])|(3[37])|(44)|(5[057])|(66)|(88)))|(3(2(1[0-6])|(21)|(3[469])|(7[159]))|((33)|(9[4-6])[\\d])|(5(0[0-4])|(5[579])|(9[\\d]))|(7([0-3579][\\d])|(4[0467])|(6[67])|(8[078])))|(4(2(29)|(5[0257])|(6[0-7])|(7[1-57]))|(5(1[0-4])|(8[\\d])|(9[5-9]))|(7(0[\\d])|(1[024589])|(2[0-27])|(3[0137])|([46][07])|(5[01])|(7[5-9])|(9[079]))|(9(7[015-9])|([89][\\d])))|(5(112)|(2(0[\\d])|(2[29])|([49]4))|(3[1568][\\d])|(52[6-9])|(7(0[01578])|(1[017])|([23]7)|(4[047])|([5-7][\\d])|(8[78])|(9[079])))|(6(2(2[1245])|(4[2-4]))|(39[\\d])|(41[179])|(5([349][\\d])|(5[0-2]))|(7(0[017])|([13][\\d])|(22)|(44)|(55)|(67)|(88)))|(9(22[128])|(3(2[0-4])|(7[\\d]))|(57[02569])|(7(2[05-9])|(3[37])|(4[\\d])|(60)|(7[2579])|(87)|(9[07]))))[\\d]{4}))",
+            "mobile": "((((200[01])|((33)|(50)|(88)|(9[0-57-9])[\\d][\\d])[\\d])|(6(1(2(2[01])|(98))|(35[0-4])|(50[\\d])|(61[23])|(7([01][017])|(4[\\d])|(55)|(9[5-9])))|(2((11)|(7[\\d])[\\d])|(2([12]1)|(9[01379]))|(5([126][\\d])|(3[0-4])))|(5(19[01])|(2(27)|(9[26]))|((30)|(59)|(7[\\d])[\\d]))|(6(2(1[5-9])|(2[0367])|(38)|(41)|(52)|(60))|((3[79])|(9[0-3])[\\d])|(4(56)|(83))|(7([07][\\d])|(1[017])|(3[07])|(4[047])|(5[057])|(67)|(8[0178])|(9[79])))|(7(2(24)|(3[237])|(4[5-9])|(7[15-8]))|(5(7[12])|(8[0589]))|(7(0[\\d])|([39][07]))|(9(0[\\d])|(7[079])))|(9(2(1[1267])|(3[01])|(5[\\d])|(7[0-4]))|((5[67])|(7[\\d])[\\d])|(6(2[0-26])|(8[\\d]))))|(7([07][\\d]{3})|(1(13[01])|(6(0[47])|(1[67])|(66))|(71[3-69])|(98[\\d]))|(2(2(2[79])|(95))|(3(2[5-9])|(6[0-6]))|(57[\\d])|(7(0[\\d])|(1[17])|(2[27])|(3[37])|(44)|(5[057])|(66)|(88)))|(3(2(1[0-6])|(21)|(3[469])|(7[159]))|((33)|(9[4-6])[\\d])|(5(0[0-4])|(5[579])|(9[\\d]))|(7([0-3579][\\d])|(4[0467])|(6[67])|(8[078])))|(4(2(29)|(5[0257])|(6[0-7])|(7[1-57]))|(5(1[0-4])|(8[\\d])|(9[5-9]))|(7(0[\\d])|(1[024589])|(2[0-27])|(3[0137])|([46][07])|(5[01])|(7[5-9])|(9[079]))|(9(7[015-9])|([89][\\d])))|(5(112)|(2(0[\\d])|(2[29])|([49]4))|(3[1568][\\d])|(52[6-9])|(7(0[01578])|(1[017])|([23]7)|(4[047])|([5-7][\\d])|(8[78])|(9[079])))|(6(2(2[1245])|(4[2-4]))|(39[\\d])|(41[179])|(5([349][\\d])|(5[0-2]))|(7(0[017])|([13][\\d])|(22)|(44)|(55)|(67)|(88)))|(9(22[128])|(3(2[0-4])|(7[\\d]))|(57[02569])|(7(2[05-9])|(3[37])|(4[\\d])|(60)|(7[2579])|(87)|(9[07]))))[\\d]{4}))",
         },
         "VA": {
             "code": "39",
             "pattern": "((06698[\\d]{1:6}))",
             "mobile": "((3[1-9][\\d]{8})|(3[2-9][\\d]{7}))",
         },
         "VC": {
```

### Comparing `phone_gen-2.3.5/phone_gen.egg-info/PKG-INFO` & `phone_gen-2.3.6/phone_gen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone-gen
-Version: 2.3.5
+Version: 2.3.6
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.3.5/phone_gen.egg-info/SOURCES.txt` & `phone_gen-2.3.6/phone_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/setup.py` & `phone_gen-2.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/tests/test_alt_pattern.py` & `phone_gen-2.3.6/tests/test_alt_pattern.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/tests/test_cli.py` & `phone_gen-2.3.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/tests/test_generator.py` & `phone_gen-2.3.6/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/tests/test_load_alt_patterns.py` & `phone_gen-2.3.6/tests/test_load_alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.5/tests/test_phone.py` & `phone_gen-2.3.6/tests/test_phone.py`

 * *Files identical despite different names*

