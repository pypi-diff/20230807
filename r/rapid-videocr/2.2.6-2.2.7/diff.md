# Comparing `tmp/rapid_videocr-2.2.6-py3-none-any.whl.zip` & `tmp/rapid_videocr-2.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18580 bytes, number of entries: 12
--rw-r--r--  2.0 unx      174 b- defN 23-Aug-05 10:27 rapid_videocr/__init__.py
--rw-r--r--  2.0 unx      811 b- defN 23-Aug-05 10:27 rapid_videocr/logger.py
--rw-r--r--  2.0 unx    10389 b- defN 23-Aug-05 10:27 rapid_videocr/main.py
--rw-r--r--  2.0 unx    13484 b- defN 23-Aug-05 10:27 rapid_videocr/rapid_videocr.py
--rw-r--r--  2.0 unx     4526 b- defN 23-Aug-05 10:27 rapid_videocr/utils.py
--rw-r--r--  2.0 unx     2996 b- defN 23-Aug-05 10:27 rapid_videocr/video_sub_finder.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     8163 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1014 b- defN 23-Aug-05 10:27 rapid_videocr-2.2.6.dist-info/RECORD
-12 files, 53079 bytes uncompressed, 16868 bytes compressed:  68.2%
+Zip file size: 18591 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      201 b- defN 23-Aug-07 01:20 rapid_videocr/__init__.py
+-rw-r--r--  2.0 unx      811 b- defN 23-Aug-07 01:20 rapid_videocr/logger.py
+-rw-r--r--  2.0 unx    10398 b- defN 23-Aug-07 01:20 rapid_videocr/main.py
+-rw-r--r--  2.0 unx    13484 b- defN 23-Aug-07 01:20 rapid_videocr/rapid_videocr.py
+-rw-r--r--  2.0 unx     4526 b- defN 23-Aug-07 01:20 rapid_videocr/utils.py
+-rw-r--r--  2.0 unx     2996 b- defN 23-Aug-07 01:20 rapid_videocr/video_sub_finder.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8163 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1014 b- defN 23-Aug-07 01:20 rapid_videocr-2.2.7.dist-info/RECORD
+12 files, 53115 bytes uncompressed, 16879 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: rapid_videocr/utils.py
 Comment: 
 
 Filename: rapid_videocr/video_sub_finder.py
 Comment: 
 
-Filename: rapid_videocr-2.2.6.dist-info/LICENSE
+Filename: rapid_videocr-2.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: rapid_videocr-2.2.6.dist-info/METADATA
+Filename: rapid_videocr-2.2.7.dist-info/METADATA
 Comment: 
 
-Filename: rapid_videocr-2.2.6.dist-info/WHEEL
+Filename: rapid_videocr-2.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: rapid_videocr-2.2.6.dist-info/entry_points.txt
+Filename: rapid_videocr-2.2.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.6.dist-info/top_level.txt
+Filename: rapid_videocr-2.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: rapid_videocr-2.2.6.dist-info/RECORD
+Filename: rapid_videocr-2.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rapid_videocr/__init__.py

```diff
@@ -1,5 +1,6 @@
 # -*- encoding: utf-8 -*-
 # @Author: SWHL
 # @Contact: liekkaskono@163.com
+from .logger import logger
 from .main import RapidVideoSubFinderOCR
 from .rapid_videocr import RapidVideOCR, RapidVideOCRError
```

## rapid_videocr/main.py

```diff
@@ -20,15 +20,15 @@
 
 class RapidVideoSubFinderOCR:
     def __init__(
         self,
         is_concat_rec: bool = False,
         concat_batch: int = 10,
         out_format: str = "all",
-        print_console: bool = False,
+        is_print_console: bool = False,
         vsf_exe_path: Optional[str] = None,
         clear_dirs: bool = True,
         run_search: bool = True,
         create_cleared_text_images: bool = True,
         create_empty_sub: Optional[str] = None,
         create_sub_from_cleared_txt_images: Optional[str] = None,
         create_sub_from_txt_results: Optional[str] = None,
@@ -67,15 +67,15 @@
             num_ocr_threads,
         )
 
         self.video_ocr = RapidVideOCR(
             is_concat_rec=is_concat_rec,
             concat_batch=concat_batch,
             out_format=out_format,
-            is_print_console=print_console,
+            is_print_console=is_print_console,
         )
         self.video_formats = [".mp4", ".avi", ".mov", ".mkv"]
 
     def __call__(self, video_path: str, output_dir: str = "outputs"):
         if Path(video_path).is_dir():
             video_list = Path(video_path).rglob("*.*")
             video_list = [
@@ -156,15 +156,15 @@
         "--concat_batch",
         type=int,
         default=10,
         help="The batch of concating image nums in concat recognition mode. Default is 10.",
     )
     videocr_param_group.add_argument(
         "-p",
-        "--print_console",
+        "--is_print_console",
         action="store_true",
         default=False,
         help="Whether to print the subtitle results to console. -p means to print.",
     )
 
     vsf_param_group = parser.add_argument_group(title="VSFParameters")
     vsf_param_group.add_argument(
```

## Comparing `rapid_videocr-2.2.6.dist-info/LICENSE` & `rapid_videocr-2.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rapid_videocr-2.2.6.dist-info/METADATA` & `rapid_videocr-2.2.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapid-videocr
-Version: 2.2.6
+Version: 2.2.7
 Summary: Tool for extracting hard subtitles from videos.
 Home-page: https://github.com/SWHL/RapidVideOCR.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: rapidocr,videocr,subtitle
 Platform: Any
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.6 Summary: Tool for
+Metadata-Version: 2.1 Name: rapid-videocr Version: 2.2.7 Summary: Tool for
 extracting hard subtitles from videos. Home-page: https://github.com/SWHL/
 RapidVideOCR.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: rapidocr,videocr,subtitle Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

