# Comparing `tmp/MyOverlay-0.2.5.tar.gz` & `tmp/MyOverlay-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.2.5.tar", last modified: Mon Aug  7 08:48:34 2023, max compression
+gzip compressed data, was "MyOverlay-0.2.6.tar", last modified: Mon Aug  7 09:08:48 2023, max compression
```

## Comparing `MyOverlay-0.2.5.tar` & `MyOverlay-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 08:48:34.057386 MyOverlay-0.2.5/
--rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      745 2023-08-07 08:48:34.057386 MyOverlay-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.2.5/README.md
--rw-rw-rw-   0        0        0      649 2023-08-07 08:48:19.000000 MyOverlay-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-07 08:48:34.057386 MyOverlay-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-07 08:48:34.027386 MyOverlay-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-08-07 08:48:34.042385 MyOverlay-0.2.5/src/MyOverlay/
--rw-rw-rw-   0        0        0      489 2023-08-07 07:50:27.000000 MyOverlay-0.2.5/src/MyOverlay/Overlay.py
--rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.2.5/src/MyOverlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:48:34.056385 MyOverlay-0.2.5/src/MyOverlay/funcs/
--rw-rw-rw-   0        0        0     5203 2023-08-07 08:48:08.000000 MyOverlay-0.2.5/src/MyOverlay/funcs/myfunctions.py
--rw-rw-rw-   0        0        0        0 2023-08-07 06:43:53.000000 MyOverlay-0.2.5/src/MyOverlay/funcs/test.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:48:34.054385 MyOverlay-0.2.5/src/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      745 2023-08-07 08:48:34.000000 MyOverlay-0.2.5/src/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-08-07 08:48:34.000000 MyOverlay-0.2.5/src/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 08:48:34.000000 MyOverlay-0.2.5/src/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-07 08:48:34.000000 MyOverlay-0.2.5/src/MyOverlay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 09:08:48.553411 MyOverlay-0.2.6/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-08-07 09:08:48.553411 MyOverlay-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.2.6/README.md
+-rw-rw-rw-   0        0        0      649 2023-08-07 09:08:29.000000 MyOverlay-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-07 09:08:48.553411 MyOverlay-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-07 09:08:48.523575 MyOverlay-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-08-07 09:08:48.538572 MyOverlay-0.2.6/src/MyOverlay/
+-rw-rw-rw-   0        0        0      489 2023-08-07 07:50:27.000000 MyOverlay-0.2.6/src/MyOverlay/Overlay.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.2.6/src/MyOverlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:08:48.552351 MyOverlay-0.2.6/src/MyOverlay/funcs/
+-rw-rw-rw-   0        0        0     5278 2023-08-07 09:08:24.000000 MyOverlay-0.2.6/src/MyOverlay/funcs/myfunctions.py
+-rw-rw-rw-   0        0        0        0 2023-08-07 06:43:53.000000 MyOverlay-0.2.6/src/MyOverlay/funcs/test.py
+drwxrwxrwx   0        0        0        0 2023-08-07 09:08:48.550388 MyOverlay-0.2.6/src/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-07 09:08:48.000000 MyOverlay-0.2.6/src/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-08-07 09:08:48.000000 MyOverlay-0.2.6/src/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 09:08:48.000000 MyOverlay-0.2.6/src/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-07 09:08:48.000000 MyOverlay-0.2.6/src/MyOverlay.egg-info/top_level.txt
```

### Comparing `MyOverlay-0.2.5/LICENSE` & `MyOverlay-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MyOverlay-0.2.5/PKG-INFO` & `MyOverlay-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.2.5
+Version: 0.2.6
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MyOverlay-0.2.5/pyproject.toml` & `MyOverlay-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "MyOverlay"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Erik Reimann", email="erikreimann28@gmail.com" },
 ]
 description = "Customized Text Only Screen Overlay"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `MyOverlay-0.2.5/src/MyOverlay/funcs/myfunctions.py` & `MyOverlay-0.2.6/src/MyOverlay/funcs/myfunctions.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         return True
     else:
         return False
 
 
 def settext(text: str, PosX: int, PosY: int, font: str = 'Segoe UI Semibold', size: int = 30, opx: int = 2):
     if pygame.display.get_active():
+        pygame.event.pump()
         font = pygame.font.SysFont(font, size, False)
         screen.fill(fuchsia)  # Transparent background
         lines = str(text).splitlines()
         for i, l in enumerate(lines):
             screen.blit(render(l, font, opx), (PosX // 2, PosY // 2 + size * i))
         pygame.display.update()
 
@@ -159,7 +160,10 @@
             return 'train train'
         case 'Trucking':
             return 'trucking trucking'
         case 'PostOP':
             return 'trucking postop'
     return None
 
+
+StartOverlay()
+print(pygame.event.pump())
```

### Comparing `MyOverlay-0.2.5/src/MyOverlay.egg-info/PKG-INFO` & `MyOverlay-0.2.6/src/MyOverlay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.2.5
+Version: 0.2.6
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

