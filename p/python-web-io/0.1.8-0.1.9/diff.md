# Comparing `tmp/python_web_io-0.1.8.tar.gz` & `tmp/python_web_io-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_web_io-0.1.8.tar", max compression
+gzip compressed data, was "python_web_io-0.1.9.tar", max compression
```

## Comparing `python_web_io-0.1.8.tar` & `python_web_io-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      550 2023-04-16 01:04:25.875413 python_web_io-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-16 00:58:22.446645 python_web_io-0.1.8/python_web_io/__main__.py
--rw-r--r--   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.8/python_web_io/cache.py
--rw-r--r--   0        0        0     1385 2023-04-16 00:58:18.317553 python_web_io-0.1.8/python_web_io/main.py
--rw-r--r--   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.8/python_web_io/override.py
--rw-r--r--   0        0        0     2736 2023-04-16 01:03:41.446254 python_web_io-0.1.8/python_web_io/server.py
--rw-r--r--   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.8/python_web_io/templates/500.html
--rw-r--r--   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.8/python_web_io/templates/base.html
--rw-r--r--   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.8/python_web_io/templates/index.html
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 python_web_io-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0      550 2023-04-16 21:08:08.588193 python_web_io-0.1.9/pyproject.toml
+-rwxr-xr-x   0        0        0       45 2023-04-16 21:02:37.686968 python_web_io-0.1.9/python_web_io/__main__.py
+-rwxr-xr-x   0        0        0      689 2023-04-16 21:02:34.117778 python_web_io-0.1.9/python_web_io/cache.py
+-rwxr-xr-x   0        0        0     1385 2023-04-16 21:02:28.562562 python_web_io-0.1.9/python_web_io/main.py
+-rwxr-xr-x   0        0        0     2311 2023-04-16 21:03:06.293387 python_web_io-0.1.9/python_web_io/override.py
+-rwxr-xr-x   0        0        0     3797 2023-04-16 21:02:21.551808 python_web_io-0.1.9/python_web_io/server.py
+-rwxr-xr-x   0        0        0      476 2023-04-16 21:02:41.473232 python_web_io-0.1.9/python_web_io/templates/500.html
+-rwxr-xr-x   0        0        0      951 2023-04-16 21:05:08.707195 python_web_io-0.1.9/python_web_io/templates/base.html
+-rwxr-xr-x   0        0        0      719 2023-04-16 21:02:49.565187 python_web_io-0.1.9/python_web_io/templates/index.html
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 python_web_io-0.1.9/PKG-INFO
```

### Comparing `python_web_io-0.1.8/pyproject.toml` & `python_web_io-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-web-io"
-version = "0.1.8"
+version = "0.1.9"
 description = "Generate a webpage as a GUI for a Python script, and serve from anywhere."
 authors = ["Zachary Smith"]
 packages = [{include = "python_web_io"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flask = "^2.2.3"
```

### Comparing `python_web_io-0.1.8/python_web_io/cache.py` & `python_web_io-0.1.9/python_web_io/cache.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.8/python_web_io/main.py` & `python_web_io-0.1.9/python_web_io/main.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.8/python_web_io/override.py` & `python_web_io-0.1.9/python_web_io/override.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,7 +61,9 @@
 
 
 def Exec(source, globals=None, locals=None):
     try:
         exec(source, globals, locals)
     except ExecInterrupt:
         pass
+    except Exception as e:
+        return e
```

### Comparing `python_web_io-0.1.8/python_web_io/server.py` & `python_web_io-0.1.9/python_web_io/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import builtins
 
-from flask import Flask, session, request, render_template
+from flask import Flask, session, request, render_template, url_for, redirect
 from python_web_io.override import (
     input,
     print,
     Exec,
 )  # input, print are listed as unused, but exist to override builtin calls made from Exec() of the user script
 from python_web_io.cache import Cache
 
@@ -18,18 +18,18 @@
 @app.errorhandler(500)
 def internal_error(error):
     """
     If the user was part-way through submitting a form when the server dies, and does not close the browser tab to clear session cookies, the app may get confused due to a mismatch between server session and user progress.
     A custom 500 error page should inform the user of this issue and direct them to clear cookies / close the tab to fix.
     """
 
-    return render_template("500.html", error=error)
+    return render_template("500.html", title=Cache.get("title"), icon=Cache.get("icon"), error=error)
 
 
-@app.route("/", methods=["GET", "POST"])
+@app.route("/index", methods=["GET", "POST"])
 def index():
     """
     Run a Python script, generating a list of IO to display.
     Stop execution after finding an input without cached response (in session storage).
     Display list of IO to client, prompt for the next input.
 
     Returns:
@@ -39,31 +39,59 @@
     # POST request indicates user is submitting input
     if request.method == "POST":
         # iterate the form inputs/submission
         # we don't support re-editing previous submissions yet (past inputs are disabled), but this approach could allow this to change in the future
         for key, value in request.form.items():
             index = int(key)
 
-            # assert does not have value assigned (raise error if already assigned, as key error or client enabling disabled inputs)
-            assert len(session["io"][index][1]) == 2
-            # if passing, reassign io element with a value arg
-            session["io"][index] = ("input", (*session["io"][index][1], value))
+            # detect form resubmission by checking if form has inputs that are already assigned
+            if len(session["io"][index][1]) < 3:
+                # if passing, reassign io element with a value arg
+                session["io"][index] = ("input", (*session["io"][index][1], value))
 
     # track input/print elements encountered over multiple re-runs of the script
     if "io" not in session:
         session["io"] = []
 
     # use a counter to track number of elements encountered in this script rerun
     session["counter"] = 0
 
     # execute the user script to collect IO elements
     # if an unencountered input is found, the script terminates early and the user is prompted to provide input
-    Exec(Cache.get("script"))
+    error = Exec(Cache.get("script"))
+
+    # if error raised, then previous input is likely invalid
+    # find last input and delete user input (and delete any elements past this point)
+    if error:
+        # find index of most recent input
+        for i in range(1, len(session["io"])+1):
+            func_name = session["io"][-i][0]
+            if func_name == 'input':
+                # delete input_value by recreating func tuple
+                input_id, input_label, _ = session["io"][-i][1]
+                session["io"][-i] = (func_name, (input_id, input_label))
+                
+                # delete all elements past this point
+                session["io"] = session["io"][:len(session["io"])-i+1]
+
+                break
 
     # render collected IO into a form - inputs with submitted values are disabled
     return render_template(
-        "index.html", title=Cache.get("title"), icon=Cache.get("icon"), io=session["io"]
+        "index.html", title=Cache.get("title"), icon=Cache.get("icon"), io=session["io"], error=error,
     )
 
 
+@app.route("/reset", methods=["POST"])
+def reset():
+    """
+    Reset the user session.
+    """
+    # clear the user session
+    session["io"] = []
+
+    # render collected IO into a form - inputs with submitted values are disabled
+    return redirect(url_for("index"))
+
+
 if __name__ == "__main__":
     app.run(debug=True)
```

### Comparing `python_web_io-0.1.8/python_web_io/templates/base.html` & `python_web_io-0.1.9/python_web_io/templates/base.html`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 <html lang="en">
 
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>{{title}} - Python Web IO App</title>
     <link rel="stylesheet" href="https://cdn.simplecss.org/simple.min.css">
-    <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>{{icon}}</text></svg>">
+    <link rel="icon"
+        href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>{{icon}}</text></svg>">
+
+    <meta http-equiv='cache-control' content='no-cache'>
+    <meta http-equiv='expires' content='0'>
+    <meta http-equiv='pragma' content='no-cache'>
 </head>
 
 <body>
     <main>
         <h1>{{title}}</h1>
-        
+
         <div class="content">
             {% block content %} {% endblock %}
         </div>
     </main>
 
     <footer>
         <p>Created with <a href="https://github.com/Cutwell/python-web-io"><code>Python Web I/O</code></a>.</p>
```

#### html2text {}

```diff
@@ -1,6 +1,9 @@
 
 
+
+
+
 ****** {{title}} ******
 {% block content %} {% endblock %}
 
 Created with Python_Web_I/O.
```

