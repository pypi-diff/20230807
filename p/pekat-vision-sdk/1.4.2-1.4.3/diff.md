# Comparing `tmp/pekat_vision_sdk-1.4.2.tar.gz` & `tmp/pekat_vision_sdk-1.4.3.tar.gz`

## Comparing `pekat_vision_sdk-1.4.2.tar` & `pekat_vision_sdk-1.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/PekatVisionSDK/__about__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/PekatVisionSDK/__init__.py
--rw-r--r--   0        0        0    12169 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/PekatVisionSDK/pekat_vision_instance.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/LICENSE
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/README.md
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/PekatVisionSDK/__about__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/PekatVisionSDK/__init__.py
+-rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/PekatVisionSDK/pekat_vision_instance.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/LICENSE
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/README.md
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 pekat_vision_sdk-1.4.3/PKG-INFO
```

### Comparing `pekat_vision_sdk-1.4.2/PekatVisionSDK/pekat_vision_instance.py` & `pekat_vision_sdk-1.4.3/PekatVisionSDK/pekat_vision_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,17 @@
         :type timeout: float
         :return: results of recognition based on response_type
         :rtype: (NDArray[np.uint8], dict) | dict
         """
         image_path = None
         numpy_image = None
 
+        if sys.version_info < (3, 10):
+            StrOrPathLike = (str, os.PathLike)
+
         if isinstance(image, StrOrPathLike):
             image_path = Path(image)
         elif isinstance(image, np.ndarray):
             numpy_image = image
         else:
             raise InvalidData()
```

### Comparing `pekat_vision_sdk-1.4.2/LICENSE` & `pekat_vision_sdk-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.2/README.md` & `pekat_vision_sdk-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.2/pyproject.toml` & `pekat_vision_sdk-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pekat_vision_sdk-1.4.2/PKG-INFO` & `pekat_vision_sdk-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pekat-vision-sdk
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python module for communication with PEKAT VISION
 Project-URL: Homepage, https://github.com/pekat-vision/pekat-vision-sdk-python
 Project-URL: repository, https://github.com/pekat-vision/pekat-vision-sdk-python.git
 Author-email: developers@pekatvision.com
 Maintainer-email: developers@pekatvision.com
 License-Expression: MIT
 License-File: LICENSE
```

