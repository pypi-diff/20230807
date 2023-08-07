# Comparing `tmp/gamey-0.3.tar.gz` & `tmp/gamey-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamey-0.3.tar", max compression
+gzip compressed data, was "gamey-0.3.1.tar", max compression
```

## Comparing `gamey-0.3.tar` & `gamey-0.3.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       51 2023-08-06 19:53:31.483350 gamey-0.3/README.md
--rw-r--r--   0        0        0     1287 2023-08-07 10:24:26.563342 gamey-0.3/gamey/__init__.py
--rw-r--r--   0        0        0      307 2023-08-07 10:25:03.276677 gamey-0.3/pyproject.toml
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 gamey-0.3/PKG-INFO
+-rw-r--r--   0        0        0       51 2023-08-06 19:53:31.483350 gamey-0.3.1/README.md
+-rw-r--r--   0        0        0     1327 2023-08-07 10:25:39.146677 gamey-0.3.1/gamey/__init__.py
+-rw-r--r--   0        0        0      309 2023-08-07 10:25:58.696678 gamey-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 gamey-0.3.1/PKG-INFO
```

### Comparing `gamey-0.3/gamey/__init__.py` & `gamey-0.3.1/gamey/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -53,9 +53,11 @@
 
 	def __init__(self, image_path, x=0, y=0):
 		self.image = p.image.load(image_path)
 		self.x = x
 		self.y = y
 		last_window.sprites.append(self)
 
-	def set_size(self, width, height):
+	def set_size(self, width, height=None):
+		if not height:
+			height = width
 		self.image = p.transform.scale(self.image, (width, height))
```

### Comparing `gamey-0.3/PKG-INFO` & `gamey-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamey
-Version: 0.3
+Version: 0.3.1
 Summary: An simple, powerful game engine built on pygame
 Author: Dylan Rogers
 Author-email: opendylan@proton.me
 Requires-Python: >=3,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

