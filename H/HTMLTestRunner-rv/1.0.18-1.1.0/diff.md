# Comparing `tmp/HTMLTestRunner-rv-1.0.18.tar.gz` & `tmp/HTMLTestRunner-rv-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTMLTestRunner-rv-1.0.18.tar", last modified: Sun Jun 26 17:15:53 2022, max compression
+gzip compressed data, was "dist\HTMLTestRunner-rv-1.1.0.tar", last modified: Mon Aug  7 02:45:51 2023, max compression
```

## Comparing `HTMLTestRunner-rv-1.0.18.tar` & `HTMLTestRunner-rv-1.1.0.tar`

### file list

```diff
@@ -1,68 +1,22 @@
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/HTMLTestRunner/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      124 2022-06-26 16:28:41.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner/__init__.py
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)    16952 2022-06-26 16:28:41.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner/runner.py
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/HTMLTestRunner/static/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     2096 2022-06-26 15:31:10.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner/static/script.js
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     1976 2022-06-26 15:31:10.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner/static/stylesheet.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.721248 HTMLTestRunner-rv-1.0.18/HTMLTestRunner/templates/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     4216 2022-06-26 15:31:10.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner/templates/template.html
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.721248 HTMLTestRunner-rv-1.0.18/HTMLTestRunner_rv.egg-info/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     2319 2022-06-26 17:15:53.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner_rv.egg-info/PKG-INFO
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     2735 2022-06-26 17:15:53.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner_rv.egg-info/SOURCES.txt
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)        1 2022-06-26 17:15:53.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner_rv.egg-info/dependency_links.txt
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)        1 2022-06-26 17:03:26.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner_rv.egg-info/not-zip-safe
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)       30 2022-06-26 17:15:53.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner_rv.egg-info/requires.txt
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)       15 2022-06-26 17:15:53.000000 HTMLTestRunner-rv-1.0.18/HTMLTestRunner_rv.egg-info/top_level.txt
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)       55 2022-06-26 15:31:10.000000 HTMLTestRunner-rv-1.0.18/MANIFEST.in
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     2319 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/PKG-INFO
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     1794 2022-06-26 16:53:02.000000 HTMLTestRunner-rv-1.0.18/README.md
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)       38 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/setup.cfg
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      910 2022-06-26 17:05:14.000000 HTMLTestRunner-rv-1.0.18/setup.py
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/venv/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/venv/lib/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.721248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/html4css1/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     7210 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/html4css1/html4css1.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.721248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/html5_polyglot/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     6261 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/html5_polyglot/math.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     7355 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/html5_polyglot/minimal.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     7801 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/html5_polyglot/plain.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)    11518 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/html5_polyglot/responsive.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)    11878 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/html5_polyglot/tuftig.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.721248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/pep_html/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     6367 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/pep_html/pep.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.717248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/big-black/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      911 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     3606 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/big-white/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      906 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     3566 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     1003 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/framing.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      261 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/opera.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      648 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/outline.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     4384 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/pretty.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      818 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/print.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      451 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      283 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/slides.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)    15800 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/default/slides.js
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/medium-black/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     4031 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/medium-white/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      944 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     3991 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/small-black/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     4030 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.725247 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/small-white/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      941 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)     4001 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
-drwxrwxr-x   0 ravikirana  (1000) ravikirana  (1000)        0 2022-06-26 17:15:53.721248 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils-0.18.1.dist-info/
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)    26094 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils-0.18.1.dist-info/SOURCES.html
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      968 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils-0.18.1.dist-info/dependency_links.html
--rw-rw-r--   0 ravikirana  (1000) ravikirana  (1000)      969 2022-06-26 16:57:20.000000 HTMLTestRunner-rv-1.0.18/venv/lib/python3.8/site-packages/docutils-0.18.1.dist-info/top_level.html
+drwxrwxrwx   0        0        0        0 2023-08-07 02:45:51.290421 HTMLTestRunner-rv-1.1.0/
+drwxrwxrwx   0        0        0        0 2023-08-07 02:45:51.259168 HTMLTestRunner-rv-1.1.0/HTMLTestRunner/
+-rw-rw-rw-   0        0        0      128 2023-08-07 02:25:08.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner/__init__.py
+-rw-rw-rw-   0        0        0    18118 2023-08-07 02:25:07.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner/runner.py
+drwxrwxrwx   0        0        0        0 2023-08-07 02:45:51.259168 HTMLTestRunner-rv-1.1.0/HTMLTestRunner/static/
+-rw-rw-rw-   0        0        0     2166 2023-07-30 05:26:01.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner/static/script.js
+-rw-rw-rw-   0        0        0     2058 2023-07-30 05:26:01.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner/static/stylesheet.css
+drwxrwxrwx   0        0        0        0 2023-08-07 02:45:51.274792 HTMLTestRunner-rv-1.1.0/HTMLTestRunner/templates/
+-rw-rw-rw-   0        0        0     4320 2023-07-30 05:26:01.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner/templates/template.html
+drwxrwxrwx   0        0        0        0 2023-08-07 02:45:51.290421 HTMLTestRunner-rv-1.1.0/HTMLTestRunner_rv.egg-info/
+-rw-rw-rw-   0        0        0     2409 2023-08-07 02:45:51.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner_rv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-08-07 02:45:51.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner_rv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 02:45:51.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner_rv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-07 02:43:57.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner_rv.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2023-08-07 02:45:51.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner_rv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-07 02:45:51.000000 HTMLTestRunner-rv-1.1.0/HTMLTestRunner_rv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11548 2023-07-30 05:26:01.000000 HTMLTestRunner-rv-1.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      123 2023-08-07 02:42:56.000000 HTMLTestRunner-rv-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2409 2023-08-07 02:45:51.290421 HTMLTestRunner-rv-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1861 2023-07-30 05:26:01.000000 HTMLTestRunner-rv-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-07 02:45:51.290421 HTMLTestRunner-rv-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-08-07 02:25:07.000000 HTMLTestRunner-rv-1.1.0/setup.py
```

### Comparing `HTMLTestRunner-rv-1.0.18/HTMLTestRunner/static/script.js` & `HTMLTestRunner-rv-1.1.0/HTMLTestRunner/static/script.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,71 +1,71 @@
-output_list = Array();
-/* level - 0:Summary; 1:Failed; 2:All */
-function showCase(level) {
-    trs = document.getElementsByTagName("tr");
-    for (var i = 0; i < trs.length; i++) {
-        tr = trs[i];
-        id = tr.id;
-        if (level == 0) {
-            if (id.substr(0, 2) == 'ft' || id.substr(0, 2) == 'pt') {
-                tr.className = 'hiddenRow';
-            }
-        } else if (level == 1) {
-            if (id.substr(0, 2) == 'ft') {
-                tr.className = '';
-            } else if (id.substr(0, 2) == 'pt') {
-                tr.className = 'hiddenRow';
-            }
-        } else if (level == 2) {
-            if (id.substr(0, 2) == 'pt') {
-                tr.className = '';
-            } else if (id.substr(0, 2) == 'ft') {
-                tr.className = 'hiddenRow';
-            }
-        } else {
-            if ((id.substr(0, 2) == 'ft') || (id.substr(0, 2) == 'pt')) {
-                tr.className = '';
-            }
-        }
-    }
-}
-
-function showClassDetail(cid, count) {
-    var id_list = Array(count);
-    var toHide = 1;
-    for (var i = 0; i < count; i++) {
-        tid0 = 't' + cid.substr(1) + '.' + (i + 1);
-        tid = 'f' + tid0;
-        tr = document.getElementById(tid);
-        if (!tr) {
-            tid = 'p' + tid0;
-            tr = document.getElementById(tid);
-        }
-        id_list[i] = tid;
-        if (tr) {
-            if (tr.className) {
-                toHide = 0;
-            }
-        }
-    }
-    for (var i = 0; i < count; i++) {
-        tid = id_list[i];
-        if (toHide) {
-            document.getElementById('div_' + tid).style.display = 'none'
-            document.getElementById(tid).className = 'hiddenRow';
-        } else {
-            document.getElementById(tid).className = '';
-        }
-    }
-}
-
-function showTestDetail(div_id) {
-    var details_div = document.getElementById(div_id)
-    var displayState = details_div.style.display
-    // alert(displayState)
-    if (displayState != 'block') {
-        displayState = 'block'
-        details_div.style.display = 'block'
-    } else {
-        details_div.style.display = 'none'
-    }
+output_list = Array();
+/* level - 0:Summary; 1:Failed; 2:All */
+function showCase(level) {
+    trs = document.getElementsByTagName("tr");
+    for (var i = 0; i < trs.length; i++) {
+        tr = trs[i];
+        id = tr.id;
+        if (level == 0) {
+            if (id.substr(0, 2) == 'ft' || id.substr(0, 2) == 'pt') {
+                tr.className = 'hiddenRow';
+            }
+        } else if (level == 1) {
+            if (id.substr(0, 2) == 'ft') {
+                tr.className = '';
+            } else if (id.substr(0, 2) == 'pt') {
+                tr.className = 'hiddenRow';
+            }
+        } else if (level == 2) {
+            if (id.substr(0, 2) == 'pt') {
+                tr.className = '';
+            } else if (id.substr(0, 2) == 'ft') {
+                tr.className = 'hiddenRow';
+            }
+        } else {
+            if ((id.substr(0, 2) == 'ft') || (id.substr(0, 2) == 'pt')) {
+                tr.className = '';
+            }
+        }
+    }
+}
+
+function showClassDetail(cid, count) {
+    var id_list = Array(count);
+    var toHide = 1;
+    for (var i = 0; i < count; i++) {
+        tid0 = 't' + cid.substr(1) + '.' + (i + 1);
+        tid = 'f' + tid0;
+        tr = document.getElementById(tid);
+        if (!tr) {
+            tid = 'p' + tid0;
+            tr = document.getElementById(tid);
+        }
+        id_list[i] = tid;
+        if (tr) {
+            if (tr.className) {
+                toHide = 0;
+            }
+        }
+    }
+    for (var i = 0; i < count; i++) {
+        tid = id_list[i];
+        if (toHide) {
+            document.getElementById('div_' + tid).style.display = 'none'
+            document.getElementById(tid).className = 'hiddenRow';
+        } else {
+            document.getElementById(tid).className = '';
+        }
+    }
+}
+
+function showTestDetail(div_id) {
+    var details_div = document.getElementById(div_id)
+    var displayState = details_div.style.display
+    // alert(displayState)
+    if (displayState != 'block') {
+        displayState = 'block'
+        details_div.style.display = 'block'
+    } else {
+        details_div.style.display = 'none'
+    }
 }
```

### Comparing `HTMLTestRunner-rv-1.0.18/HTMLTestRunner/templates/template.html` & `HTMLTestRunner-rv-1.1.0/HTMLTestRunner/templates/template.html`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-<!DOCTYPE html>
-<html>
-<head>
-    <title>{{title}}</title>
-    <meta name="generator" content="{{ generator }}"/>
-    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
-    <link rel="stylesheet" href="stylesheet.css">
-    <script src="script.js"></script>
-    <style>
-        {{ style }}
-    </style>
-    <script>
-        {{ script }}
-    </script>
-</head>
-<body>
-<div class='heading'>
-    <h1 style="margin-left:1ex;">{{ title }}</h1>
-    {% for attribute in report_attrs %}
-    <p class='attribute'><strong>{{ attribute[0] }} : </strong> {{attribute[1]}}</p>
-    {% endfor %}
-</div>
-<div>
-    <p id='show_detail_line'><b>Show</b>
-        <button><a href='javascript:showCase(0)' style="color:#660066;">Summary</a></button>
-        <button><a href='javascript:showCase(1)' style="color:#660066;">Failed</a></button>
-        <button><a href='javascript:showCase(2)' style="color:#660066;">Passed</a></button>
-        <button><a href='javascript:showCase(3)' style="color:#660066;">All</a></button>
-    </p>
-    <table id='result_table'>
-        <colgroup>
-            <col align='left'/>
-            <col align='right'/>
-            <col align='right'/>
-            <col align='right'/>
-            <col align='right'/>
-            <col align='right'/>
-        </colgroup>
-        <tr id='header_row'>
-            <td>Test Group/Test case</td>
-            <td>Count</td>
-            <td>Pass</td>
-            <td>Fail</td>
-            <td>Error</td>
-            <td>View</td>
-        </tr>
-        {% for cls in report['class_testcases'] %}
-        <tr class='{{ cls["style"]}}' style="font-weight:bold;color:white;">
-            <td><a href="javascript:showClassDetail('{{ cls['cid']}}','{{ cls['count']}}')">{{ cls['desc'] }}</a></td>
-            <td>{{ cls['count'] }}</td>
-            <td>{{ cls['pass'] }}</td>
-            <td>{{ cls['fail'] }}</td>
-            <td>{{ cls['error'] }}</td>
-            <td>
-                <button><a href="javascript:showClassDetail('{{ cls['cid']}}','{{ cls['count'] }}')"
-                           style="color:#660066;">Detail</a></button>
-            </td>
-        </tr>
-            {% for testcase in cls['fun_testcases'] %}
-            <tr id="{{testcase['tid']}}" class='{{ testcase["class"] }}'>
-                <td class='{{ testcase["style"] }}'>
-                    <div class='testcase'>
-                        <a class="popup_link" onfocus='this.blur();'
-                           href="javascript:showTestDetail('div_{{testcase['tid']}}')">{{testcase['desc']}}</a>
-                    </div>
-                </td>
-                <td colspan='5' align='center'>
-                    <div>
-                        <!--css div popup start-->
-                        <button>
-                            <a class="popup_link" onfocus='this.blur();'
-                               href="javascript:showTestDetail('div_{{testcase['tid']}}')" style="color:#660066;">
-                                {{ testcase['status'] }}
-                            </a></button>
-                        <div id='div_{{ testcase["tid"] }}' class="popup_window">
-                            <div style='text-align: right; color:red;cursor:pointer'>
-                                <a onfocus='this.blur();'
-                                   onclick="document.getElementById('div_{{testcase['tid']}}').style.display = 'none'; "
-                                   style="color:red;">
-                                    [x]</a>
-                            </div>
-                            <pre>{{ testcase['log'] }}</pre>
-                            <pre style="color: red;">{{ testcase['error'] }}</pre>
-                        </div>
-                        <!--css div popup end-->
-                    </div>
-                </td>
-            </tr>
-            {% endfor %}
-        {% endfor %}
-
-        <tr id='total_row'>
-            <td>Total</td>
-            <td>{{report['count']}}</td>
-            <td>{{report['pass']}}</td>
-            <td>{{report['fail']}}</td>
-            <td>{{report['error']}}</td>
-            <td>&nbsp;</td>
-        </tr>
-    </table>
-</div>
-<br><br>
-<div id='ending'><b>Time Elapsed: </b>{{ stop_time }}</div>
-</body>
+<!DOCTYPE html>
+<html>
+<head>
+    <title>{{title}}</title>
+    <meta name="generator" content="{{ generator }}"/>
+    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
+    <link rel="stylesheet" href="stylesheet.css">
+    <script src="script.js"></script>
+    <style>
+        {{ style }}
+    </style>
+    <script>
+        {{ script }}
+    </script>
+</head>
+<body>
+<div class='heading'>
+    <h1 style="margin-left:1ex;">{{ title }}</h1>
+    {% for attribute in report_attrs %}
+    <p class='attribute'><strong>{{ attribute[0] }} : </strong> {{attribute[1]}}</p>
+    {% endfor %}
+</div>
+<div>
+    <p id='show_detail_line'><b>Show</b>
+        <button><a href='javascript:showCase(0)' style="color:#660066;">Summary</a></button>
+        <button><a href='javascript:showCase(1)' style="color:#660066;">Failed</a></button>
+        <button><a href='javascript:showCase(2)' style="color:#660066;">Passed</a></button>
+        <button><a href='javascript:showCase(3)' style="color:#660066;">All</a></button>
+    </p>
+    <table id='result_table'>
+        <colgroup>
+            <col align='left'/>
+            <col align='right'/>
+            <col align='right'/>
+            <col align='right'/>
+            <col align='right'/>
+            <col align='right'/>
+        </colgroup>
+        <tr id='header_row'>
+            <td>Test Group/Test case</td>
+            <td>Count</td>
+            <td>Pass</td>
+            <td>Fail</td>
+            <td>Error</td>
+            <td>View</td>
+        </tr>
+        {% for cls in report['class_testcases'] %}
+        <tr class='{{ cls["style"]}}' style="font-weight:bold;color:white;">
+            <td><a href="javascript:showClassDetail('{{ cls['cid']}}','{{ cls['count']}}')">{{ cls['desc'] }}</a></td>
+            <td>{{ cls['count'] }}</td>
+            <td>{{ cls['pass'] }}</td>
+            <td>{{ cls['fail'] }}</td>
+            <td>{{ cls['error'] }}</td>
+            <td>
+                <button><a href="javascript:showClassDetail('{{ cls['cid']}}','{{ cls['count'] }}')"
+                           style="color:#660066;">Detail</a></button>
+            </td>
+        </tr>
+            {% for testcase in cls['fun_testcases'] %}
+            <tr id="{{testcase['tid']}}" class='{{ testcase["class"] }}'>
+                <td class='{{ testcase["style"] }}'>
+                    <div class='testcase'>
+                        <a class="popup_link" onfocus='this.blur();'
+                           href="javascript:showTestDetail('div_{{testcase['tid']}}')">{{testcase['desc']}}</a>
+                    </div>
+                </td>
+                <td colspan='5' align='center'>
+                    <div>
+                        <!--css div popup start-->
+                        <button>
+                            <a class="popup_link" onfocus='this.blur();'
+                               href="javascript:showTestDetail('div_{{testcase['tid']}}')" style="color:#660066;">
+                                {{ testcase['status'] }}
+                            </a></button>
+                        <div id='div_{{ testcase["tid"] }}' class="popup_window">
+                            <div style='text-align: right; color:red;cursor:pointer'>
+                                <a onfocus='this.blur();'
+                                   onclick="document.getElementById('div_{{testcase['tid']}}').style.display = 'none'; "
+                                   style="color:red;">
+                                    [x]</a>
+                            </div>
+                            <pre>{{ testcase['log'] }}</pre>
+                            <pre style="color: red;">{{ testcase['error'] }}</pre>
+                        </div>
+                        <!--css div popup end-->
+                    </div>
+                </td>
+            </tr>
+            {% endfor %}
+        {% endfor %}
+
+        <tr id='total_row'>
+            <td>Total</td>
+            <td>{{report['count']}}</td>
+            <td>{{report['pass']}}</td>
+            <td>{{report['fail']}}</td>
+            <td>{{report['error']}}</td>
+            <td>&nbsp;</td>
+        </tr>
+    </table>
+</div>
+<br><br>
+<div id='ending'><b>Time Elapsed: </b>{{ stop_time }}</div>
+</body>
 </html>
```

### Comparing `HTMLTestRunner-rv-1.0.18/HTMLTestRunner_rv.egg-info/PKG-INFO` & `HTMLTestRunner-rv-1.1.0/HTMLTestRunner_rv.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,84 @@
-Metadata-Version: 2.1
-Name: HTMLTestRunner-rv
-Version: 1.0.18
-Summary: HTMLTestRunner for unit test framework
-Home-page: https://github.com/ravikiranb36/HTMLTestRunner.io.git
-Author: Ravikirana B
-Author-email: ravikiranb36@gmail.com
-License: MIT
-Keywords: HtmlTestRunner TestRunner Html Reports
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# HTMLTestRunner
-```text
-HTMLTestRunner for python3 
-
-A TestRunner for use with the Python unit testing framework. 
-It generates a HTML report to show the result at a glance.
-It logs stdout to *.txt file with timestamp
-Easy to find bugs
-```
-#[<span style="color: grey;"> Click here for HTMLTestRunner-rv documentation</span>](https://ravikiranb36.github.io/htmltestrunner-rv.github.io/)
-
-#Installation:
-```bash
-pip install HTMLTestRunner-rv
-```
-
-# Creating suite
-```python
-my_test_suite = unittest.TestSuite()
-```
-
-# output to a file
-```python
-runner = HTMLTestRunner(
-title='My unit test', open_in_browser=True)
-```
-
-# run the test
-```python
-runner.run(my_test_suite)
-```
-
-#Example code:
-```python
-import unittest
-
-from HTMLTestRunner.runner import HTMLTestRunner
-from tests.test_1 import TestCase1
-from tests.test_2 import TestCase2
-
-test1 = unittest.TestLoader().loadTestsFromTestCase(TestCase1)
-test2 = unittest.TestLoader().loadTestsFromTestCase(TestCase2)
-suite = unittest.TestSuite([test1, test2])
-runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
-                        open_in_browser=True, description="HTMLTestReport", tested_by="Ravikirana B",
-                        add_traceback=False)
-
-runner.run(suite)
-```
-## Now you can pass external css styling and javascript for report
-### Example:
-```python
-style = """
-    .heading {
-    margin-top: 0ex;
-    margin-bottom: 1ex;
-    border-style:ridge;
-    color:white;
-    background-color:#999900;
-    font-weight:bold;
-    }
-"""
-script = """
-    Your script
-"""
-runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
-                        open_in_browser=True, description="HTMLTestReport", script=script, style=style)
-```
-
+Metadata-Version: 2.1
+Name: HTMLTestRunner-rv
+Version: 1.1.0
+Summary: HTMLTestRunner for unit test framework
+Home-page: https://github.com/ravikiranb36/HTMLTestRunner.io.git
+Author: Ravikirana B
+Author-email: ravikiranb36@gmail.com
+License: MIT
+Keywords: HtmlTestRunner TestRunner Html Reports
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# HTMLTestRunner
+```text
+HTMLTestRunner for python3 
+
+A TestRunner for use with the Python unit testing framework. 
+It generates a HTML report to show the result at a glance.
+It logs stdout to *.txt file with timestamp
+Easy to find bugs
+```
+#[<span style="color: grey;"> Click here for HTMLTestRunner-rv documentation</span>](https://ravikiranb36.github.io/htmltestrunner-rv.github.io/)
+
+#Installation:
+```bash
+pip install HTMLTestRunner-rv
+```
+
+# Creating suite
+```python
+my_test_suite = unittest.TestSuite()
+```
+
+# output to a file
+```python
+runner = HTMLTestRunner(
+title='My unit test', open_in_browser=True)
+```
+
+# run the test
+```python
+runner.run(my_test_suite)
+```
+
+#Example code:
+```python
+import unittest
+
+from HTMLTestRunner.runner import HTMLTestRunner
+from tests.test_1 import TestCase1
+from tests.test_2 import TestCase2
+
+test1 = unittest.TestLoader().loadTestsFromTestCase(TestCase1)
+test2 = unittest.TestLoader().loadTestsFromTestCase(TestCase2)
+suite = unittest.TestSuite([test1, test2])
+runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
+                        open_in_browser=True, description="HTMLTestReport", tested_by="Ravikirana B",
+                        add_traceback=False)
+
+runner.run(suite)
+```
+## Now you can pass external css styling and javascript for report
+### Example:
+```python
+style = """
+    .heading {
+    margin-top: 0ex;
+    margin-bottom: 1ex;
+    border-style:ridge;
+    color:white;
+    background-color:#999900;
+    font-weight:bold;
+    }
+"""
+script = """
+    Your script
+"""
+runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
+                        open_in_browser=True, description="HTMLTestReport", script=script, style=style)
+```
```

### Comparing `HTMLTestRunner-rv-1.0.18/PKG-INFO` & `HTMLTestRunner-rv-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,84 @@
-Metadata-Version: 2.1
-Name: HTMLTestRunner-rv
-Version: 1.0.18
-Summary: HTMLTestRunner for unit test framework
-Home-page: https://github.com/ravikiranb36/HTMLTestRunner.io.git
-Author: Ravikirana B
-Author-email: ravikiranb36@gmail.com
-License: MIT
-Keywords: HtmlTestRunner TestRunner Html Reports
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# HTMLTestRunner
-```text
-HTMLTestRunner for python3 
-
-A TestRunner for use with the Python unit testing framework. 
-It generates a HTML report to show the result at a glance.
-It logs stdout to *.txt file with timestamp
-Easy to find bugs
-```
-#[<span style="color: grey;"> Click here for HTMLTestRunner-rv documentation</span>](https://ravikiranb36.github.io/htmltestrunner-rv.github.io/)
-
-#Installation:
-```bash
-pip install HTMLTestRunner-rv
-```
-
-# Creating suite
-```python
-my_test_suite = unittest.TestSuite()
-```
-
-# output to a file
-```python
-runner = HTMLTestRunner(
-title='My unit test', open_in_browser=True)
-```
-
-# run the test
-```python
-runner.run(my_test_suite)
-```
-
-#Example code:
-```python
-import unittest
-
-from HTMLTestRunner.runner import HTMLTestRunner
-from tests.test_1 import TestCase1
-from tests.test_2 import TestCase2
-
-test1 = unittest.TestLoader().loadTestsFromTestCase(TestCase1)
-test2 = unittest.TestLoader().loadTestsFromTestCase(TestCase2)
-suite = unittest.TestSuite([test1, test2])
-runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
-                        open_in_browser=True, description="HTMLTestReport", tested_by="Ravikirana B",
-                        add_traceback=False)
-
-runner.run(suite)
-```
-## Now you can pass external css styling and javascript for report
-### Example:
-```python
-style = """
-    .heading {
-    margin-top: 0ex;
-    margin-bottom: 1ex;
-    border-style:ridge;
-    color:white;
-    background-color:#999900;
-    font-weight:bold;
-    }
-"""
-script = """
-    Your script
-"""
-runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
-                        open_in_browser=True, description="HTMLTestReport", script=script, style=style)
-```
-
+Metadata-Version: 2.1
+Name: HTMLTestRunner-rv
+Version: 1.1.0
+Summary: HTMLTestRunner for unit test framework
+Home-page: https://github.com/ravikiranb36/HTMLTestRunner.io.git
+Author: Ravikirana B
+Author-email: ravikiranb36@gmail.com
+License: MIT
+Keywords: HtmlTestRunner TestRunner Html Reports
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# HTMLTestRunner
+```text
+HTMLTestRunner for python3 
+
+A TestRunner for use with the Python unit testing framework. 
+It generates a HTML report to show the result at a glance.
+It logs stdout to *.txt file with timestamp
+Easy to find bugs
+```
+#[<span style="color: grey;"> Click here for HTMLTestRunner-rv documentation</span>](https://ravikiranb36.github.io/htmltestrunner-rv.github.io/)
+
+#Installation:
+```bash
+pip install HTMLTestRunner-rv
+```
+
+# Creating suite
+```python
+my_test_suite = unittest.TestSuite()
+```
+
+# output to a file
+```python
+runner = HTMLTestRunner(
+title='My unit test', open_in_browser=True)
+```
+
+# run the test
+```python
+runner.run(my_test_suite)
+```
+
+#Example code:
+```python
+import unittest
+
+from HTMLTestRunner.runner import HTMLTestRunner
+from tests.test_1 import TestCase1
+from tests.test_2 import TestCase2
+
+test1 = unittest.TestLoader().loadTestsFromTestCase(TestCase1)
+test2 = unittest.TestLoader().loadTestsFromTestCase(TestCase2)
+suite = unittest.TestSuite([test1, test2])
+runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
+                        open_in_browser=True, description="HTMLTestReport", tested_by="Ravikirana B",
+                        add_traceback=False)
+
+runner.run(suite)
+```
+## Now you can pass external css styling and javascript for report
+### Example:
+```python
+style = """
+    .heading {
+    margin-top: 0ex;
+    margin-bottom: 1ex;
+    border-style:ridge;
+    color:white;
+    background-color:#999900;
+    font-weight:bold;
+    }
+"""
+script = """
+    Your script
+"""
+runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
+                        open_in_browser=True, description="HTMLTestReport", script=script, style=style)
+```
```

### Comparing `HTMLTestRunner-rv-1.0.18/README.md` & `HTMLTestRunner-rv-1.1.0/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# HTMLTestRunner
-```text
-HTMLTestRunner for python3 
-
-A TestRunner for use with the Python unit testing framework. 
-It generates a HTML report to show the result at a glance.
-It logs stdout to *.txt file with timestamp
-Easy to find bugs
-```
-#[<span style="color: grey;"> Click here for HTMLTestRunner-rv documentation</span>](https://ravikiranb36.github.io/htmltestrunner-rv.github.io/)
-
-#Installation:
-```bash
-pip install HTMLTestRunner-rv
-```
-
-# Creating suite
-```python
-my_test_suite = unittest.TestSuite()
-```
-
-# output to a file
-```python
-runner = HTMLTestRunner(
-title='My unit test', open_in_browser=True)
-```
-
-# run the test
-```python
-runner.run(my_test_suite)
-```
-
-#Example code:
-```python
-import unittest
-
-from HTMLTestRunner.runner import HTMLTestRunner
-from tests.test_1 import TestCase1
-from tests.test_2 import TestCase2
-
-test1 = unittest.TestLoader().loadTestsFromTestCase(TestCase1)
-test2 = unittest.TestLoader().loadTestsFromTestCase(TestCase2)
-suite = unittest.TestSuite([test1, test2])
-runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
-                        open_in_browser=True, description="HTMLTestReport", tested_by="Ravikirana B",
-                        add_traceback=False)
-
-runner.run(suite)
-```
-## Now you can pass external css styling and javascript for report
-### Example:
-```python
-style = """
-    .heading {
-    margin-top: 0ex;
-    margin-bottom: 1ex;
-    border-style:ridge;
-    color:white;
-    background-color:#999900;
-    font-weight:bold;
-    }
-"""
-script = """
-    Your script
-"""
-runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
-                        open_in_browser=True, description="HTMLTestReport", script=script, style=style)
+# HTMLTestRunner
+```text
+HTMLTestRunner for python3 
+
+A TestRunner for use with the Python unit testing framework. 
+It generates a HTML report to show the result at a glance.
+It logs stdout to *.txt file with timestamp
+Easy to find bugs
+```
+#[<span style="color: grey;"> Click here for HTMLTestRunner-rv documentation</span>](https://ravikiranb36.github.io/htmltestrunner-rv.github.io/)
+
+#Installation:
+```bash
+pip install HTMLTestRunner-rv
+```
+
+# Creating suite
+```python
+my_test_suite = unittest.TestSuite()
+```
+
+# output to a file
+```python
+runner = HTMLTestRunner(
+title='My unit test', open_in_browser=True)
+```
+
+# run the test
+```python
+runner.run(my_test_suite)
+```
+
+#Example code:
+```python
+import unittest
+
+from HTMLTestRunner.runner import HTMLTestRunner
+from tests.test_1 import TestCase1
+from tests.test_2 import TestCase2
+
+test1 = unittest.TestLoader().loadTestsFromTestCase(TestCase1)
+test2 = unittest.TestLoader().loadTestsFromTestCase(TestCase2)
+suite = unittest.TestSuite([test1, test2])
+runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
+                        open_in_browser=True, description="HTMLTestReport", tested_by="Ravikirana B",
+                        add_traceback=False)
+
+runner.run(suite)
+```
+## Now you can pass external css styling and javascript for report
+### Example:
+```python
+style = """
+    .heading {
+    margin-top: 0ex;
+    margin-bottom: 1ex;
+    border-style:ridge;
+    color:white;
+    background-color:#999900;
+    font-weight:bold;
+    }
+"""
+script = """
+    Your script
+"""
+runner = HTMLTestRunner(log=True, verbosity=2, output='report', title='Test report', report_name='report',
+                        open_in_browser=True, description="HTMLTestReport", script=script, style=style)
 ```
```

