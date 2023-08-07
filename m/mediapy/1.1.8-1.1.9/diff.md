# Comparing `tmp/mediapy-1.1.8.tar.gz` & `tmp/mediapy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediapy-1.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mediapy-1.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mediapy-1.1.8.tar` & `mediapy-1.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11358 2023-06-28 10:26:55.361774 mediapy-1.1.8/LICENSE
--rw-r--r--   0        0        0     3738 2023-06-28 10:26:55.361774 mediapy-1.1.8/README.md
--rw-r--r--   0        0        0    68015 2023-06-28 10:26:55.361774 mediapy-1.1.8/mediapy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 10:26:55.361774 mediapy-1.1.8/mediapy/py.typed
--rw-r--r--   0        0        0     2243 2023-06-28 10:26:55.373774 mediapy-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 mediapy-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-07 16:49:45.735440 mediapy-1.1.9/LICENSE
+-rw-r--r--   0        0        0     3738 2023-08-07 16:49:45.735440 mediapy-1.1.9/README.md
+-rw-r--r--   0        0        0    68136 2023-08-07 16:49:45.735440 mediapy-1.1.9/mediapy/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 16:49:45.735440 mediapy-1.1.9/mediapy/py.typed
+-rw-r--r--   0        0        0     2243 2023-08-07 16:49:45.743440 mediapy-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 mediapy-1.1.9/PKG-INFO
```

### Comparing `mediapy-1.1.8/LICENSE` & `mediapy-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mediapy-1.1.8/README.md` & `mediapy-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mediapy-1.1.8/mediapy/__init__.py` & `mediapy-1.1.9/mediapy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
       w.add_image(darken_image(image))
 ```
 """
 
 from __future__ import annotations
 
 __docformat__ = 'google'
-__version__ = '1.1.8'
+__version__ = '1.1.9'
 __version_info__ = tuple(int(num) for num in __version__.split('.'))
 
 import base64
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 import contextlib
 import functools
 import importlib
@@ -1213,15 +1213,15 @@
       'null',
       '-',
   ]
   with subprocess.Popen(
       command, stderr=subprocess.PIPE, encoding='utf-8'
   ) as proc:
     _, err = proc.communicate()
-  bps = num_images = width = rotation = None
+  bps = fps = num_images = width = height = rotation = None
   for line in err.split('\n'):
     if match := re.search(r', bitrate: *([0-9.]+) kb/s', line):
       bps = int(match.group(1)) * 1000
     if matches := re.findall(r'frame= *([0-9]+) ', line):
       num_images = int(matches[-1])
     if 'Stream #0:' in line and ': Video:' in line:
       if not (match := re.search(r', ([0-9]+)x([0-9]+)', line)):
@@ -1230,15 +1230,18 @@
       if match := re.search(r', ([0-9.]+) fps', line):
         fps = float(match.group(1))
       elif str(path).endswith('.gif'):
         # Some GIF files lack a framerate attribute; use a reasonable default.
         fps = 10
       else:
         raise RuntimeError(f'Unable to parse video framerate in line {line}')
-    if match := re.fullmatch(r'\s*rotate\s*:\s*(\d+)', line):
+    if (
+        (match := re.fullmatch(r'\s*rotate\s*:\s*(\d+)', line)) or
+        (match := re.fullmatch(r'\s*.*rotation of -?(\d+)\s*.*\sdegrees', line))
+        ):
       rotation = int(match.group(1))
   if not num_images:
     raise RuntimeError(f'Unable to find frames in video: {err}')
   if not width:
     raise RuntimeError(f'Unable to parse video header: {err}')
   # By default, ffmpeg enables "-autorotate"; we just fix the dimensions.
   if rotation in (90, 270):
```

### Comparing `mediapy-1.1.8/pyproject.toml` & `mediapy-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mediapy-1.1.8/PKG-INFO` & `mediapy-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediapy
-Version: 1.1.8
+Version: 1.1.9
 Summary: Read/write/show images and videos in an IPython notebook
 Keywords: 
 Author-email: Google LLC <mediapy-owners@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

