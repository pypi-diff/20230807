# Comparing `tmp/Flask-Beginner-0.0.2.tar.gz` & `tmp/Flask-Beginner-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Beginner-0.0.2.tar", last modified: Sat Aug  5 17:26:41 2023, max compression
+gzip compressed data, was "Flask-Beginner-0.0.3.tar", last modified: Mon Aug  7 13:58:12 2023, max compression
```

## Comparing `Flask-Beginner-0.0.2.tar` & `Flask-Beginner-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 17:26:41.766151 Flask-Beginner-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-08-05 17:26:41.764150 Flask-Beginner-0.0.2/Flask_Beginner.egg-info/
--rw-rw-rw-   0        0        0     2070 2023-08-05 17:26:41.000000 Flask-Beginner-0.0.2/Flask_Beginner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-08-05 17:26:41.000000 Flask-Beginner-0.0.2/Flask_Beginner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 17:26:41.000000 Flask-Beginner-0.0.2/Flask_Beginner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-05 17:26:41.000000 Flask-Beginner-0.0.2/Flask_Beginner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-08-05 17:26:41.000000 Flask-Beginner-0.0.2/Flask_Beginner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-08-05 17:26:41.000000 Flask-Beginner-0.0.2/Flask_Beginner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2070 2023-08-05 17:26:41.766151 Flask-Beginner-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2023-08-05 17:18:45.000000 Flask-Beginner-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 17:26:41.765149 Flask-Beginner-0.0.2/flask_beginner/
--rw-rw-rw-   0        0        0      278 2023-08-05 15:43:39.000000 Flask-Beginner-0.0.2/flask_beginner/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-08-05 17:16:19.000000 Flask-Beginner-0.0.2/flask_beginner/beginner.py
--rw-rw-rw-   0        0        0      712 2023-08-05 17:26:41.767151 Flask-Beginner-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-08-05 15:43:39.000000 Flask-Beginner-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 13:58:12.408977 Flask-Beginner-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-08-07 13:58:12.406976 Flask-Beginner-0.0.3/Flask_Beginner.egg-info/
+-rw-rw-rw-   0        0        0     2412 2023-08-07 13:58:12.000000 Flask-Beginner-0.0.3/Flask_Beginner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-08-07 13:58:12.000000 Flask-Beginner-0.0.3/Flask_Beginner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 13:58:12.000000 Flask-Beginner-0.0.3/Flask_Beginner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-07 13:58:12.000000 Flask-Beginner-0.0.3/Flask_Beginner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-08-07 13:58:12.000000 Flask-Beginner-0.0.3/Flask_Beginner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-07 13:58:12.000000 Flask-Beginner-0.0.3/Flask_Beginner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1062 2023-08-05 15:43:39.000000 Flask-Beginner-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2412 2023-08-07 13:58:12.408977 Flask-Beginner-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1373 2023-08-07 13:53:40.000000 Flask-Beginner-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 13:58:12.407977 Flask-Beginner-0.0.3/flask_beginner/
+-rw-rw-rw-   0        0        0      278 2023-08-05 15:43:39.000000 Flask-Beginner-0.0.3/flask_beginner/__init__.py
+-rw-rw-rw-   0        0        0     1925 2023-08-07 13:42:27.000000 Flask-Beginner-0.0.3/flask_beginner/beginner.py
+-rw-rw-rw-   0        0        0      712 2023-08-07 13:58:12.409977 Flask-Beginner-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-08-05 15:43:39.000000 Flask-Beginner-0.0.3/setup.py
```

### Comparing `Flask-Beginner-0.0.2/Flask_Beginner.egg-info/PKG-INFO` & `Flask-Beginner-0.0.3/Flask_Beginner.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Beginner
-Version: 0.0.2
+Version: 0.0.3
 Summary: a quick project directory maker for flask
 Home-page: https://github.com/r1cardohj/flask-beginner
 Author: r1cardohj
 License: MIT
 Description: # flask-beginner
         
         a quick project directory maker for flask.^_^
@@ -32,31 +32,43 @@
         │  .gitignore
         │  README.md
         │  requirements.txt
         │  test.py
         │  wsgi.py
         │
         └─myapp
+            │  __init__.py
             │  extensions.py
             │  forms.py
             │  models.py
             │  settings.py
             │
             ├─blueprints
             │      __init__.py
             │
             ├─static
             └─templates
+                │  base.html
+                └─errors
+                    │  404.html
+                    │  400.html
+                    │  500.html
         ```
         
         **Version**
         
         v 0.0.1 2023.8.6 create
+        
         v 0.0.2 2023.8.6 add app file `__init__.py`
         
+         V 0.0.3 2023.8.7:
+            
+            1. do not replace the original file
+            2. Code optimization
+        
         ## zh-hans
         
         憋死我了一直写英文。
         
         flask-beginner是用于 ~~偷懒~~ 
         
         是用于创建我自己用的比较顺手的一个flask项目结构，
```

### Comparing `Flask-Beginner-0.0.2/PKG-INFO` & `Flask-Beginner-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Beginner
-Version: 0.0.2
+Version: 0.0.3
 Summary: a quick project directory maker for flask
 Home-page: https://github.com/r1cardohj/flask-beginner
 Author: r1cardohj
 License: MIT
 Description: # flask-beginner
         
         a quick project directory maker for flask.^_^
@@ -32,31 +32,43 @@
         │  .gitignore
         │  README.md
         │  requirements.txt
         │  test.py
         │  wsgi.py
         │
         └─myapp
+            │  __init__.py
             │  extensions.py
             │  forms.py
             │  models.py
             │  settings.py
             │
             ├─blueprints
             │      __init__.py
             │
             ├─static
             └─templates
+                │  base.html
+                └─errors
+                    │  404.html
+                    │  400.html
+                    │  500.html
         ```
         
         **Version**
         
         v 0.0.1 2023.8.6 create
+        
         v 0.0.2 2023.8.6 add app file `__init__.py`
         
+         V 0.0.3 2023.8.7:
+            
+            1. do not replace the original file
+            2. Code optimization
+        
         ## zh-hans
         
         憋死我了一直写英文。
         
         flask-beginner是用于 ~~偷懒~~ 
         
         是用于创建我自己用的比较顺手的一个flask项目结构，
```

### Comparing `Flask-Beginner-0.0.2/README.md` & `Flask-Beginner-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -25,31 +25,43 @@
 │  .gitignore
 │  README.md
 │  requirements.txt
 │  test.py
 │  wsgi.py
 │
 └─myapp
+    │  __init__.py
     │  extensions.py
     │  forms.py
     │  models.py
     │  settings.py
     │
     ├─blueprints
     │      __init__.py
     │
     ├─static
     └─templates
+        │  base.html
+        └─errors
+            │  404.html
+            │  400.html
+            │  500.html
 ```
 
 **Version**
 
 v 0.0.1 2023.8.6 create
+
 v 0.0.2 2023.8.6 add app file `__init__.py`
 
+ V 0.0.3 2023.8.7:
+    
+    1. do not replace the original file
+    2. Code optimization
+
 ## zh-hans
 
 憋死我了一直写英文。
 
 flask-beginner是用于 ~~偷懒~~ 
 
 是用于创建我自己用的比较顺手的一个flask项目结构，
```

### Comparing `Flask-Beginner-0.0.2/setup.cfg` & `Flask-Beginner-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2046 6c61 736b 2d42 6567 696e 6e65   = Flask-Beginne
 00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e30  r..version = 0.0
-00000030: 2e32 0d0a 6175 7468 6f72 203d 2072 3163  .2..author = r1c
+00000030: 2e33 0d0a 6175 7468 6f72 203d 2072 3163  .3..author = r1c
 00000040: 6172 646f 686a 0d0a 6465 7363 7269 7074  ardohj..descript
 00000050: 696f 6e20 3d20 6120 7175 6963 6b20 7072  ion = a quick pr
 00000060: 6f6a 6563 7420 6469 7265 6374 6f72 7920  oject directory 
 00000070: 6d61 6b65 7220 666f 7220 666c 6173 6b0d  maker for flask.
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
 000000a0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
```

