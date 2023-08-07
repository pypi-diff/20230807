# Comparing `tmp/parsagon-0.9.3.tar.gz` & `tmp/parsagon-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.9.3.tar", last modified: Thu Aug  3 12:37:40 2023, max compression
+gzip compressed data, was "parsagon-0.9.4.tar", last modified: Mon Aug  7 01:06:35 2023, max compression
```

## Comparing `parsagon-0.9.3.tar` & `parsagon-0.9.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-03 12:37:40.360222 parsagon-0.9.3/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-03 12:37:40.359412 parsagon-0.9.3/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.3/README.md
--rw-r--r--   0 amsuh    (10002)    18010     1158 2023-08-03 12:36:46.000000 parsagon-0.9.3/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-08-03 12:37:40.360480 parsagon-0.9.3/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-03 12:37:40.341464 parsagon-0.9.3/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.3/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-03 12:37:40.348941 parsagon-0.9.3/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.9.3/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     5590 2023-08-02 06:48:17.000000 parsagon-0.9.3/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.3/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.3/src/parsagon/exceptions.py
--rw-r--r--   0 amsuh    (10002)    18010    15391 2023-08-03 06:45:34.000000 parsagon-0.9.3/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010    14448 2023-08-02 10:31:32.000000 parsagon-0.9.3/src/parsagon/highlights.js
--rw-r--r--   0 amsuh    (10002)    18010     9218 2023-08-02 10:12:43.000000 parsagon-0.9.3/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.3/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-03 12:37:40.358291 parsagon-0.9.3/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.3/src/parsagon/tests/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.3/src/parsagon/tests/api_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.3/src/parsagon/tests/cli_mocks.py
--rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.3/src/parsagon/tests/conftest.py
--rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.3/src/parsagon/tests/test_executor.py
--rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.3/src/parsagon/tests/test_invalid_args.py
--rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.3/src/parsagon/tests/test_pipeline_operations.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-03 12:37:40.352179 parsagon-0.9.3/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-03 12:37:40.000000 parsagon-0.9.3/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      709 2023-08-03 12:37:40.000000 parsagon-0.9.3/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-08-03 12:37:40.000000 parsagon-0.9.3/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-08-03 12:37:40.000000 parsagon-0.9.3/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      263 2023-08-03 12:37:40.000000 parsagon-0.9.3/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010        9 2023-08-03 12:37:40.000000 parsagon-0.9.3/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-07 01:06:35.782816 parsagon-0.9.4/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-07 01:06:35.782498 parsagon-0.9.4/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1321 2023-07-07 07:03:35.000000 parsagon-0.9.4/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1158 2023-08-07 01:05:50.000000 parsagon-0.9.4/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-08-07 01:06:35.782926 parsagon-0.9.4/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-07 01:06:35.767992 parsagon-0.9.4/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.4/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-07 01:06:35.774113 parsagon-0.9.4/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-07-07 07:03:35.000000 parsagon-0.9.4/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     5853 2023-08-06 10:20:20.000000 parsagon-0.9.4/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.9.4/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      819 2023-07-07 07:03:35.000000 parsagon-0.9.4/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    15391 2023-08-03 06:45:34.000000 parsagon-0.9.4/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010    14871 2023-08-04 23:48:32.000000 parsagon-0.9.4/src/parsagon/highlights.js
+-rw-r--r--   0 amsuh    (10002)    18010    11323 2023-08-06 10:23:22.000000 parsagon-0.9.4/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     2947 2023-07-18 08:23:24.000000 parsagon-0.9.4/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-07 01:06:35.781781 parsagon-0.9.4/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.9.4/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-07-07 07:03:35.000000 parsagon-0.9.4/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-07-07 07:03:35.000000 parsagon-0.9.4/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-07-07 07:03:35.000000 parsagon-0.9.4/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010      645 2023-07-30 02:55:30.000000 parsagon-0.9.4/src/parsagon/tests/test_executor.py
+-rw-r--r--   0 amsuh    (10002)    18010      676 2023-07-07 07:03:35.000000 parsagon-0.9.4/src/parsagon/tests/test_invalid_args.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-07-07 07:03:35.000000 parsagon-0.9.4/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-08-07 01:06:35.777351 parsagon-0.9.4/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1711 2023-08-07 01:06:35.000000 parsagon-0.9.4/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      709 2023-08-07 01:06:35.000000 parsagon-0.9.4/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-08-07 01:06:35.000000 parsagon-0.9.4/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-08-07 01:06:35.000000 parsagon-0.9.4/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      263 2023-08-07 01:06:35.000000 parsagon-0.9.4/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010        9 2023-08-07 01:06:35.000000 parsagon-0.9.4/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.9.3/PKG-INFO` & `parsagon-0.9.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.9.3
+Version: 0.9.4
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.9.3/README.md` & `parsagon-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/pyproject.toml` & `parsagon-0.9.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 parsagon = ["highlights.js"]
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.9.3"
+version = "0.9.4"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
```

### Comparing `parsagon-0.9.3/src/parsagon/api.py` & `parsagon-0.9.4/src/parsagon/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,22 @@
     _api_call(
         httpx.post,
         "/transformers/custom-function/",
         json={"pipeline": pipeline_id, "call_id": call_id, **custom_function.to_json()},
     )
 
 
+def add_examples_to_custom_function(pipeline_id, call_id, custom_function):
+    _api_call(
+        httpx.post,
+        "/transformers/custom-function/add-examples/",
+        json={"pipeline": pipeline_id, "call_id": call_id, **custom_function.to_json()},
+    )
+
+
 def get_pipeline(pipeline_name):
     with RaiseProgramNotFound(pipeline_name):
         return _api_call(
             httpx.get,
             f"/pipelines/name/{pipeline_name}/",
         )
```

### Comparing `parsagon-0.9.3/src/parsagon/custom_function.py` & `parsagon-0.9.4/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/src/parsagon/exceptions.py` & `parsagon-0.9.4/src/parsagon/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/src/parsagon/executor.py` & `parsagon-0.9.4/src/parsagon/executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/src/parsagon/highlights.js` & `parsagon-0.9.4/src/parsagon/highlights.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -144,50 +144,70 @@
         const rect = rects[0];
         if (rect.width * rect.height === 0) {
             element.style.display = 'block';
         }
     }
 }
 
+const DUMMY_FRAGMENT = document.createDocumentFragment()
+
+function isValidSelector(selector) {
+    console.log(selector);
+    try {
+        DUMMY_FRAGMENT.querySelector(selector)
+    } catch {
+        console.log("false");
+        return false
+    }
+    console.log("true");
+    return true
+}
+
 function getSimilar(elements) {
+    console.log(0);
     let tag = '*';
     if (elements.every((elem) => elem.tagName === elements[0].tagName)) {
         tag = elements[0].tagName.toLowerCase();
         tag = tag.replace(':', '\\:');
     }
 
     const classLists = elements.map((elem) => [...elem.classList]);
     const commonClasses = classLists
         .reduce((a, b) => a.filter((c) => b.includes(c)))
         .filter(
             (className) =>
             className !== TARGET_STORED_CLASSNAME &&
-            className !== MOUSE_VISITED_CLASSNAME
+            className !== MOUSE_VISITED_CLASSNAME &&
+            isValidSelector("." + className)
         )
-        .map((className) => className.replace(':', '\\:'));
+        .map((className) => className.replace(':', '\\:').replace('.', '\\.').replace('[', '\\[').replace(']', '\\]').replace('=', '\\='));
+    console.log(1);
     const classString = commonClasses.join('.');
+    console.log(2);
 
     const siblingIndexes = elements.map(
         (elem) =>
         Array.prototype.indexOf.call(elem.parentNode.children, elem) + 1
     );
     let siblingIndex = null;
     if (siblingIndexes.every((index) => index === siblingIndexes[0])) {
         siblingIndex = siblingIndexes[0];
     }
+    console.log(3);
 
     let elemString = tag;
     if (classString) {
         elemString += '.' + classString;
     }
     if (siblingIndex !== null) {
         elemString += `:nth-child(${siblingIndex})`;
     }
 
     const parentElements = elements.map((elem) => elem.parentElement);
+    console.log(4);
     if (parentElements.some((elem) => elem === null)) {
         return elemString;
     } else {
         return `${getSimilar(parentElements)} > ${elemString}`;
     }
 }
 
@@ -356,15 +376,14 @@
     for (const elem of autocompleteElements) {
         removeAutocompleteCSS(elem);
         addTargetStoredCSS(elem);
     }
 };
 
 function handleClick(e) {
-    console.log(window.currentFieldType)
     if (window.currentFieldType === null) {
         return;
     }
 
     e.preventDefault();
     e.stopImmediatePropagation();
 
@@ -376,27 +395,29 @@
     }
 
     if (srcElement.classList.contains(TARGET_STORED_CLASSNAME)) {
         removeTargetStoredCSS(srcElement);
         try {
             addAutocompletes();
         } catch (e) {
+            console.log(e);
             // carry on even if autocomplete runs into invalid CSS classes/IDs
         }
     } else {
         if (
             window.maxExamples &&
             getNumExamples() >= window.maxExamples
         ) {
             return;
         }
         addTargetStoredCSS(srcElement);
         try {
             addAutocompletes();
         } catch (e) {
+            console.log(e);
             // carry on even if autocomplete runs into invalid CSS classes/IDs
         }
     }
 };
 
 function handleMouseDown(e) {
     if (window.currentFieldType === null) {
@@ -501,20 +522,17 @@
     makeVisible(srcElement);
 
     addMouseVisitedCSS(srcElement);
     window.prevDOM = srcElement;
 };
 
 function handleKeyDown(e) {
-    console.log(1);
     if (window.currentFieldType === null) {
-        console.log(2);
         return;
     }
-    console.log(window.currentFieldType);
 
     e.preventDefault();
     e.stopImmediatePropagation();
 
     const key = e.key;
     if (key === "Backspace" || key === "Delete") {
         clearCSS();
```

### Comparing `parsagon-0.9.3/src/parsagon/main.py` & `parsagon-0.9.4/src/parsagon/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from halo import Halo
 
 from parsagon.api import (
     get_program_sketches,
     create_pipeline,
     delete_pipeline,
     create_custom_function,
+    add_examples_to_custom_function,
     create_pipeline_run,
     get_pipeline,
     get_pipelines,
     get_pipeline_code,
     get_run,
     APIException,
 )
@@ -72,14 +73,42 @@
         "--program",
         dest="program_name",
         type=str,
         help="the name of the program",
     )
     parser_detail.set_defaults(func=detail)
 
+    # Update
+    parser_update = subparsers.add_parser(
+        "update",
+        description="Updates a created program.",
+    )
+    parser_update.add_argument(
+        "program_name",
+        type=str,
+        help="the name of the program to update",
+    )
+    parser_update.add_argument(
+        "--variables",
+        type=json.loads,
+        default="{}",
+        help="a JSON object mapping variables to values",
+    )
+    parser_update.add_argument(
+        "--headless",
+        action="store_true",
+        help="run the browser in headless mode",
+    )
+    parser_update.add_argument(
+        "--infer",
+        action="store_true",
+        help="let Parsagon infer all elements to be scraped",
+    )
+    parser_update.set_defaults(func=update)
+
     # Run
     parser_run = subparsers.add_parser(
         "run",
         description="Runs a created program.",
     )
     parser_run.add_argument(
         "program_name",
@@ -200,14 +229,42 @@
         else:
             logger.info("Discarded program.")
             break
 
     logger.info("Done.")
 
 
+def update(program_name, variables={}, headless=False, infer=False, verbose=False):
+    pipeline = get_pipeline(program_name)
+    abridged_program = pipeline["abridged_sketch"]
+    # Make the program runnable
+    variables_str = ", ".join(f"{k}={repr(v)}" for k, v in variables.items())
+    abridged_program += f"\n\noutput = func({variables_str})"
+    abridged_program += "\nprint(f'Program finished and returned a value of:\\n{output}\\n')\n"
+
+    # Execute the abridged program to gather examples
+    executor = Executor(headless=headless, infer=infer)
+    executor.execute(abridged_program)
+
+    pipeline_id = pipeline["id"]
+    try:
+        for call_id, custom_function in executor.custom_functions.items():
+            debug_suffix = f" ({custom_function.name})"
+            description = custom_functions_to_descriptions.get(custom_function.name)
+            description = " to " + description if description else ""
+            if verbose:
+                description += debug_suffix
+            logger.info(f"  Saving function{description}...")
+            add_examples_to_custom_function(pipeline_id, call_id, custom_function)
+        logger.info(f"Saved.")
+    except Exception as e:
+        print(e)
+        logger.info(f"An error occurred while saving the program. The program was not updated.")
+
+
 def detail(program_name=None, verbose=False):
     if program_name:
         data = [get_pipeline(program_name)]
     else:
         data = get_pipelines()
     for pipeline in data:
         print(
```

### Comparing `parsagon-0.9.3/src/parsagon/settings.py` & `parsagon-0.9.4/src/parsagon/settings.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/src/parsagon/tests/api_mocks.py` & `parsagon-0.9.4/src/parsagon/tests/api_mocks.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/src/parsagon/tests/test_executor.py` & `parsagon-0.9.4/src/parsagon/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/src/parsagon/tests/test_invalid_args.py` & `parsagon-0.9.4/src/parsagon/tests/test_invalid_args.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/src/parsagon/tests/test_pipeline_operations.py` & `parsagon-0.9.4/src/parsagon/tests/test_pipeline_operations.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.9.3/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.9.4/src/parsagon.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.9.3
+Version: 0.9.4
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `parsagon-0.9.3/src/parsagon.egg-info/SOURCES.txt` & `parsagon-0.9.4/src/parsagon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

