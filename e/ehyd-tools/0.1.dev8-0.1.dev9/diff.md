# Comparing `tmp/ehyd_tools-0.1.dev8-py3-none-any.whl.zip` & `tmp/ehyd_tools-0.1.dev9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 16192 bytes, number of entries: 14
+Zip file size: 16189 bytes, number of entries: 14
 -rwxrwxrwx  2.0 unx        0 b- defN 20-Apr-05 19:25 ehyd_tools/__init__.py
 -rwxrwxrwx  2.0 unx      272 b- defN 20-Apr-05 19:25 ehyd_tools/__main__.py
 -rwxrwxrwx  2.0 unx     2833 b- defN 20-Apr-18 08:44 ehyd_tools/arg_parser.py
 -rwxrwxrwx  2.0 unx     7829 b- defN 20-Apr-18 10:40 ehyd_tools/cl_tool.py
 -rwxrwxrwx  2.0 unx     6344 b- defN 20-Apr-18 10:32 ehyd_tools/data_processing.py
 -rwxrwxrwx  2.0 unx     4925 b- defN 20-Apr-14 05:46 ehyd_tools/deprecated.py
--rwxrwxrwx  2.0 unx     7876 b- defN 20-Apr-18 11:15 ehyd_tools/in_out.py
+-rwxrwxrwx  2.0 unx     7858 b- defN 20-Apr-23 19:46 ehyd_tools/in_out.py
 -rwxrwxrwx  2.0 unx     2838 b- defN 20-Apr-05 19:25 ehyd_tools/sww_utils.py
--rwxrwxrwx  2.0 unx      292 b- defN 20-Apr-18 11:17 ehyd_tools-0.1.dev8.data/scripts/ehyd_tools
--rwxrwxrwx  2.0 unx     1063 b- defN 20-Apr-18 11:17 ehyd_tools-0.1.dev8.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     5196 b- defN 20-Apr-18 11:17 ehyd_tools-0.1.dev8.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 20-Apr-18 11:17 ehyd_tools-0.1.dev8.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       11 b- defN 20-Apr-18 11:17 ehyd_tools-0.1.dev8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1152 b- defN 20-Apr-18 11:17 ehyd_tools-0.1.dev8.dist-info/RECORD
-14 files, 40723 bytes uncompressed, 14272 bytes compressed:  65.0%
+-rwxrwxrwx  2.0 unx      292 b- defN 20-Apr-24 13:09 ehyd_tools-0.1.dev9.data/scripts/ehyd_tools
+-rwxrwxrwx  2.0 unx     1063 b- defN 20-Apr-24 13:09 ehyd_tools-0.1.dev9.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx     5219 b- defN 20-Apr-24 13:09 ehyd_tools-0.1.dev9.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 20-Apr-24 13:09 ehyd_tools-0.1.dev9.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       11 b- defN 20-Apr-24 13:09 ehyd_tools-0.1.dev9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1152 b- defN 20-Apr-24 13:09 ehyd_tools-0.1.dev9.dist-info/RECORD
+14 files, 40728 bytes uncompressed, 14269 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: ehyd_tools/in_out.py
 Comment: 
 
 Filename: ehyd_tools/sww_utils.py
 Comment: 
 
-Filename: ehyd_tools-0.1.dev8.data/scripts/ehyd_tools
+Filename: ehyd_tools-0.1.dev9.data/scripts/ehyd_tools
 Comment: 
 
-Filename: ehyd_tools-0.1.dev8.dist-info/LICENSE
+Filename: ehyd_tools-0.1.dev9.dist-info/LICENSE
 Comment: 
 
-Filename: ehyd_tools-0.1.dev8.dist-info/METADATA
+Filename: ehyd_tools-0.1.dev9.dist-info/METADATA
 Comment: 
 
-Filename: ehyd_tools-0.1.dev8.dist-info/WHEEL
+Filename: ehyd_tools-0.1.dev9.dist-info/WHEEL
 Comment: 
 
-Filename: ehyd_tools-0.1.dev8.dist-info/top_level.txt
+Filename: ehyd_tools-0.1.dev9.dist-info/top_level.txt
 Comment: 
 
-Filename: ehyd_tools-0.1.dev8.dist-info/RECORD
+Filename: ehyd_tools-0.1.dev9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ehyd_tools/in_out.py

```diff
@@ -77,15 +77,15 @@
     """
     fn = path.join(check_path(export_path), '{}.{}'.format(filename, save_as))
 
     if save_as == 'csv':
         series.to_csv(fn, **csv_args(unix))
 
     elif save_as == 'parquet':
-        series.to_frame().to_parquet(fn, compression=None)
+        series.to_frame().to_parquet(fn)
 
     else:
         raise NotImplementedError('Sorry, but only csv files are implemented. Maybe there will be more options soon.')
 
     return fn
```

## Comparing `ehyd_tools-0.1.dev8.dist-info/LICENSE` & `ehyd_tools-0.1.dev9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ehyd_tools-0.1.dev8.dist-info/METADATA` & `ehyd_tools-0.1.dev9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehyd-tools
-Version: 0.1.dev8
+Version: 0.1.dev9
 Summary: Various tools for exporting and analyzing >10a rain time-series from the "ehyd.gv.at" platform of the Austian government.
 Home-page: https://github.com/MarkusPic/ehyd_tools
 Author: Markus Pichler
 Author-email: markus.pichler@tugraz.at
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.14)
 Requires-Dist: pandas (>=1)
 Requires-Dist: matplotlib (>=3)
 Requires-Dist: requests
 Requires-Dist: fastparquet
+Requires-Dist: pyarrow
 
 © [Institute of Urban Water Management and Landscape Water Engineering](https://www.tugraz.at), [Graz University of Technology](https://www.tugraz.at/home/) and [Markus Pichler](mailto:markus.pichler@tugraz.at)
 
 # eHYD Tools
 
 [![license](https://img.shields.io/github/license/markuspic/ehyd_tools.svg?style=flat)](https://github.com/MarkusPic/ehyd_tools/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/ehyd_tools.svg)](https://pypi.python.org/pypi/ehyd-tools)
```

## Comparing `ehyd_tools-0.1.dev8.dist-info/RECORD` & `ehyd_tools-0.1.dev9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ehyd_tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ehyd_tools/__main__.py,sha256=bqAERisUZuCh4JtV6rjnHlPOUUY62tfVUnS7skkzKjY,272
 ehyd_tools/arg_parser.py,sha256=9CvHg0tTdzJW3SOWS5iFGxO9mPpV_0WHIEVaZ0tcH_M,2833
 ehyd_tools/cl_tool.py,sha256=OBdYO0dmqWJ_KyE7kdaFAe0mBoh3uJpxvr8w_dSatf0,7829
 ehyd_tools/data_processing.py,sha256=0rP5E12M3qxTxYxs4cQXyMzwLYRUqLQz3VOlxvSQJKc,6344
 ehyd_tools/deprecated.py,sha256=u2zlMxYVONok5r3o1kIAioPXuLi3dhwKYa1PVm81I3k,4925
-ehyd_tools/in_out.py,sha256=0rR_nedu8_H8-1w-GBDIUSrmvmRNogg8EXtpy0FW7AM,7876
+ehyd_tools/in_out.py,sha256=JO-tvOZZNsGZ2qEbajQg74GFHK51xCWE0qmOfYm0gCw,7858
 ehyd_tools/sww_utils.py,sha256=A_z39yqjOLAo_RZ8CFN0DPxXBTaBX1zopMkSOmrNREc,2838
-ehyd_tools-0.1.dev8.data/scripts/ehyd_tools,sha256=JdhWruVeN96FMPvqJ5HxZpxoVDUquT0SMs7aOx9LmWg,292
-ehyd_tools-0.1.dev8.dist-info/LICENSE,sha256=Gb7p8qLfOkyeIr3EwWdid6hms_Gk-_58Lg2Uu1Q9B10,1063
-ehyd_tools-0.1.dev8.dist-info/METADATA,sha256=E_TQ96znfonU-9ZgYCdcYre8S8b9blq--owWRV_E2cY,5196
-ehyd_tools-0.1.dev8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-ehyd_tools-0.1.dev8.dist-info/top_level.txt,sha256=8KQnVfDnNEoEhSBWS5YRwRBrlrPgukg3EaWEZo1If4A,11
-ehyd_tools-0.1.dev8.dist-info/RECORD,,
+ehyd_tools-0.1.dev9.data/scripts/ehyd_tools,sha256=JdhWruVeN96FMPvqJ5HxZpxoVDUquT0SMs7aOx9LmWg,292
+ehyd_tools-0.1.dev9.dist-info/LICENSE,sha256=Gb7p8qLfOkyeIr3EwWdid6hms_Gk-_58Lg2Uu1Q9B10,1063
+ehyd_tools-0.1.dev9.dist-info/METADATA,sha256=xvq2o5Zzoy4ZfgY5yw5CYpJ4lLmso0opsZbY6-iE6g0,5219
+ehyd_tools-0.1.dev9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+ehyd_tools-0.1.dev9.dist-info/top_level.txt,sha256=8KQnVfDnNEoEhSBWS5YRwRBrlrPgukg3EaWEZo1If4A,11
+ehyd_tools-0.1.dev9.dist-info/RECORD,,
```

