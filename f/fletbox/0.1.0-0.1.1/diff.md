# Comparing `tmp/fletbox-0.1.0.tar.gz` & `tmp/fletbox-0.1.1.tar.gz`

## Comparing `fletbox-0.1.0.tar` & `fletbox-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fletbox-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 fletbox-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 fletbox-0.1.0/src/fletbox/__init__.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 fletbox-0.1.0/src/fletbox/fletbox.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fletbox-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fletbox-0.1.0/LICENSE
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 fletbox-0.1.0/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fletbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 fletbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fletbox-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 fletbox-0.1.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 fletbox-0.1.1/src/fletbox/__init__.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 fletbox-0.1.1/src/fletbox/fletbox.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fletbox-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 fletbox-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 fletbox-0.1.1/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 fletbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 fletbox-0.1.1/PKG-INFO
```

### Comparing `fletbox-0.1.0/.github/workflows/python-package.yml` & `fletbox-0.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `fletbox-0.1.0/src/fletbox/fletbox.py` & `fletbox-0.1.1/src/fletbox/fletbox.py`

 * *Files identical despite different names*

### Comparing `fletbox-0.1.0/LICENSE` & `fletbox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fletbox-0.1.0/README.md` & `fletbox-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,84 @@
 # FletBox <img src=https://openclipart.org/download/183014 height=45 align=top>
 A box for flet, abusing contextmanagers and decorators.
 
-FletBox is a wrapper around [flet](https://flet.dev/), handling the routing & syntax for you.
+FletBox is a gradio/nicegui style wrapper around [flet](https://flet.dev/), handling the routing & syntax for you.
 
 ## Usage
 
 ### Installation
 ```
 pip install fletbox
 ```
 
-### General Example
+### Import
 ```python
 import flet as ft
 from fletbox import FletBox, Builder, Factory
+```
 
-#pass normal ft.app kwargs to FletBox, can also be set (eg. fb.port=8000)
-fb = FletBox()
+### Initialization
+*NOTE: you can pass normal ft.app kwargs to FletBox.*
+```python
+fb = FletBox(view=ft.AppView.WEB_BROWSER)
+```
+kwargs can also be set via edict.
+```python
+fb.kwargs.port = 8550
+```
 
-#fletbox decorator for routing, use page.go(YOUR_ROUTE_HERE) for traveling between views
+### Main Block, decorators and routing
+The view routing is handled in the background.
+
+This decorator is used for routing, and all decorated views take two inputs, page and builder.
+```python
 @fb.view("/")
 def test(page: ft.Page, builder: Builder) -> Builder:
-    #builder.layout is contextmanagers, remap via layout=builder.layout
-    with builder.layout.Container(expand=True, margin=-10, gradient=page.standard_gradient):
-        #can also do with YOUR_X as YOUR_Y: since control is yielded in contextmanager
-        with builder.layout.Row() as row:
-            row.controls.append(ft.ElevatedButton("FletBox"))
-            #builder attrs for creating deepest control
-            builder.ElevatedButton("FletBox")
-            #assign if modification/reads are required
-            textfield = builder.TextField(label="FletBox", text_size=20)
-    #returning builder is optional
-    return builder
+# returning builder is optional (will replace generated builder if returned).
+```
+
+EXTRA: the standard page.go function can be used for traveling between routes.
+```python
+page.go("/")
+```
+
+### Main Block, contextmanagers (with statements)
+The syntax is drastically altered from the standard flet library.
+
+```python
+@fb.view("/")
+def test(page: ft.Page, builder: Builder) -> None:
+    #builder.layout is contextmanagers. TIP: remap via layout=builder.layout
+    with builder.layout.Container(expand=True, margin=-10, gradient=page.standard_gradient): #can used stored attributes using "page" as a shared storage
+        with builder.layout.Row() as row: #can be assigned, or not
+            row.controls.append(ft.ElevatedButton("FletBox")) #see above
+            builder.ElevatedButton("FletBox") #IMPORTANT: root builder attrs are used for creating deepest control (not layout)
+            textfield = builder.TextField(label="FletBox", text_size=20) #can be assigned, or not - for modification/reads
+
+    @builder.postexec #OPTIONAL: postexec decorator - run function after view load
+    def postfunc():
+        pass #YOUR_POST_FUNCTION_HERE
 
 #can define whatever non-view-specific thing you want, passing target is optional
 def shared_methods(page: ft.Page):
     page.fonts = {
         "Raleway": "assets/Raleway[wght].ttf"
     }
-    page.theme = ft.Theme(color_scheme_seed="pink", visual_density="COMFORTABLE", font_family="Raleway", use_material3=False)
+    page.theme = ft.Theme(color_scheme_seed="pink", visual_density="COMFORTABLE", font_family="Raleway")
     page.standard_gradient = ft.LinearGradient(begin=ft.alignment.bottom_left, end=ft.alignment.top_right, colors=["#F7C35A", "#FBAFAB"])
+```
 
-#pass normal ft.app kwargs to fb.app, can also be set (eg. fb.port=8000)
+And finally we run the application.
+*NOTE: you can pass normal ft.app kwargs to fb.app.*
+```python
+#pass normal ft.app kwargs to fb.app
 fb.app(target=shared_methods)
 ```
+
+## Other Usage
 ### Custom Elements
 ```python
 import flet as ft
 from fletbox import FletBox, Builder, Factory
 
 #module with custom components
 import flet_material as fm
```

### Comparing `fletbox-0.1.0/pyproject.toml` & `fletbox-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fletbox"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Xynon", email="" },
 ]
 description = "A box for flet, abusing contextmanagers and decorators"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fletbox-0.1.0/PKG-INFO` & `fletbox-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fletbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: A box for flet, abusing contextmanagers and decorators
 Project-URL: Homepage, https://github.com/Xynonners/fletbox
 Project-URL: Bug Tracker, https://github.com/Xynonners/fletbox/issues
 Author: Xynon
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,57 +15,88 @@
 Requires-Dist: flet
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # FletBox <img src=https://openclipart.org/download/183014 height=45 align=top>
 A box for flet, abusing contextmanagers and decorators.
 
-FletBox is a wrapper around [flet](https://flet.dev/), handling the routing & syntax for you.
+FletBox is a gradio/nicegui style wrapper around [flet](https://flet.dev/), handling the routing & syntax for you.
 
 ## Usage
 
 ### Installation
 ```
 pip install fletbox
 ```
 
-### General Example
+### Import
 ```python
 import flet as ft
 from fletbox import FletBox, Builder, Factory
+```
 
-#pass normal ft.app kwargs to FletBox, can also be set (eg. fb.port=8000)
-fb = FletBox()
+### Initialization
+*NOTE: you can pass normal ft.app kwargs to FletBox.*
+```python
+fb = FletBox(view=ft.AppView.WEB_BROWSER)
+```
+kwargs can also be set via edict.
+```python
+fb.kwargs.port = 8550
+```
 
-#fletbox decorator for routing, use page.go(YOUR_ROUTE_HERE) for traveling between views
+### Main Block, decorators and routing
+The view routing is handled in the background.
+
+This decorator is used for routing, and all decorated views take two inputs, page and builder.
+```python
 @fb.view("/")
 def test(page: ft.Page, builder: Builder) -> Builder:
-    #builder.layout is contextmanagers, remap via layout=builder.layout
-    with builder.layout.Container(expand=True, margin=-10, gradient=page.standard_gradient):
-        #can also do with YOUR_X as YOUR_Y: since control is yielded in contextmanager
-        with builder.layout.Row() as row:
-            row.controls.append(ft.ElevatedButton("FletBox"))
-            #builder attrs for creating deepest control
-            builder.ElevatedButton("FletBox")
-            #assign if modification/reads are required
-            textfield = builder.TextField(label="FletBox", text_size=20)
-    #returning builder is optional
-    return builder
+# returning builder is optional (will replace generated builder if returned).
+```
+
+EXTRA: the standard page.go function can be used for traveling between routes.
+```python
+page.go("/")
+```
+
+### Main Block, contextmanagers (with statements)
+The syntax is drastically altered from the standard flet library.
+
+```python
+@fb.view("/")
+def test(page: ft.Page, builder: Builder) -> None:
+    #builder.layout is contextmanagers. TIP: remap via layout=builder.layout
+    with builder.layout.Container(expand=True, margin=-10, gradient=page.standard_gradient): #can used stored attributes using "page" as a shared storage
+        with builder.layout.Row() as row: #can be assigned, or not
+            row.controls.append(ft.ElevatedButton("FletBox")) #see above
+            builder.ElevatedButton("FletBox") #IMPORTANT: root builder attrs are used for creating deepest control (not layout)
+            textfield = builder.TextField(label="FletBox", text_size=20) #can be assigned, or not - for modification/reads
+
+    @builder.postexec #OPTIONAL: postexec decorator - run function after view load
+    def postfunc():
+        pass #YOUR_POST_FUNCTION_HERE
 
 #can define whatever non-view-specific thing you want, passing target is optional
 def shared_methods(page: ft.Page):
     page.fonts = {
         "Raleway": "assets/Raleway[wght].ttf"
     }
-    page.theme = ft.Theme(color_scheme_seed="pink", visual_density="COMFORTABLE", font_family="Raleway", use_material3=False)
+    page.theme = ft.Theme(color_scheme_seed="pink", visual_density="COMFORTABLE", font_family="Raleway")
     page.standard_gradient = ft.LinearGradient(begin=ft.alignment.bottom_left, end=ft.alignment.top_right, colors=["#F7C35A", "#FBAFAB"])
+```
 
-#pass normal ft.app kwargs to fb.app, can also be set (eg. fb.port=8000)
+And finally we run the application.
+*NOTE: you can pass normal ft.app kwargs to fb.app.*
+```python
+#pass normal ft.app kwargs to fb.app
 fb.app(target=shared_methods)
 ```
+
+## Other Usage
 ### Custom Elements
 ```python
 import flet as ft
 from fletbox import FletBox, Builder, Factory
 
 #module with custom components
 import flet_material as fm
```

